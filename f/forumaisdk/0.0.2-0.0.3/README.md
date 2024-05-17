# Comparing `tmp/forumaisdk-0.0.2.tar.gz` & `tmp/forumaisdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forumaisdk-0.0.2.tar", last modified: Thu Apr 18 16:51:06 2024, max compression
+gzip compressed data, was "forumaisdk-0.0.3.tar", last modified: Fri May 17 10:19:20 2024, max compression
```

## Comparing `forumaisdk-0.0.2.tar` & `forumaisdk-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/ModelMarketSDK/
--rw-r--r--   0 runner    (1001) docker     (127)   579187 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/LLMMarket.json
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/ModelMarket.py
--rw-r--r--   0 runner    (1001) docker     (127)   196960 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/USDC.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/forumaisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:19:20.538982 forumaisdk-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 10:19:12.000000 forumaisdk-0.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:19:20.534982 forumaisdk-0.0.3/ModelMarketSDK/
+-rw-r--r--   0 runner    (1001) docker     (127)   601393 2024-05-17 10:19:12.000000 forumaisdk-0.0.3/ModelMarketSDK/LLMMarket.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-05-17 10:19:12.000000 forumaisdk-0.0.3/ModelMarketSDK/ModelMarket.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193256 2024-05-17 10:19:12.000000 forumaisdk-0.0.3/ModelMarketSDK/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 10:19:12.000000 forumaisdk-0.0.3/ModelMarketSDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-17 10:19:20.538982 forumaisdk-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-17 10:19:12.000000 forumaisdk-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:19:20.538982 forumaisdk-0.0.3/forumaisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-17 10:19:20.000000 forumaisdk-0.0.3/forumaisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 10:19:20.000000 forumaisdk-0.0.3/forumaisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:19:20.000000 forumaisdk-0.0.3/forumaisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-17 10:19:20.000000 forumaisdk-0.0.3/forumaisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 10:19:20.000000 forumaisdk-0.0.3/forumaisdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-17 10:19:12.000000 forumaisdk-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:19:20.538982 forumaisdk-0.0.3/setup.cfg
```

### Comparing `forumaisdk-0.0.2/LICENSE` & `forumaisdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `forumaisdk-0.0.2/ModelMarketSDK/ModelMarket.py` & `forumaisdk-0.0.3/ModelMarketSDK/ModelMarket.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,24 +20,24 @@
         self.web3 = Web3(Web3.HTTPProvider(self.rpc))
         script_dir = os.path.dirname(__file__)  # Get the script's directory
         file_path = os.path.join(script_dir, "LLMMarket.json")
         f = open(file_path)
         data = json.load(f)
         f.close()
         abi = data["abi"]
-        self.llm_market = self.web3.eth.contract(address="0x4D26F6e4bb4dd9BC5f9E9Cb8714fFf324B57Dae9", abi=abi)
+        self.llm_market = self.web3.eth.contract(address="0x6b0934eeF1BeD7F3f53fE1E647096666286Df443", abi=abi)
         self.private_key = private_key
         self.public_key = public_key
         script_dir = os.path.dirname(__file__)  # Get the script's directory
         file_path = os.path.join(script_dir, "USDC.json")
         f = open(file_path)
         data = json.load(f)
         f.close()
         abi = data["abi"]
-        self.usdc = self.web3.eth.contract(address="0xFab79D18EcC2076369FD7e7391d5F8C1A98beb3c", abi=abi)
+        self.usdc = self.web3.eth.contract(address="0xC1e229808C9A2Dc675d1E415C03FaD1C41C92b2b", abi=abi)
         print("Initialized!")
 
     # returns all the nodes
     def get_hosts(self):
         return self.llm_market.functions.getHosts().call()
 
     # checks if a node is currently paused
@@ -46,15 +46,15 @@
 
     # returns the usd token balance of a given address
     def get_token_balance(self, address):
         return self.usdc.functions.balanceOf(address).call()
 
     # mints the usdc token (note: only a testnet functionality)
     def mint_token(self):
-        unsent_minting_tx = self.usdc.functions.mint().build_transaction({
+        unsent_minting_tx = self.usdc.functions.mint(5*(10**18)).build_transaction({
             "from": self.public_key,
             "nonce": self.web3.eth.get_transaction_count(self.public_key),
             "gasPrice": self.web3.eth.gas_price,
         })
         signed_tx = self.web3.eth.account.sign_transaction(unsent_minting_tx, private_key=self.private_key)
 
         tx_hash = self.web3.eth.send_raw_transaction(signed_tx.rawTransaction)
```

