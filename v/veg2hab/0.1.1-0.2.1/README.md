# Comparing `tmp/veg2hab-0.1.1.tar.gz` & `tmp/veg2hab-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veg2hab-0.1.1.tar", max compression
+gzip compressed data, was "veg2hab-0.2.1.tar", max compression
```

## Comparing `veg2hab-0.1.1.tar` & `veg2hab-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7626 2024-04-26 10:24:39.656747 veg2hab-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     2993 2024-04-26 10:24:39.656747 veg2hab-0.1.1/README.md
--rw-r--r--   0        0        0      855 2024-04-26 10:24:40.052746 veg2hab-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       72 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/__init__.py
--rw-r--r--   0        0        0     1173 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/__main__.py
--rw-r--r--   0        0        0     5396 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/access_db.py
--rw-r--r--   0        0        0      411 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/constants.py
--rw-r--r--   0        0        0     6384 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/criteria.py
--rw-r--r--   0        0        0     7489 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/definitietabel.py
--rw-r--r--   0        0        0     5202 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/enums.py
--rw-r--r--   0        0        0      576 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/fgr.py
--rw-r--r--   0        0        0    10773 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/habitat.py
--rw-r--r--   0        0        0     5030 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/io/arcgis.py
--rw-r--r--   0        0        0     2328 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/io/cli.py
--rw-r--r--   0        0        0     4078 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/io/common.py
--rw-r--r--   0        0        0     2941 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/main.py
--rw-r--r--   0        0        0    11233 2024-04-26 10:24:40.052746 veg2hab-0.1.1/veg2hab/mozaiek.py
--rw-r--r--   0        0        0 13900219 2024-04-26 10:24:40.104746 veg2hab-0.1.1/veg2hab/package_data/FGR.json
--rw-r--r--   0        0        0      130 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
--rw-r--r--   0        0        0      130 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/package_data/opgeschoonde_waswordt.xlsx
--rw-r--r--   0        0        0     3085 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/package_data/toolbox.pyt
--rw-r--r--   0        0        0    13084 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/validation.py
--rw-r--r--   0        0        0    15069 2024-04-26 10:24:40.804745 veg2hab-0.1.1/veg2hab/vegetatietypen.py
--rw-r--r--   0        0        0    45254 2024-04-26 10:24:40.808745 veg2hab-0.1.1/veg2hab/vegkartering.py
--rw-r--r--   0        0        0     4585 2024-04-26 10:24:40.808745 veg2hab-0.1.1/veg2hab/waswordtlijst.py
--rw-r--r--   0        0        0     3872 1970-01-01 00:00:00.000000 veg2hab-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     7626 2024-05-07 08:48:39.707739 veg2hab-0.2.1/LICENSE.md
+-rw-r--r--   0        0        0    13020 2024-05-07 08:48:39.707739 veg2hab-0.2.1/README.md
+-rw-r--r--   0        0        0     1311 2024-05-07 08:48:40.103738 veg2hab-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/__init__.py
+-rw-r--r--   0        0        0     1173 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/__main__.py
+-rw-r--r--   0        0        0     6513 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/access_db.py
+-rw-r--r--   0        0        0      411 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/constants.py
+-rw-r--r--   0        0        0     6384 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/criteria.py
+-rw-r--r--   0        0        0     7489 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/definitietabel.py
+-rw-r--r--   0        0        0     5414 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/enums.py
+-rw-r--r--   0        0        0      576 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/fgr.py
+-rw-r--r--   0        0        0    14411 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/habitat.py
+-rw-r--r--   0        0        0     5030 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/io/arcgis.py
+-rw-r--r--   0        0        0     2328 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/io/cli.py
+-rw-r--r--   0        0        0     4296 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/io/common.py
+-rw-r--r--   0        0        0     2941 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/main.py
+-rw-r--r--   0        0        0    11093 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/mozaiek.py
+-rw-r--r--   0        0        0 13900219 2024-05-07 08:48:40.155738 veg2hab-0.2.1/veg2hab/package_data/FGR.json
+-rw-r--r--   0        0        0    39387 2024-05-07 08:48:40.795737 veg2hab-0.2.1/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
+-rw-r--r--   0        0        0    19152 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/package_data/opgeschoonde_waswordt.xlsx
+-rw-r--r--   0        0        0     3094 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/package_data/toolbox.pyt
+-rw-r--r--   0        0        0    13084 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/validation.py
+-rw-r--r--   0        0        0    15069 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/vegetatietypen.py
+-rw-r--r--   0        0        0    46327 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/vegkartering.py
+-rw-r--r--   0        0        0     4585 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/waswordtlijst.py
+-rw-r--r--   0        0        0    14049 1970-01-01 00:00:00.000000 veg2hab-0.2.1/PKG-INFO
```

### Comparing `veg2hab-0.1.1/LICENSE.md` & `veg2hab-0.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/__main__.py` & `veg2hab-0.2.1/veg2hab/__main__.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/access_db.py` & `veg2hab-0.2.1/veg2hab/access_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     return pd.read_csv(
         folder / f"{table_name.value}.csv",
         usecols=list(col_names.keys()),
         dtype=col_names,
     )
 
 
-def unpack_access_db(access_db_path: str, output_folder: Path):
+def _unpack_access_db(access_db_path: str, output_folder: Path):
     assert output_folder.is_dir()
     try:
         subprocess.run(
             ["mdb-export", "--version"],
             check=True,
         )
     except Exception as e:
@@ -90,14 +90,34 @@
 
         except subprocess.CalledProcessError as e:
             raise RuntimeError(
                 f"Er is iets fout gegaan bij het uitpakken van de access database: {e.stderr.decode()}"
             ) from e
 
 
+def _group_lokale_vegtypen_en_bedekking_to_str(rows: pd.DataFrame) -> str:
+    """
+    Ontvangt een setje rijen van 1 locatie (vlak) met lokale vegetatietypen en bedekkingspercentages.
+    Hier wordt een string van gemaakt uiteindelijk in de output komt zonder verdere bewerkingen.
+    """
+    assert all(
+        col in rows.columns for col in ["Locatie", "Vegetatietype", "Bedekking_num"]
+    ), "Locatie, Vegetatietype en Bedekking_num moeten kolommen zijn in _group_lokale_vegtypen_en_bedekking_to_str"
+
+    assert (
+        rows["Locatie"].nunique() == 1
+    ), "_group_lokale_vegtypen_en_bedekking_to_str moet op een groupby over Locatie uitgevoerd worden; nu is locatie niet hetzelfde in 1 group"
+
+    return_strings = [
+        f"{row['Vegetatietype']} ({row['Bedekking_num']}%)"
+        for _, row in rows.iterrows()
+    ]
+    return ", ".join(return_strings)
+
+
 def read_access_tables(acces_mdb: Path) -> Tuple[pd.DataFrame, pd.DataFrame]:
     """Read the tables from the access database and return them as pandas dataframes"""
     # TODO fix circular imports
     from veg2hab.vegetatietypen import SBB as _SBB
     from veg2hab.vegkartering import VegTypeInfo
 
     if not acces_mdb.is_file() and not acces_mdb.suffix == ".mdb":
