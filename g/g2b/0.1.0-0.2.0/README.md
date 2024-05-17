# Comparing `tmp/g2b-0.1.0-py3-none-any.whl.zip` & `tmp/g2b-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9526 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 18:20 g2b/__init__.py
--rw-r--r--  2.0 unx    15321 b- defN 24-May-09 18:20 g2b/g2b.py
--rw-r--r--  2.0 unx     1063 b- defN 24-May-09 18:20 g2b-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7282 b- defN 24-May-09 18:20 g2b-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-09 18:20 g2b-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       37 b- defN 24-May-09 18:20 g2b-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 24-May-09 18:20 g2b-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      593 b- defN 24-May-09 18:20 g2b-0.1.0.dist-info/RECORD
-8 files, 24392 bytes uncompressed, 8496 bytes compressed:  65.2%
+Zip file size: 9224 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 24-May-17 19:34 g2b/__init__.py
+-rw-r--r--  2.0 unx    13924 b- defN 24-May-17 19:34 g2b/g2b.py
+-rw-r--r--  2.0 unx     1063 b- defN 24-May-17 19:34 g2b-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7256 b- defN 24-May-17 19:34 g2b-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 19:34 g2b-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       37 b- defN 24-May-17 19:34 g2b-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-May-17 19:34 g2b-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 24-May-17 19:34 g2b-0.2.0.dist-info/RECORD
+8 files, 22969 bytes uncompressed, 8194 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: g2b/__init__.py
 Comment: 
 
 Filename: g2b/g2b.py
 Comment: 
 
-Filename: g2b-0.1.0.dist-info/LICENSE
+Filename: g2b-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: g2b-0.1.0.dist-info/METADATA
+Filename: g2b-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: g2b-0.1.0.dist-info/WHEEL
+Filename: g2b-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: g2b-0.1.0.dist-info/entry_points.txt
+Filename: g2b-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: g2b-0.1.0.dist-info/top_level.txt
+Filename: g2b-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: g2b-0.1.0.dist-info/RECORD
+Filename: g2b-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## g2b/g2b.py