### Comparing `forumaisdk-0.0.2/ModelMarketSDK/USDC.json` & `forumaisdk-0.0.3/ModelMarketSDK/USDC.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7534672764278895%*

 * *Differences: {"'abi'": "{13: {'inputs': [OrderedDict([('internalType', 'uint256'), ('name', 'value'), ('type', "*

 * *          "'uint256')])]}}",*

 * * "'allSourcePaths'": "{'1': "*

 * *                     "'/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/ERC20.sol', "*

 * *                     "'2': "*

 * *                     "'/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/IERC20.sol', "*

 * *                     "'3': "*

 * *                     "'/home/c […]*

```diff
@@ -218,15 +218,21 @@
                     "type": "uint8"
                 }
             ],
             "stateMutability": "view",
             "type": "function"
         },
         {
-            "inputs": [],
+            "inputs": [
+                {
+                    "internalType": "uint256",
+                    "name": "value",
+                    "type": "uint256"
+                }
+            ],
             "name": "mint",
             "outputs": [],
             "stateMutability": "nonpayable",
             "type": "function"
         },
         {
             "inputs": [],
@@ -318,66 +324,66 @@
                 }
             ],
             "stateMutability": "nonpayable",
             "type": "function"
         }
     ],
     "allSourcePaths": {
-        "1": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/interfaces/draft-IERC6093.sol",
-        "2": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/ERC20.sol",
-        "3": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/IERC20.sol",
-        "4": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/extensions/IERC20Metadata.sol",
-        "5": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/utils/Context.sol",
-        "6": "contracts/ExampleUSDC.sol"
+        "0": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/interfaces/draft-IERC6093.sol",
+        "1": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/ERC20.sol",
+        "2": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/IERC20.sol",
+        "3": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/extensions/IERC20Metadata.sol",
+        "4": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/utils/Context.sol",
+        "5": "contracts/ExampleUSDC.sol"
     },
     "ast": {
         "absolutePath": "contracts/ExampleUSDC.sol",
         "exportedSymbols": {
             "ERC20": [
-                668
+                541
             ],
             "USDC": [
-                38
+                26
             ]
         },
-        "id": 39,
+        "id": 27,
         "nodeType": "SourceUnit",
         "nodes": [
             {
                 "id": 1,
                 "literals": [
                     "solidity",
                     ">=",
                     "0.8",
                     ".2",
                     "<",
                     "0.9",
                     ".0"
                 ],
                 "nodeType": "PragmaDirective",
-                "src": "0:31:6"
+                "src": "0:31:5"
             },
             {
                 "absolutePath": "/home/cedric/.brownie/packages/OpenZeppelin/openzeppelin-contracts@5.0.1/contracts/token/ERC20/ERC20.sol",
                 "file": "@openzeppelin/contracts/token/ERC20/ERC20.sol",
                 "id": 3,
                 "nameLocation": "-1:-1:-1",
                 "nodeType": "ImportDirective",
-                "scope": 39,
-                "sourceUnit": 669,
-                "src": "34:68:6",
+                "scope": 27,
+                "sourceUnit": 542,
+                "src": "34:68:5",
                 "symbolAliases": [
                     {
                         "foreign": {
                             "id": 2,
                             "name": "ERC20",
                             "nodeType": "Identifier",
                             "overloadedDeclarations": [],
-                            "referencedDeclaration": 668,
-                            "src": "42:5:6",
+                            "referencedDeclaration": 541,
+                            "src": "42:5:5",
                             "typeDescriptions": {}
                         },
                         "nameLocation": "-1:-1:-1"
                     }
                 ],
                 "unitAlias": ""
             },
@@ -385,47 +391,47 @@
                 "abstract": false,
                 "baseContracts": [
                     {
                         "baseName": {
                             "id": 4,
                             "name": "ERC20",
                             "nameLocations": [
-                                "121:5:6"
+                                "121:5:5"
                             ],
                             "nodeType": "IdentifierPath",
-                            "referencedDeclaration": 668,
-                            "src": "121:5:6"
+                            "referencedDeclaration": 541,
+                            "src": "121:5:5"
                         },
                         "id": 5,
                         "nodeType": "InheritanceSpecifier",
-                        "src": "121:5:6"
+                        "src": "121:5:5"
                     }
                 ],
                 "canonicalName": "USDC",
                 "contractDependencies": [],
                 "contractKind": "contract",
                 "fullyImplemented": true,
-                "id": 38,
+                "id": 26,
                 "linearizedBaseContracts": [
-                    38,
-                    668,
-                    714,
-                    913,
-                    887,
-                    943
+                    26,
+                    541,
+                    583,
+                    782,
+                    756,
+                    812
                 ],
                 "name": "USDC",
-                "nameLocation": "113:4:6",
+                "nameLocation": "113:4:5",
                 "nodeType": "ContractDefinition",
                 "nodes": [
                     {
                         "body": {
                             "id": 12,
                             "nodeType": "Block",
-                            "src": "170:2:6",
+                            "src": "170:2:5",
                             "statements": []
                         },
                         "id": 13,
                         "implemented": true,
                         "kind": "constructor",
                         "modifiers": [
                             {
@@ -435,15 +441,15 @@
                                         "id": 8,
                                         "isConstant": false,
                                         "isLValue": false,
                                         "isPure": true,
                                         "kind": "string",
                                         "lValueRequested": false,
                                         "nodeType": "Literal",
-                                        "src": "154:6:6",
+                                        "src": "154:6:5",
                                         "typeDescriptions": {
                                             "typeIdentifier": "t_stringliteral_d6aca1be9729c13d677335161321649cccae6a591554772516700f986f942eaa",
                                             "typeString": "literal_string \"USDC\""
                                         },
                                         "value": "USDC"
                                     },
                                     {
@@ -451,431 +457,278 @@
                                         "id": 9,
                                         "isConstant": false,
                                         "isLValue": false,
                                         "isPure": true,
                                         "kind": "string",
                                         "lValueRequested": false,
                                         "nodeType": "Literal",
-                                        "src": "162:6:6",
+                                        "src": "162:6:5",
                                         "typeDescriptions": {
                                             "typeIdentifier": "t_stringliteral_d6aca1be9729c13d677335161321649cccae6a591554772516700f986f942eaa",
                                             "typeString": "literal_string \"USDC\""
                                         },
                                         "value": "USDC"
                                     }
                                 ],
                                 "id": 10,
                                 "kind": "baseConstructorSpecifier",
                                 "modifierName": {
                                     "id": 7,
                                     "name": "ERC20",
                                     "nameLocations": [
-                                        "148:5:6"
+                                        "148:5:5"
                                     ],
                                     "nodeType": "IdentifierPath",
-                                    "referencedDeclaration": 668,
-                                    "src": "148:5:6"
+                                    "referencedDeclaration": 541,
+                                    "src": "148:5:5"
                                 },
                                 "nodeType": "ModifierInvocation",
-                                "src": "148:21:6"
+                                "src": "148:21:5"
                             }
                         ],
                         "name": "",
                         "nameLocation": "-1:-1:-1",
                         "nodeType": "FunctionDefinition",
                         "parameters": {
                             "id": 6,
                             "nodeType": "ParameterList",
                             "parameters": [],
-                            "src": "145:2:6"
+                            "src": "145:2:5"
                         },
                         "returnParameters": {
                             "id": 11,
                             "nodeType": "ParameterList",
                             "parameters": [],
-                            "src": "170:0:6"
+                            "src": "170:0:5"
                         },
-                        "scope": 38,
-                        "src": "134:38:6",
+                        "scope": 26,
+                        "src": "134:38:5",
                         "stateMutability": "nonpayable",
                         "virtual": false,
                         "visibility": "public"
                     },
                     {
                         "body": {
-                            "id": 27,
+                            "id": 24,
                             "nodeType": "Block",
-                            "src": "202:49:6",
+                            "src": "215:41:5",
                             "statements": [
                                 {
                                     "expression": {
                                         "arguments": [
                                             {
                                                 "expression": {
-                                                    "id": 17,
+                                                    "id": 19,
                                                     "name": "msg",
                                                     "nodeType": "Identifier",
                                                     "overloadedDeclarations": [],
                                                     "referencedDeclaration": -15,
-                                                    "src": "218:3:6",
+                                                    "src": "231:3:5",
                                                     "typeDescriptions": {
                                                         "typeIdentifier": "t_magic_message",
                                                         "typeString": "msg"
                                                     }
                                                 },
-                                                "id": 18,
+                                                "id": 20,
                                                 "isConstant": false,
                                                 "isLValue": false,
                                                 "isPure": false,
                                                 "lValueRequested": false,
-                                                "memberLocation": "222:6:6",
+                                                "memberLocation": "235:6:5",
                                                 "memberName": "sender",
                                                 "nodeType": "MemberAccess",
-                                                "src": "218:10:6",
+                                                "src": "231:10:5",
                                                 "typeDescriptions": {
                                                     "typeIdentifier": "t_address",
                                                     "typeString": "address"
                                                 }
                                             },
                                             {
-                                                "commonType": {
-                                                    "typeIdentifier": "t_rational_5000000_by_1",
-                                                    "typeString": "int_const 5000000"
-                                                },
-                                                "id": 24,
-                                                "isConstant": false,
-                                                "isLValue": false,
-                                                "isPure": true,
-                                                "lValueRequested": false,
-                                                "leftExpression": {
-                                                    "hexValue": "35",
-                                                    "id": 19,
-                                                    "isConstant": false,
-                                                    "isLValue": false,
-                                                    "isPure": true,
-                                                    "kind": "number",
-                                                    "lValueRequested": false,
-                                                    "nodeType": "Literal",
-                                                    "src": "230:1:6",
-                                                    "typeDescriptions": {
-                                                        "typeIdentifier": "t_rational_5_by_1",
-                                                        "typeString": "int_const 5"
-                                                    },
-                                                    "value": "5"
-                                                },
-                                                "nodeType": "BinaryOperation",
-                                                "operator": "*",
-                                                "rightExpression": {
-                                                    "components": [
-                                                        {
-                                                            "commonType": {
-                                                                "typeIdentifier": "t_rational_1000000_by_1",
-                                                                "typeString": "int_const 1000000"
-                                                            },
-                                                            "id": 22,
-                                                            "isConstant": false,
-                                                            "isLValue": false,
-                                                            "isPure": true,
-                                                            "lValueRequested": false,
-                                                            "leftExpression": {
-                                                                "hexValue": "3130",
-                                                                "id": 20,
-                                                                "isConstant": false,
-                                                                "isLValue": false,
-                                                                "isPure": true,
-                                                                "kind": "number",
-                                                                "lValueRequested": false,
-                                                                "nodeType": "Literal",
-                                                                "src": "235:2:6",
-                                                                "typeDescriptions": {
-                                                                    "typeIdentifier": "t_rational_10_by_1",
-                                                                    "typeString": "int_const 10"
-                                                                },
-                                                                "value": "10"
-                                                            },
-                                                            "nodeType": "BinaryOperation",
-                                                            "operator": "**",
-                                                            "rightExpression": {
-                                                                "hexValue": "36",
-                                                                "id": 21,
-                                                                "isConstant": false,
-                                                                "isLValue": false,
-                                                                "isPure": true,
-                                                                "kind": "number",
-                                                                "lValueRequested": false,
-                                                                "nodeType": "Literal",
-                                                                "src": "241:1:6",
-                                                                "typeDescriptions": {
-                                                                    "typeIdentifier": "t_rational_6_by_1",
-                                                                    "typeString": "int_const 6"
-                                                                },
-                                                                "value": "6"
-                                                            },
-                                                            "src": "235:7:6",
-                                                            "typeDescriptions": {
-                                                                "typeIdentifier": "t_rational_1000000_by_1",
-                                                                "typeString": "int_const 1000000"
-                                                            }
-                                                        }
-                                                    ],
-                                                    "id": 23,
-                                                    "isConstant": false,
-                                                    "isInlineArray": false,
-                                                    "isLValue": false,
-                                                    "isPure": true,
-                                                    "lValueRequested": false,
-                                                    "nodeType": "TupleExpression",
-                                                    "src": "234:9:6",
-                                                    "typeDescriptions": {
-                                                        "typeIdentifier": "t_rational_1000000_by_1",
-                                                        "typeString": "int_const 1000000"
-                                                    }
-                                                },
-                                                "src": "230:13:6",
+                                                "id": 21,
+                                                "name": "value",
+                                                "nodeType": "Identifier",
+                                                "overloadedDeclarations": [],
+                                                "referencedDeclaration": 15,
+                                                "src": "243:5:5",
                                                 "typeDescriptions": {
-                                                    "typeIdentifier": "t_rational_5000000_by_1",
-                                                    "typeString": "int_const 5000000"
+                                                    "typeIdentifier": "t_uint256",
+                                                    "typeString": "uint256"
                                                 }
                                             }
                                         ],
                                         "expression": {
                                             "argumentTypes": [
                                                 {
                                                     "typeIdentifier": "t_address",
                                                     "typeString": "address"
                                                 },
                                                 {
-                                                    "typeIdentifier": "t_rational_5000000_by_1",
-                                                    "typeString": "int_const 5000000"
+                                                    "typeIdentifier": "t_uint256",
+                                                    "typeString": "uint256"
                                                 }
                                             ],
-                                            "id": 16,
+                                            "id": 18,
                                             "name": "_mint",
                                             "nodeType": "Identifier",
                                             "overloadedDeclarations": [],
-                                            "referencedDeclaration": 508,
-                                            "src": "212:5:6",
+                                            "referencedDeclaration": 381,
+                                            "src": "225:5:5",
                                             "typeDescriptions": {
                                                 "typeIdentifier": "t_function_internal_nonpayable$_t_address_$_t_uint256_$returns$__$",
                                                 "typeString": "function (address,uint256)"
                                             }
                                         },
-                                        "id": 25,
+                                        "id": 22,
                                         "isConstant": false,
                                         "isLValue": false,
                                         "isPure": false,
                                         "kind": "functionCall",
                                         "lValueRequested": false,
                                         "nameLocations": [],
                                         "names": [],
                                         "nodeType": "FunctionCall",
-                                        "src": "212:32:6",
+                                        "src": "225:24:5",
                                         "tryCall": false,
                                         "typeDescriptions": {
                                             "typeIdentifier": "t_tuple$__$",
                                             "typeString": "tuple()"
                                         }
                                     },
-                                    "id": 26,
+                                    "id": 23,
                                     "nodeType": "ExpressionStatement",
-                                    "src": "212:32:6"
+                                    "src": "225:24:5"
                                 }
                             ]
                         },
-                        "functionSelector": "1249c58b",
-                        "id": 28,
+                        "functionSelector": "a0712d68",
+                        "id": 25,
                         "implemented": true,
                         "kind": "function",
                         "modifiers": [],
                         "name": "mint",
-                        "nameLocation": "187:4:6",
+                        "nameLocation": "187:4:5",
                         "nodeType": "FunctionDefinition",
                         "parameters": {
-                            "id": 14,
-                            "nodeType": "ParameterList",
-                            "parameters": [],
-                            "src": "191:2:6"
-                        },
-                        "returnParameters": {
-                            "id": 15,
-                            "nodeType": "ParameterList",
-                            "parameters": [],
-                            "src": "202:0:6"
-                        },
-                        "scope": 38,
-                        "src": "178:73:6",
-                        "stateMutability": "nonpayable",
-                        "virtual": false,
-                        "visibility": "external"
-                    },
-                    {
-                        "baseFunctions": [
-                            232
-                        ],
-                        "body": {
-                            "id": 36,
-                            "nodeType": "Block",
-                            "src": "314:25:6",
-                            "statements": [
-                                {
-                                    "expression": {
-                                        "hexValue": "36",
-                                        "id": 34,
-                                        "isConstant": false,
-                                        "isLValue": false,
-                                        "isPure": true,
-                                        "kind": "number",
-                                        "lValueRequested": false,
-                                        "nodeType": "Literal",
-                                        "src": "331:1:6",
-                                        "typeDescriptions": {
-                                            "typeIdentifier": "t_rational_6_by_1",
-                                            "typeString": "int_const 6"
-                                        },
-                                        "value": "6"
-                                    },
-                                    "functionReturnParameters": 33,
-                                    "id": 35,
-                                    "nodeType": "Return",
-                                    "src": "324:8:6"
-                                }
-                            ]
-                        },
-                        "functionSelector": "313ce567",
-                        "id": 37,
-                        "implemented": true,
-                        "kind": "function",
-                        "modifiers": [],
-                        "name": "decimals",
-                        "nameLocation": "266:8:6",
-                        "nodeType": "FunctionDefinition",
-                        "overrides": {
-                            "id": 30,
-                            "nodeType": "OverrideSpecifier",
-                            "overrides": [],
-                            "src": "289:8:6"
-                        },
-                        "parameters": {
-                            "id": 29,
-                            "nodeType": "ParameterList",
-                            "parameters": [],
-                            "src": "274:2:6"
-                        },
-                        "returnParameters": {
-                            "id": 33,
+                            "id": 16,
                             "nodeType": "ParameterList",
                             "parameters": [
                                 {
                                     "constant": false,
-                                    "id": 32,
+                                    "id": 15,
                                     "mutability": "mutable",
-                                    "name": "",
-                                    "nameLocation": "-1:-1:-1",
+                                    "name": "value",
+                                    "nameLocation": "200:5:5",
                                     "nodeType": "VariableDeclaration",
-                                    "scope": 37,
-                                    "src": "307:5:6",
+                                    "scope": 25,
+                                    "src": "192:13:5",
                                     "stateVariable": false,
                                     "storageLocation": "default",
                                     "typeDescriptions": {
-                                        "typeIdentifier": "t_uint8",
-                                        "typeString": "uint8"
+                                        "typeIdentifier": "t_uint256",
+                                        "typeString": "uint256"
                                     },
                                     "typeName": {
-                                        "id": 31,
-                                        "name": "uint8",
+                                        "id": 14,
+                                        "name": "uint256",
                                         "nodeType": "ElementaryTypeName",
-                                        "src": "307:5:6",
+                                        "src": "192:7:5",
                                         "typeDescriptions": {
-                                            "typeIdentifier": "t_uint8",
-                                            "typeString": "uint8"
+                                            "typeIdentifier": "t_uint256",
+                                            "typeString": "uint256"
                                         }
                                     },
                                     "visibility": "internal"
                                 }
                             ],
-                            "src": "306:7:6"
+                            "src": "191:15:5"
+                        },
+                        "returnParameters": {
+                            "id": 17,
+                            "nodeType": "ParameterList",
+                            "parameters": [],
+                            "src": "215:0:5"
                         },
-                        "scope": 38,
-                        "src": "257:82:6",
-                        "stateMutability": "view",
+                        "scope": 26,
+                        "src": "178:78:5",
+                        "stateMutability": "nonpayable",
                         "virtual": false,
-                        "visibility": "public"
+                        "visibility": "external"
                     }
                 ],
-                "scope": 39,
-                "src": "104:239:6",
+                "scope": 27,
+                "src": "104:156:5",
                 "usedErrors": [
-                    684,
-                    689,
-                    694,
-                    703,
-                    708,
-                    713
+                    553,
+                    558,
+                    563,
+                    572,
+                    577,
+                    582
                 ],
                 "usedEvents": [
-                    821,
-                    830
+                    690,
+                    699
                 ]
             }
         ],
-        "src": "0:343:6"
+        "src": "0:260:5"
     },
-    "bytecode": "608060405234801561001057600080fd5b506040805180820182526004808252635553444360e01b602080840182905284518086019095529184529083015290600361004b8382610101565b5060046100588282610101565b5050506101c0565b634e487b7160e01b600052604160045260246000fd5b600181811c9082168061008a57607f821691505b6020821081036100aa57634e487b7160e01b600052602260045260246000fd5b50919050565b601f8211156100fc576000816000526020600020601f850160051c810160208610156100d95750805b601f850160051c820191505b818110156100f8578281556001016100e5565b5050505b505050565b81516001600160401b0381111561011a5761011a610060565b61012e816101288454610076565b846100b0565b602080601f831160018114610163576000841561014b5750858301515b600019600386901b1c1916600185901b1785556100f8565b600085815260208120601f198616915b8281101561019257888601518255948401946001909101908401610173565b50858210156101b05787850151600019600388901b60f8161c191681555b5050505050600190811b01905550565b61077f806101cf6000396000f3fe608060405234801561001057600080fd5b506004361061009e5760003560e01c8063313ce56711610066578063313ce5671461011357806370a082311461012257806395d89b411461014b578063a9059cbb14610153578063dd62ed3e1461016657600080fd5b806306fdde03146100a3578063095ea7b3146100c15780631249c58b146100e457806318160ddd146100ee57806323b872dd14610100575b600080fd5b6100ab61019f565b6040516100b891906105c8565b60405180910390f35b6100d46100cf366004610633565b610231565b60405190151581526020016100b8565b6100ec61024b565b005b6002545b6040519081526020016100b8565b6100d461010e36600461065d565b61025a565b604051600681526020016100b8565b6100f2610130366004610699565b6001600160a01b031660009081526020819052604090205490565b6100ab61027e565b6100d4610161366004610633565b61028d565b6100f26101743660046106bb565b6001600160a01b03918216600090815260016020908152604080832093909416825291909152205490565b6060600380546101ae906106ee565b80601f01602080910402602001604051908101604052809291908181526020018280546101da906106ee565b80156102275780601f106101fc57610100808354040283529160200191610227565b820191906000526020600020905b81548152906001019060200180831161020a57829003601f168201915b5050505050905090565b60003361023f81858561029b565b60019150505b92915050565b61025833624c4b406102ad565b565b6000336102688582856102ec565b61027385858561036a565b506001949350505050565b6060600480546101ae906106ee565b60003361023f81858561036a565b6102a883838360016103c9565b505050565b6001600160a01b0382166102dc5760405163ec442f0560e01b8152600060048201526024015b60405180910390fd5b6102e86000838361049e565b5050565b6001600160a01b038381166000908152600160209081526040808320938616835292905220546000198114610364578181101561035557604051637dc7a0d960e11b81526001600160a01b038416600482015260248101829052604481018390526064016102d3565b610364848484840360006103c9565b50505050565b6001600160a01b03831661039457604051634b637e8f60e11b8152600060048201526024016102d3565b6001600160a01b0382166103be5760405163ec442f0560e01b8152600060048201526024016102d3565b6102a883838361049e565b6001600160a01b0384166103f35760405163e602df0560e01b8152600060048201526024016102d3565b6001600160a01b03831661041d57604051634a1406b160e11b8152600060048201526024016102d3565b6001600160a01b038085166000908152600160209081526040808320938716835292905220829055801561036457826001600160a01b0316846001600160a01b03167f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9258460405161049091815260200190565b60405180910390a350505050565b6001600160a01b0383166104c95780600260008282546104be9190610728565b9091555061053b9050565b6001600160a01b0383166000908152602081905260409020548181101561051c5760405163391434e360e21b81526001600160a01b038516600482015260248101829052604481018390526064016102d3565b6001600160a01b03841660009081526020819052604090209082900390555b6001600160a01b03821661055757600280548290039055610576565b6001600160a01b03821660009081526020819052604090208054820190555b816001600160a01b0316836001600160a01b03167fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef836040516105bb91815260200190565b60405180910390a3505050565b60006020808352835180602085015260005b818110156105f6578581018301518582016040015282016105da565b506000604082860101526040601f19601f8301168501019250505092915050565b80356001600160a01b038116811461062e57600080fd5b919050565b6000806040838503121561064657600080fd5b61064f83610617565b946020939093013593505050565b60008060006060848603121561067257600080fd5b61067b84610617565b925061068960208501610617565b9150604084013590509250925092565b6000602082840312156106ab57600080fd5b6106b482610617565b9392505050565b600080604083850312156106ce57600080fd5b6106d783610617565b91506106e560208401610617565b90509250929050565b600181811c9082168061070257607f821691505b60208210810361072257634e487b7160e01b600052602260045260246000fd5b50919050565b8082018082111561024557634e487b7160e01b600052601160045260246000fdfea26469706673582212207ce3bb5838214d8592b0d420a3f00611810814b9ad464f848b86e08d0e1bfa9364736f6c63430008170033",
-    "bytecodeSha1": "527a7012de694a55122f771eb497c163f3d67461",
+    "bytecode": "608060405234801561001057600080fd5b506040805180820182526004808252635553444360e01b602080840182905284518086019095529184529083015290600361004b8382610101565b5060046100588282610101565b5050506101c0565b634e487b7160e01b600052604160045260246000fd5b600181811c9082168061008a57607f821691505b6020821081036100aa57634e487b7160e01b600052602260045260246000fd5b50919050565b601f8211156100fc576000816000526020600020601f850160051c810160208610156100d95750805b601f850160051c820191505b818110156100f8578281556001016100e5565b5050505b505050565b81516001600160401b0381111561011a5761011a610060565b61012e816101288454610076565b846100b0565b602080601f831160018114610163576000841561014b5750858301515b600019600386901b1c1916600185901b1785556100f8565b600085815260208120601f198616915b8281101561019257888601518255948401946001909101908401610173565b50858210156101b05787850151600019600388901b60f8161c191681555b5050505050600190811b01905550565b6107a1806101cf6000396000f3fe608060405234801561001057600080fd5b506004361061009e5760003560e01c806370a082311161006657806370a082311461011857806395d89b4114610141578063a0712d6814610149578063a9059cbb1461015e578063dd62ed3e1461017157600080fd5b806306fdde03146100a3578063095ea7b3146100c157806318160ddd146100e457806323b872dd146100f6578063313ce56714610109575b600080fd5b6100ab6101aa565b6040516100b891906105d1565b60405180910390f35b6100d46100cf36600461063c565b61023c565b60405190151581526020016100b8565b6002545b6040519081526020016100b8565b6100d4610104366004610666565b610256565b604051601281526020016100b8565b6100e86101263660046106a2565b6001600160a01b031660009081526020819052604090205490565b6100ab61027a565b61015c6101573660046106c4565b610289565b005b6100d461016c36600461063c565b610296565b6100e861017f3660046106dd565b6001600160a01b03918216600090815260016020908152604080832093909416825291909152205490565b6060600380546101b990610710565b80601f01602080910402602001604051908101604052809291908181526020018280546101e590610710565b80156102325780601f1061020757610100808354040283529160200191610232565b820191906000526020600020905b81548152906001019060200180831161021557829003601f168201915b5050505050905090565b60003361024a8185856102a4565b60019150505b92915050565b6000336102648582856102b6565b61026f858585610339565b506001949350505050565b6060600480546101b990610710565b6102933382610398565b50565b60003361024a818585610339565b6102b183838360016103d2565b505050565b6001600160a01b038381166000908152600160209081526040808320938616835292905220546000198114610333578181101561032457604051637dc7a0d960e11b81526001600160a01b038416600482015260248101829052604481018390526064015b60405180910390fd5b610333848484840360006103d2565b50505050565b6001600160a01b03831661036357604051634b637e8f60e11b81526000600482015260240161031b565b6001600160a01b03821661038d5760405163ec442f0560e01b81526000600482015260240161031b565b6102b18383836104a7565b6001600160a01b0382166103c25760405163ec442f0560e01b81526000600482015260240161031b565b6103ce600083836104a7565b5050565b6001600160a01b0384166103fc5760405163e602df0560e01b81526000600482015260240161031b565b6001600160a01b03831661042657604051634a1406b160e11b81526000600482015260240161031b565b6001600160a01b038085166000908152600160209081526040808320938716835292905220829055801561033357826001600160a01b0316846001600160a01b03167f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9258460405161049991815260200190565b60405180910390a350505050565b6001600160a01b0383166104d25780600260008282546104c7919061074a565b909155506105449050565b6001600160a01b038316600090815260208190526040902054818110156105255760405163391434e360e21b81526001600160a01b0385166004820152602481018290526044810183905260640161031b565b6001600160a01b03841660009081526020819052604090209082900390555b6001600160a01b0382166105605760028054829003905561057f565b6001600160a01b03821660009081526020819052604090208054820190555b816001600160a01b0316836001600160a01b03167fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef836040516105c491815260200190565b60405180910390a3505050565b60006020808352835180602085015260005b818110156105ff578581018301518582016040015282016105e3565b506000604082860101526040601f19601f8301168501019250505092915050565b80356001600160a01b038116811461063757600080fd5b919050565b6000806040838503121561064f57600080fd5b61065883610620565b946020939093013593505050565b60008060006060848603121561067b57600080fd5b61068484610620565b925061069260208501610620565b9150604084013590509250925092565b6000602082840312156106b457600080fd5b6106bd82610620565b9392505050565b6000602082840312156106d657600080fd5b5035919050565b600080604083850312156106f057600080fd5b6106f983610620565b915061070760208401610620565b90509250929050565b600181811c9082168061072457607f821691505b60208210810361074457634e487b7160e01b600052602260045260246000fd5b50919050565b8082018082111561025057634e487b7160e01b600052601160045260246000fdfea26469706673582212209ca60becb493221a7cad525a9cc53486e7d32e693890081d97fcdb7c653cc0b164736f6c63430008170033",
+    "bytecodeSha1": "0d77bcd4ddf8967bc886f5cc4c6d0ac93dd30c77",
     "compiler": {
         "evm_version": "istanbul",
         "optimizer": {
             "enabled": true,
             "runs": 200
         },
         "version": "0.8.23+commit.f704f362"
     },
     "contractName": "USDC",
     "coverageMap": {
         "branches": {
-            "1": {},
-            "2": {
+            "0": {},
+            "1": {
                 "ERC20._approve": {
                     "37": [
                         10061,
                         10080,
                         false
                     ],
                     "38": [
                         10159,
                         10180,
                         false
                     ]
                 },
                 "ERC20._mint": {
-                    "32": [
+                    "36": [
                         7791,
                         7812,
                         false
                     ]
                 },
                 "ERC20._spendAllowance": {
-                    "33": [
+                    "32": [
                         10828,
                         10865,
                         false
                     ],
-                    "34": [
+                    "33": [
                         10885,
                         10909,
                         false
                     ]
                 },
                 "ERC20._transfer": {
-                    "35": [
+                    "34": [
                         5739,
                         5757,
                         false
                     ],
-                    "36": [
+                    "35": [
                         5834,
                         5850,
                         false
                     ]
                 },
                 "ERC20._update": {
                     "39": [
@@ -891,22 +744,22 @@
                     "41": [
                         6910,
                         6926,
                         false
                     ]
                 }
             },
+            "2": {},
             "3": {},
             "4": {},
-            "5": {},
-            "6": {}
+            "5": {}
         },
         "statements": {
-            "1": {},
-            "2": {
+            "0": {},
+            "1": {
                 "ERC20._approve": {
                     "14": [
                         9073,
                         9110
                     ],
                     "22": [
                         10057,
@@ -922,43 +775,43 @@
                     ],
                     "25": [
                         10328,
                         10364
                     ]
                 },
                 "ERC20._mint": {
-                    "15": [
+                    "20": [
                         7787,
                         7878
                     ],
-                    "16": [
+                    "21": [
                         7887,
                         7922
                     ]
                 },
                 "ERC20._spendAllowance": {
-                    "17": [
+                    "15": [
                         10881,
                         11011
                     ],
-                    "18": [
+                    "16": [
                         11052,
                         11109
                     ]
                 },
                 "ERC20._transfer": {
-                    "19": [
+                    "17": [
                         5735,
                         5821
                     ],
-                    "20": [
+                    "18": [
                         5830,
                         5916
                     ],
-                    "21": [
+                    "19": [
                         5925,
                         5949
                     ]
                 },
                 "ERC20._update": {
                     "26": [
                         6496,
@@ -1003,22 +856,28 @@
                 },
                 "ERC20.balanceOf": {
                     "2": [
                         3383,
                         3408
                     ]
                 },
+                "ERC20.decimals": {
+                    "1": [
+                        3068,
+                        3077
+                    ]
+                },
                 "ERC20.name": {
                     "4": [
                         2144,
                         2156
                     ]
                 },
                 "ERC20.symbol": {
-                    "12": [
+                    "11": [
                         2348,
                         2362
                     ]
                 },
                 "ERC20.totalSupply": {
                     "0": [
                         3215,
@@ -1029,62 +888,56 @@
                     "13": [
                         3733,
                         3760
                     ]
                 },
                 "ERC20.transferFrom": {
                     "10": [
-                        5229,
-                        5255
-                    ],
-                    "11": [
                         5265,
                         5276
                     ],
-                    "9": [
+                    "8": [
                         5182,
                         5219
+                    ],
+                    "9": [
+                        5229,
+                        5255
                     ]
                 }
             },
+            "2": {},
             "3": {},
-            "4": {},
-            "5": {
+            "4": {
                 "Context._msgSender": {
                     "5": [
                         728,
                         745
                     ]
                 }
             },
-            "6": {
-                "USDC.decimals": {
-                    "1": [
-                        324,
-                        332
-                    ]
-                },
+            "5": {
                 "USDC.mint": {
-                    "8": [
-                        212,
-                        244
+                    "12": [
+                        225,
+                        249
                     ]
                 }
             }
         }
     },
     "dependencies": [
         "OpenZeppelin/openzeppelin-contracts@5.0.1/Context",
         "OpenZeppelin/openzeppelin-contracts@5.0.1/ERC20",
         "OpenZeppelin/openzeppelin-contracts@5.0.1/IERC20",
         "OpenZeppelin/openzeppelin-contracts@5.0.1/IERC20Errors",
         "OpenZeppelin/openzeppelin-contracts@5.0.1/IERC20Metadata"
     ],
-    "deployedBytecode": "608060405234801561001057600080fd5b506004361061009e5760003560e01c8063313ce56711610066578063313ce5671461011357806370a082311461012257806395d89b411461014b578063a9059cbb14610153578063dd62ed3e1461016657600080fd5b806306fdde03146100a3578063095ea7b3146100c15780631249c58b146100e457806318160ddd146100ee57806323b872dd14610100575b600080fd5b6100ab61019f565b6040516100b891906105c8565b60405180910390f35b6100d46100cf366004610633565b610231565b60405190151581526020016100b8565b6100ec61024b565b005b6002545b6040519081526020016100b8565b6100d461010e36600461065d565b61025a565b604051600681526020016100b8565b6100f2610130366004610699565b6001600160a01b031660009081526020819052604090205490565b6100ab61027e565b6100d4610161366004610633565b61028d565b6100f26101743660046106bb565b6001600160a01b03918216600090815260016020908152604080832093909416825291909152205490565b6060600380546101ae906106ee565b80601f01602080910402602001604051908101604052809291908181526020018280546101da906106ee565b80156102275780601f106101fc57610100808354040283529160200191610227565b820191906000526020600020905b81548152906001019060200180831161020a57829003601f168201915b5050505050905090565b60003361023f81858561029b565b60019150505b92915050565b61025833624c4b406102ad565b565b6000336102688582856102ec565b61027385858561036a565b506001949350505050565b6060600480546101ae906106ee565b60003361023f81858561036a565b6102a883838360016103c9565b505050565b6001600160a01b0382166102dc5760405163ec442f0560e01b8152600060048201526024015b60405180910390fd5b6102e86000838361049e565b5050565b6001600160a01b038381166000908152600160209081526040808320938616835292905220546000198114610364578181101561035557604051637dc7a0d960e11b81526001600160a01b038416600482015260248101829052604481018390526064016102d3565b610364848484840360006103c9565b50505050565b6001600160a01b03831661039457604051634b637e8f60e11b8152600060048201526024016102d3565b6001600160a01b0382166103be5760405163ec442f0560e01b8152600060048201526024016102d3565b6102a883838361049e565b6001600160a01b0384166103f35760405163e602df0560e01b8152600060048201526024016102d3565b6001600160a01b03831661041d57604051634a1406b160e11b8152600060048201526024016102d3565b6001600160a01b038085166000908152600160209081526040808320938716835292905220829055801561036457826001600160a01b0316846001600160a01b03167f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9258460405161049091815260200190565b60405180910390a350505050565b6001600160a01b0383166104c95780600260008282546104be9190610728565b9091555061053b9050565b6001600160a01b0383166000908152602081905260409020548181101561051c5760405163391434e360e21b81526001600160a01b038516600482015260248101829052604481018390526064016102d3565b6001600160a01b03841660009081526020819052604090209082900390555b6001600160a01b03821661055757600280548290039055610576565b6001600160a01b03821660009081526020819052604090208054820190555b816001600160a01b0316836001600160a01b03167fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef836040516105bb91815260200190565b60405180910390a3505050565b60006020808352835180602085015260005b818110156105f6578581018301518582016040015282016105da565b506000604082860101526040601f19601f8301168501019250505092915050565b80356001600160a01b038116811461062e57600080fd5b919050565b6000806040838503121561064657600080fd5b61064f83610617565b946020939093013593505050565b60008060006060848603121561067257600080fd5b61067b84610617565b925061068960208501610617565b9150604084013590509250925092565b6000602082840312156106ab57600080fd5b6106b482610617565b9392505050565b600080604083850312156106ce57600080fd5b6106d783610617565b91506106e560208401610617565b90509250929050565b600181811c9082168061070257607f821691505b60208210810361072257634e487b7160e01b600052602260045260246000fd5b50919050565b8082018082111561024557634e487b7160e01b600052601160045260246000fdfea26469706673582212207ce3bb5838214d8592b0d420a3f00611810814b9ad464f848b86e08d0e1bfa9364736f6c63430008170033",
-    "deployedSourceMap": "104:239:6:-:0;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;2074:89:2;;;:::i;:::-;;;;;;;:::i;:::-;;;;;;;;4293:186;;;;;;:::i;:::-;;:::i;:::-;;;1169:14:8;;1162:22;1144:41;;1132:2;1117:18;4293:186:2;1004:187:8;178:73:6;;;:::i;:::-;;3144:97:2;3222:12;;3144:97;;;1342:25:8;;;1330:2;1315:18;3144:97:2;1196:177:8;5039:244:2;;;;;;:::i;:::-;;:::i;257:82:6:-;;;331:1;1853:36:8;;1841:2;1826:18;257:82:6;1711:184:8;3299:116:2;;;;;;:::i;:::-;-1:-1:-1;;;;;3390:18:2;3364:7;3390:18;;;;;;;;;;;;3299:116;2276:93;;;:::i;3610:178::-;;;;;;:::i;:::-;;:::i;3846:140::-;;;;;;:::i;:::-;-1:-1:-1;;;;;3952:18:2;;;3926:7;3952:18;;;:11;:18;;;;;;;;:27;;;;;;;;;;;;;3846:140;2074:89;2119:13;2151:5;2144:12;;;;;:::i;:::-;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;:::i;:::-;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;2074:89;:::o;4293:186::-;4366:4;735:10:5;4420:31:2;735:10:5;4436:7:2;4445:5;4420:8;:31::i;:::-;4468:4;4461:11;;;4293:186;;;;;:::o;178:73:6:-;212:32;218:10;230:13;212:5;:32::i;:::-;178:73::o;5039:244:2:-;5126:4;735:10:5;5182:37:2;5198:4;735:10:5;5213:5:2;5182:15;:37::i;:::-;5229:26;5239:4;5245:2;5249:5;5229:9;:26::i;:::-;-1:-1:-1;5272:4:2;;5039:244;-1:-1:-1;;;;5039:244:2:o;2276:93::-;2323:13;2355:7;2348:14;;;;;:::i;3610:178::-;3679:4;735:10:5;3733:27:2;735:10:5;3750:2:2;3754:5;3733:9;:27::i;8989:128::-;9073:37;9082:5;9089:7;9098:5;9105:4;9073:8;:37::i;:::-;8989:128;;;:::o;7721:208::-;-1:-1:-1;;;;;7791:21:2;;7787:91;;7835:32;;-1:-1:-1;;;7835:32:2;;7864:1;7835:32;;;2887:51:8;2860:18;;7835:32:2;;;;;;;;7787:91;7887:35;7903:1;7907:7;7916:5;7887:7;:35::i;:::-;7721:208;;:::o;10663:477::-;-1:-1:-1;;;;;3952:18:2;;;10762:24;3952:18;;;:11;:18;;;;;;;;:27;;;;;;;;;;-1:-1:-1;;10828:37:2;;10824:310;;10904:5;10885:16;:24;10881:130;;;10936:60;;-1:-1:-1;;;10936:60:2;;-1:-1:-1;;;;;3169:32:8;;10936:60:2;;;3151:51:8;3218:18;;;3211:34;;;3261:18;;;3254:34;;;3124:18;;10936:60:2;2949:345:8;10881:130:2;11052:57;11061:5;11068:7;11096:5;11077:16;:24;11103:5;11052:8;:57::i;:::-;10752:388;10663:477;;;:::o;5656:300::-;-1:-1:-1;;;;;5739:18:2;;5735:86;;5780:30;;-1:-1:-1;;;5780:30:2;;5807:1;5780:30;;;2887:51:8;2860:18;;5780:30:2;2741:203:8;5735:86:2;-1:-1:-1;;;;;5834:16:2;;5830:86;;5873:32;;-1:-1:-1;;;5873:32:2;;5902:1;5873:32;;;2887:51:8;2860:18;;5873:32:2;2741:203:8;5830:86:2;5925:24;5933:4;5939:2;5943:5;5925:7;:24::i;9949:432::-;-1:-1:-1;;;;;10061:19:2;;10057:89;;10103:32;;-1:-1:-1;;;10103:32:2;;10132:1;10103:32;;;2887:51:8;2860:18;;10103:32:2;2741:203:8;10057:89:2;-1:-1:-1;;;;;10159:21:2;;10155:90;;10203:31;;-1:-1:-1;;;10203:31:2;;10231:1;10203:31;;;2887:51:8;2860:18;;10203:31:2;2741:203:8;10155:90:2;-1:-1:-1;;;;;10254:18:2;;;;;;;:11;:18;;;;;;;;:27;;;;;;;;;:35;;;10299:76;;;;10349:7;-1:-1:-1;;;;;10333:31:2;10342:5;-1:-1:-1;;;;;10333:31:2;;10358:5;10333:31;;;;1342:25:8;;1330:2;1315:18;;1196:177;10333:31:2;;;;;;;;9949:432;;;;:::o;6271:1107::-;-1:-1:-1;;;;;6360:18:2;;6356:540;;6512:5;6496:12;;:21;;;;;;;:::i;:::-;;;;-1:-1:-1;6356:540:2;;-1:-1:-1;6356:540:2;;-1:-1:-1;;;;;6570:15:2;;6548:19;6570:15;;;;;;;;;;;6603:19;;;6599:115;;;6649:50;;-1:-1:-1;;;6649:50:2;;-1:-1:-1;;;;;3169:32:8;;6649:50:2;;;3151:51:8;3218:18;;;3211:34;;;3261:18;;;3254:34;;;3124:18;;6649:50:2;2949:345:8;6599:115:2;-1:-1:-1;;;;;6834:15:2;;:9;:15;;;;;;;;;;6852:19;;;;6834:37;;6356:540;-1:-1:-1;;;;;6910:16:2;;6906:425;;7073:12;:21;;;;;;;6906:425;;;-1:-1:-1;;;;;7284:13:2;;:9;:13;;;;;;;;;;:22;;;;;;6906:425;7361:2;-1:-1:-1;;;;;7346:25:2;7355:4;-1:-1:-1;;;;;7346:25:2;;7365:5;7346:25;;;;1342::8;;1330:2;1315:18;;1196:177;7346:25:2;;;;;;;;6271:1107;;;:::o;14:548:8:-;126:4;155:2;184;173:9;166:21;216:6;210:13;259:6;254:2;243:9;239:18;232:34;284:1;294:140;308:6;305:1;302:13;294:140;;;403:14;;;399:23;;393:30;369:17;;;388:2;365:26;358:66;323:10;;294:140;;;298:3;483:1;478:2;469:6;458:9;454:22;450:31;443:42;553:2;546;542:7;537:2;529:6;525:15;521:29;510:9;506:45;502:54;494:62;;;;14:548;;;;:::o;567:173::-;635:20;;-1:-1:-1;;;;;684:31:8;;674:42;;664:70;;730:1;727;720:12;664:70;567:173;;;:::o;745:254::-;813:6;821;874:2;862:9;853:7;849:23;845:32;842:52;;;890:1;887;880:12;842:52;913:29;932:9;913:29;:::i;:::-;903:39;989:2;974:18;;;;961:32;;-1:-1:-1;;;745:254:8:o;1378:328::-;1455:6;1463;1471;1524:2;1512:9;1503:7;1499:23;1495:32;1492:52;;;1540:1;1537;1530:12;1492:52;1563:29;1582:9;1563:29;:::i;:::-;1553:39;;1611:38;1645:2;1634:9;1630:18;1611:38;:::i;:::-;1601:48;;1696:2;1685:9;1681:18;1668:32;1658:42;;1378:328;;;;;:::o;1900:186::-;1959:6;2012:2;2000:9;1991:7;1987:23;1983:32;1980:52;;;2028:1;2025;2018:12;1980:52;2051:29;2070:9;2051:29;:::i;:::-;2041:39;1900:186;-1:-1:-1;;;1900:186:8:o;2091:260::-;2159:6;2167;2220:2;2208:9;2199:7;2195:23;2191:32;2188:52;;;2236:1;2233;2226:12;2188:52;2259:29;2278:9;2259:29;:::i;:::-;2249:39;;2307:38;2341:2;2330:9;2326:18;2307:38;:::i;:::-;2297:48;;2091:260;;;;;:::o;2356:380::-;2435:1;2431:12;;;;2478;;;2499:61;;2553:4;2545:6;2541:17;2531:27;;2499:61;2606:2;2598:6;2595:14;2575:18;2572:38;2569:161;;2652:10;2647:3;2643:20;2640:1;2633:31;2687:4;2684:1;2677:15;2715:4;2712:1;2705:15;2569:161;;2356:380;;;:::o;3299:222::-;3364:9;;;3385:10;;;3382:133;;;3437:10;3432:3;3428:20;3425:1;3418:31;3472:4;3469:1;3462:15;3500:4;3497:1;3490:15",
+    "deployedBytecode": "608060405234801561001057600080fd5b506004361061009e5760003560e01c806370a082311161006657806370a082311461011857806395d89b4114610141578063a0712d6814610149578063a9059cbb1461015e578063dd62ed3e1461017157600080fd5b806306fdde03146100a3578063095ea7b3146100c157806318160ddd146100e457806323b872dd146100f6578063313ce56714610109575b600080fd5b6100ab6101aa565b6040516100b891906105d1565b60405180910390f35b6100d46100cf36600461063c565b61023c565b60405190151581526020016100b8565b6002545b6040519081526020016100b8565b6100d4610104366004610666565b610256565b604051601281526020016100b8565b6100e86101263660046106a2565b6001600160a01b031660009081526020819052604090205490565b6100ab61027a565b61015c6101573660046106c4565b610289565b005b6100d461016c36600461063c565b610296565b6100e861017f3660046106dd565b6001600160a01b03918216600090815260016020908152604080832093909416825291909152205490565b6060600380546101b990610710565b80601f01602080910402602001604051908101604052809291908181526020018280546101e590610710565b80156102325780601f1061020757610100808354040283529160200191610232565b820191906000526020600020905b81548152906001019060200180831161021557829003601f168201915b5050505050905090565b60003361024a8185856102a4565b60019150505b92915050565b6000336102648582856102b6565b61026f858585610339565b506001949350505050565b6060600480546101b990610710565b6102933382610398565b50565b60003361024a818585610339565b6102b183838360016103d2565b505050565b6001600160a01b038381166000908152600160209081526040808320938616835292905220546000198114610333578181101561032457604051637dc7a0d960e11b81526001600160a01b038416600482015260248101829052604481018390526064015b60405180910390fd5b610333848484840360006103d2565b50505050565b6001600160a01b03831661036357604051634b637e8f60e11b81526000600482015260240161031b565b6001600160a01b03821661038d5760405163ec442f0560e01b81526000600482015260240161031b565b6102b18383836104a7565b6001600160a01b0382166103c25760405163ec442f0560e01b81526000600482015260240161031b565b6103ce600083836104a7565b5050565b6001600160a01b0384166103fc5760405163e602df0560e01b81526000600482015260240161031b565b6001600160a01b03831661042657604051634a1406b160e11b81526000600482015260240161031b565b6001600160a01b038085166000908152600160209081526040808320938716835292905220829055801561033357826001600160a01b0316846001600160a01b03167f8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b9258460405161049991815260200190565b60405180910390a350505050565b6001600160a01b0383166104d25780600260008282546104c7919061074a565b909155506105449050565b6001600160a01b038316600090815260208190526040902054818110156105255760405163391434e360e21b81526001600160a01b0385166004820152602481018290526044810183905260640161031b565b6001600160a01b03841660009081526020819052604090209082900390555b6001600160a01b0382166105605760028054829003905561057f565b6001600160a01b03821660009081526020819052604090208054820190555b816001600160a01b0316836001600160a01b03167fddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef836040516105c491815260200190565b60405180910390a3505050565b60006020808352835180602085015260005b818110156105ff578581018301518582016040015282016105e3565b506000604082860101526040601f19601f8301168501019250505092915050565b80356001600160a01b038116811461063757600080fd5b919050565b6000806040838503121561064f57600080fd5b61065883610620565b946020939093013593505050565b60008060006060848603121561067b57600080fd5b61068484610620565b925061069260208501610620565b9150604084013590509250925092565b6000602082840312156106b457600080fd5b6106bd82610620565b9392505050565b6000602082840312156106d657600080fd5b5035919050565b600080604083850312156106f057600080fd5b6106f983610620565b915061070760208401610620565b90509250929050565b600181811c9082168061072457607f821691505b60208210810361074457634e487b7160e01b600052602260045260246000fd5b50919050565b8082018082111561025057634e487b7160e01b600052601160045260246000fdfea26469706673582212209ca60becb493221a7cad525a9cc53486e7d32e693890081d97fcdb7c653cc0b164736f6c63430008170033",
+    "deployedSourceMap": "104:156:5:-:0;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;2074:89:1;;;:::i;:::-;;;;;;;:::i;:::-;;;;;;;;4293:186;;;;;;:::i;:::-;;:::i;:::-;;;1169:14:6;;1162:22;1144:41;;1132:2;1117:18;4293:186:1;1004:187:6;3144:97:1;3222:12;;3144:97;;;1342:25:6;;;1330:2;1315:18;3144:97:1;1196:177:6;5039:244:1;;;;;;:::i;:::-;;:::i;3002:82::-;;;3075:2;1853:36:6;;1841:2;1826:18;3002:82:1;1711:184:6;3299:116:1;;;;;;:::i;:::-;-1:-1:-1;;;;;3390:18:1;3364:7;3390:18;;;;;;;;;;;;3299:116;2276:93;;;:::i;178:78:5:-;;;;;;:::i;:::-;;:::i;:::-;;3610:178:1;;;;;;:::i;:::-;;:::i;3846:140::-;;;;;;:::i;:::-;-1:-1:-1;;;;;3952:18:1;;;3926:7;3952:18;;;:11;:18;;;;;;;;:27;;;;;;;;;;;;;3846:140;2074:89;2119:13;2151:5;2144:12;;;;;:::i;:::-;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;:::i;:::-;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;2074:89;:::o;4293:186::-;4366:4;735:10:4;4420:31:1;735:10:4;4436:7:1;4445:5;4420:8;:31::i;:::-;4468:4;4461:11;;;4293:186;;;;;:::o;5039:244::-;5126:4;735:10:4;5182:37:1;5198:4;735:10:4;5213:5:1;5182:15;:37::i;:::-;5229:26;5239:4;5245:2;5249:5;5229:9;:26::i;:::-;-1:-1:-1;5272:4:1;;5039:244;-1:-1:-1;;;;5039:244:1:o;2276:93::-;2323:13;2355:7;2348:14;;;;;:::i;178:78:5:-;225:24;231:10;243:5;225;:24::i;:::-;178:78;:::o;3610:178:1:-;3679:4;735:10:4;3733:27:1;735:10:4;3750:2:1;3754:5;3733:9;:27::i;8989:128::-;9073:37;9082:5;9089:7;9098:5;9105:4;9073:8;:37::i;:::-;8989:128;;;:::o;10663:477::-;-1:-1:-1;;;;;3952:18:1;;;10762:24;3952:18;;;:11;:18;;;;;;;;:27;;;;;;;;;;-1:-1:-1;;10828:37:1;;10824:310;;10904:5;10885:16;:24;10881:130;;;10936:60;;-1:-1:-1;;;10936:60:1;;-1:-1:-1;;;;;3146:32:6;;10936:60:1;;;3128:51:6;3195:18;;;3188:34;;;3238:18;;;3231:34;;;3101:18;;10936:60:1;;;;;;;;10881:130;11052:57;11061:5;11068:7;11096:5;11077:16;:24;11103:5;11052:8;:57::i;:::-;10752:388;10663:477;;;:::o;5656:300::-;-1:-1:-1;;;;;5739:18:1;;5735:86;;5780:30;;-1:-1:-1;;;5780:30:1;;5807:1;5780:30;;;3422:51:6;3395:18;;5780:30:1;3276:203:6;5735:86:1;-1:-1:-1;;;;;5834:16:1;;5830:86;;5873:32;;-1:-1:-1;;;5873:32:1;;5902:1;5873:32;;;3422:51:6;3395:18;;5873:32:1;3276:203:6;5830:86:1;5925:24;5933:4;5939:2;5943:5;5925:7;:24::i;7721:208::-;-1:-1:-1;;;;;7791:21:1;;7787:91;;7835:32;;-1:-1:-1;;;7835:32:1;;7864:1;7835:32;;;3422:51:6;3395:18;;7835:32:1;3276:203:6;7787:91:1;7887:35;7903:1;7907:7;7916:5;7887:7;:35::i;:::-;7721:208;;:::o;9949:432::-;-1:-1:-1;;;;;10061:19:1;;10057:89;;10103:32;;-1:-1:-1;;;10103:32:1;;10132:1;10103:32;;;3422:51:6;3395:18;;10103:32:1;3276:203:6;10057:89:1;-1:-1:-1;;;;;10159:21:1;;10155:90;;10203:31;;-1:-1:-1;;;10203:31:1;;10231:1;10203:31;;;3422:51:6;3395:18;;10203:31:1;3276:203:6;10155:90:1;-1:-1:-1;;;;;10254:18:1;;;;;;;:11;:18;;;;;;;;:27;;;;;;;;;:35;;;10299:76;;;;10349:7;-1:-1:-1;;;;;10333:31:1;10342:5;-1:-1:-1;;;;;10333:31:1;;10358:5;10333:31;;;;1342:25:6;;1330:2;1315:18;;1196:177;10333:31:1;;;;;;;;9949:432;;;;:::o;6271:1107::-;-1:-1:-1;;;;;6360:18:1;;6356:540;;6512:5;6496:12;;:21;;;;;;;:::i;:::-;;;;-1:-1:-1;6356:540:1;;-1:-1:-1;6356:540:1;;-1:-1:-1;;;;;6570:15:1;;6548:19;6570:15;;;;;;;;;;;6603:19;;;6599:115;;;6649:50;;-1:-1:-1;;;6649:50:1;;-1:-1:-1;;;;;3146:32:6;;6649:50:1;;;3128:51:6;3195:18;;;3188:34;;;3238:18;;;3231:34;;;3101:18;;6649:50:1;2926:345:6;6599:115:1;-1:-1:-1;;;;;6834:15:1;;:9;:15;;;;;;;;;;6852:19;;;;6834:37;;6356:540;-1:-1:-1;;;;;6910:16:1;;6906:425;;7073:12;:21;;;;;;;6906:425;;;-1:-1:-1;;;;;7284:13:1;;:9;:13;;;;;;;;;;:22;;;;;;6906:425;7361:2;-1:-1:-1;;;;;7346:25:1;7355:4;-1:-1:-1;;;;;7346:25:1;;7365:5;7346:25;;;;1342::6;;1330:2;1315:18;;1196:177;7346:25:1;;;;;;;;6271:1107;;;:::o;14:548:6:-;126:4;155:2;184;173:9;166:21;216:6;210:13;259:6;254:2;243:9;239:18;232:34;284:1;294:140;308:6;305:1;302:13;294:140;;;403:14;;;399:23;;393:30;369:17;;;388:2;365:26;358:66;323:10;;294:140;;;298:3;483:1;478:2;469:6;458:9;454:22;450:31;443:42;553:2;546;542:7;537:2;529:6;525:15;521:29;510:9;506:45;502:54;494:62;;;;14:548;;;;:::o;567:173::-;635:20;;-1:-1:-1;;;;;684:31:6;;674:42;;664:70;;730:1;727;720:12;664:70;567:173;;;:::o;745:254::-;813:6;821;874:2;862:9;853:7;849:23;845:32;842:52;;;890:1;887;880:12;842:52;913:29;932:9;913:29;:::i;:::-;903:39;989:2;974:18;;;;961:32;;-1:-1:-1;;;745:254:6:o;1378:328::-;1455:6;1463;1471;1524:2;1512:9;1503:7;1499:23;1495:32;1492:52;;;1540:1;1537;1530:12;1492:52;1563:29;1582:9;1563:29;:::i;:::-;1553:39;;1611:38;1645:2;1634:9;1630:18;1611:38;:::i;:::-;1601:48;;1696:2;1685:9;1681:18;1668:32;1658:42;;1378:328;;;;;:::o;1900:186::-;1959:6;2012:2;2000:9;1991:7;1987:23;1983:32;1980:52;;;2028:1;2025;2018:12;1980:52;2051:29;2070:9;2051:29;:::i;:::-;2041:39;1900:186;-1:-1:-1;;;1900:186:6:o;2091:180::-;2150:6;2203:2;2191:9;2182:7;2178:23;2174:32;2171:52;;;2219:1;2216;2209:12;2171:52;-1:-1:-1;2242:23:6;;2091:180;-1:-1:-1;2091:180:6:o;2276:260::-;2344:6;2352;2405:2;2393:9;2384:7;2380:23;2376:32;2373:52;;;2421:1;2418;2411:12;2373:52;2444:29;2463:9;2444:29;:::i;:::-;2434:39;;2492:38;2526:2;2515:9;2511:18;2492:38;:::i;:::-;2482:48;;2276:260;;;;;:::o;2541:380::-;2620:1;2616:12;;;;2663;;;2684:61;;2738:4;2730:6;2726:17;2716:27;;2684:61;2791:2;2783:6;2780:14;2760:18;2757:38;2754:161;;2837:10;2832:3;2828:20;2825:1;2818:31;2872:4;2869:1;2862:15;2900:4;2897:1;2890:15;2754:161;;2541:380;;;:::o;3484:222::-;3549:9;;;3570:10;;;3567:133;;;3622:10;3617:3;3613:20;3610:1;3603:31;3657:4;3654:1;3647:15;3685:4;3682:1;3675:15",
     "language": "Solidity",
     "natspec": {
         "errors": {
             "ERC20InsufficientAllowance(address,uint256,uint256)": [
                 {
                     "details": "Indicates a failure with the `spender`\u2019s `allowance`. Used in transfers.",
                     "params": {
@@ -1175,3930 +1028,4040 @@
                 "details": "See {IERC20-transferFrom}. Emits an {Approval} event indicating the updated allowance. This is not required by the EIP. See the note at the beginning of {ERC20}. NOTE: Does not update the allowance if the current allowance is the maximum `uint256`. Requirements: - `from` and `to` cannot be the zero address. - `from` must have a balance of at least `value`. - the caller must have allowance for ``from``'s tokens of at least `value`."
             }
         },
         "version": 1
     },
     "offset": [
         104,
-        343
+        260
     ],
-    "opcodes": "PUSH1 0x80 PUSH1 0x40 MSTORE CALLVALUE DUP1 ISZERO PUSH2 0x10 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST POP PUSH1 0x4 CALLDATASIZE LT PUSH2 0x9E JUMPI PUSH1 0x0 CALLDATALOAD PUSH1 0xE0 SHR DUP1 PUSH4 0x313CE567 GT PUSH2 0x66 JUMPI DUP1 PUSH4 0x313CE567 EQ PUSH2 0x113 JUMPI DUP1 PUSH4 0x70A08231 EQ PUSH2 0x122 JUMPI DUP1 PUSH4 0x95D89B41 EQ PUSH2 0x14B JUMPI DUP1 PUSH4 0xA9059CBB EQ PUSH2 0x153 JUMPI DUP1 PUSH4 0xDD62ED3E EQ PUSH2 0x166 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST DUP1 PUSH4 0x6FDDE03 EQ PUSH2 0xA3 JUMPI DUP1 PUSH4 0x95EA7B3 EQ PUSH2 0xC1 JUMPI DUP1 PUSH4 0x1249C58B EQ PUSH2 0xE4 JUMPI DUP1 PUSH4 0x18160DDD EQ PUSH2 0xEE JUMPI DUP1 PUSH4 0x23B872DD EQ PUSH2 0x100 JUMPI JUMPDEST PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0xAB PUSH2 0x19F JUMP JUMPDEST PUSH1 0x40 MLOAD PUSH2 0xB8 SWAP2 SWAP1 PUSH2 0x5C8 JUMP JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 RETURN JUMPDEST PUSH2 0xD4 PUSH2 0xCF CALLDATASIZE PUSH1 0x4 PUSH2 0x633 JUMP JUMPDEST PUSH2 0x231 JUMP JUMPDEST PUSH1 0x40 MLOAD SWAP1 ISZERO ISZERO DUP2 MSTORE PUSH1 0x20 ADD PUSH2 0xB8 JUMP JUMPDEST PUSH2 0xEC PUSH2 0x24B JUMP JUMPDEST STOP JUMPDEST PUSH1 0x2 SLOAD JUMPDEST PUSH1 0x40 MLOAD SWAP1 DUP2 MSTORE PUSH1 0x20 ADD PUSH2 0xB8 JUMP JUMPDEST PUSH2 0xD4 PUSH2 0x10E CALLDATASIZE PUSH1 0x4 PUSH2 0x65D JUMP JUMPDEST PUSH2 0x25A JUMP JUMPDEST PUSH1 0x40 MLOAD PUSH1 0x6 DUP2 MSTORE PUSH1 0x20 ADD PUSH2 0xB8 JUMP JUMPDEST PUSH2 0xF2 PUSH2 0x130 CALLDATASIZE PUSH1 0x4 PUSH2 0x699 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 SLOAD SWAP1 JUMP JUMPDEST PUSH2 0xAB PUSH2 0x27E JUMP JUMPDEST PUSH2 0xD4 PUSH2 0x161 CALLDATASIZE PUSH1 0x4 PUSH2 0x633 JUMP JUMPDEST PUSH2 0x28D JUMP JUMPDEST PUSH2 0xF2 PUSH2 0x174 CALLDATASIZE PUSH1 0x4 PUSH2 0x6BB JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB SWAP2 DUP3 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x1 PUSH1 0x20 SWAP1 DUP2 MSTORE PUSH1 0x40 DUP1 DUP4 KECCAK256 SWAP4 SWAP1 SWAP5 AND DUP3 MSTORE SWAP2 SWAP1 SWAP2 MSTORE KECCAK256 SLOAD SWAP1 JUMP JUMPDEST PUSH1 0x60 PUSH1 0x3 DUP1 SLOAD PUSH2 0x1AE SWAP1 PUSH2 0x6EE JUMP JUMPDEST DUP1 PUSH1 0x1F ADD PUSH1 0x20 DUP1 SWAP2 DIV MUL PUSH1 0x20 ADD PUSH1 0x40 MLOAD SWAP1 DUP2 ADD PUSH1 0x40 MSTORE DUP1 SWAP3 SWAP2 SWAP1 DUP2 DUP2 MSTORE PUSH1 0x20 ADD DUP3 DUP1 SLOAD PUSH2 0x1DA SWAP1 PUSH2 0x6EE JUMP JUMPDEST DUP1 ISZERO PUSH2 0x227 JUMPI DUP1 PUSH1 0x1F LT PUSH2 0x1FC JUMPI PUSH2 0x100 DUP1 DUP4 SLOAD DIV MUL DUP4 MSTORE SWAP2 PUSH1 0x20 ADD SWAP2 PUSH2 0x227 JUMP JUMPDEST DUP3 ADD SWAP2 SWAP1 PUSH1 0x0 MSTORE PUSH1 0x20 PUSH1 0x0 KECCAK256 SWAP1 JUMPDEST DUP2 SLOAD DUP2 MSTORE SWAP1 PUSH1 0x1 ADD SWAP1 PUSH1 0x20 ADD DUP1 DUP4 GT PUSH2 0x20A JUMPI DUP3 SWAP1 SUB PUSH1 0x1F AND DUP3 ADD SWAP2 JUMPDEST POP POP POP POP POP SWAP1 POP SWAP1 JUMP JUMPDEST PUSH1 0x0 CALLER PUSH2 0x23F DUP2 DUP6 DUP6 PUSH2 0x29B JUMP JUMPDEST PUSH1 0x1 SWAP2 POP POP JUMPDEST SWAP3 SWAP2 POP POP JUMP JUMPDEST PUSH2 0x258 CALLER PUSH3 0x4C4B40 PUSH2 0x2AD JUMP JUMPDEST JUMP JUMPDEST PUSH1 0x0 CALLER PUSH2 0x268 DUP6 DUP3 DUP6 PUSH2 0x2EC JUMP JUMPDEST PUSH2 0x273 DUP6 DUP6 DUP6 PUSH2 0x36A JUMP JUMPDEST POP PUSH1 0x1 SWAP5 SWAP4 POP POP POP POP JUMP JUMPDEST PUSH1 0x60 PUSH1 0x4 DUP1 SLOAD PUSH2 0x1AE SWAP1 PUSH2 0x6EE JUMP JUMPDEST PUSH1 0x0 CALLER PUSH2 0x23F DUP2 DUP6 DUP6 PUSH2 0x36A JUMP JUMPDEST PUSH2 0x2A8 DUP4 DUP4 DUP4 PUSH1 0x1 PUSH2 0x3C9 JUMP JUMPDEST POP POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH2 0x2DC JUMPI PUSH1 0x40 MLOAD PUSH4 0xEC442F05 PUSH1 0xE0 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 REVERT JUMPDEST PUSH2 0x2E8 PUSH1 0x0 DUP4 DUP4 PUSH2 0x49E JUMP JUMPDEST POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 DUP2 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x1 PUSH1 0x20 SWAP1 DUP2 MSTORE PUSH1 0x40 DUP1 DUP4 KECCAK256 SWAP4 DUP7 AND DUP4 MSTORE SWAP3 SWAP1 MSTORE KECCAK256 SLOAD PUSH1 0x0 NOT DUP2 EQ PUSH2 0x364 JUMPI DUP2 DUP2 LT ISZERO PUSH2 0x355 JUMPI PUSH1 0x40 MLOAD PUSH4 0x7DC7A0D9 PUSH1 0xE1 SHL DUP2 MSTORE PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP5 AND PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 DUP2 ADD DUP3 SWAP1 MSTORE PUSH1 0x44 DUP2 ADD DUP4 SWAP1 MSTORE PUSH1 0x64 ADD PUSH2 0x2D3 JUMP JUMPDEST PUSH2 0x364 DUP5 DUP5 DUP5 DUP5 SUB PUSH1 0x0 PUSH2 0x3C9 JUMP JUMPDEST POP POP POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH2 0x394 JUMPI PUSH1 0x40 MLOAD PUSH4 0x4B637E8F PUSH1 0xE1 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x2D3 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH2 0x3BE JUMPI PUSH1 0x40 MLOAD PUSH4 0xEC442F05 PUSH1 0xE0 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x2D3 JUMP JUMPDEST PUSH2 0x2A8 DUP4 DUP4 DUP4 PUSH2 0x49E JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP5 AND PUSH2 0x3F3 JUMPI PUSH1 0x40 MLOAD PUSH4 0xE602DF05 PUSH1 0xE0 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x2D3 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH2 0x41D JUMPI PUSH1 0x40 MLOAD PUSH4 0x4A1406B1 PUSH1 0xE1 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x2D3 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP1 DUP6 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x1 PUSH1 0x20 SWAP1 DUP2 MSTORE PUSH1 0x40 DUP1 DUP4 KECCAK256 SWAP4 DUP8 AND DUP4 MSTORE SWAP3 SWAP1 MSTORE KECCAK256 DUP3 SWAP1 SSTORE DUP1 ISZERO PUSH2 0x364 JUMPI DUP3 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND DUP5 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND PUSH32 0x8C5BE1E5EBEC7D5BD14F71427D1E84F3DD0314C0F7B2291E5B200AC8C7C3B925 DUP5 PUSH1 0x40 MLOAD PUSH2 0x490 SWAP2 DUP2 MSTORE PUSH1 0x20 ADD SWAP1 JUMP JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 LOG3 POP POP POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH2 0x4C9 JUMPI DUP1 PUSH1 0x2 PUSH1 0x0 DUP3 DUP3 SLOAD PUSH2 0x4BE SWAP2 SWAP1 PUSH2 0x728 JUMP JUMPDEST SWAP1 SWAP2 SSTORE POP PUSH2 0x53B SWAP1 POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 SLOAD DUP2 DUP2 LT ISZERO PUSH2 0x51C JUMPI PUSH1 0x40 MLOAD PUSH4 0x391434E3 PUSH1 0xE2 SHL DUP2 MSTORE PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP6 AND PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 DUP2 ADD DUP3 SWAP1 MSTORE PUSH1 0x44 DUP2 ADD DUP4 SWAP1 MSTORE PUSH1 0x64 ADD PUSH2 0x2D3 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP5 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 SWAP1 DUP3 SWAP1 SUB SWAP1 SSTORE JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH2 0x557 JUMPI PUSH1 0x2 DUP1 SLOAD DUP3 SWAP1 SUB SWAP1 SSTORE PUSH2 0x576 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 DUP1 SLOAD DUP3 ADD SWAP1 SSTORE JUMPDEST DUP2 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND DUP4 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND PUSH32 0xDDF252AD1BE2C89B69C2B068FC378DAA952BA7F163C4A11628F55A4DF523B3EF DUP4 PUSH1 0x40 MLOAD PUSH2 0x5BB SWAP2 DUP2 MSTORE PUSH1 0x20 ADD SWAP1 JUMP JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 LOG3 POP POP POP JUMP JUMPDEST PUSH1 0x0 PUSH1 0x20 DUP1 DUP4 MSTORE DUP4 MLOAD DUP1 PUSH1 0x20 DUP6 ADD MSTORE PUSH1 0x0 JUMPDEST DUP2 DUP2 LT ISZERO PUSH2 0x5F6 JUMPI DUP6 DUP2 ADD DUP4 ADD MLOAD DUP6 DUP3 ADD PUSH1 0x40 ADD MSTORE DUP3 ADD PUSH2 0x5DA JUMP JUMPDEST POP PUSH1 0x0 PUSH1 0x40 DUP3 DUP7 ADD ADD MSTORE PUSH1 0x40 PUSH1 0x1F NOT PUSH1 0x1F DUP4 ADD AND DUP6 ADD ADD SWAP3 POP POP POP SWAP3 SWAP2 POP POP JUMP JUMPDEST DUP1 CALLDATALOAD PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP2 AND DUP2 EQ PUSH2 0x62E JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST SWAP2 SWAP1 POP JUMP JUMPDEST PUSH1 0x0 DUP1 PUSH1 0x40 DUP4 DUP6 SUB SLT ISZERO PUSH2 0x646 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x64F DUP4 PUSH2 0x617 JUMP JUMPDEST SWAP5 PUSH1 0x20 SWAP4 SWAP1 SWAP4 ADD CALLDATALOAD SWAP4 POP POP POP JUMP JUMPDEST PUSH1 0x0 DUP1 PUSH1 0x0 PUSH1 0x60 DUP5 DUP7 SUB SLT ISZERO PUSH2 0x672 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x67B DUP5 PUSH2 0x617 JUMP JUMPDEST SWAP3 POP PUSH2 0x689 PUSH1 0x20 DUP6 ADD PUSH2 0x617 JUMP JUMPDEST SWAP2 POP PUSH1 0x40 DUP5 ADD CALLDATALOAD SWAP1 POP SWAP3 POP SWAP3 POP SWAP3 JUMP JUMPDEST PUSH1 0x0 PUSH1 0x20 DUP3 DUP5 SUB SLT ISZERO PUSH2 0x6AB JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x6B4 DUP3 PUSH2 0x617 JUMP JUMPDEST SWAP4 SWAP3 POP POP POP JUMP JUMPDEST PUSH1 0x0 DUP1 PUSH1 0x40 DUP4 DUP6 SUB SLT ISZERO PUSH2 0x6CE JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x6D7 DUP4 PUSH2 0x617 JUMP JUMPDEST SWAP2 POP PUSH2 0x6E5 PUSH1 0x20 DUP5 ADD PUSH2 0x617 JUMP JUMPDEST SWAP1 POP SWAP3 POP SWAP3 SWAP1 POP JUMP JUMPDEST PUSH1 0x1 DUP2 DUP2 SHR SWAP1 DUP3 AND DUP1 PUSH2 0x702 JUMPI PUSH1 0x7F DUP3 AND SWAP2 POP JUMPDEST PUSH1 0x20 DUP3 LT DUP2 SUB PUSH2 0x722 JUMPI PUSH4 0x4E487B71 PUSH1 0xE0 SHL PUSH1 0x0 MSTORE PUSH1 0x22 PUSH1 0x4 MSTORE PUSH1 0x24 PUSH1 0x0 REVERT JUMPDEST POP SWAP2 SWAP1 POP JUMP JUMPDEST DUP1 DUP3 ADD DUP1 DUP3 GT ISZERO PUSH2 0x245 JUMPI PUSH4 0x4E487B71 PUSH1 0xE0 SHL PUSH1 0x0 MSTORE PUSH1 0x11 PUSH1 0x4 MSTORE PUSH1 0x24 PUSH1 0x0 REVERT INVALID LOG2 PUSH5 0x6970667358 0x22 SLT KECCAK256 PUSH29 0xE3BB5838214D8592B0D420A3F00611810814B9AD464F848B86E08D0E1B STATICCALL SWAP4 PUSH5 0x736F6C6343 STOP ADDMOD OR STOP CALLER ",
+    "opcodes": "PUSH1 0x80 PUSH1 0x40 MSTORE CALLVALUE DUP1 ISZERO PUSH2 0x10 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST POP PUSH1 0x4 CALLDATASIZE LT PUSH2 0x9E JUMPI PUSH1 0x0 CALLDATALOAD PUSH1 0xE0 SHR DUP1 PUSH4 0x70A08231 GT PUSH2 0x66 JUMPI DUP1 PUSH4 0x70A08231 EQ PUSH2 0x118 JUMPI DUP1 PUSH4 0x95D89B41 EQ PUSH2 0x141 JUMPI DUP1 PUSH4 0xA0712D68 EQ PUSH2 0x149 JUMPI DUP1 PUSH4 0xA9059CBB EQ PUSH2 0x15E JUMPI DUP1 PUSH4 0xDD62ED3E EQ PUSH2 0x171 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST DUP1 PUSH4 0x6FDDE03 EQ PUSH2 0xA3 JUMPI DUP1 PUSH4 0x95EA7B3 EQ PUSH2 0xC1 JUMPI DUP1 PUSH4 0x18160DDD EQ PUSH2 0xE4 JUMPI DUP1 PUSH4 0x23B872DD EQ PUSH2 0xF6 JUMPI DUP1 PUSH4 0x313CE567 EQ PUSH2 0x109 JUMPI JUMPDEST PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0xAB PUSH2 0x1AA JUMP JUMPDEST PUSH1 0x40 MLOAD PUSH2 0xB8 SWAP2 SWAP1 PUSH2 0x5D1 JUMP JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 RETURN JUMPDEST PUSH2 0xD4 PUSH2 0xCF CALLDATASIZE PUSH1 0x4 PUSH2 0x63C JUMP JUMPDEST PUSH2 0x23C JUMP JUMPDEST PUSH1 0x40 MLOAD SWAP1 ISZERO ISZERO DUP2 MSTORE PUSH1 0x20 ADD PUSH2 0xB8 JUMP JUMPDEST PUSH1 0x2 SLOAD JUMPDEST PUSH1 0x40 MLOAD SWAP1 DUP2 MSTORE PUSH1 0x20 ADD PUSH2 0xB8 JUMP JUMPDEST PUSH2 0xD4 PUSH2 0x104 CALLDATASIZE PUSH1 0x4 PUSH2 0x666 JUMP JUMPDEST PUSH2 0x256 JUMP JUMPDEST PUSH1 0x40 MLOAD PUSH1 0x12 DUP2 MSTORE PUSH1 0x20 ADD PUSH2 0xB8 JUMP JUMPDEST PUSH2 0xE8 PUSH2 0x126 CALLDATASIZE PUSH1 0x4 PUSH2 0x6A2 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 SLOAD SWAP1 JUMP JUMPDEST PUSH2 0xAB PUSH2 0x27A JUMP JUMPDEST PUSH2 0x15C PUSH2 0x157 CALLDATASIZE PUSH1 0x4 PUSH2 0x6C4 JUMP JUMPDEST PUSH2 0x289 JUMP JUMPDEST STOP JUMPDEST PUSH2 0xD4 PUSH2 0x16C CALLDATASIZE PUSH1 0x4 PUSH2 0x63C JUMP JUMPDEST PUSH2 0x296 JUMP JUMPDEST PUSH2 0xE8 PUSH2 0x17F CALLDATASIZE PUSH1 0x4 PUSH2 0x6DD JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB SWAP2 DUP3 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x1 PUSH1 0x20 SWAP1 DUP2 MSTORE PUSH1 0x40 DUP1 DUP4 KECCAK256 SWAP4 SWAP1 SWAP5 AND DUP3 MSTORE SWAP2 SWAP1 SWAP2 MSTORE KECCAK256 SLOAD SWAP1 JUMP JUMPDEST PUSH1 0x60 PUSH1 0x3 DUP1 SLOAD PUSH2 0x1B9 SWAP1 PUSH2 0x710 JUMP JUMPDEST DUP1 PUSH1 0x1F ADD PUSH1 0x20 DUP1 SWAP2 DIV MUL PUSH1 0x20 ADD PUSH1 0x40 MLOAD SWAP1 DUP2 ADD PUSH1 0x40 MSTORE DUP1 SWAP3 SWAP2 SWAP1 DUP2 DUP2 MSTORE PUSH1 0x20 ADD DUP3 DUP1 SLOAD PUSH2 0x1E5 SWAP1 PUSH2 0x710 JUMP JUMPDEST DUP1 ISZERO PUSH2 0x232 JUMPI DUP1 PUSH1 0x1F LT PUSH2 0x207 JUMPI PUSH2 0x100 DUP1 DUP4 SLOAD DIV MUL DUP4 MSTORE SWAP2 PUSH1 0x20 ADD SWAP2 PUSH2 0x232 JUMP JUMPDEST DUP3 ADD SWAP2 SWAP1 PUSH1 0x0 MSTORE PUSH1 0x20 PUSH1 0x0 KECCAK256 SWAP1 JUMPDEST DUP2 SLOAD DUP2 MSTORE SWAP1 PUSH1 0x1 ADD SWAP1 PUSH1 0x20 ADD DUP1 DUP4 GT PUSH2 0x215 JUMPI DUP3 SWAP1 SUB PUSH1 0x1F AND DUP3 ADD SWAP2 JUMPDEST POP POP POP POP POP SWAP1 POP SWAP1 JUMP JUMPDEST PUSH1 0x0 CALLER PUSH2 0x24A DUP2 DUP6 DUP6 PUSH2 0x2A4 JUMP JUMPDEST PUSH1 0x1 SWAP2 POP POP JUMPDEST SWAP3 SWAP2 POP POP JUMP JUMPDEST PUSH1 0x0 CALLER PUSH2 0x264 DUP6 DUP3 DUP6 PUSH2 0x2B6 JUMP JUMPDEST PUSH2 0x26F DUP6 DUP6 DUP6 PUSH2 0x339 JUMP JUMPDEST POP PUSH1 0x1 SWAP5 SWAP4 POP POP POP POP JUMP JUMPDEST PUSH1 0x60 PUSH1 0x4 DUP1 SLOAD PUSH2 0x1B9 SWAP1 PUSH2 0x710 JUMP JUMPDEST PUSH2 0x293 CALLER DUP3 PUSH2 0x398 JUMP JUMPDEST POP JUMP JUMPDEST PUSH1 0x0 CALLER PUSH2 0x24A DUP2 DUP6 DUP6 PUSH2 0x339 JUMP JUMPDEST PUSH2 0x2B1 DUP4 DUP4 DUP4 PUSH1 0x1 PUSH2 0x3D2 JUMP JUMPDEST POP POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 DUP2 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x1 PUSH1 0x20 SWAP1 DUP2 MSTORE PUSH1 0x40 DUP1 DUP4 KECCAK256 SWAP4 DUP7 AND DUP4 MSTORE SWAP3 SWAP1 MSTORE KECCAK256 SLOAD PUSH1 0x0 NOT DUP2 EQ PUSH2 0x333 JUMPI DUP2 DUP2 LT ISZERO PUSH2 0x324 JUMPI PUSH1 0x40 MLOAD PUSH4 0x7DC7A0D9 PUSH1 0xE1 SHL DUP2 MSTORE PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP5 AND PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 DUP2 ADD DUP3 SWAP1 MSTORE PUSH1 0x44 DUP2 ADD DUP4 SWAP1 MSTORE PUSH1 0x64 ADD JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 REVERT JUMPDEST PUSH2 0x333 DUP5 DUP5 DUP5 DUP5 SUB PUSH1 0x0 PUSH2 0x3D2 JUMP JUMPDEST POP POP POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH2 0x363 JUMPI PUSH1 0x40 MLOAD PUSH4 0x4B637E8F PUSH1 0xE1 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x31B JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH2 0x38D JUMPI PUSH1 0x40 MLOAD PUSH4 0xEC442F05 PUSH1 0xE0 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x31B JUMP JUMPDEST PUSH2 0x2B1 DUP4 DUP4 DUP4 PUSH2 0x4A7 JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH2 0x3C2 JUMPI PUSH1 0x40 MLOAD PUSH4 0xEC442F05 PUSH1 0xE0 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x31B JUMP JUMPDEST PUSH2 0x3CE PUSH1 0x0 DUP4 DUP4 PUSH2 0x4A7 JUMP JUMPDEST POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP5 AND PUSH2 0x3FC JUMPI PUSH1 0x40 MLOAD PUSH4 0xE602DF05 PUSH1 0xE0 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x31B JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH2 0x426 JUMPI PUSH1 0x40 MLOAD PUSH4 0x4A1406B1 PUSH1 0xE1 SHL DUP2 MSTORE PUSH1 0x0 PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 ADD PUSH2 0x31B JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP1 DUP6 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x1 PUSH1 0x20 SWAP1 DUP2 MSTORE PUSH1 0x40 DUP1 DUP4 KECCAK256 SWAP4 DUP8 AND DUP4 MSTORE SWAP3 SWAP1 MSTORE KECCAK256 DUP3 SWAP1 SSTORE DUP1 ISZERO PUSH2 0x333 JUMPI DUP3 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND DUP5 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND PUSH32 0x8C5BE1E5EBEC7D5BD14F71427D1E84F3DD0314C0F7B2291E5B200AC8C7C3B925 DUP5 PUSH1 0x40 MLOAD PUSH2 0x499 SWAP2 DUP2 MSTORE PUSH1 0x20 ADD SWAP1 JUMP JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 LOG3 POP POP POP POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH2 0x4D2 JUMPI DUP1 PUSH1 0x2 PUSH1 0x0 DUP3 DUP3 SLOAD PUSH2 0x4C7 SWAP2 SWAP1 PUSH2 0x74A JUMP JUMPDEST SWAP1 SWAP2 SSTORE POP PUSH2 0x544 SWAP1 POP JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP4 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 SLOAD DUP2 DUP2 LT ISZERO PUSH2 0x525 JUMPI PUSH1 0x40 MLOAD PUSH4 0x391434E3 PUSH1 0xE2 SHL DUP2 MSTORE PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP6 AND PUSH1 0x4 DUP3 ADD MSTORE PUSH1 0x24 DUP2 ADD DUP3 SWAP1 MSTORE PUSH1 0x44 DUP2 ADD DUP4 SWAP1 MSTORE PUSH1 0x64 ADD PUSH2 0x31B JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP5 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 SWAP1 DUP3 SWAP1 SUB SWAP1 SSTORE JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH2 0x560 JUMPI PUSH1 0x2 DUP1 SLOAD DUP3 SWAP1 SUB SWAP1 SSTORE PUSH2 0x57F JUMP JUMPDEST PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP3 AND PUSH1 0x0 SWAP1 DUP2 MSTORE PUSH1 0x20 DUP2 SWAP1 MSTORE PUSH1 0x40 SWAP1 KECCAK256 DUP1 SLOAD DUP3 ADD SWAP1 SSTORE JUMPDEST DUP2 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND DUP4 PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB AND PUSH32 0xDDF252AD1BE2C89B69C2B068FC378DAA952BA7F163C4A11628F55A4DF523B3EF DUP4 PUSH1 0x40 MLOAD PUSH2 0x5C4 SWAP2 DUP2 MSTORE PUSH1 0x20 ADD SWAP1 JUMP JUMPDEST PUSH1 0x40 MLOAD DUP1 SWAP2 SUB SWAP1 LOG3 POP POP POP JUMP JUMPDEST PUSH1 0x0 PUSH1 0x20 DUP1 DUP4 MSTORE DUP4 MLOAD DUP1 PUSH1 0x20 DUP6 ADD MSTORE PUSH1 0x0 JUMPDEST DUP2 DUP2 LT ISZERO PUSH2 0x5FF JUMPI DUP6 DUP2 ADD DUP4 ADD MLOAD DUP6 DUP3 ADD PUSH1 0x40 ADD MSTORE DUP3 ADD PUSH2 0x5E3 JUMP JUMPDEST POP PUSH1 0x0 PUSH1 0x40 DUP3 DUP7 ADD ADD MSTORE PUSH1 0x40 PUSH1 0x1F NOT PUSH1 0x1F DUP4 ADD AND DUP6 ADD ADD SWAP3 POP POP POP SWAP3 SWAP2 POP POP JUMP JUMPDEST DUP1 CALLDATALOAD PUSH1 0x1 PUSH1 0x1 PUSH1 0xA0 SHL SUB DUP2 AND DUP2 EQ PUSH2 0x637 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST SWAP2 SWAP1 POP JUMP JUMPDEST PUSH1 0x0 DUP1 PUSH1 0x40 DUP4 DUP6 SUB SLT ISZERO PUSH2 0x64F JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x658 DUP4 PUSH2 0x620 JUMP JUMPDEST SWAP5 PUSH1 0x20 SWAP4 SWAP1 SWAP4 ADD CALLDATALOAD SWAP4 POP POP POP JUMP JUMPDEST PUSH1 0x0 DUP1 PUSH1 0x0 PUSH1 0x60 DUP5 DUP7 SUB SLT ISZERO PUSH2 0x67B JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x684 DUP5 PUSH2 0x620 JUMP JUMPDEST SWAP3 POP PUSH2 0x692 PUSH1 0x20 DUP6 ADD PUSH2 0x620 JUMP JUMPDEST SWAP2 POP PUSH1 0x40 DUP5 ADD CALLDATALOAD SWAP1 POP SWAP3 POP SWAP3 POP SWAP3 JUMP JUMPDEST PUSH1 0x0 PUSH1 0x20 DUP3 DUP5 SUB SLT ISZERO PUSH2 0x6B4 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x6BD DUP3 PUSH2 0x620 JUMP JUMPDEST SWAP4 SWAP3 POP POP POP JUMP JUMPDEST PUSH1 0x0 PUSH1 0x20 DUP3 DUP5 SUB SLT ISZERO PUSH2 0x6D6 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST POP CALLDATALOAD SWAP2 SWAP1 POP JUMP JUMPDEST PUSH1 0x0 DUP1 PUSH1 0x40 DUP4 DUP6 SUB SLT ISZERO PUSH2 0x6F0 JUMPI PUSH1 0x0 DUP1 REVERT JUMPDEST PUSH2 0x6F9 DUP4 PUSH2 0x620 JUMP JUMPDEST SWAP2 POP PUSH2 0x707 PUSH1 0x20 DUP5 ADD PUSH2 0x620 JUMP JUMPDEST SWAP1 POP SWAP3 POP SWAP3 SWAP1 POP JUMP JUMPDEST PUSH1 0x1 DUP2 DUP2 SHR SWAP1 DUP3 AND DUP1 PUSH2 0x724 JUMPI PUSH1 0x7F DUP3 AND SWAP2 POP JUMPDEST PUSH1 0x20 DUP3 LT DUP2 SUB PUSH2 0x744 JUMPI PUSH4 0x4E487B71 PUSH1 0xE0 SHL PUSH1 0x0 MSTORE PUSH1 0x22 PUSH1 0x4 MSTORE PUSH1 0x24 PUSH1 0x0 REVERT JUMPDEST POP SWAP2 SWAP1 POP JUMP JUMPDEST DUP1 DUP3 ADD DUP1 DUP3 GT ISZERO PUSH2 0x250 JUMPI PUSH4 0x4E487B71 PUSH1 0xE0 SHL PUSH1 0x0 MSTORE PUSH1 0x11 PUSH1 0x4 MSTORE PUSH1 0x24 PUSH1 0x0 REVERT INVALID LOG2 PUSH5 0x6970667358 0x22 SLT KECCAK256 SWAP13 0xA6 SIGNEXTEND 0xEC 0xB4 SWAP4 0x22 BYTE PUSH29 0xAD525A9CC53486E7D32E693890081D97FCDB7C653CC0B164736F6C6343 STOP ADDMOD OR STOP CALLER ",
     "pcMap": {
         "0": {
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "PUSH1",
-            "path": "6",
+            "path": "5",
             "value": "0x80"
         },
         "100": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "DUP1",
-            "path": "6"
+            "path": "5"
         },
         "1001": {
+            "op": "PUSH1",
+            "value": "0xE0"
+        },
+        "1003": {
+            "op": "SHL"
+        },
+        "1004": {
+            "fn": "ERC20._approve",
+            "offset": [
+                10103,
+                10135
+            ],
+            "op": "DUP2",
+            "path": "1"
+        },
+        "1005": {
+            "fn": "ERC20._approve",
+            "offset": [
+                10103,
+                10135
+            ],
+            "op": "MSTORE",
+            "path": "1"
+        },
+        "1006": {
+            "fn": "ERC20._approve",
+            "offset": [
+                10132,
+                10133
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x0"
+        },
+        "1008": {
+            "fn": "ERC20._approve",
+            "offset": [
+                10103,
+                10135
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x4"
+        },
+        "101": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "REVERT",
+            "path": "5"
+        },
+        "1010": {
             "fn": "ERC20._approve",
             "offset": [
                 10103,
                 10135
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1002": {
+        "1011": {
             "fn": "ERC20._approve",
             "offset": [
                 10103,
                 10135
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "1003": {
+        "1012": {
             "op": "MSTORE"
         },
-        "1004": {
+        "1013": {
             "op": "PUSH1",
             "value": "0x24"
         },
-        "1006": {
+        "1015": {
             "op": "ADD"
         },
-        "1007": {
+        "1016": {
             "fn": "ERC20._approve",
             "offset": [
                 10103,
                 10135
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x2D3"
+            "path": "1",
+            "value": "0x31B"
         },
-        "101": {
+        "1019": {
+            "op": "JUMP"
+        },
+        "102": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "REVERT",
-            "path": "6"
-        },
-        "1010": {
-            "op": "JUMP"
+            "op": "JUMPDEST",
+            "path": "5"
         },
-        "1011": {
+        "1020": {
             "fn": "ERC20._approve",
             "offset": [
                 10057,
                 10146
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1012": {
+        "1021": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1014": {
+        "1023": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1016": {
+        "1025": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1018": {
+        "1027": {
             "op": "SHL"
         },
-        "1019": {
+        "1028": {
             "op": "SUB"
         },
-        "102": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "JUMPDEST",
-            "path": "6"
-        },
-        "1020": {
+        "1029": {
             "fn": "ERC20._approve",
             "offset": [
                 10159,
                 10180
             ],
             "op": "DUP4",
-            "path": "2",
+            "path": "1",
             "statement": 23
         },
-        "1021": {
+        "103": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "DUP1",
+            "path": "5"
+        },
+        "1030": {
             "branch": 38,
             "fn": "ERC20._approve",
             "offset": [
                 10159,
                 10180
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1022": {
+        "1031": {
             "fn": "ERC20._approve",
             "offset": [
                 10155,
                 10245
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x41D"
+            "path": "1",
+            "value": "0x426"
         },
-        "1025": {
+        "1034": {
             "branch": 38,
             "fn": "ERC20._approve",
             "offset": [
                 10155,
                 10245
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "1026": {
+        "1035": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1028": {
+        "1037": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1029": {
+        "1038": {
             "op": "PUSH4",
             "value": "0x4A1406B1"
         },
-        "103": {
+        "104": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "DUP1",
-            "path": "6"
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0x6FDDE03"
         },
-        "1034": {
+        "1043": {
             "op": "PUSH1",
             "value": "0xE1"
         },
-        "1036": {
+        "1045": {
             "op": "SHL"
         },
-        "1037": {
+        "1046": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1038": {
+        "1047": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1039": {
+        "1048": {
             "fn": "ERC20._approve",
             "offset": [
                 10231,
                 10232
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "104": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x6FDDE03"
-        },
-        "1041": {
+        "1050": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "1043": {
+        "1052": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1044": {
+        "1053": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "1045": {
+        "1054": {
             "op": "MSTORE"
         },
-        "1046": {
+        "1055": {
             "op": "PUSH1",
             "value": "0x24"
         },
-        "1048": {
+        "1057": {
             "op": "ADD"
         },
-        "1049": {
+        "1058": {
             "fn": "ERC20._approve",
             "offset": [
                 10203,
                 10234
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x2D3"
+            "path": "1",
+            "value": "0x31B"
         },
-        "1052": {
+        "1061": {
             "op": "JUMP"
         },
-        "1053": {
+        "1062": {
             "fn": "ERC20._approve",
             "offset": [
                 10155,
                 10245
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1054": {
+        "1063": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1056": {
+        "1065": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1058": {
+        "1067": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1060": {
+        "1069": {
             "op": "SHL"
         },
-        "1061": {
+        "1070": {
             "op": "SUB"
         },
-        "1062": {
+        "1071": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "DUP1",
-            "path": "2",
+            "path": "1",
             "statement": 24
         },
-        "1063": {
+        "1072": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "1064": {
+        "1073": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1065": {
+        "1074": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "1067": {
+        "1076": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1068": {
+        "1077": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1069": {
+        "1078": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1070": {
+        "1079": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10265
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1"
         },
-        "1072": {
+        "1081": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "1074": {
+        "1083": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1075": {
+        "1084": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1076": {
+        "1085": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1077": {
+        "1086": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1079": {
+        "1088": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "1080": {
+        "1089": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "1081": {
+        "109": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
+        },
+        "1090": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10272
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "1082": {
+        "1091": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "SWAP4",
-            "path": "2"
+            "path": "1"
         },
-        "1083": {
+        "1092": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "DUP8",
-            "path": "2"
+            "path": "1"
         },
-        "1084": {
+        "1093": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1085": {
+        "1094": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "1086": {
+        "1095": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1087": {
+        "1096": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "SWAP3",
-            "path": "2"
+            "path": "1"
         },
-        "1088": {
+        "1097": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1089": {
+        "1098": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10281
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "109": {
+        "1099": {
+            "fn": "ERC20._approve",
+            "offset": [
+                10254,
+                10281
+            ],
+            "op": "KECCAK256",
+            "path": "1"
+        },
+        "11": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "EQ",
-            "path": "6"
+            "op": "JUMPI",
+            "path": "5"
         },
-        "1090": {
-            "fn": "ERC20._approve",
+        "110": {
+            "fn": null,
             "offset": [
-                10254,
-                10281
+                104,
+                260
             ],
-            "op": "KECCAK256",
-            "path": "2"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0xA3"
         },
-        "1091": {
+        "1100": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10289
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1092": {
+        "1101": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10289
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1093": {
+        "1102": {
             "fn": "ERC20._approve",
             "offset": [
                 10254,
                 10289
             ],
             "op": "SSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1094": {
+        "1103": {
             "fn": "ERC20._approve",
             "offset": [
                 10299,
                 10375
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "1095": {
+        "1104": {
             "fn": "ERC20._approve",
             "offset": [
                 10299,
                 10375
             ],
             "op": "ISZERO",
-            "path": "2"
+            "path": "1"
         },
-        "1096": {
+        "1105": {
             "fn": "ERC20._approve",
             "offset": [
                 10299,
                 10375
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x364"
+            "path": "1",
+            "value": "0x333"
         },
-        "1099": {
+        "1108": {
             "fn": "ERC20._approve",
             "offset": [
                 10299,
                 10375
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "11": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "JUMPI",
-            "path": "6"
-        },
-        "110": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0xA3"
-        },
-        "1100": {
+        "1109": {
             "fn": "ERC20._approve",
             "offset": [
                 10349,
                 10356
             ],
             "op": "DUP3",
-            "path": "2",
+            "path": "1",
             "statement": 25
         },
-        "1101": {
+        "1110": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1103": {
+        "1112": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1105": {
+        "1114": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1107": {
+        "1116": {
             "op": "SHL"
         },
-        "1108": {
+        "1117": {
             "op": "SUB"
         },
-        "1109": {
+        "1118": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1110": {
+        "1119": {
             "fn": "ERC20._approve",
             "offset": [
                 10342,
                 10347
             ],
             "op": "DUP5",
-            "path": "2"
+            "path": "1"
         },
-        "1111": {
+        "1120": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1113": {
+        "1122": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1115": {
+        "1124": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1117": {
+        "1126": {
             "op": "SHL"
         },
-        "1118": {
+        "1127": {
             "op": "SUB"
         },
-        "1119": {
+        "1128": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1120": {
+        "1129": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "PUSH32",
-            "path": "2",
+            "path": "1",
             "value": "0x8C5BE1E5EBEC7D5BD14F71427D1E84F3DD0314C0F7B2291E5B200AC8C7C3B925"
         },
         "113": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "JUMPI",
-            "path": "6"
+            "path": "5"
         },
         "114": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "DUP1",
-            "path": "6"
+            "path": "5"
         },
         "115": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "PUSH4",
-            "path": "6",
+            "path": "5",
             "value": "0x95EA7B3"
         },
-        "1153": {
+        "1162": {
             "fn": "ERC20._approve",
             "offset": [
                 10358,
                 10363
             ],
             "op": "DUP5",
-            "path": "2"
+            "path": "1"
         },
-        "1154": {
+        "1163": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1156": {
+        "1165": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1157": {
+        "1166": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x490"
+            "path": "1",
+            "value": "0x499"
         },
-        "1160": {
+        "1169": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "1161": {
+        "1170": {
             "op": "DUP2"
         },
-        "1162": {
+        "1171": {
             "op": "MSTORE"
         },
-        "1163": {
+        "1172": {
             "op": "PUSH1",
             "value": "0x20"
         },
-        "1165": {
+        "1174": {
             "op": "ADD"
         },
-        "1166": {
+        "1175": {
             "op": "SWAP1"
         },
-        "1167": {
+        "1176": {
             "op": "JUMP"
         },
-        "1168": {
+        "1177": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1169": {
+        "1178": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1171": {
+        "1180": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1172": {
+        "1181": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "1173": {
+        "1182": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "1174": {
+        "1183": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "SUB",
-            "path": "2"
+            "path": "1"
         },
-        "1175": {
+        "1184": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1176": {
+        "1185": {
             "fn": "ERC20._approve",
             "offset": [
                 10333,
                 10364
             ],
             "op": "LOG3",
-            "path": "2"
+            "path": "1"
         },
-        "1177": {
+        "1186": {
             "fn": "ERC20._approve",
             "offset": [
                 9949,
                 10381
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "1178": {
+        "1187": {
             "fn": "ERC20._approve",
             "offset": [
                 9949,
                 10381
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "1179": {
+        "1188": {
             "fn": "ERC20._approve",
             "offset": [
                 9949,
                 10381
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "1180": {
+        "1189": {
             "fn": "ERC20._approve",
             "offset": [
                 9949,
                 10381
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "1181": {
+        "1190": {
             "fn": "ERC20._approve",
             "jump": "o",
             "offset": [
                 9949,
                 10381
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "1182": {
+        "1191": {
             "fn": "ERC20._update",
             "offset": [
                 6271,
                 7378
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1183": {
+        "1192": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1185": {
+        "1194": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1187": {
+        "1196": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1189": {
+        "1198": {
             "op": "SHL"
         },
-        "1190": {
+        "1199": {
             "op": "SUB"
         },
-        "1191": {
+        "12": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH1",
+            "path": "5",
+            "value": "0x0"
+        },
+        "120": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
+        },
+        "1200": {
             "fn": "ERC20._update",
             "offset": [
                 6360,
                 6378
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "1192": {
+        "1201": {
             "branch": 39,
             "fn": "ERC20._update",
             "offset": [
                 6360,
                 6378
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1193": {
+        "1202": {
             "fn": "ERC20._update",
             "offset": [
                 6356,
                 6896
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x4C9"
+            "path": "1",
+            "value": "0x4D2"
         },
-        "1196": {
+        "1205": {
             "branch": 39,
             "fn": "ERC20._update",
             "offset": [
                 6356,
                 6896
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "1197": {
+        "1206": {
             "fn": "ERC20._update",
             "offset": [
                 6512,
                 6517
             ],
             "op": "DUP1",
-            "path": "2",
+            "path": "1",
             "statement": 26
         },
-        "1198": {
+        "1207": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6508
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x2"
         },
-        "12": {
-            "fn": null,
+        "1209": {
+            "fn": "ERC20._update",
             "offset": [
-                104,
-                343
+                6496,
+                6508
             ],
             "op": "PUSH1",
-            "path": "6",
+            "path": "1",
             "value": "0x0"
         },
-        "120": {
+        "121": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "EQ",
-            "path": "6"
-        },
-        "1200": {
-            "fn": "ERC20._update",
-            "offset": [
-                6496,
-                6508
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x0"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0xC1"
         },
-        "1202": {
+        "1211": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1203": {
+        "1212": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1204": {
+        "1213": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1205": {
+        "1214": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x4BE"
+            "path": "1",
+            "value": "0x4C7"
         },
-        "1208": {
+        "1217": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "1209": {
+        "1218": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "SWAP1",
-            "path": "2"
-        },
-        "121": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0xC1"
+            "path": "1"
         },
-        "1210": {
+        "1219": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x728"
+            "path": "1",
+            "value": "0x74A"
         },
-        "1213": {
+        "1222": {
             "fn": "ERC20._update",
             "jump": "i",
             "offset": [
                 6496,
                 6517
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "1214": {
+        "1223": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1215": {
+        "1224": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1216": {
+        "1225": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "1217": {
+        "1226": {
             "fn": "ERC20._update",
             "offset": [
                 6496,
                 6517
             ],
             "op": "SSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1218": {
+        "1227": {
             "op": "POP"
         },
-        "1219": {
+        "1228": {
             "fn": "ERC20._update",
             "offset": [
                 6356,
                 6896
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x53B"
+            "path": "1",
+            "value": "0x544"
         },
-        "1222": {
+        "1231": {
             "fn": "ERC20._update",
             "offset": [
                 6356,
                 6896
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1223": {
+        "1232": {
             "op": "POP"
         },
-        "1224": {
+        "1233": {
             "fn": "ERC20._update",
             "offset": [
                 6356,
                 6896
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "1225": {
+        "1234": {
             "fn": "ERC20._update",
             "offset": [
                 6356,
                 6896
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1226": {
+        "1235": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1228": {
+        "1237": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1230": {
+        "1239": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1232": {
+        "124": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "JUMPI",
+            "path": "5"
+        },
+        "1241": {
             "op": "SHL"
         },
-        "1233": {
+        "1242": {
             "op": "SUB"
         },
-        "1234": {
+        "1243": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "1235": {
+        "1244": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1236": {
+        "1245": {
             "fn": "ERC20._update",
             "offset": [
                 6548,
                 6567
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "1238": {
+        "1247": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1239": {
+        "1248": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "124": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "JUMPI",
-            "path": "6"
-        },
-        "1240": {
+        "1249": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1241": {
+        "125": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "DUP1",
+            "path": "5"
+        },
+        "1250": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "1243": {
+        "1252": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1244": {
+        "1253": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1245": {
+        "1254": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1246": {
+        "1255": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1248": {
+        "1257": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1249": {
+        "1258": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "KECCAK256",
-            "path": "2"
-        },
-        "125": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "DUP1",
-            "path": "6"
+            "path": "1"
         },
-        "1250": {
+        "1259": {
             "fn": "ERC20._update",
             "offset": [
                 6570,
                 6585
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1251": {
+        "126": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0x18160DDD"
+        },
+        "1260": {
             "fn": "ERC20._update",
             "offset": [
                 6603,
                 6622
             ],
             "op": "DUP2",
-            "path": "2",
+            "path": "1",
             "statement": 27
         },
-        "1252": {
+        "1261": {
             "fn": "ERC20._update",
             "offset": [
                 6603,
                 6622
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1253": {
+        "1262": {
             "branch": 40,
             "fn": "ERC20._update",
             "offset": [
                 6603,
                 6622
             ],
             "op": "LT",
-            "path": "2"
+            "path": "1"
         },
-        "1254": {
+        "1263": {
             "fn": "ERC20._update",
             "offset": [
                 6599,
                 6714
             ],
             "op": "ISZERO",
-            "path": "2"
+            "path": "1"
         },
-        "1255": {
+        "1264": {
             "fn": "ERC20._update",
             "offset": [
                 6599,
                 6714
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x51C"
+            "path": "1",
+            "value": "0x525"
         },
-        "1258": {
+        "1267": {
             "branch": 40,
             "fn": "ERC20._update",
             "offset": [
                 6599,
                 6714
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "1259": {
+        "1268": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "126": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x1249C58B"
-        },
-        "1261": {
+        "1270": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1262": {
+        "1271": {
             "op": "PUSH4",
             "value": "0x391434E3"
         },
-        "1267": {
+        "1276": {
             "op": "PUSH1",
             "value": "0xE2"
         },
-        "1269": {
+        "1278": {
             "op": "SHL"
         },
-        "1270": {
+        "1279": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1271": {
+        "1280": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1272": {
+        "1281": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1274": {
+        "1283": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1276": {
+        "1285": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1278": {
+        "1287": {
             "op": "SHL"
         },
-        "1279": {
+        "1288": {
             "op": "SUB"
         },
-        "1280": {
+        "1289": {
             "op": "DUP6"
         },
-        "1281": {
+        "1290": {
             "op": "AND"
         },
-        "1282": {
+        "1291": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "1284": {
+        "1293": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1285": {
+        "1294": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "1286": {
+        "1295": {
             "op": "MSTORE"
         },
-        "1287": {
+        "1296": {
             "op": "PUSH1",
             "value": "0x24"
         },
-        "1289": {
+        "1298": {
             "op": "DUP2"
         },
-        "1290": {
+        "1299": {
             "op": "ADD"
         },
-        "1291": {
+        "1300": {
             "op": "DUP3"
         },
-        "1292": {
+        "1301": {
             "op": "SWAP1"
         },
-        "1293": {
+        "1302": {
             "op": "MSTORE"
         },
-        "1294": {
+        "1303": {
             "op": "PUSH1",
             "value": "0x44"
         },
-        "1296": {
+        "1305": {
             "op": "DUP2"
         },
-        "1297": {
+        "1306": {
             "op": "ADD"
         },
-        "1298": {
+        "1307": {
             "op": "DUP4"
         },
-        "1299": {
+        "1308": {
             "op": "SWAP1"
         },
-        "1300": {
+        "1309": {
             "op": "MSTORE"
         },
-        "1301": {
+        "131": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
+        },
+        "1310": {
             "op": "PUSH1",
             "value": "0x64"
         },
-        "1303": {
+        "1312": {
             "op": "ADD"
         },
-        "1304": {
+        "1313": {
             "fn": "ERC20._update",
             "offset": [
                 6649,
                 6699
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x2D3"
+            "path": "1",
+            "value": "0x31B"
         },
-        "1307": {
+        "1316": {
             "op": "JUMP"
         },
-        "1308": {
+        "1317": {
             "fn": "ERC20._update",
             "offset": [
                 6599,
                 6714
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1309": {
+        "1318": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "131": {
+        "132": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "EQ",
-            "path": "6"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0xE4"
         },
-        "1311": {
+        "1320": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1313": {
+        "1322": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1315": {
+        "1324": {
             "op": "SHL"
         },
-        "1316": {
+        "1325": {
             "op": "SUB"
         },
-        "1317": {
+        "1326": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "DUP5",
-            "path": "2",
+            "path": "1",
             "statement": 28
         },
-        "1318": {
+        "1327": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1319": {
+        "1328": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6843
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "132": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0xE4"
-        },
-        "1321": {
+        "1330": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1322": {
+        "1331": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1323": {
+        "1332": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1324": {
+        "1333": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "1326": {
+        "1335": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1327": {
+        "1336": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1328": {
+        "1337": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1329": {
+        "1338": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1331": {
+        "1340": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1332": {
+        "1341": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6849
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "1333": {
+        "1342": {
             "fn": "ERC20._update",
             "offset": [
                 6852,
                 6871
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1334": {
+        "1343": {
             "fn": "ERC20._update",
             "offset": [
                 6852,
                 6871
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1335": {
+        "1344": {
             "fn": "ERC20._update",
             "offset": [
                 6852,
                 6871
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1336": {
+        "1345": {
             "fn": "ERC20._update",
             "offset": [
                 6852,
                 6871
             ],
             "op": "SUB",
-            "path": "2"
+            "path": "1"
         },
-        "1337": {
+        "1346": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6871
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1338": {
+        "1347": {
             "fn": "ERC20._update",
             "offset": [
                 6834,
                 6871
             ],
             "op": "SSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1339": {
+        "1348": {
             "fn": "ERC20._update",
             "offset": [
                 6356,
                 6896
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1340": {
+        "1349": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1342": {
+        "135": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "JUMPI",
+            "path": "5"
+        },
+        "1351": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1344": {
+        "1353": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1346": {
+        "1355": {
             "op": "SHL"
         },
-        "1347": {
+        "1356": {
             "op": "SUB"
         },
-        "1348": {
+        "1357": {
             "fn": "ERC20._update",
             "offset": [
                 6910,
                 6926
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1349": {
+        "1358": {
             "branch": 41,
             "fn": "ERC20._update",
             "offset": [
                 6910,
                 6926
             ],
             "op": "AND",
-            "path": "2"
-        },
-        "135": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "JUMPI",
-            "path": "6"
+            "path": "1"
         },
-        "1350": {
+        "1359": {
             "fn": "ERC20._update",
             "offset": [
                 6906,
                 7331
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x557"
+            "path": "1",
+            "value": "0x560"
         },
-        "1353": {
+        "136": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "DUP1",
+            "path": "5"
+        },
+        "1362": {
             "branch": 41,
             "fn": "ERC20._update",
             "offset": [
                 6906,
                 7331
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "1354": {
+        "1363": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7085
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "statement": 29,
             "value": "0x2"
         },
-        "1356": {
+        "1365": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7094
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "1357": {
+        "1366": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7094
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1358": {
+        "1367": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7094
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1359": {
+        "1368": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7094
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "136": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "DUP1",
-            "path": "6"
-        },
-        "1360": {
+        "1369": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7094
             ],
             "op": "SUB",
-            "path": "2"
+            "path": "1"
         },
-        "1361": {
+        "137": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0x23B872DD"
+        },
+        "1370": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7094
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1362": {
+        "1371": {
             "fn": "ERC20._update",
             "offset": [
                 7073,
                 7094
             ],
             "op": "SSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1363": {
+        "1372": {
             "fn": "ERC20._update",
             "offset": [
                 6906,
                 7331
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x576"
+            "path": "1",
+            "value": "0x57F"
         },
-        "1366": {
+        "1375": {
             "fn": "ERC20._update",
             "offset": [
                 6906,
                 7331
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "1367": {
+        "1376": {
             "fn": "ERC20._update",
             "offset": [
                 6906,
                 7331
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1368": {
+        "1377": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "137": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x18160DDD"
-        },
-        "1370": {
+        "1379": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1372": {
+        "1381": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1374": {
+        "1383": {
             "op": "SHL"
         },
-        "1375": {
+        "1384": {
             "op": "SUB"
         },
-        "1376": {
+        "1385": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "DUP3",
-            "path": "2",
+            "path": "1",
             "statement": 30
         },
-        "1377": {
+        "1386": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1378": {
+        "1387": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7293
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "1380": {
+        "1389": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1381": {
+        "1390": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1382": {
+        "1391": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1383": {
+        "1392": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "1385": {
+        "1394": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "1386": {
+        "1395": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1387": {
+        "1396": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1388": {
+        "1397": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1390": {
+        "1399": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1391": {
+        "14": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "DUP1",
+            "path": "5"
+        },
+        "1400": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7297
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "1392": {
+        "1401": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7306
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "1393": {
+        "1402": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7306
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1394": {
+        "1403": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7306
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "1395": {
+        "1404": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7306
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "1396": {
+        "1405": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7306
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1397": {
+        "1406": {
             "fn": "ERC20._update",
             "offset": [
                 7284,
                 7306
             ],
             "op": "SSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "1398": {
+        "1407": {
             "fn": "ERC20._update",
             "offset": [
                 6906,
                 7331
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1399": {
+        "1408": {
             "fn": "ERC20._update",
             "offset": [
                 7361,
                 7363
             ],
             "op": "DUP2",
-            "path": "2",
+            "path": "1",
             "statement": 31
         },
-        "14": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "DUP1",
-            "path": "6"
-        },
-        "1400": {
+        "1409": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1402": {
+        "1411": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1404": {
+        "1413": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1406": {
+        "1415": {
             "op": "SHL"
         },
-        "1407": {
+        "1416": {
             "op": "SUB"
         },
-        "1408": {
+        "1417": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1409": {
+        "1418": {
             "fn": "ERC20._update",
             "offset": [
                 7355,
                 7359
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "1410": {
+        "1419": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1412": {
+        "142": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
+        },
+        "1421": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "1414": {
+        "1423": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "1416": {
+        "1425": {
             "op": "SHL"
         },
-        "1417": {
+        "1426": {
             "op": "SUB"
         },
-        "1418": {
+        "1427": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "1419": {
+        "1428": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "PUSH32",
-            "path": "2",
+            "path": "1",
             "value": "0xDDF252AD1BE2C89B69C2B068FC378DAA952BA7F163C4A11628F55A4DF523B3EF"
         },
-        "142": {
+        "143": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "EQ",
-            "path": "6"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0xF6"
         },
-        "143": {
+        "146": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0xEE"
+            "op": "JUMPI",
+            "path": "5"
         },
-        "1452": {
+        "1461": {
             "fn": "ERC20._update",
             "offset": [
                 7365,
                 7370
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "1453": {
+        "1462": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1455": {
+        "1464": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1456": {
+        "1465": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x5BB"
+            "path": "1",
+            "value": "0x5C4"
         },
-        "1459": {
+        "1468": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "146": {
+        "1469": {
+            "op": "DUP2"
+        },
+        "147": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "JUMPI",
-            "path": "6"
-        },
-        "1460": {
-            "op": "DUP2"
+            "op": "DUP1",
+            "path": "5"
         },
-        "1461": {
+        "1470": {
             "op": "MSTORE"
         },
-        "1462": {
+        "1471": {
             "op": "PUSH1",
             "value": "0x20"
         },
-        "1464": {
+        "1473": {
             "op": "ADD"
         },
-        "1465": {
+        "1474": {
             "op": "SWAP1"
         },
-        "1466": {
+        "1475": {
             "op": "JUMP"
         },
-        "1467": {
+        "1476": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1468": {
+        "1477": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "147": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "DUP1",
-            "path": "6"
-        },
-        "1470": {
+        "1479": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "1471": {
+        "148": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0x313CE567"
+        },
+        "1480": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "1472": {
+        "1481": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "1473": {
+        "1482": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "SUB",
-            "path": "2"
+            "path": "1"
         },
-        "1474": {
+        "1483": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "1475": {
+        "1484": {
             "fn": "ERC20._update",
             "offset": [
                 7346,
                 7371
             ],
             "op": "LOG3",
-            "path": "2"
+            "path": "1"
         },
-        "1476": {
+        "1485": {
             "fn": "ERC20._update",
             "offset": [
                 6271,
                 7378
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "1477": {
+        "1486": {
             "fn": "ERC20._update",
             "offset": [
                 6271,
                 7378
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "1478": {
+        "1487": {
             "fn": "ERC20._update",
             "offset": [
                 6271,
                 7378
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "1479": {
+        "1488": {
             "fn": "ERC20._update",
             "jump": "o",
             "offset": [
                 6271,
                 7378
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "148": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x23B872DD"
-        },
-        "1480": {
+        "1489": {
             "op": "JUMPDEST"
         },
-        "1481": {
+        "1490": {
             "op": "PUSH1",
             "value": "0x0"
         },
-        "1483": {
+        "1492": {
             "op": "PUSH1",
             "value": "0x20"
         },
-        "1485": {
+        "1494": {
             "op": "DUP1"
         },
-        "1486": {
+        "1495": {
             "op": "DUP4"
         },
-        "1487": {
+        "1496": {
             "op": "MSTORE"
         },
-        "1488": {
+        "1497": {
             "op": "DUP4"
         },
-        "1489": {
+        "1498": {
             "op": "MLOAD"
         },
-        "1490": {
+        "1499": {
             "op": "DUP1"
         },
-        "1491": {
+        "15": {
+            "dev": "Cannot send ether to nonpayable function",
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "REVERT",
+            "path": "5"
+        },
+        "1500": {
             "op": "PUSH1",
             "value": "0x20"
         },
-        "1493": {
+        "1502": {
             "op": "DUP6"
         },
-        "1494": {
+        "1503": {
             "op": "ADD"
         },
-        "1495": {
+        "1504": {
             "op": "MSTORE"
         },
-        "1496": {
+        "1505": {
             "op": "PUSH1",
             "value": "0x0"
         },
-        "1498": {
+        "1507": {
             "op": "JUMPDEST"
         },
-        "1499": {
+        "1508": {
             "op": "DUP2"
         },
-        "15": {
-            "dev": "Cannot send ether to nonpayable function",
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "REVERT",
-            "path": "6"
-        },
-        "1500": {
+        "1509": {
             "op": "DUP2"
         },
-        "1501": {
+        "1510": {
             "op": "LT"
         },
-        "1502": {
+        "1511": {
             "op": "ISZERO"
         },
-        "1503": {
+        "1512": {
             "op": "PUSH2",
-            "value": "0x5F6"
+            "value": "0x5FF"
         },
-        "1506": {
+        "1515": {
             "op": "JUMPI"
         },
-        "1507": {
+        "1516": {
             "op": "DUP6"
         },
-        "1508": {
+        "1517": {
             "op": "DUP2"
         },
-        "1509": {
+        "1518": {
             "op": "ADD"
         },
-        "1510": {
+        "1519": {
             "op": "DUP4"
         },
-        "1511": {
+        "1520": {
             "op": "ADD"
         },
-        "1512": {
+        "1521": {
             "op": "MLOAD"
         },
-        "1513": {
+        "1522": {
             "op": "DUP6"
         },
-        "1514": {
+        "1523": {
             "op": "DUP3"
         },
-        "1515": {
+        "1524": {
             "op": "ADD"
         },
-        "1516": {
+        "1525": {
             "op": "PUSH1",
             "value": "0x40"
         },
-        "1518": {
+        "1527": {
             "op": "ADD"
         },
-        "1519": {
+        "1528": {
             "op": "MSTORE"
         },
-        "1520": {
+        "1529": {
             "op": "DUP3"
         },
-        "1521": {
+        "153": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
+        },
+        "1530": {
             "op": "ADD"
         },
-        "1522": {
+        "1531": {
             "op": "PUSH2",
-            "value": "0x5DA"
+            "value": "0x5E3"
         },
-        "1525": {
+        "1534": {
             "op": "JUMP"
         },
-        "1526": {
+        "1535": {
             "op": "JUMPDEST"
         },
-        "1527": {
+        "1536": {
             "op": "POP"
         },
-        "1528": {
+        "1537": {
             "op": "PUSH1",
             "value": "0x0"
         },
-        "153": {
+        "1539": {
+            "op": "PUSH1",
+            "value": "0x40"
+        },
+        "154": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "EQ",
-            "path": "6"
-        },
-        "1530": {
-            "op": "PUSH1",
-            "value": "0x40"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x109"
         },
-        "1532": {
+        "1541": {
             "op": "DUP3"
         },
-        "1533": {
+        "1542": {
             "op": "DUP7"
         },
-        "1534": {
+        "1543": {
             "op": "ADD"
         },
-        "1535": {
+        "1544": {
             "op": "ADD"
         },
-        "1536": {
+        "1545": {
             "op": "MSTORE"
         },
-        "1537": {
+        "1546": {
             "op": "PUSH1",
             "value": "0x40"
         },
-        "1539": {
+        "1548": {
             "op": "PUSH1",
             "value": "0x1F"
         },
-        "154": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x100"
-        },
-        "1541": {
+        "1550": {
             "op": "NOT"
         },
-        "1542": {
+        "1551": {
             "op": "PUSH1",
             "value": "0x1F"
         },
-        "1544": {
+        "1553": {
             "op": "DUP4"
         },
-        "1545": {
+        "1554": {
             "op": "ADD"
         },
-        "1546": {
+        "1555": {
             "op": "AND"
         },
-        "1547": {
+        "1556": {
             "op": "DUP6"
         },
-        "1548": {
+        "1557": {
             "op": "ADD"
         },
-        "1549": {
+        "1558": {
             "op": "ADD"
         },
-        "1550": {
+        "1559": {
             "op": "SWAP3"
         },
-        "1551": {
+        "1560": {
             "op": "POP"
         },
-        "1552": {
+        "1561": {
             "op": "POP"
         },
-        "1553": {
+        "1562": {
             "op": "POP"
         },
-        "1554": {
+        "1563": {
             "op": "SWAP3"
         },
-        "1555": {
+        "1564": {
             "op": "SWAP2"
         },
-        "1556": {
+        "1565": {
             "op": "POP"
         },
-        "1557": {
+        "1566": {
             "op": "POP"
         },
-        "1558": {
+        "1567": {
             "jump": "o",
             "op": "JUMP"
         },
-        "1559": {
-            "op": "JUMPDEST"
-        },
-        "1560": {
-            "op": "DUP1"
-        },
-        "1561": {
-            "op": "CALLDATALOAD"
-        },
-        "1562": {
-            "op": "PUSH1",
-            "value": "0x1"
-        },
-        "1564": {
-            "op": "PUSH1",
-            "value": "0x1"
-        },
-        "1566": {
-            "op": "PUSH1",
-            "value": "0xA0"
-        },
         "1568": {
-            "op": "SHL"
+            "op": "JUMPDEST"
         },
         "1569": {
-            "op": "SUB"
+            "op": "DUP1"
         },
         "157": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "JUMPI",
-            "path": "6"
+            "path": "5"
         },
         "1570": {
-            "op": "DUP2"
+            "op": "CALLDATALOAD"
         },
         "1571": {
-            "op": "AND"
-        },
-        "1572": {
-            "op": "DUP2"
+            "op": "PUSH1",
+            "value": "0x1"
         },
         "1573": {
-            "op": "EQ"
+            "op": "PUSH1",
+            "value": "0x1"
         },
-        "1574": {
-            "op": "PUSH2",
-            "value": "0x62E"
+        "1575": {
+            "op": "PUSH1",
+            "value": "0xA0"
         },
         "1577": {
-            "op": "JUMPI"
+            "op": "SHL"
         },
         "1578": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "SUB"
+        },
+        "1579": {
+            "op": "DUP2"
         },
         "158": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "JUMPDEST",
-            "path": "6"
+            "path": "5"
         },
         "1580": {
-            "op": "DUP1"
+            "op": "AND"
         },
         "1581": {
-            "op": "REVERT"
+            "op": "DUP2"
         },
         "1582": {
-            "op": "JUMPDEST"
+            "op": "EQ"
         },
         "1583": {
-            "op": "SWAP2"
-        },
-        "1584": {
-            "op": "SWAP1"
-        },
-        "1585": {
-            "op": "POP"
+            "op": "PUSH2",
+            "value": "0x637"
         },
         "1586": {
-            "jump": "o",
-            "op": "JUMP"
+            "op": "JUMPI"
         },
         "1587": {
-            "op": "JUMPDEST"
-        },
-        "1588": {
             "op": "PUSH1",
             "value": "0x0"
         },
+        "1589": {
+            "op": "DUP1"
+        },
         "159": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "PUSH1",
-            "path": "6",
+            "path": "5",
             "value": "0x0"
         },
         "1590": {
-            "op": "DUP1"
+            "op": "REVERT"
         },
         "1591": {
-            "op": "PUSH1",
-            "value": "0x40"
+            "op": "JUMPDEST"
+        },
+        "1592": {
+            "op": "SWAP2"
         },
         "1593": {
-            "op": "DUP4"
+            "op": "SWAP1"
         },
         "1594": {
-            "op": "DUP6"
+            "op": "POP"
         },
         "1595": {
-            "op": "SUB"
+            "jump": "o",
+            "op": "JUMP"
         },
         "1596": {
-            "op": "SLT"
+            "op": "JUMPDEST"
         },
         "1597": {
-            "op": "ISZERO"
+            "op": "PUSH1",
+            "value": "0x0"
         },
-        "1598": {
-            "op": "PUSH2",
-            "value": "0x646"
+        "1599": {
+            "op": "DUP1"
         },
         "16": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "JUMPDEST",
-            "path": "6"
+            "path": "5"
         },
-        "1601": {
-            "op": "JUMPI"
+        "1600": {
+            "op": "PUSH1",
+            "value": "0x40"
         },
         "1602": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "DUP4"
+        },
+        "1603": {
+            "op": "DUP6"
         },
         "1604": {
-            "op": "DUP1"
+            "op": "SUB"
         },
         "1605": {
-            "op": "REVERT"
+            "op": "SLT"
         },
         "1606": {
-            "op": "JUMPDEST"
+            "op": "ISZERO"
         },
         "1607": {
             "op": "PUSH2",
             "value": "0x64F"
         },
         "161": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "DUP1",
-            "path": "6"
+            "path": "5"
         },
         "1610": {
-            "op": "DUP4"
+            "op": "JUMPI"
         },
         "1611": {
-            "op": "PUSH2",
-            "value": "0x617"
+            "op": "PUSH1",
+            "value": "0x0"
+        },
+        "1613": {
+            "op": "DUP1"
         },
         "1614": {
-            "jump": "i",
-            "op": "JUMP"
+            "op": "REVERT"
         },
         "1615": {
             "op": "JUMPDEST"
         },
         "1616": {
-            "op": "SWAP5"
-        },
-        "1617": {
-            "op": "PUSH1",
-            "value": "0x20"
+            "op": "PUSH2",
+            "value": "0x658"
         },
         "1619": {
-            "op": "SWAP4"
+            "op": "DUP4"
         },
         "162": {
             "first_revert": true,
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "REVERT",
-            "path": "6"
+            "path": "5"
         },
         "1620": {
-            "op": "SWAP1"
-        },
-        "1621": {
-            "op": "SWAP4"
-        },
-        "1622": {
-            "op": "ADD"
+            "op": "PUSH2",
+            "value": "0x620"
         },
         "1623": {
-            "op": "CALLDATALOAD"
+            "jump": "i",
+            "op": "JUMP"
         },
         "1624": {
-            "op": "SWAP4"
+            "op": "JUMPDEST"
         },
         "1625": {
-            "op": "POP"
+            "op": "SWAP5"
         },
         "1626": {
-            "op": "POP"
-        },
-        "1627": {
-            "op": "POP"
+            "op": "PUSH1",
+            "value": "0x20"
         },
         "1628": {
-            "jump": "o",
-            "op": "JUMP"
+            "op": "SWAP4"
         },
         "1629": {
-            "op": "JUMPDEST"
+            "op": "SWAP1"
         },
         "163": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
         "1630": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "SWAP4"
+        },
+        "1631": {
+            "op": "ADD"
         },
         "1632": {
-            "op": "DUP1"
+            "op": "CALLDATALOAD"
         },
         "1633": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "SWAP4"
+        },
+        "1634": {
+            "op": "POP"
         },
         "1635": {
-            "op": "PUSH1",
-            "value": "0x60"
+            "op": "POP"
+        },
+        "1636": {
+            "op": "POP"
         },
         "1637": {
-            "op": "DUP5"
+            "jump": "o",
+            "op": "JUMP"
         },
         "1638": {
-            "op": "DUP7"
+            "op": "JUMPDEST"
         },
         "1639": {
-            "op": "SUB"
+            "op": "PUSH1",
+            "value": "0x0"
         },
         "164": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xAB"
         },
-        "1640": {
-            "op": "SLT"
-        },
         "1641": {
-            "op": "ISZERO"
+            "op": "DUP1"
         },
         "1642": {
-            "op": "PUSH2",
-            "value": "0x672"
+            "op": "PUSH1",
+            "value": "0x0"
         },
-        "1645": {
-            "op": "JUMPI"
+        "1644": {
+            "op": "PUSH1",
+            "value": "0x60"
         },
         "1646": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "DUP5"
+        },
+        "1647": {
+            "op": "DUP7"
         },
         "1648": {
-            "op": "DUP1"
+            "op": "SUB"
         },
         "1649": {
-            "op": "REVERT"
+            "op": "SLT"
         },
         "1650": {
-            "op": "JUMPDEST"
+            "op": "ISZERO"
         },
         "1651": {
             "op": "PUSH2",
             "value": "0x67B"
         },
         "1654": {
-            "op": "DUP5"
+            "op": "JUMPI"
         },
         "1655": {
-            "op": "PUSH2",
-            "value": "0x617"
+            "op": "PUSH1",
+            "value": "0x0"
+        },
+        "1657": {
+            "op": "DUP1"
         },
         "1658": {
-            "jump": "i",
-            "op": "JUMP"
+            "op": "REVERT"
         },
         "1659": {
             "op": "JUMPDEST"
         },
         "1660": {
-            "op": "SWAP3"
+            "op": "PUSH2",
+            "value": "0x684"
         },
-        "1661": {
-            "op": "POP"
+        "1663": {
+            "op": "DUP5"
         },
-        "1662": {
+        "1664": {
             "op": "PUSH2",
-            "value": "0x689"
-        },
-        "1665": {
-            "op": "PUSH1",
-            "value": "0x20"
+            "value": "0x620"
         },
         "1667": {
-            "op": "DUP6"
+            "jump": "i",
+            "op": "JUMP"
         },
         "1668": {
-            "op": "ADD"
+            "op": "JUMPDEST"
         },
         "1669": {
-            "op": "PUSH2",
-            "value": "0x617"
+            "op": "SWAP3"
         },
         "167": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x19F"
+            "path": "1",
+            "value": "0x1AA"
         },
-        "1672": {
-            "jump": "i",
-            "op": "JUMP"
+        "1670": {
+            "op": "POP"
         },
-        "1673": {
-            "op": "JUMPDEST"
+        "1671": {
+            "op": "PUSH2",
+            "value": "0x692"
         },
         "1674": {
-            "op": "SWAP2"
-        },
-        "1675": {
-            "op": "POP"
-        },
-        "1676": {
             "op": "PUSH1",
-            "value": "0x40"
+            "value": "0x20"
         },
-        "1678": {
-            "op": "DUP5"
+        "1676": {
+            "op": "DUP6"
         },
-        "1679": {
+        "1677": {
             "op": "ADD"
         },
-        "1680": {
-            "op": "CALLDATALOAD"
+        "1678": {
+            "op": "PUSH2",
+            "value": "0x620"
         },
         "1681": {
-            "op": "SWAP1"
+            "jump": "i",
+            "op": "JUMP"
         },
         "1682": {
-            "op": "POP"
+            "op": "JUMPDEST"
         },
         "1683": {
-            "op": "SWAP3"
+            "op": "SWAP2"
         },
         "1684": {
             "op": "POP"
         },
         "1685": {
-            "op": "SWAP3"
-        },
-        "1686": {
-            "op": "POP"
+            "op": "PUSH1",
+            "value": "0x40"
         },
         "1687": {
-            "op": "SWAP3"
+            "op": "DUP5"
         },
         "1688": {
-            "jump": "o",
-            "op": "JUMP"
+            "op": "ADD"
         },
         "1689": {
-            "op": "JUMPDEST"
+            "op": "CALLDATALOAD"
         },
         "1690": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "SWAP1"
+        },
+        "1691": {
+            "op": "POP"
         },
         "1692": {
-            "op": "PUSH1",
-            "value": "0x20"
+            "op": "SWAP3"
+        },
+        "1693": {
+            "op": "POP"
         },
         "1694": {
-            "op": "DUP3"
+            "op": "SWAP3"
         },
         "1695": {
-            "op": "DUP5"
+            "op": "POP"
         },
         "1696": {
-            "op": "SUB"
+            "op": "SWAP3"
         },
         "1697": {
-            "op": "SLT"
+            "jump": "o",
+            "op": "JUMP"
         },
         "1698": {
-            "op": "ISZERO"
+            "op": "JUMPDEST"
         },
         "1699": {
-            "op": "PUSH2",
-            "value": "0x6AB"
+            "op": "PUSH1",
+            "value": "0x0"
         },
         "17": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "POP",
-            "path": "6"
+            "path": "5"
         },
         "170": {
             "fn": "ERC20.name",
             "jump": "i",
             "offset": [
                 2074,
                 2163
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "1702": {
-            "op": "JUMPI"
+        "1701": {
+            "op": "PUSH1",
+            "value": "0x20"
         },
         "1703": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "DUP3"
+        },
+        "1704": {
+            "op": "DUP5"
         },
         "1705": {
-            "op": "DUP1"
+            "op": "SUB"
         },
         "1706": {
-            "op": "REVERT"
+            "op": "SLT"
         },
         "1707": {
-            "op": "JUMPDEST"
+            "op": "ISZERO"
         },
         "1708": {
             "op": "PUSH2",
             "value": "0x6B4"
         },
         "171": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
         "1711": {
-            "op": "DUP3"
+            "op": "JUMPI"
         },
         "1712": {
-            "op": "PUSH2",
-            "value": "0x617"
+            "op": "PUSH1",
+            "value": "0x0"
+        },
+        "1714": {
+            "op": "DUP1"
         },
         "1715": {
-            "jump": "i",
-            "op": "JUMP"
+            "op": "REVERT"
         },
         "1716": {
             "op": "JUMPDEST"
         },
         "1717": {
-            "op": "SWAP4"
-        },
-        "1718": {
-            "op": "SWAP3"
-        },
-        "1719": {
-            "op": "POP"
+            "op": "PUSH2",
+            "value": "0x6BD"
         },
         "172": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
         "1720": {
-            "op": "POP"
+            "op": "DUP3"
         },
         "1721": {
-            "op": "POP"
+            "op": "PUSH2",
+            "value": "0x620"
         },
-        "1722": {
-            "jump": "o",
+        "1724": {
+            "jump": "i",
             "op": "JUMP"
         },
-        "1723": {
+        "1725": {
             "op": "JUMPDEST"
         },
-        "1724": {
-            "op": "PUSH1",
-            "value": "0x0"
-        },
         "1726": {
-            "op": "DUP1"
+            "op": "SWAP4"
         },
         "1727": {
-            "op": "PUSH1",
-            "value": "0x40"
+            "op": "SWAP3"
+        },
+        "1728": {
+            "op": "POP"
         },
         "1729": {
-            "op": "DUP4"
+            "op": "POP"
         },
         "1730": {
-            "op": "DUP6"
+            "op": "POP"
         },
         "1731": {
-            "op": "SUB"
+            "jump": "o",
+            "op": "JUMP"
         },
         "1732": {
-            "op": "SLT"
+            "op": "JUMPDEST"
         },
         "1733": {
-            "op": "ISZERO"
+            "op": "PUSH1",
+            "value": "0x0"
         },
-        "1734": {
-            "op": "PUSH2",
-            "value": "0x6CE"
+        "1735": {
+            "op": "PUSH1",
+            "value": "0x20"
         },
         "1737": {
-            "op": "JUMPI"
+            "op": "DUP3"
         },
         "1738": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "DUP5"
+        },
+        "1739": {
+            "op": "SUB"
         },
         "174": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
         "1740": {
-            "op": "DUP1"
+            "op": "SLT"
         },
         "1741": {
-            "op": "REVERT"
+            "op": "ISZERO"
         },
         "1742": {
-            "op": "JUMPDEST"
-        },
-        "1743": {
             "op": "PUSH2",
-            "value": "0x6D7"
+            "value": "0x6D6"
+        },
+        "1745": {
+            "op": "JUMPI"
         },
         "1746": {
-            "op": "DUP4"
+            "op": "PUSH1",
+            "value": "0x0"
         },
-        "1747": {
-            "op": "PUSH2",
-            "value": "0x617"
+        "1748": {
+            "op": "DUP1"
+        },
+        "1749": {
+            "op": "REVERT"
         },
         "175": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xB8"
         },
         "1750": {
-            "jump": "i",
-            "op": "JUMP"
+            "op": "JUMPDEST"
         },
         "1751": {
-            "op": "JUMPDEST"
+            "op": "POP"
         },
         "1752": {
-            "op": "SWAP2"
+            "op": "CALLDATALOAD"
         },
         "1753": {
-            "op": "POP"
+            "op": "SWAP2"
         },
         "1754": {
-            "op": "PUSH2",
-            "value": "0x6E5"
+            "op": "SWAP1"
+        },
+        "1755": {
+            "op": "POP"
+        },
+        "1756": {
+            "jump": "o",
+            "op": "JUMP"
         },
         "1757": {
-            "op": "PUSH1",
-            "value": "0x20"
+            "op": "JUMPDEST"
         },
-        "1759": {
-            "op": "DUP5"
+        "1758": {
+            "op": "PUSH1",
+            "value": "0x0"
         },
         "1760": {
-            "op": "ADD"
+            "op": "DUP1"
         },
         "1761": {
-            "op": "PUSH2",
-            "value": "0x617"
+            "op": "PUSH1",
+            "value": "0x40"
+        },
+        "1763": {
+            "op": "DUP4"
         },
         "1764": {
-            "jump": "i",
-            "op": "JUMP"
+            "op": "DUP6"
         },
         "1765": {
-            "op": "JUMPDEST"
+            "op": "SUB"
         },
         "1766": {
-            "op": "SWAP1"
+            "op": "SLT"
         },
         "1767": {
-            "op": "POP"
+            "op": "ISZERO"
         },
         "1768": {
-            "op": "SWAP3"
-        },
-        "1769": {
-            "op": "POP"
-        },
-        "1770": {
-            "op": "SWAP3"
+            "op": "PUSH2",
+            "value": "0x6F0"
         },
         "1771": {
-            "op": "SWAP1"
+            "op": "JUMPI"
         },
         "1772": {
-            "op": "POP"
-        },
-        "1773": {
-            "jump": "o",
-            "op": "JUMP"
+            "op": "PUSH1",
+            "value": "0x0"
         },
         "1774": {
-            "op": "JUMPDEST"
+            "op": "DUP1"
         },
         "1775": {
-            "op": "PUSH1",
-            "value": "0x1"
-        },
-        "1777": {
-            "op": "DUP2"
+            "op": "REVERT"
         },
-        "1778": {
-            "op": "DUP2"
+        "1776": {
+            "op": "JUMPDEST"
         },
-        "1779": {
-            "op": "SHR"
+        "1777": {
+            "op": "PUSH2",
+            "value": "0x6F9"
         },
         "178": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
         "1780": {
-            "op": "SWAP1"
+            "op": "DUP4"
         },
         "1781": {
-            "op": "DUP3"
+            "op": "PUSH2",
+            "value": "0x620"
         },
-        "1782": {
-            "op": "AND"
+        "1784": {
+            "jump": "i",
+            "op": "JUMP"
         },
-        "1783": {
-            "op": "DUP1"
+        "1785": {
+            "op": "JUMPDEST"
         },
-        "1784": {
-            "op": "PUSH2",
-            "value": "0x702"
+        "1786": {
+            "op": "SWAP2"
         },
         "1787": {
-            "op": "JUMPI"
+            "op": "POP"
         },
         "1788": {
-            "op": "PUSH1",
-            "value": "0x7F"
+            "op": "PUSH2",
+            "value": "0x707"
         },
         "179": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "SWAP1",
-            "path": "2"
-        },
-        "1790": {
-            "op": "DUP3"
+            "path": "1"
         },
         "1791": {
-            "op": "AND"
-        },
-        "1792": {
-            "op": "SWAP2"
+            "op": "PUSH1",
+            "value": "0x20"
         },
         "1793": {
-            "op": "POP"
+            "op": "DUP5"
         },
         "1794": {
-            "op": "JUMPDEST"
+            "op": "ADD"
         },
         "1795": {
-            "op": "PUSH1",
-            "value": "0x20"
-        },
-        "1797": {
-            "op": "DUP3"
+            "op": "PUSH2",
+            "value": "0x620"
         },
         "1798": {
-            "op": "LT"
+            "jump": "i",
+            "op": "JUMP"
         },
         "1799": {
-            "op": "DUP2"
+            "op": "JUMPDEST"
         },
         "18": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "PUSH1",
-            "path": "6",
+            "path": "5",
             "value": "0x4"
         },
         "180": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x5C8"
+            "path": "1",
+            "value": "0x5D1"
         },
         "1800": {
-            "op": "SUB"
+            "op": "SWAP1"
         },
         "1801": {
-            "op": "PUSH2",
-            "value": "0x722"
+            "op": "POP"
+        },
+        "1802": {
+            "op": "SWAP3"
+        },
+        "1803": {
+            "op": "POP"
         },
         "1804": {
-            "op": "JUMPI"
+            "op": "SWAP3"
         },
         "1805": {
-            "op": "PUSH4",
-            "value": "0x4E487B71"
+            "op": "SWAP1"
+        },
+        "1806": {
+            "op": "POP"
+        },
+        "1807": {
+            "jump": "o",
+            "op": "JUMP"
+        },
+        "1808": {
+            "op": "JUMPDEST"
         },
-        "1810": {
+        "1809": {
             "op": "PUSH1",
-            "value": "0xE0"
+            "value": "0x1"
+        },
+        "1811": {
+            "op": "DUP2"
         },
         "1812": {
-            "op": "SHL"
+            "op": "DUP2"
         },
         "1813": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "SHR"
+        },
+        "1814": {
+            "op": "SWAP1"
         },
         "1815": {
-            "op": "MSTORE"
+            "op": "DUP3"
         },
         "1816": {
-            "op": "PUSH1",
-            "value": "0x22"
+            "op": "AND"
         },
-        "1818": {
-            "op": "PUSH1",
-            "value": "0x4"
+        "1817": {
+            "op": "DUP1"
         },
-        "1820": {
-            "op": "MSTORE"
+        "1818": {
+            "op": "PUSH2",
+            "value": "0x724"
         },
         "1821": {
-            "op": "PUSH1",
-            "value": "0x24"
+            "op": "JUMPI"
         },
-        "1823": {
+        "1822": {
             "op": "PUSH1",
-            "value": "0x0"
+            "value": "0x7F"
+        },
+        "1824": {
+            "op": "DUP3"
         },
         "1825": {
-            "op": "REVERT"
+            "op": "AND"
         },
         "1826": {
-            "op": "JUMPDEST"
+            "op": "SWAP2"
         },
         "1827": {
             "op": "POP"
         },
         "1828": {
-            "op": "SWAP2"
+            "op": "JUMPDEST"
         },
         "1829": {
-            "op": "SWAP1"
+            "op": "PUSH1",
+            "value": "0x20"
         },
         "183": {
             "fn": "ERC20.name",
             "jump": "i",
             "offset": [
                 2074,
                 2163
             ],
             "op": "JUMP",
-            "path": "2"
-        },
-        "1830": {
-            "op": "POP"
+            "path": "1"
         },
         "1831": {
-            "jump": "o",
-            "op": "JUMP"
+            "op": "DUP3"
         },
         "1832": {
-            "op": "JUMPDEST"
+            "op": "LT"
         },
         "1833": {
-            "op": "DUP1"
+            "op": "DUP2"
         },
         "1834": {
-            "op": "DUP3"
+            "op": "SUB"
         },
         "1835": {
-            "op": "ADD"
-        },
-        "1836": {
-            "op": "DUP1"
-        },
-        "1837": {
-            "op": "DUP3"
+            "op": "PUSH2",
+            "value": "0x744"
         },
         "1838": {
-            "op": "GT"
+            "op": "JUMPI"
         },
         "1839": {
-            "op": "ISZERO"
+            "op": "PUSH4",
+            "value": "0x4E487B71"
         },
         "184": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "1840": {
-            "op": "PUSH2",
-            "value": "0x245"
+        "1844": {
+            "op": "PUSH1",
+            "value": "0xE0"
         },
-        "1843": {
-            "op": "JUMPI"
+        "1846": {
+            "op": "SHL"
         },
-        "1844": {
-            "op": "PUSH4",
-            "value": "0x4E487B71"
+        "1847": {
+            "op": "PUSH1",
+            "value": "0x0"
         },
         "1849": {
-            "op": "PUSH1",
-            "value": "0xE0"
+            "op": "MSTORE"
         },
         "185": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "1851": {
-            "op": "SHL"
+        "1850": {
+            "op": "PUSH1",
+            "value": "0x22"
         },
         "1852": {
             "op": "PUSH1",
-            "value": "0x0"
+            "value": "0x4"
         },
         "1854": {
             "op": "MSTORE"
         },
         "1855": {
             "op": "PUSH1",
-            "value": "0x11"
+            "value": "0x24"
         },
         "1857": {
             "op": "PUSH1",
-            "value": "0x4"
+            "value": "0x0"
         },
         "1859": {
-            "op": "MSTORE"
+            "op": "REVERT"
         },
         "1860": {
-            "op": "PUSH1",
-            "value": "0x24"
+            "op": "JUMPDEST"
+        },
+        "1861": {
+            "op": "POP"
         },
         "1862": {
-            "op": "PUSH1",
-            "value": "0x0"
+            "op": "SWAP2"
+        },
+        "1863": {
+            "op": "SWAP1"
         },
         "1864": {
-            "op": "REVERT"
+            "op": "POP"
+        },
+        "1865": {
+            "jump": "o",
+            "op": "JUMP"
+        },
+        "1866": {
+            "op": "JUMPDEST"
+        },
+        "1867": {
+            "op": "DUP1"
+        },
+        "1868": {
+            "op": "DUP3"
+        },
+        "1869": {
+            "op": "ADD"
         },
         "187": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
+        },
+        "1870": {
+            "op": "DUP1"
+        },
+        "1871": {
+            "op": "DUP3"
+        },
+        "1872": {
+            "op": "GT"
+        },
+        "1873": {
+            "op": "ISZERO"
+        },
+        "1874": {
+            "op": "PUSH2",
+            "value": "0x250"
+        },
+        "1877": {
+            "op": "JUMPI"
+        },
+        "1878": {
+            "op": "PUSH4",
+            "value": "0x4E487B71"
         },
         "188": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
+        },
+        "1883": {
+            "op": "PUSH1",
+            "value": "0xE0"
+        },
+        "1885": {
+            "op": "SHL"
+        },
+        "1886": {
+            "op": "PUSH1",
+            "value": "0x0"
+        },
+        "1888": {
+            "op": "MSTORE"
+        },
+        "1889": {
+            "op": "PUSH1",
+            "value": "0x11"
         },
         "189": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
+        },
+        "1891": {
+            "op": "PUSH1",
+            "value": "0x4"
+        },
+        "1893": {
+            "op": "MSTORE"
+        },
+        "1894": {
+            "op": "PUSH1",
+            "value": "0x24"
+        },
+        "1896": {
+            "op": "PUSH1",
+            "value": "0x0"
+        },
+        "1898": {
+            "op": "REVERT"
         },
         "190": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "SUB",
-            "path": "2"
+            "path": "1"
         },
         "191": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
         "192": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "RETURN",
-            "path": "2"
+            "path": "1"
         },
         "193": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
         "194": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xD4"
         },
         "197": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xCF"
         },
         "2": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "PUSH1",
-            "path": "6",
+            "path": "5",
             "value": "0x40"
         },
         "20": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "CALLDATASIZE",
-            "path": "6"
+            "path": "5"
         },
         "200": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "CALLDATASIZE",
-            "path": "2"
+            "path": "1"
         },
         "201": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
         "203": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x633"
+            "path": "1",
+            "value": "0x63C"
         },
         "206": {
             "fn": "ERC20.approve",
             "jump": "i",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
         "207": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
         "208": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x231"
+            "path": "1",
+            "value": "0x23C"
         },
         "21": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "LT",
-            "path": "6"
+            "path": "5"
         },
         "211": {
             "fn": "ERC20.approve",
             "jump": "i",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
         "212": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
         "213": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
         "215": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
         "216": {
             "op": "SWAP1"
         },
         "217": {
             "op": "ISZERO"
         },
@@ -5108,18 +5071,18 @@
         "219": {
             "op": "DUP2"
         },
         "22": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "PUSH2",
-            "path": "6",
+            "path": "5",
             "value": "0x9E"
         },
         "220": {
             "op": "MSTORE"
         },
         "221": {
             "op": "PUSH1",
@@ -5131,4841 +5094,4862 @@
         "224": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xB8"
         },
         "227": {
             "op": "JUMP"
         },
         "228": {
-            "fn": "USDC.mint",
-            "offset": [
-                178,
-                251
-            ],
-            "op": "JUMPDEST",
-            "path": "6"
-        },
-        "229": {
-            "fn": "USDC.mint",
-            "offset": [
-                178,
-                251
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0xEC"
-        },
-        "232": {
-            "fn": "USDC.mint",
-            "offset": [
-                178,
-                251
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x24B"
-        },
-        "235": {
-            "fn": "USDC.mint",
-            "jump": "i",
-            "offset": [
-                178,
-                251
-            ],
-            "op": "JUMP",
-            "path": "6"
-        },
-        "236": {
-            "fn": "USDC.mint",
-            "offset": [
-                178,
-                251
-            ],
-            "op": "JUMPDEST",
-            "path": "6"
-        },
-        "237": {
-            "fn": "USDC.mint",
-            "offset": [
-                178,
-                251
-            ],
-            "op": "STOP",
-            "path": "6"
-        },
-        "238": {
             "fn": "ERC20.totalSupply",
             "offset": [
                 3144,
                 3241
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "239": {
+        "229": {
             "fn": "ERC20.totalSupply",
             "offset": [
                 3222,
                 3234
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "statement": 0,
             "value": "0x2"
         },
-        "241": {
+        "231": {
             "fn": "ERC20.totalSupply",
             "offset": [
                 3222,
                 3234
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "242": {
+        "232": {
             "fn": "ERC20.totalSupply",
             "offset": [
                 3144,
                 3241
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "243": {
+        "233": {
             "fn": "ERC20.totalSupply",
             "offset": [
                 3144,
                 3241
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "245": {
+        "235": {
             "fn": "ERC20.totalSupply",
             "offset": [
                 3144,
                 3241
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "246": {
+        "236": {
             "op": "SWAP1"
         },
-        "247": {
+        "237": {
             "op": "DUP2"
         },
-        "248": {
+        "238": {
             "op": "MSTORE"
         },
-        "249": {
+        "239": {
             "op": "PUSH1",
             "value": "0x20"
         },
-        "25": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "JUMPI",
-            "path": "6"
-        },
-        "251": {
+        "241": {
             "op": "ADD"
         },
-        "252": {
+        "242": {
             "fn": "ERC20.totalSupply",
             "offset": [
                 3144,
                 3241
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xB8"
         },
-        "255": {
+        "245": {
             "op": "JUMP"
         },
-        "256": {
+        "246": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "257": {
+        "247": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xD4"
         },
-        "26": {
+        "25": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "PUSH1",
-            "path": "6",
-            "value": "0x0"
+            "op": "JUMPI",
+            "path": "5"
         },
-        "260": {
+        "250": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x10E"
+            "path": "1",
+            "value": "0x104"
         },
-        "263": {
+        "253": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "CALLDATASIZE",
-            "path": "2"
+            "path": "1"
         },
-        "264": {
+        "254": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "266": {
+        "256": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x65D"
+            "path": "1",
+            "value": "0x666"
         },
-        "269": {
+        "259": {
             "fn": "ERC20.transferFrom",
             "jump": "i",
             "offset": [
                 5039,
                 5283
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "270": {
+        "26": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH1",
+            "path": "5",
+            "value": "0x0"
+        },
+        "260": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "271": {
+        "261": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x25A"
+            "path": "1",
+            "value": "0x256"
         },
-        "274": {
+        "264": {
             "fn": "ERC20.transferFrom",
             "jump": "i",
             "offset": [
                 5039,
                 5283
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "275": {
-            "fn": "USDC.decimals",
+        "265": {
+            "fn": "ERC20.decimals",
             "offset": [
-                257,
-                339
+                3002,
+                3084
             ],
             "op": "JUMPDEST",
-            "path": "6"
+            "path": "1"
         },
-        "276": {
-            "fn": "USDC.decimals",
+        "266": {
+            "fn": "ERC20.decimals",
             "offset": [
-                257,
-                339
+                3002,
+                3084
             ],
             "op": "PUSH1",
-            "path": "6",
+            "path": "1",
             "value": "0x40"
         },
-        "278": {
-            "fn": "USDC.decimals",
+        "268": {
+            "fn": "ERC20.decimals",
             "offset": [
-                257,
-                339
+                3002,
+                3084
             ],
             "op": "MLOAD",
-            "path": "6"
+            "path": "1"
         },
-        "279": {
-            "fn": "USDC.decimals",
+        "269": {
+            "fn": "ERC20.decimals",
             "offset": [
-                331,
-                332
+                3075,
+                3077
             ],
             "op": "PUSH1",
-            "path": "6",
+            "path": "1",
             "statement": 1,
-            "value": "0x6"
+            "value": "0x12"
         },
-        "28": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "CALLDATALOAD",
-            "path": "6"
-        },
-        "281": {
+        "271": {
             "op": "DUP2"
         },
-        "282": {
+        "272": {
             "op": "MSTORE"
         },
-        "283": {
+        "273": {
             "op": "PUSH1",
             "value": "0x20"
         },
-        "285": {
+        "275": {
             "op": "ADD"
         },
-        "286": {
-            "fn": "USDC.decimals",
+        "276": {
+            "fn": "ERC20.decimals",
             "offset": [
-                257,
-                339
+                3002,
+                3084
             ],
             "op": "PUSH2",
-            "path": "6",
+            "path": "1",
             "value": "0xB8"
         },
-        "289": {
+        "279": {
             "op": "JUMP"
         },
-        "29": {
+        "28": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "PUSH1",
-            "path": "6",
-            "value": "0xE0"
+            "op": "CALLDATALOAD",
+            "path": "5"
         },
-        "290": {
+        "280": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "291": {
+        "281": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0xF2"
+            "path": "1",
+            "value": "0xE8"
         },
-        "294": {
+        "284": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x130"
+            "path": "1",
+            "value": "0x126"
         },
-        "297": {
+        "287": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "CALLDATASIZE",
-            "path": "2"
+            "path": "1"
         },
-        "298": {
+        "288": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "300": {
+        "29": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH1",
+            "path": "5",
+            "value": "0xE0"
+        },
+        "290": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x699"
+            "path": "1",
+            "value": "0x6A2"
         },
-        "303": {
+        "293": {
             "fn": "ERC20.balanceOf",
             "jump": "i",
             "offset": [
                 3299,
                 3415
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "304": {
+        "294": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "305": {
+        "295": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "307": {
+        "297": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "309": {
+        "299": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "31": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "SHR",
-            "path": "6"
-        },
-        "311": {
+        "301": {
             "op": "SHL"
         },
-        "312": {
+        "302": {
             "op": "SUB"
         },
-        "313": {
+        "303": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "AND",
-            "path": "2",
+            "path": "1",
             "statement": 2
         },
-        "314": {
+        "304": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3364,
                 3371
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "316": {
+        "306": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "317": {
+        "307": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "318": {
+        "308": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "319": {
+        "309": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "32": {
+        "31": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "DUP1",
-            "path": "6"
+            "op": "SHR",
+            "path": "5"
         },
-        "321": {
+        "311": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "322": {
+        "312": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "323": {
+        "313": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "324": {
+        "314": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "326": {
+        "316": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "327": {
+        "317": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "328": {
+        "318": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "329": {
+        "319": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3390,
                 3408
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "33": {
+        "32": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x313CE567"
+            "op": "DUP1",
+            "path": "5"
         },
-        "330": {
+        "320": {
             "fn": "ERC20.balanceOf",
             "offset": [
                 3299,
                 3415
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "331": {
+        "321": {
             "fn": "ERC20.symbol",
             "offset": [
                 2276,
                 2369
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "332": {
+        "322": {
             "fn": "ERC20.symbol",
             "offset": [
                 2276,
                 2369
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xAB"
         },
-        "335": {
+        "325": {
             "fn": "ERC20.symbol",
             "offset": [
                 2276,
                 2369
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x27E"
+            "path": "1",
+            "value": "0x27A"
         },
-        "338": {
+        "328": {
             "fn": "ERC20.symbol",
             "jump": "i",
             "offset": [
                 2276,
                 2369
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
+        },
+        "329": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "JUMPDEST",
+            "path": "5"
+        },
+        "33": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0x70A08231"
+        },
+        "330": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x15C"
+        },
+        "333": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x157"
+        },
+        "336": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "CALLDATASIZE",
+            "path": "5"
+        },
+        "337": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "PUSH1",
+            "path": "5",
+            "value": "0x4"
         },
         "339": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x6C4"
+        },
+        "342": {
+            "fn": "USDC.mint",
+            "jump": "i",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "JUMP",
+            "path": "5"
+        },
+        "343": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "JUMPDEST",
+            "path": "5"
+        },
+        "344": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x289"
+        },
+        "347": {
+            "fn": "USDC.mint",
+            "jump": "i",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "JUMP",
+            "path": "5"
+        },
+        "348": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "JUMPDEST",
+            "path": "5"
+        },
+        "349": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "STOP",
+            "path": "5"
+        },
+        "350": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "340": {
+        "351": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "value": "0xD4"
         },
-        "343": {
+        "354": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x161"
+            "path": "1",
+            "value": "0x16C"
         },
-        "346": {
+        "357": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "CALLDATASIZE",
-            "path": "2"
+            "path": "1"
         },
-        "347": {
+        "358": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "349": {
+        "360": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x633"
+            "path": "1",
+            "value": "0x63C"
         },
-        "352": {
+        "363": {
             "fn": "ERC20.transfer",
             "jump": "i",
             "offset": [
                 3610,
                 3788
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "353": {
+        "364": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "354": {
+        "365": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x28D"
+            "path": "1",
+            "value": "0x296"
         },
-        "357": {
+        "368": {
             "fn": "ERC20.transfer",
             "jump": "i",
             "offset": [
                 3610,
                 3788
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "358": {
+        "369": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "359": {
+        "370": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0xF2"
+            "path": "1",
+            "value": "0xE8"
         },
-        "362": {
+        "373": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x174"
+            "path": "1",
+            "value": "0x17F"
         },
-        "365": {
+        "376": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "CALLDATASIZE",
-            "path": "2"
+            "path": "1"
         },
-        "366": {
+        "377": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "368": {
+        "379": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x6BB"
+            "path": "1",
+            "value": "0x6DD"
+        },
+        "38": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "GT",
+            "path": "5"
         },
-        "371": {
+        "382": {
             "fn": "ERC20.allowance",
             "jump": "i",
             "offset": [
                 3846,
                 3986
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "372": {
+        "383": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "373": {
+        "384": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "375": {
+        "386": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "377": {
+        "388": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "379": {
-            "op": "SHL"
-        },
-        "38": {
+        "39": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "GT",
-            "path": "6"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x66"
         },
-        "380": {
+        "390": {
+            "op": "SHL"
+        },
+        "391": {
             "op": "SUB"
         },
-        "381": {
+        "392": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "SWAP2",
-            "path": "2",
+            "path": "1",
             "statement": 3
         },
-        "382": {
+        "393": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "383": {
+        "394": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "384": {
+        "395": {
             "fn": "ERC20.allowance",
             "offset": [
                 3926,
                 3933
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "386": {
+        "397": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "387": {
+        "398": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "388": {
+        "399": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "389": {
+        "4": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "MSTORE",
+            "path": "5"
+        },
+        "400": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3963
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1"
         },
-        "39": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x66"
-        },
-        "391": {
+        "402": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "393": {
+        "404": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "394": {
+        "405": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "395": {
+        "406": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "396": {
+        "407": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "398": {
+        "409": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "399": {
+        "410": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "4": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "MSTORE",
-            "path": "6"
-        },
-        "400": {
+        "411": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "401": {
+        "412": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP4",
-            "path": "2"
+            "path": "1"
         },
-        "402": {
+        "413": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "403": {
+        "414": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP5",
-            "path": "2"
+            "path": "1"
         },
-        "404": {
+        "415": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "405": {
+        "416": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "406": {
+        "417": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "407": {
+        "418": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "408": {
+        "419": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "409": {
+        "42": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "JUMPI",
+            "path": "5"
+        },
+        "420": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "410": {
+        "421": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "411": {
+        "422": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "412": {
+        "423": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "413": {
+        "424": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "414": {
+        "425": {
             "fn": "ERC20.allowance",
             "offset": [
                 3846,
                 3986
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "415": {
+        "426": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "416": {
+        "427": {
             "fn": "ERC20.name",
             "offset": [
                 2119,
                 2132
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x60"
         },
-        "418": {
+        "429": {
             "fn": "ERC20.name",
             "offset": [
                 2151,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "statement": 4,
             "value": "0x3"
         },
-        "42": {
+        "43": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "JUMPI",
-            "path": "6"
+            "op": "DUP1",
+            "path": "5"
         },
-        "420": {
+        "431": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "421": {
+        "432": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "422": {
+        "433": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x1AE"
+            "path": "1",
+            "value": "0x1B9"
         },
-        "425": {
+        "436": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "426": {
+        "437": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x6EE"
+            "path": "1",
+            "value": "0x710"
         },
-        "429": {
+        "44": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0x70A08231"
+        },
+        "440": {
             "fn": "ERC20.name",
             "jump": "i",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "43": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "DUP1",
-            "path": "6"
-        },
-        "430": {
+        "441": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "431": {
+        "442": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "432": {
+        "443": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1F"
         },
-        "434": {
+        "445": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "435": {
+        "446": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "437": {
+        "448": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "438": {
+        "449": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "439": {
+        "450": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DIV",
-            "path": "2"
+            "path": "1"
         },
-        "44": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x313CE567"
-        },
-        "440": {
+        "451": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MUL",
-            "path": "2"
+            "path": "1"
         },
-        "441": {
+        "452": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "443": {
+        "454": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "444": {
+        "455": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "446": {
+        "457": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "447": {
+        "458": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "448": {
+        "459": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "449": {
+        "460": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "450": {
+        "461": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "452": {
+        "463": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "453": {
+        "464": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "454": {
+        "465": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP3",
-            "path": "2"
+            "path": "1"
         },
-        "455": {
+        "466": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "456": {
+        "467": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "457": {
+        "468": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "458": {
+        "469": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "459": {
+        "470": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "460": {
+        "471": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "462": {
+        "473": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "463": {
+        "474": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "464": {
+        "475": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "465": {
+        "476": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "466": {
+        "477": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x1DA"
+            "path": "1",
+            "value": "0x1E5"
         },
-        "469": {
+        "480": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "470": {
+        "481": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x6EE"
+            "path": "1",
+            "value": "0x710"
         },
-        "473": {
+        "484": {
             "fn": "ERC20.name",
             "jump": "i",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "474": {
+        "485": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "475": {
+        "486": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "476": {
+        "487": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ISZERO",
-            "path": "2"
+            "path": "1"
         },
-        "477": {
+        "488": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x227"
+            "path": "1",
+            "value": "0x232"
         },
-        "480": {
+        "49": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
+        },
+        "491": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "481": {
+        "492": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "482": {
+        "493": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1F"
         },
-        "484": {
+        "495": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "LT",
-            "path": "2"
+            "path": "1"
         },
-        "485": {
+        "496": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x1FC"
+            "path": "1",
+            "value": "0x207"
         },
-        "488": {
+        "499": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "489": {
-            "fn": "ERC20.name",
+        "5": {
+            "fn": null,
             "offset": [
-                2144,
-                2156
+                104,
+                260
             ],
-            "op": "PUSH2",
-            "path": "2",
-            "value": "0x100"
+            "op": "CALLVALUE",
+            "path": "5"
         },
-        "49": {
+        "50": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "EQ",
-            "path": "6"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x118"
         },
-        "492": {
+        "500": {
+            "fn": "ERC20.name",
+            "offset": [
+                2144,
+                2156
+            ],
+            "op": "PUSH2",
+            "path": "1",
+            "value": "0x100"
+        },
+        "503": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "493": {
+        "504": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "494": {
+        "505": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "495": {
+        "506": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DIV",
-            "path": "2"
+            "path": "1"
         },
-        "496": {
+        "507": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MUL",
-            "path": "2"
+            "path": "1"
         },
-        "497": {
+        "508": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "498": {
+        "509": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "499": {
+        "510": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "5": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "CALLVALUE",
-            "path": "6"
-        },
-        "50": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x113"
-        },
-        "500": {
+        "511": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "502": {
+        "513": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "503": {
+        "514": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "504": {
+        "515": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x227"
+            "path": "1",
+            "value": "0x232"
         },
-        "507": {
+        "518": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "508": {
+        "519": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "509": {
+        "520": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "510": {
+        "521": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "511": {
+        "522": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "512": {
+        "523": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "513": {
+        "524": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "515": {
+        "526": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "516": {
+        "527": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "518": {
+        "529": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "520": {
+        "53": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "JUMPI",
+            "path": "5"
+        },
+        "531": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "521": {
+        "532": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "522": {
+        "533": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "523": {
+        "534": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "524": {
+        "535": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "525": {
+        "536": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "526": {
+        "537": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "527": {
+        "538": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "528": {
+        "539": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1"
         },
-        "53": {
+        "54": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "JUMPI",
-            "path": "6"
+            "op": "DUP1",
+            "path": "5"
         },
-        "530": {
+        "541": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "531": {
+        "542": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "532": {
+        "543": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "534": {
+        "545": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "535": {
+        "546": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "536": {
+        "547": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "537": {
+        "548": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "GT",
-            "path": "2"
+            "path": "1"
         },
-        "538": {
+        "549": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x20A"
+            "path": "1",
+            "value": "0x215"
         },
-        "54": {
+        "55": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "DUP1",
-            "path": "6"
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0x95D89B41"
         },
-        "541": {
+        "552": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "542": {
+        "553": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "543": {
+        "554": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "544": {
+        "555": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SUB",
-            "path": "2"
+            "path": "1"
         },
-        "545": {
+        "556": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1F"
         },
-        "547": {
+        "558": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "548": {
+        "559": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "549": {
+        "560": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "55": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x70A08231"
-        },
-        "550": {
+        "561": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "551": {
+        "562": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "552": {
+        "563": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "553": {
+        "564": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "554": {
+        "565": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "555": {
+        "566": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "556": {
+        "567": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "557": {
+        "568": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "558": {
+        "569": {
             "fn": "ERC20.name",
             "offset": [
                 2144,
                 2156
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "559": {
+        "570": {
             "fn": "ERC20.name",
             "offset": [
                 2074,
                 2163
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "560": {
+        "571": {
             "fn": "ERC20.name",
             "jump": "o",
             "offset": [
                 2074,
                 2163
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "561": {
+        "572": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "562": {
+        "573": {
             "fn": "ERC20.approve",
             "offset": [
                 4366,
                 4370
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "564": {
+        "575": {
             "fn": "Context._msgSender",
             "offset": [
                 735,
                 745
             ],
             "op": "CALLER",
-            "path": "5",
+            "path": "4",
             "statement": 5
         },
-        "565": {
+        "576": {
             "fn": "ERC20.approve",
             "offset": [
                 4420,
                 4451
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "statement": 6,
-            "value": "0x23F"
+            "value": "0x24A"
         },
-        "568": {
+        "579": {
             "fn": "Context._msgSender",
             "offset": [
                 735,
                 745
             ],
             "op": "DUP2",
-            "path": "5"
+            "path": "4"
         },
-        "569": {
+        "580": {
             "fn": "ERC20.approve",
             "offset": [
                 4436,
                 4443
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "570": {
+        "581": {
             "fn": "ERC20.approve",
             "offset": [
                 4445,
                 4450
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "571": {
+        "582": {
             "fn": "ERC20.approve",
             "offset": [
                 4420,
                 4428
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x29B"
+            "path": "1",
+            "value": "0x2A4"
         },
-        "574": {
+        "585": {
             "fn": "ERC20.approve",
             "jump": "i",
             "offset": [
                 4420,
                 4451
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "575": {
+        "586": {
             "fn": "ERC20.approve",
             "offset": [
                 4420,
                 4451
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "576": {
+        "587": {
             "fn": "ERC20.approve",
             "offset": [
                 4468,
                 4472
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "statement": 7,
             "value": "0x1"
         },
-        "578": {
+        "589": {
             "fn": "ERC20.approve",
             "offset": [
                 4461,
                 4472
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "579": {
+        "590": {
             "fn": "ERC20.approve",
             "offset": [
                 4461,
                 4472
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "580": {
+        "591": {
             "fn": "ERC20.approve",
             "offset": [
                 4461,
                 4472
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "581": {
+        "592": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "582": {
+        "593": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "SWAP3",
-            "path": "2"
+            "path": "1"
         },
-        "583": {
+        "594": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "SWAP2",
-            "path": "2"
+            "path": "1"
         },
-        "584": {
+        "595": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "585": {
+        "596": {
             "fn": "ERC20.approve",
             "offset": [
                 4293,
                 4479
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "586": {
+        "597": {
             "fn": "ERC20.approve",
             "jump": "o",
             "offset": [
                 4293,
                 4479
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "587": {
-            "fn": "USDC.mint",
+        "598": {
+            "fn": "ERC20.transferFrom",
             "offset": [
-                178,
-                251
+                5039,
+                5283
             ],
             "op": "JUMPDEST",
-            "path": "6"
-        },
-        "588": {
-            "fn": "USDC.mint",
-            "offset": [
-                212,
-                244
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "statement": 8,
-            "value": "0x258"
-        },
-        "591": {
-            "fn": "USDC.mint",
-            "offset": [
-                218,
-                228
-            ],
-            "op": "CALLER",
-            "path": "6"
-        },
-        "592": {
-            "fn": "USDC.mint",
-            "offset": [
-                230,
-                243
-            ],
-            "op": "PUSH3",
-            "path": "6",
-            "value": "0x4C4B40"
-        },
-        "596": {
-            "fn": "USDC.mint",
-            "offset": [
-                212,
-                217
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x2AD"
+            "path": "1"
         },
         "599": {
-            "fn": "USDC.mint",
-            "jump": "i",
+            "fn": "ERC20.transferFrom",
             "offset": [
-                212,
-                244
+                5126,
+                5130
             ],
-            "op": "JUMP",
-            "path": "6"
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x0"
         },
         "6": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "DUP1",
-            "path": "6"
+            "path": "5"
         },
         "60": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "EQ",
-            "path": "6"
-        },
-        "600": {
-            "fn": "USDC.mint",
-            "offset": [
-                212,
-                244
-            ],
-            "op": "JUMPDEST",
-            "path": "6"
+            "path": "5"
         },
         "601": {
-            "fn": "USDC.mint",
-            "jump": "o",
-            "offset": [
-                178,
-                251
-            ],
-            "op": "JUMP",
-            "path": "6"
-        },
-        "602": {
-            "fn": "ERC20.transferFrom",
-            "offset": [
-                5039,
-                5283
-            ],
-            "op": "JUMPDEST",
-            "path": "2"
-        },
-        "603": {
-            "fn": "ERC20.transferFrom",
-            "offset": [
-                5126,
-                5130
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x0"
-        },
-        "605": {
             "fn": "Context._msgSender",
             "offset": [
                 735,
                 745
             ],
             "op": "CALLER",
-            "path": "5"
+            "path": "4"
         },
-        "606": {
+        "602": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5182,
                 5219
             ],
             "op": "PUSH2",
-            "path": "2",
-            "statement": 9,
-            "value": "0x268"
+            "path": "1",
+            "statement": 8,
+            "value": "0x264"
         },
-        "609": {
+        "605": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5198,
                 5202
             ],
             "op": "DUP6",
-            "path": "2"
-        },
-        "61": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x122"
+            "path": "1"
         },
-        "610": {
+        "606": {
             "fn": "Context._msgSender",
             "offset": [
                 735,
                 745
             ],
             "op": "DUP3",
-            "path": "5"
+            "path": "4"
         },
-        "611": {
+        "607": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5213,
                 5218
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "612": {
+        "608": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5182,
                 5197
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x2EC"
+            "path": "1",
+            "value": "0x2B6"
         },
-        "615": {
+        "61": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x141"
+        },
+        "611": {
             "fn": "ERC20.transferFrom",
             "jump": "i",
             "offset": [
                 5182,
                 5219
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "616": {
+        "612": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5182,
                 5219
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "617": {
+        "613": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5229,
                 5255
             ],
             "op": "PUSH2",
-            "path": "2",
-            "statement": 10,
-            "value": "0x273"
+            "path": "1",
+            "statement": 9,
+            "value": "0x26F"
         },
-        "620": {
+        "616": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5239,
                 5243
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "621": {
+        "617": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5245,
                 5247
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "622": {
+        "618": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5249,
                 5254
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "623": {
+        "619": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5229,
                 5238
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x36A"
+            "path": "1",
+            "value": "0x339"
         },
-        "626": {
+        "622": {
             "fn": "ERC20.transferFrom",
             "jump": "i",
             "offset": [
                 5229,
                 5255
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "627": {
+        "623": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5229,
                 5255
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "628": {
+        "624": {
             "op": "POP"
         },
-        "629": {
+        "625": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5272,
                 5276
             ],
             "op": "PUSH1",
-            "path": "2",
-            "statement": 11,
+            "path": "1",
+            "statement": 10,
             "value": "0x1"
         },
-        "631": {
+        "627": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5272,
                 5276
             ],
             "op": "SWAP5",
-            "path": "2"
+            "path": "1"
         },
-        "632": {
+        "628": {
             "fn": "ERC20.transferFrom",
             "offset": [
                 5039,
                 5283
             ],
             "op": "SWAP4",
-            "path": "2"
+            "path": "1"
         },
-        "633": {
+        "629": {
             "op": "POP"
         },
-        "634": {
+        "630": {
             "op": "POP"
         },
-        "635": {
+        "631": {
             "op": "POP"
         },
-        "636": {
+        "632": {
             "op": "POP"
         },
-        "637": {
+        "633": {
             "fn": "ERC20.transferFrom",
             "jump": "o",
             "offset": [
                 5039,
                 5283
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "638": {
+        "634": {
             "fn": "ERC20.symbol",
             "offset": [
                 2276,
                 2369
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "639": {
+        "635": {
             "fn": "ERC20.symbol",
             "offset": [
                 2323,
                 2336
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x60"
         },
+        "637": {
+            "fn": "ERC20.symbol",
+            "offset": [
+                2355,
+                2362
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "statement": 11,
+            "value": "0x4"
+        },
+        "639": {
+            "fn": "ERC20.symbol",
+            "offset": [
+                2348,
+                2362
+            ],
+            "op": "DUP1",
+            "path": "1"
+        },
         "64": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "JUMPI",
-            "path": "6"
+            "path": "5"
         },
-        "641": {
+        "640": {
             "fn": "ERC20.symbol",
             "offset": [
-                2355,
+                2348,
                 2362
             ],
-            "op": "PUSH1",
-            "path": "2",
-            "statement": 12,
-            "value": "0x4"
+            "op": "SLOAD",
+            "path": "1"
         },
-        "643": {
+        "641": {
             "fn": "ERC20.symbol",
             "offset": [
                 2348,
                 2362
             ],
-            "op": "DUP1",
-            "path": "2"
+            "op": "PUSH2",
+            "path": "1",
+            "value": "0x1B9"
         },
         "644": {
             "fn": "ERC20.symbol",
             "offset": [
                 2348,
                 2362
             ],
-            "op": "SLOAD",
-            "path": "2"
+            "op": "SWAP1",
+            "path": "1"
         },
         "645": {
             "fn": "ERC20.symbol",
             "offset": [
                 2348,
                 2362
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x1AE"
+            "path": "1",
+            "value": "0x710"
         },
         "648": {
             "fn": "ERC20.symbol",
+            "jump": "i",
             "offset": [
                 2348,
                 2362
             ],
-            "op": "SWAP1",
-            "path": "2"
+            "op": "JUMP",
+            "path": "1"
         },
         "649": {
-            "fn": "ERC20.symbol",
+            "fn": "USDC.mint",
             "offset": [
-                2348,
-                2362
+                178,
+                256
             ],
-            "op": "PUSH2",
-            "path": "2",
-            "value": "0x6EE"
+            "op": "JUMPDEST",
+            "path": "5"
         },
         "65": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "DUP1",
-            "path": "6"
+            "path": "5"
         },
-        "652": {
-            "fn": "ERC20.symbol",
+        "650": {
+            "fn": "USDC.mint",
+            "offset": [
+                225,
+                249
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "statement": 12,
+            "value": "0x293"
+        },
+        "653": {
+            "fn": "USDC.mint",
+            "offset": [
+                231,
+                241
+            ],
+            "op": "CALLER",
+            "path": "5"
+        },
+        "654": {
+            "fn": "USDC.mint",
+            "offset": [
+                243,
+                248
+            ],
+            "op": "DUP3",
+            "path": "5"
+        },
+        "655": {
+            "fn": "USDC.mint",
+            "offset": [
+                225,
+                230
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x398"
+        },
+        "658": {
+            "fn": "USDC.mint",
             "jump": "i",
             "offset": [
-                2348,
-                2362
+                225,
+                249
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "5"
         },
-        "653": {
+        "659": {
+            "fn": "USDC.mint",
+            "offset": [
+                225,
+                249
+            ],
+            "op": "JUMPDEST",
+            "path": "5"
+        },
+        "66": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0xA0712D68"
+        },
+        "660": {
+            "fn": "USDC.mint",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "POP",
+            "path": "5"
+        },
+        "661": {
+            "fn": "USDC.mint",
+            "jump": "o",
+            "offset": [
+                178,
+                256
+            ],
+            "op": "JUMP",
+            "path": "5"
+        },
+        "662": {
             "fn": "ERC20.transfer",
             "offset": [
                 3610,
                 3788
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "654": {
+        "663": {
             "fn": "ERC20.transfer",
             "offset": [
                 3679,
                 3683
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "656": {
+        "665": {
             "fn": "Context._msgSender",
             "offset": [
                 735,
                 745
             ],
             "op": "CALLER",
-            "path": "5"
+            "path": "4"
         },
-        "657": {
+        "666": {
             "fn": "ERC20.transfer",
             "offset": [
                 3733,
                 3760
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "statement": 13,
-            "value": "0x23F"
-        },
-        "66": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0x95D89B41"
+            "value": "0x24A"
         },
-        "660": {
+        "669": {
             "fn": "Context._msgSender",
             "offset": [
                 735,
                 745
             ],
             "op": "DUP2",
-            "path": "5"
+            "path": "4"
         },
-        "661": {
+        "670": {
             "fn": "ERC20.transfer",
             "offset": [
                 3750,
                 3752
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "662": {
+        "671": {
             "fn": "ERC20.transfer",
             "offset": [
                 3754,
                 3759
             ],
             "op": "DUP6",
-            "path": "2"
+            "path": "1"
         },
-        "663": {
+        "672": {
             "fn": "ERC20.transfer",
             "offset": [
                 3733,
                 3742
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x36A"
+            "path": "1",
+            "value": "0x339"
         },
-        "666": {
+        "675": {
             "fn": "ERC20.transfer",
             "jump": "i",
             "offset": [
                 3733,
                 3760
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "667": {
+        "676": {
             "fn": "ERC20._approve",
             "offset": [
                 8989,
                 9117
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "668": {
+        "677": {
             "fn": "ERC20._approve",
             "offset": [
                 9073,
                 9110
             ],
             "op": "PUSH2",
-            "path": "2",
+            "path": "1",
             "statement": 14,
-            "value": "0x2A8"
+            "value": "0x2B1"
         },
-        "671": {
+        "680": {
             "fn": "ERC20._approve",
             "offset": [
                 9082,
                 9087
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "672": {
+        "681": {
             "fn": "ERC20._approve",
             "offset": [
                 9089,
                 9096
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "673": {
+        "682": {
             "fn": "ERC20._approve",
             "offset": [
                 9098,
                 9103
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "674": {
+        "683": {
             "fn": "ERC20._approve",
             "offset": [
                 9105,
                 9109
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1"
         },
-        "676": {
+        "685": {
             "fn": "ERC20._approve",
             "offset": [
                 9073,
                 9081
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x3C9"
+            "path": "1",
+            "value": "0x3D2"
         },
-        "679": {
+        "688": {
             "fn": "ERC20._approve",
             "jump": "i",
             "offset": [
                 9073,
                 9110
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "680": {
+        "689": {
             "fn": "ERC20._approve",
             "offset": [
                 9073,
                 9110
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "681": {
+        "690": {
             "fn": "ERC20._approve",
             "offset": [
                 8989,
                 9117
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "682": {
+        "691": {
             "fn": "ERC20._approve",
             "offset": [
                 8989,
                 9117
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "683": {
+        "692": {
             "fn": "ERC20._approve",
             "offset": [
                 8989,
                 9117
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "684": {
+        "693": {
             "fn": "ERC20._approve",
             "jump": "o",
             "offset": [
                 8989,
                 9117
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "685": {
-            "fn": "ERC20._mint",
+        "694": {
+            "fn": "ERC20._spendAllowance",
             "offset": [
-                7721,
-                7929
+                10663,
+                11140
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "686": {
+        "695": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "688": {
+        "697": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "690": {
+        "699": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "692": {
-            "op": "SHL"
-        },
-        "693": {
-            "op": "SUB"
-        },
-        "694": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7791,
-                7812
-            ],
-            "op": "DUP3",
-            "path": "2",
-            "statement": 15
-        },
-        "695": {
-            "branch": 32,
-            "fn": "ERC20._mint",
-            "offset": [
-                7791,
-                7812
-            ],
-            "op": "AND",
-            "path": "2"
-        },
-        "696": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7787,
-                7878
-            ],
-            "op": "PUSH2",
-            "path": "2",
-            "value": "0x2DC"
-        },
-        "699": {
-            "branch": 32,
-            "fn": "ERC20._mint",
-            "offset": [
-                7787,
-                7878
-            ],
-            "op": "JUMPI",
-            "path": "2"
-        },
         "7": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "ISZERO",
-            "path": "6"
-        },
-        "700": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x40"
-        },
-        "702": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "MLOAD",
-            "path": "2"
-        },
-        "703": {
-            "op": "PUSH4",
-            "value": "0xEC442F05"
-        },
-        "708": {
-            "op": "PUSH1",
-            "value": "0xE0"
-        },
-        "71": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "EQ",
-            "path": "6"
-        },
-        "710": {
-            "op": "SHL"
-        },
-        "711": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "DUP2",
-            "path": "2"
-        },
-        "712": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "MSTORE",
-            "path": "2"
-        },
-        "713": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7864,
-                7865
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x0"
-        },
-        "715": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x4"
-        },
-        "717": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "DUP3",
-            "path": "2"
-        },
-        "718": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "ADD",
-            "path": "2"
-        },
-        "719": {
-            "op": "MSTORE"
-        },
-        "72": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x14B"
-        },
-        "720": {
-            "op": "PUSH1",
-            "value": "0x24"
-        },
-        "722": {
-            "op": "ADD"
-        },
-        "723": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "JUMPDEST",
-            "path": "2"
-        },
-        "724": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x40"
-        },
-        "726": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "MLOAD",
-            "path": "2"
-        },
-        "727": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "DUP1",
-            "path": "2"
-        },
-        "728": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "SWAP2",
-            "path": "2"
-        },
-        "729": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "SUB",
-            "path": "2"
-        },
-        "730": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "SWAP1",
-            "path": "2"
-        },
-        "731": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7835,
-                7867
-            ],
-            "op": "REVERT",
-            "path": "2"
-        },
-        "732": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7787,
-                7878
-            ],
-            "op": "JUMPDEST",
-            "path": "2"
-        },
-        "733": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7887,
-                7922
-            ],
-            "op": "PUSH2",
-            "path": "2",
-            "statement": 16,
-            "value": "0x2E8"
-        },
-        "736": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7903,
-                7904
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x0"
-        },
-        "738": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7907,
-                7914
-            ],
-            "op": "DUP4",
-            "path": "2"
-        },
-        "739": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7916,
-                7921
-            ],
-            "op": "DUP4",
-            "path": "2"
-        },
-        "740": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7887,
-                7894
-            ],
-            "op": "PUSH2",
-            "path": "2",
-            "value": "0x49E"
-        },
-        "743": {
-            "fn": "ERC20._mint",
-            "jump": "i",
-            "offset": [
-                7887,
-                7922
-            ],
-            "op": "JUMP",
-            "path": "2"
-        },
-        "744": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7887,
-                7922
-            ],
-            "op": "JUMPDEST",
-            "path": "2"
-        },
-        "745": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7721,
-                7929
-            ],
-            "op": "POP",
-            "path": "2"
-        },
-        "746": {
-            "fn": "ERC20._mint",
-            "offset": [
-                7721,
-                7929
-            ],
-            "op": "POP",
-            "path": "2"
-        },
-        "747": {
-            "fn": "ERC20._mint",
-            "jump": "o",
-            "offset": [
-                7721,
-                7929
-            ],
-            "op": "JUMP",
-            "path": "2"
-        },
-        "748": {
-            "fn": "ERC20._spendAllowance",
-            "offset": [
-                10663,
-                11140
-            ],
-            "op": "JUMPDEST",
-            "path": "2"
-        },
-        "749": {
-            "op": "PUSH1",
-            "value": "0x1"
-        },
-        "75": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "JUMPI",
-            "path": "6"
-        },
-        "751": {
-            "op": "PUSH1",
-            "value": "0x1"
-        },
-        "753": {
-            "op": "PUSH1",
-            "value": "0xA0"
+            "path": "5"
         },
-        "755": {
+        "701": {
             "op": "SHL"
         },
-        "756": {
+        "702": {
             "op": "SUB"
         },
-        "757": {
+        "703": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "758": {
+        "704": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "759": {
+        "705": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "AND",
-            "path": "2"
-        },
-        "76": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "DUP1",
-            "path": "6"
+            "path": "1"
         },
-        "760": {
+        "706": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10762,
                 10786
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "762": {
+        "708": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "763": {
+        "709": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
+        },
+        "71": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
         },
-        "764": {
+        "710": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "765": {
+        "711": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3963
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x1"
         },
-        "767": {
+        "713": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x20"
         },
-        "769": {
+        "715": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "SWAP1",
-            "path": "2"
-        },
-        "77": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0xA9059CBB"
+            "path": "1"
         },
-        "770": {
+        "716": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "771": {
+        "717": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "772": {
+        "718": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "774": {
+        "72": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x149"
+        },
+        "720": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP1",
-            "path": "2"
+            "path": "1"
         },
-        "775": {
+        "721": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "776": {
+        "722": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3970
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "777": {
+        "723": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP4",
-            "path": "2"
+            "path": "1"
         },
-        "778": {
+        "724": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "DUP7",
-            "path": "2"
+            "path": "1"
         },
-        "779": {
+        "725": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "780": {
+        "726": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "781": {
+        "727": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "782": {
+        "728": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP3",
-            "path": "2"
+            "path": "1"
         },
-        "783": {
+        "729": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SWAP1",
-            "path": "2"
+            "path": "1"
         },
-        "784": {
+        "730": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "785": {
+        "731": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "KECCAK256",
-            "path": "2"
+            "path": "1"
         },
-        "786": {
+        "732": {
             "fn": "ERC20.allowance",
             "offset": [
                 3952,
                 3979
             ],
             "op": "SLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "787": {
+        "733": {
             "op": "PUSH1",
             "value": "0x0"
         },
-        "789": {
+        "735": {
             "op": "NOT"
         },
-        "790": {
+        "736": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10828,
                 10865
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "791": {
-            "branch": 33,
+        "737": {
+            "branch": 32,
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10828,
                 10865
             ],
             "op": "EQ",
-            "path": "2"
+            "path": "1"
         },
-        "792": {
+        "738": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10824,
                 11134
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x364"
+            "path": "1",
+            "value": "0x333"
         },
-        "795": {
-            "branch": 33,
+        "741": {
+            "branch": 32,
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10824,
                 11134
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "796": {
+        "742": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10904,
                 10909
             ],
             "op": "DUP2",
-            "path": "2",
-            "statement": 17
+            "path": "1",
+            "statement": 15
         },
-        "797": {
+        "743": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10885,
                 10901
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "798": {
-            "branch": 34,
+        "744": {
+            "branch": 33,
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10885,
                 10909
             ],
             "op": "LT",
-            "path": "2"
+            "path": "1"
         },
-        "799": {
+        "745": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10881,
                 11011
             ],
             "op": "ISZERO",
-            "path": "2"
+            "path": "1"
         },
-        "8": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x10"
-        },
-        "800": {
+        "746": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10881,
                 11011
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x355"
+            "path": "1",
+            "value": "0x324"
         },
-        "803": {
-            "branch": 34,
+        "749": {
+            "branch": 33,
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10881,
                 11011
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "804": {
+        "75": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "JUMPI",
+            "path": "5"
+        },
+        "750": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "806": {
+        "752": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "807": {
+        "753": {
             "op": "PUSH4",
             "value": "0x7DC7A0D9"
         },
-        "812": {
+        "758": {
             "op": "PUSH1",
             "value": "0xE1"
         },
-        "814": {
+        "76": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "DUP1",
+            "path": "5"
+        },
+        "760": {
             "op": "SHL"
         },
-        "815": {
+        "761": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "816": {
+        "762": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "817": {
+        "763": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "819": {
+        "765": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "82": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "EQ",
-            "path": "6"
-        },
-        "821": {
+        "767": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "823": {
+        "769": {
             "op": "SHL"
         },
-        "824": {
+        "77": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0xA9059CBB"
+        },
+        "770": {
             "op": "SUB"
         },
-        "825": {
+        "771": {
             "op": "DUP5"
         },
-        "826": {
+        "772": {
             "op": "AND"
         },
-        "827": {
+        "773": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "829": {
+        "775": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
             "op": "DUP3",
-            "path": "2"
-        },
-        "83": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x153"
+            "path": "1"
         },
-        "830": {
+        "776": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "831": {
+        "777": {
             "op": "MSTORE"
         },
-        "832": {
+        "778": {
             "op": "PUSH1",
             "value": "0x24"
         },
-        "834": {
+        "780": {
             "op": "DUP2"
         },
-        "835": {
+        "781": {
             "op": "ADD"
         },
-        "836": {
+        "782": {
             "op": "DUP3"
         },
-        "837": {
+        "783": {
             "op": "SWAP1"
         },
-        "838": {
+        "784": {
             "op": "MSTORE"
         },
-        "839": {
+        "785": {
             "op": "PUSH1",
             "value": "0x44"
         },
-        "841": {
+        "787": {
             "op": "DUP2"
         },
-        "842": {
+        "788": {
             "op": "ADD"
         },
-        "843": {
+        "789": {
             "op": "DUP4"
         },
-        "844": {
+        "790": {
             "op": "SWAP1"
         },
-        "845": {
+        "791": {
             "op": "MSTORE"
         },
-        "846": {
+        "792": {
             "op": "PUSH1",
             "value": "0x64"
         },
-        "848": {
+        "794": {
             "op": "ADD"
         },
-        "849": {
+        "795": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10936,
                 10996
             ],
+            "op": "JUMPDEST",
+            "path": "1"
+        },
+        "796": {
+            "fn": "ERC20._spendAllowance",
+            "offset": [
+                10936,
+                10996
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x40"
+        },
+        "798": {
+            "fn": "ERC20._spendAllowance",
+            "offset": [
+                10936,
+                10996
+            ],
+            "op": "MLOAD",
+            "path": "1"
+        },
+        "799": {
+            "fn": "ERC20._spendAllowance",
+            "offset": [
+                10936,
+                10996
+            ],
+            "op": "DUP1",
+            "path": "1"
+        },
+        "8": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x2D3"
+            "path": "5",
+            "value": "0x10"
         },
-        "852": {
-            "op": "JUMP"
+        "800": {
+            "fn": "ERC20._spendAllowance",
+            "offset": [
+                10936,
+                10996
+            ],
+            "op": "SWAP2",
+            "path": "1"
         },
-        "853": {
+        "801": {
+            "fn": "ERC20._spendAllowance",
+            "offset": [
+                10936,
+                10996
+            ],
+            "op": "SUB",
+            "path": "1"
+        },
+        "802": {
+            "fn": "ERC20._spendAllowance",
+            "offset": [
+                10936,
+                10996
+            ],
+            "op": "SWAP1",
+            "path": "1"
+        },
+        "803": {
+            "fn": "ERC20._spendAllowance",
+            "offset": [
+                10936,
+                10996
+            ],
+            "op": "REVERT",
+            "path": "1"
+        },
+        "804": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10881,
                 11011
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "854": {
+        "805": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11052,
                 11109
             ],
             "op": "PUSH2",
-            "path": "2",
-            "statement": 18,
-            "value": "0x364"
+            "path": "1",
+            "statement": 16,
+            "value": "0x333"
         },
-        "857": {
+        "808": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11061,
                 11066
             ],
             "op": "DUP5",
-            "path": "2"
+            "path": "1"
         },
-        "858": {
+        "809": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11068,
                 11075
             ],
             "op": "DUP5",
-            "path": "2"
+            "path": "1"
         },
-        "859": {
+        "810": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11096,
                 11101
             ],
             "op": "DUP5",
-            "path": "2"
+            "path": "1"
         },
-        "86": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "JUMPI",
-            "path": "6"
-        },
-        "860": {
+        "811": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11077,
                 11093
             ],
             "op": "DUP5",
-            "path": "2"
+            "path": "1"
         },
-        "861": {
+        "812": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11077,
                 11101
             ],
             "op": "SUB",
-            "path": "2"
+            "path": "1"
         },
-        "862": {
+        "813": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11103,
                 11108
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "864": {
+        "815": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11052,
                 11060
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x3C9"
+            "path": "1",
+            "value": "0x3D2"
         },
-        "867": {
+        "818": {
             "fn": "ERC20._spendAllowance",
             "jump": "i",
             "offset": [
                 11052,
                 11109
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "868": {
+        "819": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 11052,
                 11109
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
+        },
+        "82": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
         },
-        "869": {
+        "820": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10752,
                 11140
             ],
             "op": "POP",
-            "path": "2"
-        },
-        "87": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "DUP1",
-            "path": "6"
+            "path": "1"
         },
-        "870": {
+        "821": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10663,
                 11140
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "871": {
+        "822": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10663,
                 11140
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "872": {
+        "823": {
             "fn": "ERC20._spendAllowance",
             "offset": [
                 10663,
                 11140
             ],
             "op": "POP",
-            "path": "2"
+            "path": "1"
         },
-        "873": {
+        "824": {
             "fn": "ERC20._spendAllowance",
             "jump": "o",
             "offset": [
                 10663,
                 11140
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "874": {
+        "825": {
             "fn": "ERC20._transfer",
             "offset": [
                 5656,
                 5956
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "875": {
+        "826": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "877": {
+        "828": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "879": {
-            "op": "PUSH1",
-            "value": "0xA0"
-        },
-        "88": {
+        "83": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "PUSH4",
-            "path": "6",
-            "value": "0xDD62ED3E"
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x15E"
         },
-        "881": {
+        "830": {
+            "op": "PUSH1",
+            "value": "0xA0"
+        },
+        "832": {
             "op": "SHL"
         },
-        "882": {
+        "833": {
             "op": "SUB"
         },
-        "883": {
+        "834": {
             "fn": "ERC20._transfer",
             "offset": [
                 5739,
                 5757
             ],
             "op": "DUP4",
-            "path": "2",
-            "statement": 19
+            "path": "1",
+            "statement": 17
         },
-        "884": {
-            "branch": 35,
+        "835": {
+            "branch": 34,
             "fn": "ERC20._transfer",
             "offset": [
                 5739,
                 5757
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "885": {
+        "836": {
             "fn": "ERC20._transfer",
             "offset": [
                 5735,
                 5821
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x394"
+            "path": "1",
+            "value": "0x363"
         },
-        "888": {
-            "branch": 35,
+        "839": {
+            "branch": 34,
             "fn": "ERC20._transfer",
             "offset": [
                 5735,
                 5821
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "889": {
+        "840": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "891": {
+        "842": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "892": {
+        "843": {
             "op": "PUSH4",
             "value": "0x4B637E8F"
         },
-        "897": {
+        "848": {
             "op": "PUSH1",
             "value": "0xE1"
         },
-        "899": {
+        "850": {
             "op": "SHL"
         },
-        "900": {
+        "851": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "901": {
+        "852": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "902": {
+        "853": {
             "fn": "ERC20._transfer",
             "offset": [
                 5807,
                 5808
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "904": {
+        "855": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "906": {
+        "857": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "907": {
+        "858": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "908": {
+        "859": {
             "op": "MSTORE"
         },
-        "909": {
+        "86": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "JUMPI",
+            "path": "5"
+        },
+        "860": {
             "op": "PUSH1",
             "value": "0x24"
         },
-        "911": {
+        "862": {
             "op": "ADD"
         },
-        "912": {
+        "863": {
             "fn": "ERC20._transfer",
             "offset": [
                 5780,
                 5810
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x2D3"
+            "path": "1",
+            "value": "0x31B"
         },
-        "915": {
+        "866": {
             "op": "JUMP"
         },
-        "916": {
+        "867": {
             "fn": "ERC20._transfer",
             "offset": [
                 5735,
                 5821
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "917": {
+        "868": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "919": {
+        "87": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "DUP1",
+            "path": "5"
+        },
+        "870": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "921": {
+        "872": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "923": {
+        "874": {
             "op": "SHL"
         },
-        "924": {
+        "875": {
             "op": "SUB"
         },
-        "925": {
+        "876": {
             "fn": "ERC20._transfer",
             "offset": [
                 5834,
                 5850
             ],
             "op": "DUP3",
-            "path": "2",
-            "statement": 20
+            "path": "1",
+            "statement": 18
         },
-        "926": {
-            "branch": 36,
+        "877": {
+            "branch": 35,
             "fn": "ERC20._transfer",
             "offset": [
                 5834,
                 5850
             ],
             "op": "AND",
-            "path": "2"
+            "path": "1"
         },
-        "927": {
+        "878": {
             "fn": "ERC20._transfer",
             "offset": [
                 5830,
                 5916
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x3BE"
+            "path": "1",
+            "value": "0x38D"
         },
-        "93": {
+        "88": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
-            "op": "EQ",
-            "path": "6"
+            "op": "PUSH4",
+            "path": "5",
+            "value": "0xDD62ED3E"
         },
-        "930": {
-            "branch": 36,
+        "881": {
+            "branch": 35,
             "fn": "ERC20._transfer",
             "offset": [
                 5830,
                 5916
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "931": {
+        "882": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "933": {
+        "884": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "934": {
+        "885": {
             "op": "PUSH4",
             "value": "0xEC442F05"
         },
-        "939": {
+        "890": {
             "op": "PUSH1",
             "value": "0xE0"
         },
-        "94": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH2",
-            "path": "6",
-            "value": "0x166"
-        },
-        "941": {
+        "892": {
             "op": "SHL"
         },
-        "942": {
+        "893": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "DUP2",
-            "path": "2"
+            "path": "1"
         },
-        "943": {
+        "894": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "MSTORE",
-            "path": "2"
+            "path": "1"
         },
-        "944": {
+        "895": {
             "fn": "ERC20._transfer",
             "offset": [
                 5902,
                 5903
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x0"
         },
-        "946": {
+        "897": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x4"
         },
-        "948": {
+        "899": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "DUP3",
-            "path": "2"
+            "path": "1"
         },
-        "949": {
+        "900": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "ADD",
-            "path": "2"
+            "path": "1"
         },
-        "950": {
+        "901": {
             "op": "MSTORE"
         },
-        "951": {
+        "902": {
             "op": "PUSH1",
             "value": "0x24"
         },
-        "953": {
+        "904": {
             "op": "ADD"
         },
-        "954": {
+        "905": {
             "fn": "ERC20._transfer",
             "offset": [
                 5873,
                 5905
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x2D3"
+            "path": "1",
+            "value": "0x31B"
         },
-        "957": {
+        "908": {
             "op": "JUMP"
         },
-        "958": {
+        "909": {
             "fn": "ERC20._transfer",
             "offset": [
                 5830,
                 5916
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
         },
-        "959": {
+        "910": {
             "fn": "ERC20._transfer",
             "offset": [
                 5925,
                 5949
             ],
             "op": "PUSH2",
-            "path": "2",
-            "statement": 21,
-            "value": "0x2A8"
+            "path": "1",
+            "statement": 19,
+            "value": "0x2B1"
         },
-        "962": {
+        "913": {
             "fn": "ERC20._transfer",
             "offset": [
                 5933,
                 5937
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "963": {
+        "914": {
             "fn": "ERC20._transfer",
             "offset": [
                 5939,
                 5941
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "964": {
+        "915": {
             "fn": "ERC20._transfer",
             "offset": [
                 5943,
                 5948
             ],
             "op": "DUP4",
-            "path": "2"
+            "path": "1"
         },
-        "965": {
+        "916": {
             "fn": "ERC20._transfer",
             "offset": [
                 5925,
                 5932
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x49E"
+            "path": "1",
+            "value": "0x4A7"
         },
-        "968": {
+        "919": {
             "fn": "ERC20._transfer",
             "jump": "i",
             "offset": [
                 5925,
                 5949
             ],
             "op": "JUMP",
-            "path": "2"
+            "path": "1"
         },
-        "969": {
-            "fn": "ERC20._approve",
+        "920": {
+            "fn": "ERC20._mint",
             "offset": [
-                9949,
-                10381
+                7721,
+                7929
+            ],
+            "op": "JUMPDEST",
+            "path": "1"
+        },
+        "921": {
+            "op": "PUSH1",
+            "value": "0x1"
+        },
+        "923": {
+            "op": "PUSH1",
+            "value": "0x1"
+        },
+        "925": {
+            "op": "PUSH1",
+            "value": "0xA0"
+        },
+        "927": {
+            "op": "SHL"
+        },
+        "928": {
+            "op": "SUB"
+        },
+        "929": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7791,
+                7812
+            ],
+            "op": "DUP3",
+            "path": "1",
+            "statement": 20
+        },
+        "93": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "EQ",
+            "path": "5"
+        },
+        "930": {
+            "branch": 36,
+            "fn": "ERC20._mint",
+            "offset": [
+                7791,
+                7812
+            ],
+            "op": "AND",
+            "path": "1"
+        },
+        "931": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7787,
+                7878
+            ],
+            "op": "PUSH2",
+            "path": "1",
+            "value": "0x3C2"
+        },
+        "934": {
+            "branch": 36,
+            "fn": "ERC20._mint",
+            "offset": [
+                7787,
+                7878
+            ],
+            "op": "JUMPI",
+            "path": "1"
+        },
+        "935": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x40"
+        },
+        "937": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "MLOAD",
+            "path": "1"
+        },
+        "938": {
+            "op": "PUSH4",
+            "value": "0xEC442F05"
+        },
+        "94": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH2",
+            "path": "5",
+            "value": "0x171"
+        },
+        "943": {
+            "op": "PUSH1",
+            "value": "0xE0"
+        },
+        "945": {
+            "op": "SHL"
+        },
+        "946": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "DUP2",
+            "path": "1"
+        },
+        "947": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "MSTORE",
+            "path": "1"
+        },
+        "948": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7864,
+                7865
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x0"
+        },
+        "950": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x4"
+        },
+        "952": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "DUP3",
+            "path": "1"
+        },
+        "953": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "ADD",
+            "path": "1"
+        },
+        "954": {
+            "op": "MSTORE"
+        },
+        "955": {
+            "op": "PUSH1",
+            "value": "0x24"
+        },
+        "957": {
+            "op": "ADD"
+        },
+        "958": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7835,
+                7867
+            ],
+            "op": "PUSH2",
+            "path": "1",
+            "value": "0x31B"
+        },
+        "961": {
+            "op": "JUMP"
+        },
+        "962": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7787,
+                7878
             ],
             "op": "JUMPDEST",
-            "path": "2"
+            "path": "1"
+        },
+        "963": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7887,
+                7922
+            ],
+            "op": "PUSH2",
+            "path": "1",
+            "statement": 21,
+            "value": "0x3CE"
+        },
+        "966": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7903,
+                7904
+            ],
+            "op": "PUSH1",
+            "path": "1",
+            "value": "0x0"
+        },
+        "968": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7907,
+                7914
+            ],
+            "op": "DUP4",
+            "path": "1"
+        },
+        "969": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7916,
+                7921
+            ],
+            "op": "DUP4",
+            "path": "1"
         },
         "97": {
             "fn": null,
             "offset": [
                 104,
-                343
+                260
             ],
             "op": "JUMPI",
-            "path": "6"
+            "path": "5"
         },
         "970": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7887,
+                7894
+            ],
+            "op": "PUSH2",
+            "path": "1",
+            "value": "0x4A7"
+        },
+        "973": {
+            "fn": "ERC20._mint",
+            "jump": "i",
+            "offset": [
+                7887,
+                7922
+            ],
+            "op": "JUMP",
+            "path": "1"
+        },
+        "974": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7887,
+                7922
+            ],
+            "op": "JUMPDEST",
+            "path": "1"
+        },
+        "975": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7721,
+                7929
+            ],
+            "op": "POP",
+            "path": "1"
+        },
+        "976": {
+            "fn": "ERC20._mint",
+            "offset": [
+                7721,
+                7929
+            ],
+            "op": "POP",
+            "path": "1"
+        },
+        "977": {
+            "fn": "ERC20._mint",
+            "jump": "o",
+            "offset": [
+                7721,
+                7929
+            ],
+            "op": "JUMP",
+            "path": "1"
+        },
+        "978": {
+            "fn": "ERC20._approve",
+            "offset": [
+                9949,
+                10381
+            ],
+            "op": "JUMPDEST",
+            "path": "1"
+        },
+        "979": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "972": {
+        "98": {
+            "fn": null,
+            "offset": [
+                104,
+                260
+            ],
+            "op": "PUSH1",
+            "path": "5",
+            "value": "0x0"
+        },
+        "981": {
             "op": "PUSH1",
             "value": "0x1"
         },
-        "974": {
+        "983": {
             "op": "PUSH1",
             "value": "0xA0"
         },
-        "976": {
+        "985": {
             "op": "SHL"
         },
-        "977": {
+        "986": {
             "op": "SUB"
         },
-        "978": {
+        "987": {
             "fn": "ERC20._approve",
             "offset": [
                 10061,
                 10080
             ],
             "op": "DUP5",
-            "path": "2",
+            "path": "1",
             "statement": 22
         },
-        "979": {
+        "988": {
             "branch": 37,
             "fn": "ERC20._approve",
             "offset": [
                 10061,
                 10080
             ],
             "op": "AND",
-            "path": "2"
-        },
-        "98": {
-            "fn": null,
-            "offset": [
-                104,
-                343
-            ],
-            "op": "PUSH1",
-            "path": "6",
-            "value": "0x0"
+            "path": "1"
         },
-        "980": {
+        "989": {
             "fn": "ERC20._approve",
             "offset": [
                 10057,
                 10146
             ],
             "op": "PUSH2",
-            "path": "2",
-            "value": "0x3F3"
+            "path": "1",
+            "value": "0x3FC"
         },
-        "983": {
+        "992": {
             "branch": 37,
             "fn": "ERC20._approve",
             "offset": [
                 10057,
                 10146
             ],
             "op": "JUMPI",
-            "path": "2"
+            "path": "1"
         },
-        "984": {
+        "993": {
             "fn": "ERC20._approve",
             "offset": [
                 10103,
                 10135
             ],
             "op": "PUSH1",
-            "path": "2",
+            "path": "1",
             "value": "0x40"
         },
-        "986": {
+        "995": {
             "fn": "ERC20._approve",
             "offset": [
                 10103,
                 10135
             ],
             "op": "MLOAD",
-            "path": "2"
+            "path": "1"
         },
-        "987": {
+        "996": {
             "op": "PUSH4",
             "value": "0xE602DF05"
-        },
-        "992": {
-            "op": "PUSH1",
-            "value": "0xE0"
-        },
-        "994": {
-            "op": "SHL"
-        },
-        "995": {
-            "fn": "ERC20._approve",
-            "offset": [
-                10103,
-                10135
-            ],
-            "op": "DUP2",
-            "path": "2"
-        },
-        "996": {
-            "fn": "ERC20._approve",
-            "offset": [
-                10103,
-                10135
-            ],
-            "op": "MSTORE",
-            "path": "2"
-        },
-        "997": {
-            "fn": "ERC20._approve",
-            "offset": [
-                10132,
-                10133
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x0"
-        },
-        "999": {
-            "fn": "ERC20._approve",
-            "offset": [
-                10103,
-                10135
-            ],
-            "op": "PUSH1",
-            "path": "2",
-            "value": "0x4"
         }
     },
-    "sha1": "d9ceabaaf80ef09ba96909bbac7b4d43456b5711",
-    "source": "pragma solidity >=0.8.2 <0.9.0;\n\n\nimport {ERC20} from \"@openzeppelin/contracts/token/ERC20/ERC20.sol\";\n\ncontract USDC is ERC20 {\n\n    constructor() ERC20(\"USDC\", \"USDC\") {}\n\n    function mint() external{\n        _mint(msg.sender, 5 * (10 ** 6));\n    }\n\n    function decimals() public view override returns (uint8) {\n        return 6;\n    }\n\n\n}",
-    "sourceMap": "104:239:6:-:0;;;134:38;;;;;;;;;-1:-1:-1;1896:113:2;;;;;;;;;;;;-1:-1:-1;;;1896:113:2;;;;;;;;;;;;;;;;;;;;;;;1962:5;:13;1896:113;1962:5;:13;:::i;:::-;-1:-1:-1;1985:7:2;:17;1995:7;1985;:17;:::i;:::-;;1896:113;;104:239:6;;14:127:8;75:10;70:3;66:20;63:1;56:31;106:4;103:1;96:15;130:4;127:1;120:15;146:380;225:1;221:12;;;;268;;;289:61;;343:4;335:6;331:17;321:27;;289:61;396:2;388:6;385:14;365:18;362:38;359:161;;442:10;437:3;433:20;430:1;423:31;477:4;474:1;467:15;505:4;502:1;495:15;359:161;;146:380;;;:::o;657:543::-;759:2;754:3;751:11;748:446;;;795:1;819:5;816:1;809:16;863:4;860:1;850:18;933:2;921:10;917:19;914:1;910:27;904:4;900:38;969:4;957:10;954:20;951:47;;;-1:-1:-1;992:4:8;951:47;1047:2;1042:3;1038:12;1035:1;1031:20;1025:4;1021:31;1011:41;;1102:82;1120:2;1113:5;1110:13;1102:82;;;1165:17;;;1146:1;1135:13;1102:82;;;1106:3;;;748:446;657:543;;;:::o;1376:1345::-;1496:10;;-1:-1:-1;;;;;1518:30:8;;1515:56;;;1551:18;;:::i;:::-;1580:97;1670:6;1630:38;1662:4;1656:11;1630:38;:::i;:::-;1624:4;1580:97;:::i;:::-;1732:4;;1789:2;1778:14;;1806:1;1801:663;;;;2508:1;2525:6;2522:89;;;-1:-1:-1;2577:19:8;;;2571:26;2522:89;-1:-1:-1;;1333:1:8;1329:11;;;1325:24;1321:29;1311:40;1357:1;1353:11;;;1308:57;2624:81;;1771:944;;1801:663;604:1;597:14;;;641:4;628:18;;-1:-1:-1;;1837:20:8;;;1955:236;1969:7;1966:1;1963:14;1955:236;;;2058:19;;;2052:26;2037:42;;2150:27;;;;2118:1;2106:14;;;;1985:19;;1955:236;;;1959:3;2219:6;2210:7;2207:19;2204:201;;;2280:19;;;2274:26;-1:-1:-1;;2363:1:8;2359:14;;;2375:3;2355:24;2351:37;2347:42;2332:58;2317:74;;2204:201;-1:-1:-1;;;;;2451:1:8;2435:14;;;2431:22;2418:36;;-1:-1:-1;1376:1345:8:o;:::-;104:239:6;;;;;;",
+    "sha1": "b9f6271545ea492fb7095639b84c284a9ebcd380",
+    "source": "pragma solidity >=0.8.2 <0.9.0;\n\n\nimport {ERC20} from \"@openzeppelin/contracts/token/ERC20/ERC20.sol\";\n\ncontract USDC is ERC20 {\n\n    constructor() ERC20(\"USDC\", \"USDC\") {}\n\n    function mint(uint256 value) external{\n        _mint(msg.sender, value);\n    }\n\n\n}",
+    "sourceMap": "104:156:5:-:0;;;134:38;;;;;;;;;-1:-1:-1;1896:113:1;;;;;;;;;;;;-1:-1:-1;;;1896:113:1;;;;;;;;;;;;;;;;;;;;;;;1962:5;:13;1896:113;1962:5;:13;:::i;:::-;-1:-1:-1;1985:7:1;:17;1995:7;1985;:17;:::i;:::-;;1896:113;;104:156:5;;14:127:6;75:10;70:3;66:20;63:1;56:31;106:4;103:1;96:15;130:4;127:1;120:15;146:380;225:1;221:12;;;;268;;;289:61;;343:4;335:6;331:17;321:27;;289:61;396:2;388:6;385:14;365:18;362:38;359:161;;442:10;437:3;433:20;430:1;423:31;477:4;474:1;467:15;505:4;502:1;495:15;359:161;;146:380;;;:::o;657:543::-;759:2;754:3;751:11;748:446;;;795:1;819:5;816:1;809:16;863:4;860:1;850:18;933:2;921:10;917:19;914:1;910:27;904:4;900:38;969:4;957:10;954:20;951:47;;;-1:-1:-1;992:4:6;951:47;1047:2;1042:3;1038:12;1035:1;1031:20;1025:4;1021:31;1011:41;;1102:82;1120:2;1113:5;1110:13;1102:82;;;1165:17;;;1146:1;1135:13;1102:82;;;1106:3;;;748:446;657:543;;;:::o;1376:1345::-;1496:10;;-1:-1:-1;;;;;1518:30:6;;1515:56;;;1551:18;;:::i;:::-;1580:97;1670:6;1630:38;1662:4;1656:11;1630:38;:::i;:::-;1624:4;1580:97;:::i;:::-;1732:4;;1789:2;1778:14;;1806:1;1801:663;;;;2508:1;2525:6;2522:89;;;-1:-1:-1;2577:19:6;;;2571:26;2522:89;-1:-1:-1;;1333:1:6;1329:11;;;1325:24;1321:29;1311:40;1357:1;1353:11;;;1308:57;2624:81;;1771:944;;1801:663;604:1;597:14;;;641:4;628:18;;-1:-1:-1;;1837:20:6;;;1955:236;1969:7;1966:1;1963:14;1955:236;;;2058:19;;;2052:26;2037:42;;2150:27;;;;2118:1;2106:14;;;;1985:19;;1955:236;;;1959:3;2219:6;2210:7;2207:19;2204:201;;;2280:19;;;2274:26;-1:-1:-1;;2363:1:6;2359:14;;;2375:3;2355:24;2351:37;2347:42;2332:58;2317:74;;2204:201;-1:-1:-1;;;;;2451:1:6;2435:14;;;2431:22;2418:36;;-1:-1:-1;1376:1345:6:o;:::-;104:156:5;;;;;;",
     "sourcePath": "contracts/ExampleUSDC.sol",
     "type": "contract"
 }
```

### Comparing `forumaisdk-0.0.2/PKG-INFO` & `forumaisdk-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forumaisdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: ForumAI Python SDK
 Author-email: ForumAISDK <forumai@github.com>
 Project-URL: Homepage, https://github.com/0xAresDev/ForumAISDK
 Project-URL: Issues, https://github.com/0xAresDev/ForumAISDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,11 +12,11 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: web3==6.15.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-dotenv
 
-Alpha implementation of the ForumAI model market python SDK. V.1.0.1
+Alpha implementation of the ForumAI model market python SDK. V.0.0.3
 
 Take a look at the docs to find out how to use it: https://forumai.gitbook.io/forumai/developer-guide/integrate-mixtral8x7b-with-python-sdk-testnet
```

### Comparing `forumaisdk-0.0.2/forumaisdk.egg-info/PKG-INFO` & `forumaisdk-0.0.3/forumaisdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forumaisdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: ForumAI Python SDK
 Author-email: ForumAISDK <forumai@github.com>
 Project-URL: Homepage, https://github.com/0xAresDev/ForumAISDK
 Project-URL: Issues, https://github.com/0xAresDev/ForumAISDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,11 +12,11 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: web3==6.15.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-dotenv
 
-Alpha implementation of the ForumAI model market python SDK. V.1.0.1
+Alpha implementation of the ForumAI model market python SDK. V.0.0.3
 
 Take a look at the docs to find out how to use it: https://forumai.gitbook.io/forumai/developer-guide/integrate-mixtral8x7b-with-python-sdk-testnet
```

### Comparing `forumaisdk-0.0.2/pyproject.toml` & `forumaisdk-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Include the ABI files
 [tool.setuptools.package-data]
 ModelMarketSDK = ["*.json"]
 
 [project]
 name = "forumaisdk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="ForumAISDK", email="forumai@github.com" },
 ]
 description = "ForumAI Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