@@ -105,15 +125,15 @@
 
     if sys.platform == "win32":
         temp_dir = None
         locatie: Union[pyodbc.Connection, Path] = connect_to_access(acces_mdb)
     elif sys.platform.startswith("linux"):
         temp_dir = tempfile.TemporaryDirectory()
         locatie: Union[pyodbc.Connection, Path] = Path(temp_dir.name)
-        unpack_access_db(acces_mdb, locatie)
+        _unpack_access_db(acces_mdb, locatie)
 
     element = read_table(
         locatie,
         TableNames.ELEMENT,
         {"ElmID": int, "intern_id": int, "Locatietype": str},
     )
     # Uitfilteren van lijnen, selecteer alleen vlakken
@@ -169,11 +189,19 @@
             VegTypeInfo.create_vegtypen_list_from_access_rows,
             perc_col="Bedekking_num",
             SBB_col="Sbb",
         )
         .reset_index(name="VegTypeInfo")
     )
 
+    lokale_vegtypen = (
+        kart_veg.groupby("Locatie")
+        .apply(_group_lokale_vegtypen_en_bedekking_to_str)
+        .reset_index(name="_LokVegTyp")
+    )
+
+    grouped_kart_veg = grouped_kart_veg.merge(lokale_vegtypen, on="Locatie")
+
     if temp_dir:
         temp_dir.cleanup()
 
     return element, grouped_kart_veg
```

### Comparing `veg2hab-0.1.1/veg2hab/criteria.py` & `veg2hab-0.2.1/veg2hab/criteria.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/definitietabel.py` & `veg2hab-0.2.1/veg2hab/definitietabel.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/enums.py` & `veg2hab-0.2.1/veg2hab/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,22 @@
             MaybeBoolean.TRUE: 4,
         }
         or_resolver = {v: k for k, v in or_order.items()}
         if not isinstance(other, MaybeBoolean):
             return NotImplemented
         return or_resolver[max(or_order[self], or_order[other])]
 
+    def __str__(self):
+        return self.name
+
 
 class Kwaliteit(Enum):
-    NVT = "Nvt"  # bijvoorbeeld in het geval van H000
-    ONBEKEND = "Onbekend"  # bijvoorbeeld in het geval van HXXXX
+    NVT = "Nvt"  # bijvoorbeeld in het geval van H0000 en HXXXX
+    # NOTE: Ik heb dit weggehaald want ik ben NVT en ONBEKEND door mekaar wezen halen, en eigenlijk past NVT ook wel bij HXXXX
+    # ONBEKEND = "Onbekend"  # bijvoorbeeld in het geval van HXXXX
     GOED = "Goed"
     MATIG = "Matig"
 
     @classmethod
     def from_letter(cls, letter: str) -> "Kwaliteit":
         if letter == "G":
             return cls.GOED
@@ -67,15 +71,15 @@
             raise ValueError("Letter moet G of M zijn")
 
     def as_letter(self) -> str:
         if self == Kwaliteit.GOED:
             return "G"
         elif self == Kwaliteit.MATIG:
             return "M"
-        elif self in [Kwaliteit.NVT, Kwaliteit.ONBEKEND]:
+        elif self in [Kwaliteit.NVT]:
             return "X"
         else:
             raise ValueError("GoedMatig is niet Goed of Matig")
 
 
 class MatchLevel(IntEnum):
     """
@@ -111,40 +115,39 @@
 
     # Meerdere even specifieke habitatvoorstellen met kloppende mitsen
     MEERDERE_KLOPPENDE_MITSEN = auto()
 
     # Er zijn PlaceholderCriteriums, dus handmatige controle
     PLACEHOLDER = auto()
 
-    # Dit gaat Veg2Hab niet op kunnen lossen
-    HANDMATIGE_CONTROLE = auto()
+    # # Dit gaat Veg2Hab niet op kunnen lossen
+    # HANDMATIGE_CONTROLE = auto()
 
-    # Er moet gewacht worden totdat alle zelfstandige habitatwaardige vegetaties
-    # zijn bepaald, pas dan kunnen de mozaiekregels worden toegepast
+    # Er is meer dan threshold % HXXXX in de omliggende vlakken
     WACHTEN_OP_MOZAIEK = auto()
 
     def toelichting(self):
         if self == KeuzeStatus.DUIDELIJK:
             return "Als alle regels gevolgd worden is er 1 duidelijke optie; er is maar 1 habitatvoorstel met kloppende mits/mozaiek."
         elif self == KeuzeStatus.GEEN_KLOPPENDE_MITSEN:
             return "Er is geen habitatvoorstel met kloppende mits/mozaiek. Er kan dus geen habitattype toegekend worden."
         elif self == KeuzeStatus.VEGTYPEN_NIET_IN_DEFTABEL:
             return "De vegetatietypen van het vlak zijn niet in de definitietabel gevonden en leiden dus niet tot een habitattype."
         elif self == KeuzeStatus.GEEN_OPGEGEVEN_VEGTYPEN:
-            return "Er zijn in de vegetatiekartering geen vegetatietypen opgegeven voor dit vlak. Er is dus geen habitattype toe te kennen."
+            return "Er zijn in de vegetatiekartering geen (habitatwaardige)vegetatietypen opgegeven voor dit vlak. Er is dus geen habitattype toe te kennen."
         elif self == KeuzeStatus.MEERDERE_KLOPPENDE_MITSEN:
             return "Er zijn meerdere habitatvoorstellen met kloppende mits/mozaiek. Er is geen duidelijke keuze te maken."
         elif self == KeuzeStatus.PLACEHOLDER:
-            return "Er zijn placeholder criteria gevonden; deze kunnen (nog) niet door Veg2Hab worden gecontroleerd."
-        elif self == KeuzeStatus.HANDMATIGE_CONTROLE:
-            assert (
-                False
-            ), "Bij KeuzeStatus.HANDMATIGE_CONTROLE moet nog een mooie toelichting, maar ik weet nu nog niet hoe of wat precies."
+            return "Er zijn placeholder mitsen/mozaiekregels gevonden; deze kunnen (nog) niet door Veg2Hab worden gecontroleerd."
+        # elif self == KeuzeStatus.HANDMATIGE_CONTROLE:
+        #     assert (
+        #         False
+        #     ), "Bij KeuzeStatus.HANDMATIGE_CONTROLE moet nog een mooie toelichting, maar ik weet nu nog niet hoe of wat precies, want deze KeuzeStatus is nog niet in gebruik."
         elif self == KeuzeStatus.WACHTEN_OP_MOZAIEK:
-            return "Veg2Hab kan nog geen mozaiekregels checken"
+            return "Er is te weinig informatie over de habitattypen van omliggende vlakken (teveel HXXXX)"
 
 
 class FGRType(Enum):
     DU = "Duinen"
     GG = "Getijdengebied"
     HL = "Heuvelland"
     HZ = "Hogere Zandgronden"
```

### Comparing `veg2hab-0.1.1/veg2hab/fgr.py` & `veg2hab-0.2.1/veg2hab/fgr.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/habitat.py` & `veg2hab-0.2.1/veg2hab/habitat.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import List, Optional, Tuple, Union
 
 from veg2hab.criteria import BeperkendCriterium, GeenCriterium
 from veg2hab.enums import KeuzeStatus, Kwaliteit, MatchLevel, MaybeBoolean
-from veg2hab.mozaiek import GeenMozaiekregel, MozaiekRegel
+from veg2hab.mozaiek import (
+    GeenMozaiekregel,
+    MozaiekRegel,
+    StandaardMozaiekregel,
+    is_mozaiek_type_present,
+)
 from veg2hab.vegetatietypen import SBB as _SBB
 from veg2hab.vegetatietypen import VvN as _VvN
 
 
 @dataclass
 class HabitatVoorstel:
     """