```diff
@@ -1,77 +1,61 @@
-"""This module provides a converter that can translate a gnucash csv export into a beancount file"""
+# -*- coding: utf-8 -*-
+"""This module provides a converter that can translate a gnucash sql file into a beancount file"""
 
+import datetime
 import logging
+import os.path
 import re
+from collections import defaultdict
 from functools import cached_property
 from pathlib import Path
 from typing import Dict, List
 
 import click
-import pandas as pd
+import piecash
 import yaml
 from beancount.core import data, amount
 from beancount.core.number import D
 from beancount.ops import validation
 from beancount.ops.validation import validate
 from beancount.parser import printer
 from beancount.parser.parser import parse_file
+from piecash._common import GnucashException
 from rich.logging import RichHandler
 from rich.progress import track
-from simpleeval import simple_eval
 
 logging.basicConfig(
     level="NOTSET",
     format="%(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     handlers=[RichHandler(omit_repeated_times=False)],
 )
 
+logger = logging.getLogger("g2b")
+
 
 class G2BException(Exception):
     """Default Error for Exceptions"""
 
 
-class GnuCashCSV2Beancount:
-    """Application to convert a gnucash csv export to a beancount ledger"""
+class GnuCash2Beancount:
+    """Application to convert a gnucash sql file to a beancount ledger"""
 
     _DEFAULT_ACCOUNT_RENAME_PATTERNS = [
         (r"\s", "-"),
         ("_", "-"),
         (r"\.$", ""),
         (r"\.", "-"),
         ("&", "-"),
         (r"\(", ""),
         (r"\)", ""),
         ("---", "-"),
     ]
     """Pattern for character replacements in account names"""
 
-    _CSV_COLUMN_NAMES = [
-        "Date",
-        "BookingID",
-        "Number",
-        "Description",
-        "Remark",
-        "Commodity",
-        "CancellationReason",
-        "Action",
-        "BookingText",
-        "FullAccountName",
-        "AccountName",
-        "ValueWithSymbol",
-        "ValueNumerical",
-        "ValueWithSymbol2",
-        "ValueNumerical2",
-        "Reconciliation",
-        "ReconciliationDate",
-        "Rate",
-    ]
-    """List of column names that will be applied to the csv export"""
-
     @cached_property
     def _configs(self) -> Dict:
         """Loads and returns the configuration as a dict"""
         with open(self._config_path, "r", encoding="utf8") as file:
             try:
                 return yaml.safe_load(file)
             except yaml.YAMLError as error:
@@ -86,15 +70,25 @@
     def _gnucash_config(self) -> Dict:
         """Returns configurations only related to gnucash"""
         return self._configs.get("gnucash")
 
     @cached_property
     def _bean_config(self) -> Dict:
         """Returns configurations only related to the beancount export"""
-        return self._configs.get("beancount")
+        config = self._configs.get("beancount")
+        switched_to_bean_event = {datetime.date.today(): "misc Changed from GnuCash to Beancount"}
+        if "events" in config:
+            config["events"].update(switched_to_bean_event)
+        else:
+            config["events"] = switched_to_bean_event
+        return config
+
+    @cached_property
+    def _fava_config(self) -> Dict:
+        return self._configs.get("fava", {})
 
     @cached_property
     def _account_rename_patterns(self) -> List:
         """Returns a list of pattern that should be used to sanitize account names"""
         return (
             self._gnucash_config.get("account_rename_patterns", [])
             + self._DEFAULT_ACCOUNT_RENAME_PATTERNS
@@ -103,269 +97,252 @@
     @cached_property
     def _non_default_account_currencies(self) -> Dict:
         """Returns a list of account currency mappings for non default accounts"""
         return self._gnucash_config.get("non_default_account_currencies", {})
 
     def __init__(self, filepath: Path, output: Path, config: Path):
         self._filepath = filepath
+        self._book = None
         self._output_path = output
         self._config_path = config
-        self._dataframe = None
-        self._logger = logging.getLogger("g2b")
-        self._logger.setLevel(self._converter_config.get("loglevel", "INFO"))
+        self._commodities = defaultdict(list)
+        logging.getLogger().setLevel(self._converter_config.get("loglevel", "INFO"))
+
+    def _read_gnucash_book(self):
+        """Reads the gnucash book"""
+        try:
+            self._book = piecash.open_book(
+                os.path.abspath(str(self._filepath)), readonly=True, open_if_lock=True
+            )
+        except GnucashException as error:
+            raise G2BException(
+                f"File does not exist or wrong format exception: {error.args[0]}"
+            ) from error
 
     def write_beancount_file(self) -> None:
         """
-        Parse the configuration file, read the csv export and convert everything such that a valid
+        Parse the gnucash file, read and convert everything such that a valid
         beancount ledger can be exported.
         """
-        self._logger.info("Start converting GnuCash CSV File to Beancount")
-        self._logger.debug("Input file: %s", self._filepath)
-        self._logger.debug("Config file: %s", self._config_path)
-        self._logger.debug("Config: %s", self._configs)
-        self._prepare_csv()
-        openings = self._get_open_account_directives()
-        transactions = self._get_transaction_directives()
+        logger.info("Start converting GnuCash file to Beancount")
+        logger.debug("Input file: %s", self._filepath)
+        logger.debug("Config file: %s", self._config_path)
+        logger.debug("Config: %s", self._configs)
+        self._read_gnucash_book()
+        transactions = self._get_transactions()
+        openings = self._get_open_account_directives(transactions)
+        events = self._get_event_directives()
+        balance_statements = self._get_balance_directives()
+        commodities = self._get_commodities()
+        prices = self._get_prices()
         with open(self._output_path, "w", encoding="utf8") as file:
-            file.write(self._get_header_str())
-            file.write(self._get_commodities_str())
-            printer.print_entries(openings + transactions, file=file)
-        self._logger.info("Finished writing beancount file: '%s'", self._output_path)
+            printer.print_entries(
+                commodities + openings + events + prices + transactions + balance_statements,
+                file=file,
+                prefix=self._get_header_str(),
+            )
+        logger.info("Finished writing beancount file: '%s'", self._output_path)
         self._verify_output()
 
-    def _prepare_csv(self) -> None:
-        """Sanitizes the gnucash export"""
-        self._logger.info("Preparing dataframe")
-        self._dataframe = pd.read_csv(self._filepath)
-        self._dataframe.columns = self._CSV_COLUMN_NAMES
-        self._dataframe["FullAccountName"] = self._dataframe["FullAccountName"].apply(
-            self._apply_renaming_patterns
-        )
-        thousands_symbol = self._gnucash_config.get("thousands_symbol", ",")
-        decimal_symbol = self._gnucash_config.get("decimal_symbol", ".")
-        for col in ["Rate", "ValueNumerical"]:
-            self._dataframe[col] = self._dataframe[col].str.replace(thousands_symbol, "")
-            self._dataframe[col] = self._dataframe[col].str.replace(decimal_symbol, ".")
-        self._dataframe["Rate"] = self._dataframe["Rate"].apply(simple_eval)
-        for col in ["Rate", "ValueNumerical"]:
-            self._dataframe[col] = pd.to_numeric(self._dataframe[col])
-        self._dataframe["Date"] = pd.to_datetime(self._dataframe["Date"], format="%d.%m.%Y")
-        self._dataframe.sort_values(by="Date", inplace=True)
-
-    def _apply_renaming_patterns(self, account_name):
-        """
-        Renames an account such that it complies with the required beancount format.
-        The naming is also being capitalized here such that always only the first latter is written
-        in capitals.
-        """
-        for pattern, replacement in self._account_rename_patterns:
-            account_name = re.sub(pattern, repl=replacement, string=account_name)
-        return account_name.title()
-
-    def _get_open_account_directives(self) -> List[data.Open]:
-        """
-        Gets a list of unique account names and their corresponding date where they first appeared.
-
-        :returns: A list of beancount open directives
-        """
-        dataframe = self._dataframe.filter(items=["Date", "FullAccountName"])
-        dataframe.drop_duplicates(subset=["FullAccountName"], inplace=True)
-        openings = []
-        for index, row in track(
-            dataframe.iterrows(), total=len(dataframe), description="Parsing Account Openings..."
-        ):
-            currency = self._non_default_account_currencies.get(
-                row["FullAccountName"], self._gnucash_config.get("default_currency")
-            )
-            openings.append(
-                data.Open(
-                    meta={"filename": self._filepath, "lineno": index},
-                    date=row["Date"].date(),
-                    account=row["FullAccountName"],
-                    currencies=[currency],
-                    booking=data.Booking.FIFO,
+    def _get_transactions(self):
+        transactions = []
+        for transaction in track(self._book.transactions, description="Parsing Transactions"):
+            skip_template = "Skipped transaction as it is malformed: %s"
+            if len(transaction.splits) == 1 and transaction.splits[0].value == 0:
+                logger.warning(skip_template, {transaction})
+                continue
+            if transaction.splits[0].account.commodity.mnemonic == "template":
+                logger.warning(skip_template, {transaction})
+                continue
+            postings = self._get_postings(transaction.splits)
+            posting_flags = [posting.flag for posting in postings]
+            transaction_flag = "!" if "!" in posting_flags else "*"
+            transactions.append(
+                data.Transaction(
+                    meta={"filename": self._filepath, "lineno": -1},
+                    date=transaction.post_date,
+                    flag=transaction_flag,
+                    payee="",
+                    narration=self._sanitize_description(transaction.description),
+                    tags=data.EMPTY_SET,
+                    links=set(),
+                    postings=postings,
                 )
             )
-        return openings
-
-    def _get_transaction_directives(self) -> List[data.Transaction]:
-        """
-        Groups every entry inside the gnucash export by the respective BookingID.
-        For each group a transaction object with all corresponding postings is created and returned.
+        transactions.sort(key=lambda txn: txn.date)
+        return transactions
 
-        :return: List of beancount transactions
-        """
-        entries = []
-        groups = self._dataframe.groupby(by="BookingID")
-        for _, group in track(groups, description="Parsing Transactions..."):
-            postings = self._get_transaction_postings(group)
-            transaction = self._get_transaction(group, postings)
-            entries.append(transaction)
-        entries = sorted(entries, key=lambda x: x.date)
-        return entries
+    def _get_postings(self, splits):
+        postings = []
+        for split in splits:
+            account_name = str(self._apply_renaming_patterns(split.account.fullname))
+            posting_currency = split.account.commodity.mnemonic.replace(" ", "")
+            units = amount.Amount(number=split.quantity * D("1.0"), currency=posting_currency)
+            not_reconciled_symbol = self._gnucash_config.get("not_reconciled_symbol")
+            flag = None
+            if self._bean_config.get("flag_postings", True):
+                flag = "!" if not_reconciled_symbol in split.reconcile_state else "*"
+            price = self._calculate_price_of_split(split)
+            posting = data.Posting(
+                account=account_name, units=units, cost=None, price=price, flag=flag, meta=None
+            )
+            self._commodities[posting_currency].append(split.transaction.post_date)
+            self._commodities[posting_currency] = [min(self._commodities[posting_currency])]
+            postings.append(posting)
+        return postings
 
-    def _get_transaction_postings(self, transaction_group) -> List[data.Posting]:
-        """
-        Returns a list of beancount postings that reflect one transaction.
+    def _calculate_price_of_split(self, split):
+        if split.account.commodity == split.transaction.currency:
+            return None
+        currency = split.transaction.currency.mnemonic.replace(" ", "")
+        if split.value == 0 and split.quantity == 0:
+            return data.Amount(D("0"), currency)
+        return data.Amount(abs(split.value / split.quantity), currency)
+
+    def _get_event_directives(self) -> List[data.Event]:
+        """Parse beancount configuration and create event directives"""
+        events = []
+        for date, event_description in self._bean_config.get("events", {}).items():
+            event_type, description = event_description.split(" ", maxsplit=1)
+            events.append(data.Event(date=date, type=event_type, description=description, meta={}))
+        return events
 
-        :param transaction_group: One transaction grouped by the gnucash BookingID
-        :return: List of postings that are part of this transaction
-        """
-        postings = []
+    def _get_balance_directives(self) -> List[data.Balance]:
+        balances = []
         default_currency = self._gnucash_config.get("default_currency")
-        for _, row in transaction_group.iterrows():
-            currency = self._non_default_account_currencies.get(
-                row["FullAccountName"], default_currency
-            )
-            # need to convert numerical value back to string as it would have otherwise the
-            # imperfections of float, e.g 2.2 could become 2.2000000000000000001234312312334
-            unit = amount.Amount(D(str(row["ValueNumerical"])), currency=currency)
-            price = float(row["Rate"]) if float(row["Rate"]) != 1.0 else None
-            if price is not None:
-                price = self._get_price_of_posting(price, currency, transaction_group)
-            postings.append(
-                data.Posting(
-                    account=row["FullAccountName"],
-                    units=unit,
-                    cost=None,
-                    price=price,
-                    flag=None,
-                    meta=None,
+        date_of_tomorrow = datetime.date.today() + datetime.timedelta(days=1)
+        for account, balance_value in self._bean_config.get("balance-values", {}).items():
+            currency = self._non_default_account_currencies.get(account, default_currency)
+            balances.append(
+                data.Balance(
+                    date=date_of_tomorrow,
+                    account=account,
+                    amount=amount.Amount(number=D(str(balance_value)), currency=currency),
+                    meta={},
+                    tolerance=None,
+                    diff_amount=None,
                 )
             )
-        return postings
+        return balances
 
-    def _get_price_of_posting(self, price, unit_currency, transaction_group) -> amount.Amount:
-        """
-        Gets the price, and it's corresponding currency of the transaction.
-        Assigns the default currency if the unit_currency differs from it. If the default and
-        unit currencies are equal though, then the gnucash export had an issue. If the transaction
-        has only two postings with two separate currencies it takes the currency of the other
-        transaction, such that beancount can estimate the correct price for it later.
-
-        :param price: The price/conversion number of the currency
-        :param unit_currency: The currency of the transaction itself
-        :param transaction_group: The dataframe group containing all postings
-        :return: The amount.Amount of the price of this transaction
-        """
-        default_currency = self._gnucash_config.get("default_currency")
-        price_currency = default_currency
-        account_currencies = [
-            self._non_default_account_currencies.get(row["FullAccountName"], default_currency)
-            for _, row in transaction_group.iterrows()
-        ]
-        if unit_currency == default_currency and len(set(account_currencies)) == 2:
-            currency_set = set(account_currencies)
-            price_currency = currency_set.difference({unit_currency}).pop()
-        price = amount.Amount(D(price), currency=price_currency)
-        return price
+    def _get_commodities(self):
+        commodities = []
+        for commodity, date in self._commodities.items():
+            meta = {"filename": self._filepath, "lineno": -1}
+            if self._fava_config.get("commodity-precision", None) is not None:
+                meta.update({"precision": self._fava_config.get("commodity-precision")})
+            commodities.append(data.Commodity(date=date[0], currency=commodity, meta=meta))
+        return commodities
 
-    def _get_transaction(self, transaction_group, postings) -> data.Transaction:
+    def _apply_renaming_patterns(self, account_name):
         """
-        Returns a beancount Transaction object by combining the transaction meta information
-        with the previously created postings.
-
-        :param transaction_group: The gnucash dataframe group
-        :param postings: The beancount postings that are part of this transaction
-        :return:
+        Renames an account such that it complies with the required beancount format.
+        The naming is also being capitalized here such that always only the first latter is written
+        in capitals.
         """
-        unique_descriptions = transaction_group["Description"].unique()
-        if len(unique_descriptions) > 1:
-            self._logger.warning(
-                "More than one description found for a transaction: %s, "
-                "using only first description: '%s'",
-                unique_descriptions,
-                transaction_group["Description"].iloc[0],
-            )
-        reconciliations = transaction_group["Reconciliation"].values
-        # if one symbol is not reconciled mark all as not reconciled with !
-        flag = "!" if self._gnucash_config.get("not_reconciled_symbol") in reconciliations else "*"
-        transaction = data.Transaction(
-            meta={"filename": self._filepath, "lineno": transaction_group.index[0]},
-            date=transaction_group["Date"].iloc[0].date(),
-            flag=flag,
-            payee=None,
-            narration=self._sanitize_description(transaction_group["Description"].iloc[0]),
-            tags=data.EMPTY_SET,
-            links=set(),
-            postings=postings,
-        )
-        return transaction
+        for pattern, replacement in self._account_rename_patterns:
+            account_name = re.sub(pattern, repl=replacement, string=account_name)
+        return account_name.title()
 
     def _sanitize_description(self, description) -> str:
         """Removes unwanted characters from a transaction narration"""
         description = description.replace("\xad", "")
         description = description.replace('"', "'")
         return description
 
     def _get_header_str(self) -> str:
         """Returns a string that combines the configured beancount options and plugins"""
         plugins = [f'plugin "{plugin}"' for plugin in self._bean_config.get("plugins")]
         options = [f'option "{key}" "{value}"' for key, value in self._bean_config.get("options")]
         header = "\n".join(plugins + [""] + options)
         return f"{header}\n\n"
 
-    def _get_commodities_str(self) -> str:
-        """
-        Returns a string with the commodities, combined from the default currency and the configured
-        non default currencies.
-        """
-        earliest_date = self._dataframe["Date"].iloc[0].date()
-        default_currency = [
-            f"{earliest_date} commodity {self._gnucash_config.get('default_currency')}"
-        ]
-        commodities_strs = [
-            f"{earliest_date} commodity {commodity}"
-            for commodity in self._non_default_account_currencies.values()
-        ]
-        joined_str = "\n".join(default_currency + commodities_strs)
-        return f"{joined_str}\n\n"
-
     def _verify_output(self) -> None:
         """
         Verifies the created beancount ledger by running the respective beancount parser and
         beancount validator. If any errors are found they are logged to the console.
         """
-        self._logger.info("Verifying output file")
+        logger.info("Verifying output file")
         entries, parsing_errors, options = parse_file(self._output_path)
         for error in parsing_errors:
-            self._logger.error(error)
+            logger.error(error)
         validation_errors = validate(
             entries=entries,
             options_map=options,
             extra_validations=validation.HARDCORE_VALIDATIONS,
         )
         for error in validation_errors:
-            self._logger.warning(error)
+            logger.warning(error)
         if not parsing_errors and not validation_errors:
-            self._logger.info("No parsing or validation errors found")
+            logger.info("No parsing or validation errors found")
         if parsing_errors:
-            self._logger.warning("Found %s parsing errors", len(parsing_errors))
+            logger.warning("Found %s parsing errors", len(parsing_errors))
         if validation_errors:
-            self._logger.warning("Found %s validation errors", len(validation_errors))
+            logger.warning("Found %s validation errors", len(validation_errors))
+
+    def _get_open_account_directives(self, transactions):
+        account_date_tuples = [
+            (posting.account, transaction.date, posting.units.currency)
+            for transaction in transactions
+            for posting in transaction.postings
+        ]
+        accounts = defaultdict(list)
+        for account, date, currency in account_date_tuples:
+            accounts[account].append((date, currency))
+        openings = []
+        for account, date_currency_tuples in accounts.items():
+            dates, currencies = zip(*date_currency_tuples)
+            openings.append(
+                data.Open(
+                    account=account,
+                    currencies=[currencies[0]],
+                    date=min(dates),
+                    meta={"filename": self._filepath, "lineno": -1},
+                    booking=None,
+                )
+            )
+        return openings
+
+    def _get_prices(self):
+        prices = []
+        for price in self._book.prices:
+            prices.append(
+                data.Price(
+                    meta={"filename": self._filepath, "lineno": -1},
+                    currency=price.commodity.mnemonic.replace(" ", ""),
+                    amount=amount.Amount(number=price.value, currency=price.currency.mnemonic),
+                    date=price.date,
+                )
+            )
+        prices.sort(key=lambda x: x.date)
+        return prices
 
 
 @click.command()
+@click.version_option(message="%(version)s")
 @click.option(
     "--input",
     "-i",
     "input_path",
     type=click.Path(exists=True),
-    help="Gnucash CSV file path",
+    help="Gnucash file path",
     required=True,
 )
 @click.option("--output", "-o", help="Output file path", required=True)
 @click.option(
     "--config", "-c", help="Config file path", type=click.Path(exists=True), required=True
 )
 def main(input_path: Path, output: Path, config: Path) -> None:
     """
-    GnuCash CSV to Beancount Converter - g2b
+    GnuCash to Beancount Converter - g2b
 
-    This tool allows you to convert a gnucash csv export into a new beancount ledger.
+    This tool allows you to convert a gnucash sql file into a new beancount ledger.
     """
-    g2b = GnuCashCSV2Beancount(input_path, output, config)
-    g2b.write_beancount_file()
+    try:
+        g2b = GnuCash2Beancount(input_path, output, config)
+        g2b.write_beancount_file()
+    except G2BException as error:
+        logging.error(error)
 
 
 if __name__ == "__main__":
-    main()  # pylint: disable=no-value-for-parameter)
+    main()  # pylint: disable=no-value-for-parameter
```

## Comparing `g2b-0.1.0.dist-info/LICENSE` & `g2b-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `g2b-0.1.0.dist-info/METADATA` & `g2b-0.2.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: g2b
-Version: 0.1.0
-Summary: Initialize a beancount ledger from a GnuCash CSV export
+Version: 0.2.0
+Summary: Initialize a beancount ledger from a GnuCash file
 License: MIT License
         
         Copyright (c) 2024 dtrai2
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,67 +20,81 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Keywords: gnucash,beancount,csv,finance,accounting
+Project-URL: Homepage, https://github.com/dtrai2/gnucash-csv-to-beancount
+Project-URL: Documentation, https://github.com/dtrai2/gnucash-csv-to-beancount/blob/main/README.md
+Project-URL: Repository, https://github.com/dtrai2/gnucash-csv-to-beancount
+Project-URL: Issues, https://github.com/dtrai2/gnucash-csv-to-beancount/issues
+Keywords: gnucash,beancount,finance,accounting
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pandas
 Requires-Dist: beancount
 Requires-Dist: click
 Requires-Dist: rich
 Requires-Dist: pyyaml
-Requires-Dist: simpleeval
+Requires-Dist: piecash
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: pylint ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
 Requires-Dist: coverage ; extra == 'dev'
 Requires-Dist: ruff ; extra == 'dev'