@@ -55,22 +60,22 @@
 
 
 @dataclass
 class HabitatKeuze:
     status: KeuzeStatus
     habtype: str  # format = "H1123"
     kwaliteit: Kwaliteit
-    zelfstandig: bool
-    opmerking: str
-    mits_opmerking: str
-    mozaiek_opmerking: str
-    debug_info: Optional[str]
     habitatvoorstellen: List[HabitatVoorstel]  # used as a refence
+    opmerking: str = ""
+    mits_opmerking: str = ""
+    mozaiek_opmerking: str = ""
+    debug_info: Optional[str] = ""
 
     def __post_init__(self):
+        # Validatie
         if self.status in [
             KeuzeStatus.DUIDELIJK,
         ]:
             assert self.habtype not in ["HXXXX", "H0000"]
         elif self.status in [
             KeuzeStatus.GEEN_KLOPPENDE_MITSEN,
             KeuzeStatus.VEGTYPEN_NIET_IN_DEFTABEL,
@@ -80,14 +85,39 @@
         elif self.status in [
             KeuzeStatus.WACHTEN_OP_MOZAIEK,
             KeuzeStatus.PLACEHOLDER,
             KeuzeStatus.MEERDERE_KLOPPENDE_MITSEN,
         ]:
             assert self.habtype == "HXXXX"
 
+        if self.habtype in ["H0000", "HXXXX"]:
+            assert self.kwaliteit == Kwaliteit.NVT
+
+    @classmethod
+    def habitatkeuze_for_postponed_mozaiekregel(
+        cls, habitatvoorstellen: List[HabitatVoorstel]
+    ):
+        return cls(
+            status=KeuzeStatus.WACHTEN_OP_MOZAIEK,
+            habtype="HXXXX",
+            kwaliteit=Kwaliteit.NVT,
+            opmerking="Er is een mozaiekregel waarvoor nog te weinig info is om een keuze te maken.",
+            habitatvoorstellen=habitatvoorstellen,
+            mits_opmerking="",
+            mozaiek_opmerking="",
+            debug_info="",
+        )
+
+    @property
+    def zelfstandig(self):
+        if self.habtype in ["H0000", "HXXXX"]:
+            return True
+
+        return is_mozaiek_type_present(self.habitatvoorstellen, GeenMozaiekregel)
+
 
 def rank_habitatkeuzes(
     keuze_en_vegtypeinfo: Tuple[HabitatKeuze, "VegTypeInfo"]
 ) -> tuple:
     """
     Returned een tuple voor het sorteren van een lijst habitatkeuzes + vegtypeinfos voor in de outputtabel
     We zetten eerst alle H0000 achteraan, daarna sorteren we op percentage, daarna op kwaliteit
@@ -132,33 +162,31 @@
         # ...zat of geen van de vegtypen in de deftabel
         if all_voorstellen[0].onderbouwend_vegtype:
             assert all_voorstellen[0].idx_in_dt is None
             return HabitatKeuze(
                 status=KeuzeStatus.VEGTYPEN_NIET_IN_DEFTABEL,
                 habtype="H0000",
                 kwaliteit=all_voorstellen[0].kwaliteit,
-                zelfstandig=True,
+                habitatvoorstellen=all_voorstellen,
                 opmerking="Geen van de opgegeven vegetatietypen is teruggevonden in de definitietabel.",
                 mits_opmerking="",
                 mozaiek_opmerking="",
                 debug_info="",
-                habitatvoorstellen=all_voorstellen,
             )
         # ...of zijn er geen vegetatietypen opgegeven voor dit vlak
         assert all_voorstellen[0].onderbouwend_vegtype is None
         return HabitatKeuze(
             status=KeuzeStatus.GEEN_OPGEGEVEN_VEGTYPEN,
             habtype="H0000",
             kwaliteit=all_voorstellen[0].kwaliteit,
-            zelfstandig=True,
+            habitatvoorstellen=all_voorstellen,
             opmerking="Er zijn geen vegetatietypen opgegeven voor dit vlak.",
             mits_opmerking="",
             mozaiek_opmerking="",
             debug_info="",
-            habitatvoorstellen=all_voorstellen,
         )
 
     sublisted_voorstellen = _sublist_per_match_level(all_voorstellen)
 
     # Per MatchLevel checken of er kloppende mitsen zijn
     for current_voorstellen in sublisted_voorstellen:
         truth_values_mits = [
@@ -183,76 +211,119 @@
             # ...is er 1 kloppende mits; Duidelijk
             if len(true_voorstellen) == 1:
                 voorstel = true_voorstellen[0]
                 return HabitatKeuze(
                     status=KeuzeStatus.DUIDELIJK,
                     habtype=voorstel.habtype,
                     kwaliteit=voorstel.kwaliteit,
-                    zelfstandig=True,
-                    opmerking=f"Er is een duidelijke keuze. Kloppende mits en kloppende mozaiek.",
-                    mits_opmerking=str(voorstel.mits),
-                    mozaiek_opmerking=str(voorstel.mozaiek),
-                    debug_info="",
                     habitatvoorstellen=[voorstel],
+                    opmerking=f"Er is een duidelijke keuze. Kloppende mits en kloppende mozaiek. Zie mits/mozk_opm voor meer info in format [opgegeven vegtype, potentieel habtype, mits/mozaiek]",
+                    mits_opmerking=f"Mits: {str(voorstel.mits)}, {str(voorstel.mits.evaluation)}",
+                    mozaiek_opmerking=f"Mozaiekregel: {str(voorstel.mozaiek)}, {str(voorstel.mozaiek.evaluation)}",
+                    debug_info="",
                 )
 
             # ...of zijn er meerdere kloppende mitsen; Alle info van de kloppende mitsen meegeven
             if len(true_voorstellen) > 1:
                 return HabitatKeuze(
                     status=KeuzeStatus.MEERDERE_KLOPPENDE_MITSEN,
                     habtype="HXXXX",
-                    kwaliteit=Kwaliteit.ONBEKEND,
-                    zelfstandig=True,
-                    opmerking=f"Er zijn meerdere habitatvoorstellen die aan hun mitsen/mozaieken voldoen; zie mits/mozk_opm voor meer info in format [opgegevenvegtype, potentieel habtype, mits/mozaiek]",
-                    mits_opmerking=f"Kloppende mitsen: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits)] for voorstel in true_voorstellen]}",
-                    mozaiek_opmerking=f"Kloppende mozaiekregels: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek)] for voorstel in true_voorstellen]}",
-                    debug_info="",
+                    kwaliteit=Kwaliteit.NVT,
                     habitatvoorstellen=true_voorstellen,
+                    opmerking=f"Er zijn meerdere habitatvoorstellen die aan hun mitsen/mozaieken voldoen; zie mits/mozk_opm voor meer info in format [opgegeven vegtype, potentieel habtype, mits/mozaiek]",
+                    mits_opmerking=f"Mitsen: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits), str(voorstel.mits.evaluation)] for voorstel in true_voorstellen]}",
+                    mozaiek_opmerking=f"Mozaiekregels: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek), str(voorstel.mozaiek.evaluation)] for voorstel in true_voorstellen]}",
+                    debug_info="",
                 )
 
             # ...of zijn er geen kloppende mitsen op het huidige match_level
             continue
 
         # Er is een niet-TRUE/FALSE truth value aanwezig. Dit kan of een CANNOT_BE_AUTOMATED zijn of een POSTPONE (of beide).
+        # We gaan eerst kijken of er een CANNOT_BE_AUTOMATED is, want dan kan de keuze in latere iteraties nog steeds niet gemaakt worden
 
         # Als er een CANNOT_BE_AUTOMATED is...
         if MaybeBoolean.CANNOT_BE_AUTOMATED in truth_values:
             # ...dan kunnen we voor de huidige voorstellen geen keuze maken
 
             # We weten wel dat habitatvoorstellen met een specifieker matchniveau dan die van
             # de current_voorstellen allemaal FALSE waren, dus die hoeven we niet terug te geven
+            # We filteren ook mits&mozaiek eruit die FALSE zijn; die hangen nm toch niet van een placeholder af.
             return_voorstellen = [
                 voorstel
                 for voorstel in all_voorstellen
                 if voorstel.match_level <= current_voorstellen[0].match_level
+                and (
+                    voorstel.mits.evaluation & voorstel.mozaiek.evaluation
+                    != MaybeBoolean.FALSE
+                )
             ]
 
             return HabitatKeuze(
                 status=KeuzeStatus.PLACEHOLDER,
                 habtype="HXXXX",
-                kwaliteit=Kwaliteit.ONBEKEND,
-                zelfstandig=True,
-                opmerking=f"Er zijn mitsen of mozaiekregels die nog niet geimplementeerde zijn. Zie mits/mozk_opm voor meer info in format [opgegevenvegtype, potentieel habtype, mits/mozaiek]",
-                mits_opmerking=f"Alle mitsen: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits)] for voorstel in all_voorstellen]}",
-                mozaiek_opmerking=f"Alle mozaiekregels: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek)] for voorstel in all_voorstellen]}",
-                debug_info="",
+                kwaliteit=Kwaliteit.NVT,
                 habitatvoorstellen=return_voorstellen,
+                opmerking=f"Er zijn mitsen of mozaiekregels die nog niet geimplementeerde zijn. Zie mits/mozk_opm voor meer info in format [opgegeven vegtype, potentieel habtype, mits/mozaiek]",
+                mits_opmerking=f"Mitsen: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits), str(voorstel.mits.evaluation)] for voorstel in return_voorstellen]}",
+                mozaiek_opmerking=f"Mozaiekregels: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek), str(voorstel.mozaiek.evaluation)] for voorstel in return_voorstellen]}",
+                debug_info="",
             )
 
         # Als er een POSTPONE is...
         if MaybeBoolean.POSTPONE in truth_values:
             # ...dan komt dat door een mozaiekregel waar nog te weinig info over omliggende vlakken voor is
-            # We returnen dan None, zodat we later nog een keer kunnen proberen.
-            return None
+
+            # We weten wel dat habitatvoorstellen met een specifieker matchniveau dan die van
+            # de current_voorstellen allemaal FALSE waren, dus die hoeven we niet terug te geven
+            # We filteren ook mits&mozaiek eruit die FALSE zijn; die hangen nm toch niet van een placeholder af.
+            return_voorstellen = [
+                voorstel
+                for voorstel in all_voorstellen
+                if voorstel.match_level <= current_voorstellen[0].match_level
+                and (
+                    voorstel.mits.evaluation & voorstel.mozaiek.evaluation
+                    != MaybeBoolean.FALSE
+                )
+            ]
+
+            # Deze keuze komt volgende iteratieronde terug
+            # Als de huidige iteratie de laatste is (bv omdat er geen voortang is gemaakt), dan komt deze keuze in de output terecht.
+            return HabitatKeuze(
+                status=KeuzeStatus.WACHTEN_OP_MOZAIEK,
+                habtype="HXXXX",
+                kwaliteit=Kwaliteit.NVT,
+                habitatvoorstellen=return_voorstellen,
+                opmerking="Dit vlak heeft mozaiekregels waarvoor nog te weinig info is om een keuze te maken. Dit gebeurt als het vlak omringd wordt door meer dan 90% HXXXX. Zie mits/mozk_opm voor meer info in format [opgegeven vegtype, potentieel habtype, mits/mozaiek]",
+                mits_opmerking=f"Mitsen: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits), str(voorstel.mits.evaluation)] for voorstel in return_voorstellen]}",
+                mozaiek_opmerking=f"Mozaiekregels: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek), str(voorstel.mozaiek.evaluation)] for voorstel in return_voorstellen]}",
+                debug_info="",
+            )
 
     # Er zijn geen kloppende mitsen gevonden;
     return HabitatKeuze(
         status=KeuzeStatus.GEEN_KLOPPENDE_MITSEN,
         habtype="H0000",
         kwaliteit=Kwaliteit.NVT,
-        zelfstandig=True,
-        opmerking=f"Er zijn geen habitatvoorstellen waarvan en de mitsen en de mozaiekregels kloppen. Zie mits/mozk_opm voor meer info in format [opgegevenvegtype, potentieel habtype, mits/mozaiek].",
-        mits_opmerking=f"Mitsen waaraan mogelijk niet is voldaan: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits)] for voorstel in all_voorstellen]}",
-        mozaiek_opmerking=f"Mozaiekregels waaraan mogelijk niet is voldaan: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek)] for voorstel in all_voorstellen]}",
-        debug_info="",
         habitatvoorstellen=all_voorstellen,
+        opmerking=f"Er zijn geen habitatvoorstellen waarvan zowel de mits als de mozaiekregel klopt. Zie mits/mozk_opm voor meer info in format [opgegeven vegtype, potentieel habtype, mits/mozaiek].",
+        mits_opmerking=f"Mitsen: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits), str(voorstel.mits.evaluation)] for voorstel in all_voorstellen]}",
+        mozaiek_opmerking=f"Mozaiekregels: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek), str(voorstel.mozaiek.evaluation)] for voorstel in all_voorstellen]}",
+        debug_info="",
+    )
+
+
+def calc_nr_of_unresolved_habitatkeuzes_per_row(gdf):
+    """
+    Telt het aantal nog niet gemaakte habitatkeuzes. Dit zijn None habkeuzes en
+    uitgestelde mozaiek-habitatkeuzes (die met status=KeuzeStatus.WACHTEN_OP_MOZAIEK per rij)
+    """
+    assert "HabitatKeuze" in gdf.columns, "HabitatKeuze kolom niet aanwezig in gdf"
+
+    return gdf.HabitatKeuze.apply(
+        lambda keuzes: sum(
+            [
+                (keuze is None or keuze.status == KeuzeStatus.WACHTEN_OP_MOZAIEK)
+                for keuze in keuzes
+            ]
+        )
     )
```

### Comparing `veg2hab-0.1.1/veg2hab/io/arcgis.py` & `veg2hab-0.2.1/veg2hab/io/arcgis.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/io/cli.py` & `veg2hab-0.2.1/veg2hab/io/cli.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/io/common.py` & `veg2hab-0.2.1/veg2hab/io/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,18 @@
         default="+",
         description='karakter waarop de vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa")) (wordt bij mutli_col gebruikt om de kolommen te scheiden)',
     )
     perc_col: Optional[str] = Field(
         default=None,
         description="kolomnaam van de percentage als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))",
     )
+    lok_vegtypen_col: Optional[str] = Field(
+        default=None,
+        description="kolomnaam van de lokale vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))",
+    )
 
 
 class Interface(metaclass=ABCMeta):
     """Singleton class that defines the interface for the different UI systems."""
 
     __instance = None
```

### Comparing `veg2hab-0.1.1/veg2hab/main.py` & `veg2hab-0.2.1/veg2hab/main.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/mozaiek.py` & `veg2hab-0.2.1/veg2hab/mozaiek.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         self._evaluation = MaybeBoolean.FALSE
 
     @property
     def evaluation(self) -> MaybeBoolean:
         return self._evaluation
 
     def __str__(self):
-        return f"{'Enkel zelfstandige vegetaties' if self.alleen_zelfstandig else 'Zowel zelfstandige als mozaiekvegetaties'} van {'goede' if self.alleen_goede_kwaliteit else 'goede en matige'} kwaliteit van {self.habtype}. Threshold: {self.mozaiek_threshold}. Geldig voor {self.keys}"
+        return f"{'zelfstndg' if self.alleen_zelfstandig else 'zelfstndg/mozk'} {'G' if self.alleen_goede_kwaliteit else 'G/M'} {self.habtype}."
 
 
 def make_buffered_boundary_overlay_gdf(
     gdf: gpd.GeoDataFrame,
     buffer: Number = 0.1,
 ) -> Union[None, gpd.GeoDataFrame]:
     """
@@ -294,14 +294,15 @@
     Geeft True als er in de lijst met habitatvoorstellen eentje met een mozaiekregel van mozaiek_type is
     NOTE: Op het moment wordt dit gebruikt om te kijken of er dummymozaiekregels zijn, en zo ja, dan wordt er HXXXX gegeven.
     NOTE: Zodra mozaiekregels geimplementeerd zijn, kan deze functie mogelijk weg
     """
     # Als we een lijst van lijsten hebben, dan flattenen we die
     if any(isinstance(i, list) for i in voorstellen):
         voorstellen = [item for sublist in voorstellen for item in sublist]
+
     return any(
         (
             voorstel.mozaiek.is_mozaiek_type_present(mozaiek_type)
             if voorstel.mozaiek is not None
             else False
         )
         for voorstel in voorstellen
```

### Comparing `veg2hab-0.1.1/veg2hab/package_data/FGR.json` & `veg2hab-0.2.1/veg2hab/package_data/FGR.json`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/package_data/toolbox.pyt` & `veg2hab-0.2.1/veg2hab/package_data/toolbox.pyt`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Type, Union
 
 import veg2hab.io.arcgis
 import veg2hab.main
 import veg2hab.constants
 import logging
 
-SUPPORTED_VERSIONS = ["0.1.0", "0.1.1"]
+SUPPORTED_VERSIONS = ["0.1.0", "0.1.1", "0.2.1"]
 
 # this instantiates the arcgis interface and configures the logging
 veg2hab.io.arcgis.ArcGISInterface.get_instance().instantiate_loggers()
 
 class Toolbox:
     def __init__(self):
         """Define the toolbox (the name of the toolbox is the name of the
```

### Comparing `veg2hab-0.1.1/veg2hab/validation.py` & `veg2hab-0.2.1/veg2hab/validation.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/vegetatietypen.py` & `veg2hab-0.2.1/veg2hab/vegetatietypen.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.1.1/veg2hab/vegkartering.py` & `veg2hab-0.2.1/veg2hab/vegkartering.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from veg2hab.access_db import read_access_tables
 from veg2hab.criteria import FGRCriterium, is_criteria_type_present
 from veg2hab.enums import KeuzeStatus, Kwaliteit
 from veg2hab.fgr import FGR
 from veg2hab.habitat import (
     HabitatVoorstel,
+    calc_nr_of_unresolved_habitatkeuzes_per_row,
     rank_habitatkeuzes,
     try_to_determine_habkeuze,
 )
 from veg2hab.mozaiek import (
     calc_mozaiek_percentages_from_overlay_gdf,
     make_buffered_boundary_overlay_gdf,
 )
@@ -276,17 +277,17 @@
             voorstel = keuze.habitatvoorstellen[0]
             series_dict = {
                 f"Habtype{idx}": keuze.habtype,
                 f"Perc{idx}": vegtypeinfo.percentage,
                 f"Opp{idx}": opp * vegtypeinfo.percentage,
                 f"Kwal{idx}": keuze.kwaliteit.as_letter(),
                 f"Opm{idx}": keuze.opmerking,
-                f"Mits_opm{idx}": keuze.mits_opmerking,
-                f"Mozk_opm{idx}": keuze.mozaiek_opmerking,
-                f"MozkDict{idx}": mozaiekregel_habtype_percentage_dict_to_string(
+                f"_Mits_opm{idx}": keuze.mits_opmerking,
+                f"_Mozk_opm{idx}": keuze.mozaiek_opmerking,
+                f"_MozkPerc{idx}": mozaiekregel_habtype_percentage_dict_to_string(
                     keuze.habitatvoorstellen[0].mozaiek_dict
                 ),
                 # f"Bron{idx}" TODO: Naam van de kartering, voegen we later toe
                 f"VvN{idx}": (
                     str(voorstel.onderbouwend_vegtype)
                     if isinstance(voorstel.onderbouwend_vegtype, _VvN)
                     else None
@@ -296,38 +297,41 @@
                     if isinstance(voorstel.onderbouwend_vegtype, _SBB)
                     else None
                 ),
                 # f"VEGlok{idx}" TODO: Doen we voor nu nog even niet
                 f"_Status{idx}": str(keuze.status),
                 f"_Uitleg{idx}": keuze.status.toelichting(),
                 f"_VvNdftbl{idx}": (
-                    str([str(voorstel.vegtype_in_dt), voorstel.idx_in_dt])
+                    str(
+                        [
+                            str(voorstel.vegtype_in_dt),
+                            voorstel.idx_in_dt,
+                            voorstel.habtype,
+                        ]
+                    )
                     if isinstance(voorstel.vegtype_in_dt, _VvN)
                     else None
                 ),
                 f"_SBBdftbl{idx}": (
-                    str([str(voorstel.vegtype_in_dt), voorstel.idx_in_dt])
+                    str(
+                        [
+                            str(voorstel.vegtype_in_dt),
+                            voorstel.idx_in_dt,
+                            voorstel.habtype,
+                        ]
+                    )
                     if isinstance(voorstel.vegtype_in_dt, _SBB)
                     else None
                 ),
                 # Als de status GEEN_OPGEGEVEN_VEGTYPEN is, dan willen we bij VgTypInf niks invullen
                 f"_VgTypInf{idx}": (
                     str(vegtypeinfo)
                     if keuze.status != KeuzeStatus.GEEN_OPGEGEVEN_VEGTYPEN
                     else None
                 ),
-                f"_ChkNodig{idx}": (
-                    True
-                    if keuze.status
-                    in [
-                        KeuzeStatus.PLACEHOLDER,
-                        KeuzeStatus.WACHTEN_OP_MOZAIEK,
-                    ]
-                    else False
-                ),
             }
 
             return pd.Series(series_dict)
 
         assert (
             False
         ), f"Er is 1 habitatkeuze maar KeuzeStatus {keuze.status} is niet DUIDELIJK, VEGTYPEN_NIET_IN_DEFTABEL of GEEN_KLOPPENDE_MITSEN"
@@ -348,17 +352,17 @@
             voorgestelde_hab_en_kwal = [voorgestelde_hab_en_kwal[0]]
         series_dict = {
             f"Habtype{idx}": keuze.habtype,
             f"Perc{idx}": str(vegtypeinfo.percentage),
             f"Opp{idx}": str(opp * vegtypeinfo.percentage),
             f"Kwal{idx}": keuze.kwaliteit.as_letter(),
             f"Opm{idx}": keuze.opmerking,
-            f"Mits_opm{idx}": keuze.mits_opmerking,
-            f"Mozk_opm{idx}": keuze.mozaiek_opmerking,
-            f"MozkDict{idx}": mozaiekregel_habtype_percentage_dict_to_string(
+            f"_Mits_opm{idx}": keuze.mits_opmerking,
+            f"_Mozk_opm{idx}": keuze.mozaiek_opmerking,
+            f"_MozkPerc{idx}": mozaiekregel_habtype_percentage_dict_to_string(
                 keuze.habitatvoorstellen[0].mozaiek_dict
             ),
             # f"Bron{idx}" TODO: Naam van de kartering, voegen we later toe
             f"VvN{idx}": str(
                 [
                     (
                         str(voorstel.onderbouwend_vegtype)
@@ -380,61 +384,53 @@
             ),
             # f"VEGlok{idx}" TODO: Doen we voor nu nog even niet
             f"_Status{idx}": str(keuze.status),
             f"_Uitleg{idx}": keuze.status.toelichting(),
             f"_VvNdftbl{idx}": str(
                 [
                     (
-                        str([str(voorstel.vegtype_in_dt), voorstel.idx_in_dt])
+                        str(
+                            [
+                                str(voorstel.vegtype_in_dt),
+                                voorstel.idx_in_dt,
+                                voorstel.habtype,
+                            ]
+                        )
                         if isinstance(voorstel.vegtype_in_dt, _VvN)
                         else None
                     )
                     for voorstel in voorstellen
                 ]
             ),
             f"_SBBdftbl{idx}": str(
                 [
                     (
-                        str([str(voorstel.vegtype_in_dt), voorstel.idx_in_dt])
+                        str(
+                            [
+                                str(voorstel.vegtype_in_dt),
+                                voorstel.idx_in_dt,
+                                voorstel.habtype,
+                            ]
+                        )
                         if isinstance(voorstel.vegtype_in_dt, _SBB)
                         else None
                     )
                     for voorstel in voorstellen
                 ]
             ),
             f"_VgTypInf{idx}": str(vegtypeinfo),
-            f"_ChkNodig{idx}": (
-                True
-                if keuze.status
-                in [
-                    KeuzeStatus.MEERDERE_KLOPPENDE_MITSEN,
-                    KeuzeStatus.PLACEHOLDER,
-                    KeuzeStatus.WACHTEN_OP_MOZAIEK,
-                ]
-                else False
-            ),
         }
 
         return pd.Series(series_dict)
 
     assert (
         False
     ), f"hab_as_final_form voor KeuzeStatus {keuze.status} is niet geimplementeerd"
 
 
-def bepaal_ChckNodig(row: gpd.GeoSeries) -> bool:
-    """
-    Bepaalt of een rij een habitattypekartering een handmatige controle nodig heeft
-    """
-    check_nodigs = [col for col in row.index if "_ChkNodig" in col]
-    if any(row[check_nodig] == True for check_nodig in check_nodigs):
-        return True
-    return False
-
-
 def build_aggregate_habtype_field(row: gpd.GeoSeries) -> str:
     """
     Maakt een samenvattende string van de habitattypen van een rij
     Hierbij worden de percentages van alle habtype/kwaliteit tuples bij elkaar
     Voorbeeld: 70% H1234 (G), 20% H0000, 10% HXXXX
     """
     habitatkeuzes = row["HabitatKeuze"]
@@ -491,37 +487,36 @@
     """
     new_columns = [
         "Area",
         "Opm",
         "Datum",
         "ElmID",
         "geometry",
-        "_ChkNodig",
         "_Samnvttng",
+        "_LokVegTyp",
         "_LokVrtNar",
     ]
     n_habtype_blocks = len([i for i in gdf.columns if "Habtype" in i])
     for i in range(1, n_habtype_blocks + 1):
         new_columns = new_columns + [
             f"Habtype{i}",
             f"Perc{i}",
             f"Opp{i}",
             f"Kwal{i}",
             f"Opm{i}",
-            f"Mits_opm{i}",
-            f"Mozk_opm{i}",
-            f"MozkDict{i}",
             f"VvN{i}",
             f"SBB{i}",
             f"_Status{i}",
             f"_Uitleg{i}",
+            f"_VgTypInf{i}",
+            f"_Mits_opm{i}",
+            f"_Mozk_opm{i}",
+            f"_MozkPerc{i}",
             f"_VvNdftbl{i}",
             f"_SBBdftbl{i}",
-            f"_VgTypInf{i}",
-            f"_ChkNodig{i}",
         ]
     return gdf[new_columns]
 
 
 def fix_crs(
     gdf: gpd.GeoDataFrame, shape_path: Path = "onbekende locatie"
 ) -> gpd.GeoDataFrame:
@@ -646,16 +641,16 @@
 
     @classmethod
     def from_access_db(
         cls,
         shape_path: Path,
         shape_elm_id_column: str,
         access_mdb_path: Path,
-        opmerkingen_column: Optional[str] = "Opmerking",
-        datum_column: Optional[str] = "Datum",
+        opmerkingen_column: Optional[str] = None,
+        datum_column: Optional[str] = None,
     ) -> Self:
         """
         Deze method wordt gebruikt om een Kartering te maken van een shapefile en
         een access database die al is opgedeeld in losse csv bestanden.
 
         # .shp shp_elm_id_column -> ElmID in Element.csv voor intern_id -> Locatie in KarteringVegetatietype.csv voor Vegetatietype ->
         #      -> Code in Vegetatietype.csv voor SbbType -> Cata_ID in SsbType.csv voor Code (hernoemd naar Sbb)
@@ -686,15 +681,15 @@
                 gdf[new_col] = None
             else:
                 gdf = gdf.rename(columns={old_col: new_col})
 
         gdf["Opp"] = gdf["geometry"].area
         gdf["_LokVrtNar"] = "Lokale typologie is primair vertaald naar SBB"
 
-        element, grouped_kart_veg = read_access_tables(access_mdb_path)
+        element, veginfo_per_locatie = read_access_tables(access_mdb_path)
 
         # Intern ID toevoegen aan de gdf
         try:
             gdf = gdf.merge(
                 element,
                 left_on=shape_elm_id_column,
                 right_on="ElmID",
@@ -711,15 +706,25 @@
             if not element.ElmID.is_unique:
                 dubbele_elmid = element.ElmID[element.ElmID.duplicated()].to_list()[:10]
                 message += f"Er zitten {len(dubbele_elmid)} dubbelingen in Element.csv, bijvoorbeeld ElmID: {dubbele_elmid[:10]}. "
             raise ValueError(message) from e
 
         # Joinen van de SBBs aan de gdf
         gdf = gdf.merge(
-            grouped_kart_veg, left_on="intern_id", right_on="Locatie", how="left"
+            veginfo_per_locatie[["Locatie", "VegTypeInfo"]],
+            left_on="intern_id",
+            right_on="Locatie",
+            how="left",
+        )
+
+        gdf = gdf.merge(
+            veginfo_per_locatie[["Locatie", "_LokVegTyp"]],
+            left_on="intern_id",
+            right_on="Locatie",
+            how="left",
         )
 
         # We laten alle NA vegtype-informatie vallen - dit kan komen door geometry die lijnen zijn in plaats van vormen,
         # maar ook aan ontbrekende waarden in een van de csv-bestanden.
         if gdf.VegTypeInfo.isnull().any():
             logging.warn(
                 f"Er zijn {gdf.VegTypeInfo.isnull().sum()} vlakken zonder VegTypeInfo in {shape_path}. Deze worden verwijderd."
@@ -740,39 +745,39 @@
         sbb_of_vvn: Literal["VvN", "SBB", "beide"],
         datum_col: Optional[str] = None,
         opmerking_col: Optional[str] = None,
         SBB_col: Optional[str] = None,
         VvN_col: Optional[str] = None,
         split_char: Optional[str] = "+",
         perc_col: Optional[str] = None,
+        lok_vegtypen_col: Optional[str] = None,
     ) -> Self:
         """
         Deze method wordt gebruikt om een Kartering te maken van een shapefile.
         Input:
         - shape_path: het pad naar de shapefile
         - ElmID_col: de kolomnaam van de ElementID in de Shapefile; uniek per vlak
         - vegtype_col_format: "single" als complexen in 1 kolom zitten of "multi" als er meerdere kolommen zijn
         - sbb_of_vvn: "VvN" als VvN de voorname vertaling is vanuit het lokale type, "SBB" voor SBB en "beide" als beide er zijn.
         - datum_col: kolomnaam van de datum als deze er is
         - opmerking_col: kolomnaam van de opmerking als deze er is
         - VvN_col: kolomnaam van de VvN vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
         - SBB_col: kolomnaam van de SBB vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
         - split_char: karakter waarop de vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa")) (wordt bij mutli_col gebruikt om de kolommen te scheiden)
-        - percentage_col: kolomnaam van de percentage als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))
+        - perc_col: kolomnaam van de percentage als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))
+        - lok_vegtypen_col: kolomnaam van de lokale vegetatietypen als deze er zijn (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
         """
 
         ###############
         ##### Valideren, opschonen en aanvullen van de shapefile
         ###############
 
         shapefile = gpd.read_file(shape_path)
 
         if ElmID_col and not shapefile[ElmID_col].is_unique:
-            # NOTE: Als we ElmID nooit door hoeven te voeren tot in de habitattypekartering kan deze ook helemaal
-            #       uit de spreadsheets gehaald worden; dan gebruiken we gewoon altijd onze eigen.
             warnings.warn(
                 f"""De kolom {ElmID_col} bevat niet-unieke waarden in {shape_path}.
                 Eerste paar dubbele waarden:
                 {
                     shapefile[ElmID_col][shapefile[ElmID_col].duplicated()].head().to_list()
                 }
                 Er worden nieuwe waarden voor {ElmID_col} gemaakt en vanaf nu gebruikt.
@@ -785,18 +790,32 @@
             ElmID_col = "ElmID"
             shapefile[ElmID_col] = range(len(shapefile))
 
         # Om niet bij splitten steeds "if split_char is not None:" te hoeven doen
         if split_char is None:
             split_char = "+"
 
+        # Vastleggen lokale vegtypen voor in de output
+        if lok_vegtypen_col is not None:
+            shapefile["_LokVegTyp"] = shapefile.apply(
+                lambda row: ", ".join(
+                    [str(row[col]) for col in lok_vegtypen_col.split(split_char)]
+                ),
+                axis=1,
+            )
+        else:
+            shapefile[
+                "_LokVegTyp"
+            ] = "Geen kolommen opgegeven voor lokale vegetatietypen"
+
         # Selectie van de te bewaren kolommen
         cols = [
             col for col in [datum_col, opmerking_col] if col in shapefile.columns
-        ] + [ElmID_col, "geometry"]
+        ] + [ElmID_col, "_LokVegTyp", "geometry"]
+
         # Uitvinden welke vegtype kolommen er mee moeten
         if vegtype_col_format == "multi":
             if SBB_col is not None:
                 SBB_col = SBB_col.split(split_char)
                 cols += SBB_col
             if VvN_col is not None:
                 VvN_col = VvN_col.split(split_char)
@@ -958,22 +977,14 @@
             mits_info_row = mits_info_df.loc[idx]
             for voorstellen in row.HabitatVoorstel:
                 for voorstel in voorstellen:
                     if voorstel.mits is None:
                         raise ValueError("Er is een habitatvoorstel zonder mits")
                     voorstel.mits.check(mits_info_row)
 
-        # NOTE: Kan weg zo als dit in bepaal_habtitatkeuzes gebeurt
-        # ### Habitatkeuzes bepalen
-        # self.gdf["HabitatKeuze"] = self.gdf["HabitatVoorstel"].apply(
-        #     lambda voorstellen: [
-        #         habitatkeuze_obv_mitsen(voorstel) for voorstel in voorstellen
-        #     ]
-        # )
-
     def bepaal_habitatkeuzes(self, fgr: FGR, max_iter: int = 20) -> None:
         """ """
         # We starten alle HabitatKeuzes op None, en dan vullen we ze steeds verder in
         self.gdf["HabitatKeuze"] = self.gdf.VegTypeInfo.apply(
             lambda voorstellen_list: [None for sublist in voorstellen_list]
         )
         self.gdf["finished_on_iteration"] = 0
@@ -983,16 +994,16 @@
 
         ### Verkrijgen overlay gdf
         # Hier staat in welke vlakken er voor hoeveel procent aan welke andere vlakken grenzen
         # Als er geen vlakken met mozaiekregels zijn of als deze vlakken allemaal nergens aan grenzen is overlayed None
         overlayed = make_buffered_boundary_overlay_gdf(self.gdf)
 
         for i in range(max_iter):
-            keuzes_still_to_determine_pre = self.gdf.HabitatKeuze.apply(
-                lambda keuzes: keuzes.count(None)
+            keuzes_still_to_determine_pre = calc_nr_of_unresolved_habitatkeuzes_per_row(
+                self.gdf
             )
             n_keuzes_still_to_determine_pre = keuzes_still_to_determine_pre.sum()
 
             #####
             # Mozaiekregels checken
             #####
             # We hoeven geen mozaiekdingen te doen als we geen vlakken met mozaiekregels hebben
@@ -1019,28 +1030,28 @@
 
                 # Deze info zetten we per ElmID om in een defaultdict
                 habtype_percentages = calc_mozaiek_percentages_from_overlay_gdf(
                     augmented_overlayed
                 )
 
                 # Met deze dicts kunnen we dan de mozaiekregels checken
-                self.check_mozaiekregels(habtype_percentages)
+                self._check_mozaiekregels(habtype_percentages)
 
             #####
             # Habitatkeuze proberen te bepalen per list habitatvoorstellen van een vegtypeingo
             #####
             self.gdf["HabitatKeuze"] = self.gdf.HabitatVoorstel.apply(
                 lambda voorstellen: [
                     try_to_determine_habkeuze(voorstel) for voorstel in voorstellen
                 ]
             )
 
-            n_keuzes_still_to_determine_post = self.gdf.HabitatKeuze.apply(
-                lambda keuzes: keuzes.count(None)
-            ).sum()
+            n_keuzes_still_to_determine_post = (
+                calc_nr_of_unresolved_habitatkeuzes_per_row(self.gdf).sum()
+            )
 
             print(
                 f"Iteratie {i}: van {n_keuzes_still_to_determine_pre} naar {n_keuzes_still_to_determine_post} keuzes nog te bepalen"
             )
 
             if (
                 n_keuzes_still_to_determine_pre == n_keuzes_still_to_determine_post
@@ -1052,29 +1063,44 @@
                 f"Maximaal aantal iteraties ({max_iter}) bereikt voor het bepalen van de habitatkeuzes."
             )
 
         # Of we hebben overal een keuze, of we komen niet verder met nog meer iteraties,
         # of we hebben max_iter bereikt
 
         if n_keuzes_still_to_determine_post > 0:
+            # NOTE
+            # NOTE: @reviewer Moet dit een warning zijn vind je? Of gewoon een print?
+            # NOTE: Het is iets wat niet alarmerend is maar wel nuttig om te weten.
+            # NOTE
             warnings.warn(
                 f"Er zijn nog {n_keuzes_still_to_determine_post} habitatkeuzes die niet bepaald konden worden."
             )
 
-    def check_mozaiekregels(self, habtype_percentages):
+        assert (
+            self.gdf.HabitatKeuze.apply(lambda keuzes: keuzes.count(None)).sum() == 0
+        ), "Er zijn nog habitatkeuzes die niet behandeld zijn en nog None zijn na bepaal_habitatkeuzes"
+
+    def _check_mozaiekregels(self, habtype_percentages):
         for row in self.gdf.itertuples():
             for idx, voorstel_list in enumerate(row.HabitatVoorstel):
                 # Als er geen habitatkeuzes zijn (want geen vegtypen opgegeven),
                 # dan hoeven we ook geen mozaiekregels te checken
                 if len(row.HabitatKeuze) == 0:
                     continue
 
-                # Als we voor deze voorstellen al een HabitatKeuze hebben hoeven we niet weer
-                # de mozaiekregels te checken
-                if row.HabitatKeuze[idx] is not None:
+                # Als we voor deze voorstellen al een HabitatKeuze hebben hoeven
+                # we niet weer de mozaiekregels te checken
+                # TODO: Nu check ik hier heel handmatig of de keuze gemaakt is, en dat moet op dezelfde manier als in
+                #       calc_nr_of_unresolved_habitatkeuzes_per_row gedaan worden :/
+                #       Na de demo moet dit even netten, een extra kolommetje in de gdf ofzo
+                #       Voor nu zijn er belangrijker dingen te doen :)
+                if (
+                    row.HabitatKeuze[idx] is not None
+                    and row.HabitatKeuze[idx].status != KeuzeStatus.WACHTEN_OP_MOZAIEK
+                ):
                     continue
 
                 percentages_dict = habtype_percentages[
                     habtype_percentages["ElmID"] == row.ElmID
                 ].dict
 
                 if len(percentages_dict) == 1:
@@ -1112,27 +1138,28 @@
                 "Opp",
                 "Opmerking",
                 "Datum",
                 "ElmID",
                 "geometry",
                 "VegTypeInfo",
                 "HabitatKeuze",
+                "_LokVegTyp",
                 "_LokVrtNar",
             ]
         ].copy()
 
         # Sorteer de keuzes eerst op niet-H0000-zijn, dan op percentage, dan op kwaliteit
         base = base.apply(sorteer_vegtypeinfos_habvoorstellen, axis=1)
 
         base = base.rename(columns={"Opp": "Area", "Opmerking": "Opm"})
 
         final = pd.concat([base, base.apply(self.row_to_final_format, axis=1)], axis=1)
-        final["_ChkNodig"] = final.apply(bepaal_ChckNodig, axis=1)
         final["_Samnvttng"] = final.apply(build_aggregate_habtype_field, axis=1)
         final = finalize_final_format(final)
+
         return final
 
     def row_to_final_format(self, row) -> pd.Series:
         """
         Maakt van een rij een dataseries met blokken kolommen volgens het Gegevens Leverings Protocol (Bijlage 3a)
         """
         keuzes = row["HabitatKeuze"]
```

### Comparing `veg2hab-0.1.1/veg2hab/waswordtlijst.py` & `veg2hab-0.2.1/veg2hab/waswordtlijst.py`

 * *Files identical despite different names*