+Requires-Dist: pre-commit ; extra == 'dev'
 
-# Gnucash CSV to Beancount
+# Gnucash to Beancount
 
-This project can convert a [Gnucash](https://github.com/Gnucash/gnucash) CSV Export into a new
+This project can convert a [Gnucash](https://github.com/Gnucash/gnucash) sql file into a new
 [beancount](https://github.com/beancount/beancount) file.
-It is not intended to continuously import gnucash data into an existing beancount ledger, as this 
+It is not intended to continuously import gnucash data into an existing beancount ledger, as this
 script will also add plugins and beancount options to the beginning of the file.
+This project started with the intention to convert a gnucash csv export, but it turned out that the
+csv exported from gnucash is not quite reliable.
+Read more about that at in the section [Unreliable Export](#unreliable-gnucash-csv-export).
+Because of that I refactored it to use the [piecash](https://pypi.org/project/piecash/) library.
+With that it has the same goal as the already existing repository from
+[henriquebastos/gnucash-to-beancount](https://github.com/henriquebastos/gnucash-to-beancount).
+The implementation in this repository does offer few configuration options though.
+
+One downside I have encountered sofar are stock splits.
+Those are currently not supported and have to be added manually to the output by following the
+official documentation
+[Beancount Stock Splits](https://beancount.github.io/docs/trading_with_beancount.html#stock-splits).
+Luckily those splits don't happen too often.
+
+## Prerequisite
+
+Your gnucash file must be in a sql format.
+I implemented it with a sqlite3 file, which was saved by GnuCash v5.4.
+If your current genucash file is not in the right format it is always possible to just save it
+as a sqlite3 file.
 
 ## Install
 
-To install `gnucash csv to beancount` simply use `pip`:
+To install `gnucash to beancount` simply use `pip`:
 
 ```bash
 pip install g2b
 ```
 
-## Usage
-
-### Create a GnuCash Export
+Test with `g2b --version` if the installation was successful.
 
-Start the export by navigating to `File > Export > Export Transactions to CSV`. 
-You can follow the official gnucash [Export Transactions](https://www.gnucash.org/docs/v4/C/gnucash-help/trans-export.html)
-Documentation.
-Consider the following points while configuring the export:
-
-- Use the comma seperator
-- Check the option `Use Qoutes`
-- **Do not** use the simple layout
+## Usage
 
 ### Create Configuration for g2b
 
 In order for a successful conversion you need to create a `yaml` configuration file.
 An example would look like this:
 
 ```yaml
@@ -93,76 +107,57 @@
   reconciled_symbol: "b"
   not_reconciled_symbol: "n"
   account_rename_patterns:  # Here you can rename accounts that might not align with the beancount format
     - ["OpenBalance", "Equity:Opening-Balance"]
     - ["Money@[Bank]", "Assets:Money at Bank"]
   non_default_account_currencies:  # Here you have to name all accounts that deviate from the default currency
     Assets:Cash:Wallet: "NZD"
-beancount:  # here you can add beancount options and plugins that should be added to output file
+beancount:  # here you can add beancount options, plugins and events that should be added to output file
+  flag_postings: false  # if false, will set all transactions automatically to '*' (default: true)
   options:
     - ["title", "Exported GnuCash Book"]  # options should be key value pairs
     - ["operating_currency", "EUR"]
   plugins:
     - "beancount.plugins.check_commodity"  # plugins can be named directly
     - "beancount.plugins.coherent_cost"
     - "beancount.plugins.nounused"
     - "beancount.plugins.auto"
+  events:
+    2024-05-05: type description string  # optional events that should be added to the output, the
+                                         # first space is used to split between space and description
+fava:  # optional configuration specific to fava
+  commodity-precision: 3  # set the render precision of values for the fava web-frontend
 ```
 
 ## Execute g2b
 
-Now that you have the gnucash export and the corresponding configuration file you can call:
+Once you created the needed configuration file you can call:
 
 ```bash
-g2b -i gnuchash.csv -c config.yaml -o my.beancount
+g2b -i book.gnucash -c config.yaml -o my.beancount
 ```
 
-The script will automatically call beancount to parse and verify the export, such that you know
-if the conversion was successful or not.
+The script will, at the end, automatically call beancount to parse and verify the export, such
+that you know if the conversion was successful or not.
 
 ## Limitations
 
-The conversion sadly doesn't work perfectly when it comes to transactions with multiple currencies,
-or currency conversions. 
-This is in part due to the gnucash export itself.
-The column `Commodity/Currency` doesn't truly reflect the currency of the transaction.
-Furthermore, the column `Ammount with Symbol` has ambiguous symbols as it doesn't use the ISO-4217
-Currency codes. 
-With that it is for example not clear if `100 $` are USD or NZD. 
-A change was already proposed back in 2017:
-[gnucash bug - use ISO 4217 currency symbols in output](https://bugs.gnucash.org/show_bug.cgi?id=791651).
-
-To work a bit around that you have to specify currencies inside the configuration file for your accounts,
-that deviate from the default currency.
-After the conversion it is still possible though that beancount will complain about transactions
-with multiple currency. 
-That is also because gnucash assigns the `Rate/Price` inside the export to the wrong account.
-For example a ledger (with default currency EUR) has a transaction from an NZD account to an EUR
-account.
-Transactions that were exported correctly will appear like this:
-
-| Date         | FullAccountName        | Amount Num | Rate/Price |
-|--------------|------------------------|------------|------------|
-| 2024-05-09   | Assets:Wallet(NZD)     | 200 $      | 0.56       |
-| 2024-05-09   | Expense:Groceries(EUR) | 111.74 €   | 1.00       |
-
-The non-default currency account `Assets:Wallet(NZD)` has here a `Rate/Price` of `0.56`, whereas
-the other position has a value of `1.00`.
-
-In some cases the export has an entry like this though:
-
-| Date         | FullAccountName        | Amount Num | Rate/Price |
-|--------------|------------------------|------------|------------|
-| 2024-05-09   | Assets:Wallet(NZD)     | 200 $      | 1.00       |
-| 2024-05-09   | Expense:Groceries(EUR) | 111.74 €   | 0.56       |
-
-Where the `Rate/Price` of `0.56` is assigned to the account with the default currenyc.
-That leads to a currency conversion from EUR to EUR, which results in problems in beancount.
-Transactions that only consist of two postings should be fine after a small change. 
-If the transaction has multiple postings though you have to fix them manually. 
-Luckily beancount will tell you with errors/warnings where you have to look to fix them.
-
-It is also possible to add the beancount option `inferred_tolerance_default`
-(see [Beancount Options](https://beancount.github.io/docs/beancount_options_reference.html)) to
-specify a tolerance for certain currencies.
-This is merely a way to mute the warnings though as it doesn't fix the problem, it just tells
-beancount to be less strict. 
+Currently, this project can not deal with stock splits.
+Those will not be added to the beancount output and have to be added manually.
+To do that follow the official
+[Documentation](https://beancount.github.io/docs/trading_with_beancount.html#stock-splits).
+
+## Unreliable Gnucash CSV Export
+
+While starting out with CSV exports I found the following issues that kept me from
+progressing with the CSV exports.
+
+- The gnucash csv export does not offer reliable currency information.
+  Transaction with values like `100 $` cannot be properly understood as it, for example, could be
+  USD or NZD.
+  An offical bug report is open since 2017:
+  [gnucash bug - use ISO 4217 currency symbols in output](https://bugs.gnucash.org/show_bug.cgi?id=791651).
+- The `Rate/Price` value is sometimes added to the wrong posting in transactions with multiple
+  currencies.
+  Because of that it wasn't easily recognizable how to convert which prices.
+- And probably the most severe issue: Some transactions were completely missing inside the export.
+  As I couldn't figure out why I decided to use the `piecash` library.
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

