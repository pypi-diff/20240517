# Comparing `tmp/veg2hab-0.2.1.tar.gz` & `tmp/veg2hab-0.2.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veg2hab-0.2.1.tar", max compression
+gzip compressed data, was "veg2hab-0.2.2a0.tar", max compression
```

## Comparing `veg2hab-0.2.1.tar` & `veg2hab-0.2.2a0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7626 2024-05-07 08:48:39.707739 veg2hab-0.2.1/LICENSE.md
--rw-r--r--   0        0        0    13020 2024-05-07 08:48:39.707739 veg2hab-0.2.1/README.md
--rw-r--r--   0        0        0     1311 2024-05-07 08:48:40.103738 veg2hab-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       72 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/__init__.py
--rw-r--r--   0        0        0     1173 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/__main__.py
--rw-r--r--   0        0        0     6513 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/access_db.py
--rw-r--r--   0        0        0      411 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/constants.py
--rw-r--r--   0        0        0     6384 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/criteria.py
--rw-r--r--   0        0        0     7489 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/definitietabel.py
--rw-r--r--   0        0        0     5414 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/enums.py
--rw-r--r--   0        0        0      576 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/fgr.py
--rw-r--r--   0        0        0    14411 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/habitat.py
--rw-r--r--   0        0        0     5030 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/io/arcgis.py
--rw-r--r--   0        0        0     2328 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/io/cli.py
--rw-r--r--   0        0        0     4296 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/io/common.py
--rw-r--r--   0        0        0     2941 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/main.py
--rw-r--r--   0        0        0    11093 2024-05-07 08:48:40.103738 veg2hab-0.2.1/veg2hab/mozaiek.py
--rw-r--r--   0        0        0 13900219 2024-05-07 08:48:40.155738 veg2hab-0.2.1/veg2hab/package_data/FGR.json
--rw-r--r--   0        0        0    39387 2024-05-07 08:48:40.795737 veg2hab-0.2.1/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
--rw-r--r--   0        0        0    19152 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/package_data/opgeschoonde_waswordt.xlsx
--rw-r--r--   0        0        0     3094 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/package_data/toolbox.pyt
--rw-r--r--   0        0        0    13084 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/validation.py
--rw-r--r--   0        0        0    15069 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/vegetatietypen.py
--rw-r--r--   0        0        0    46327 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/vegkartering.py
--rw-r--r--   0        0        0     4585 2024-05-07 08:48:40.799737 veg2hab-0.2.1/veg2hab/waswordtlijst.py
--rw-r--r--   0        0        0    14049 1970-01-01 00:00:00.000000 veg2hab-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7626 2024-05-17 01:04:43.905056 veg2hab-0.2.2a0/LICENSE.md
+-rw-r--r--   0        0        0    12995 2024-05-17 01:04:43.905056 veg2hab-0.2.2a0/README.md
+-rw-r--r--   0        0        0     1328 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/__init__.py
+-rw-r--r--   0        0        0     1086 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/__main__.py
+-rw-r--r--   0        0        0     6540 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/access_db.py
+-rw-r--r--   0        0        0      411 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/constants.py
+-rw-r--r--   0        0        0     6408 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/criteria.py
+-rw-r--r--   0        0        0     8640 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/definitietabel.py
+-rw-r--r--   0        0        0     5151 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/enums.py
+-rw-r--r--   0        0        0      576 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/fgr.py
+-rw-r--r--   0        0        0    15989 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/habitat.py
+-rw-r--r--   0        0        0     6946 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/io/arcgis.py
+-rw-r--r--   0        0        0     2673 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/io/cli.py
+-rw-r--r--   0        0        0     5305 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/io/common.py
+-rw-r--r--   0        0        0     3051 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/main.py
+-rw-r--r--   0        0        0    10867 2024-05-17 01:04:44.297060 veg2hab-0.2.2a0/veg2hab/mozaiek.py
+-rw-r--r--   0        0        0 13900219 2024-05-17 01:04:44.345060 veg2hab-0.2.2a0/veg2hab/package_data/FGR.json
+-rw-r--r--   0        0        0      130 2024-05-17 01:04:45.073068 veg2hab-0.2.2a0/veg2hab/package_data/opgeschoonde_definitietabel.xlsx
+-rw-r--r--   0        0        0      130 2024-05-17 01:04:45.073068 veg2hab-0.2.2a0/veg2hab/package_data/opgeschoonde_waswordt.xlsx
+-rw-r--r--   0        0        0     2653 2024-05-17 01:04:45.073068 veg2hab-0.2.2a0/veg2hab/package_data/veg2hab.pyt
+-rw-r--r--   0        0        0    13084 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/validation.py
+-rw-r--r--   0        0        0    15272 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/vegetatietypen.py
+-rw-r--r--   0        0        0    47885 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/vegkartering.py
+-rw-r--r--   0        0        0     4585 2024-05-17 01:04:45.077068 veg2hab-0.2.2a0/veg2hab/waswordtlijst.py
+-rw-r--r--   0        0        0    14101 1970-01-01 00:00:00.000000 veg2hab-0.2.2a0/PKG-INFO
```

### Comparing `veg2hab-0.2.1/LICENSE.md` & `veg2hab-0.2.2a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.1/README.md` & `veg2hab-0.2.2a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,35 +24,35 @@
 
 veg2hab wordt gedistribueerd via PyPI, waar alle toekomstige versies aan toe worden gevoegd.
 
 ## Installatie instructies
 
 ### Installatie binnen ArcGIS Pro
 
-Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger. 
-Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven: 
+Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger.
+Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven:
 
  1. Open ArcGIS Pro
- 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren): 
-    - Open de 'Package Manager'  
+ 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren):
+    - Open de 'Package Manager'
         <img src="./images/package_manager.png" alt="package manager" width="400"/>
-    - Klik op het tandwiel naast 'Active Environment'  
-    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.  
-        <img src="./images/new_environment.png" alt="new python environment" width="400"/>  
+    - Klik op het tandwiel naast 'Active Environment'
+    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.
+        <img src="./images/new_environment.png" alt="new python environment" width="400"/>
         <img src="./images/environment_location.png" alt="location of new environment" width="400"/>
     - Selecteer de environment en druk op 'OK'.
  3. Download en installeer veg2hab:
-    - Klik op 'New notebook'  
+    - Klik op 'New notebook'
         <img src="./images/new_notebook.png" alt="new notebook" width="400"/>
-    - Download veg2hab met het commando `!pip install --upgrade veg2hab`  
+    - Download veg2hab met het commando `!pip install --upgrade veg2hab`
         <img src="./images/notebook_prompts.png" alt="prompts in notebook to install veg2hab" width="400"/>
     - Installeer veg2hab met het commando `import veg2hab`
  4. Installeer de veg2hab Python Toolbox:
     - Gebruik het commando `veg2hab.installatie_instructies()` om de locatie van de toolbox te vinden
-    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie  
+    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie
         <img src="./images/add_toolbox.png" alt="adding the veg2hab Python Toolbox" width="400"/>
 
 Als het goed is, wordt de veg2hab toolbox nu getoond in de Geoprocessing tab:
 
 <img src="./images/geoprocessing_tab.png" alt="geoprocessing tab" width="400"/>
 
 
@@ -67,31 +67,31 @@
 
 ### Gebruik in ArcGIS Pro
 
 De omzetting van veg2hab van vegetatiekarteringen naar habitattypekaarten gebeurt in tools in de veg2hab Python Toolbox. Om de omzetting te doen, dient de gebruiker eerst de betreffende vegetatiekarteringen in te laden als kaart in ArcGIS Pro.
 
 De omzettool komt in twee smaken:
 1. `digitale_standaard`, voor het omzetten van vegetatiekarteringen die de landelijke digitale standaard gebruiken, die bestaat uit een shapefile gecombineerd met een access database. De gebruiker voert in welke vegetatiekarteringen omgezet moet worden en waar de bijhorende access database te vinden is.
-2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat. 
+2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat.
 
 Let op:
 - Wanneer de gebruiker beschikt over een access database, raden wij aan de  `digitale_standaard` omzetting te gebruiken, ook als de shapefile alle informatie bevat. Hierbij is de kans op handmatige fouten kleiner.
-- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN). 
+- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN).
 
 
 ### Bronbestanden die veg2hab gebruikt
 
-veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen. 
+veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen.
 
-Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker: 
+Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker:
 
  - [WasWordtLijst](./data/5.%20Was-wordt-lijst-vegetatietypen-en-habitattypen-09-02-2021.xlsx) (versie 09-feb-2021): dit bestand wordt gebruikt om landelijke vegetatietypologieën in elkaar om te zetten
  - [DefinitieTabel](./data/definitietabel%20habitattypen%20(versie%2024%20maart%202009)_0.xls) (versie 24 maart 2009): dit is een samenvatting van de profieldocumenten
  - [Fysisch-Geografische Regio kaart](./data/bronbestanden/FGR.json) (versie 2013, [link naar origineel op Nationaal georegister](https://nationaalgeoregister.nl/geonetwork/srv/dut/catalog.search#/metadata/c8b5668f-c354-42f3-aafc-d15ae54cf170))
-  
+
 Let op: bij volgende versies komen er waarschijnlijk meer bronbestanden bij.
 
 
 
 ## Handleiding voor ontwikkelaars
 ### Lokale ontwikkeling
 Download de git repository:
@@ -120,15 +120,15 @@
 poetry run pytest tests/
 ```
 
 ### Nieuwe release
 1. Zorg ervoor dat de laatste bronbestanden in package_data staan met `poetry run python release.py create-package-data`.
 2. Maak een nieuwe versie met poetry (major, minor, patch): `poetry version {{rule}}`
 3. Pas de [\_\_init\_\_.py](veg2hab/__init__.py) __version__ variabele aan zodat deze overeen komt met de nieuw poetry version
-4. Pas [toolbox.pyt](veg2hab/package_data/toolbox.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan toolbox.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
+4. Pas [veg2hab.pyt](veg2hab/package_data/veg2hab.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan veg2hab.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
 5. Draai `python release.py check-versions` om te checken dat je geen fouten hebt gemaakt.
 6. Push nu eerst je nieuwe wijzigingen (mochten die er zijn), naar github. (`git add`, `git commit`, `git push`)
 7. Maak een nieuwe tag: `git tag v$(poetry version -s)`
 8. Push de tag naar git `git push origin tag v$(poetry version -s)`
 9. Github actions zal automatisch de nieuwe versie op PyPI zetten.
 
 
@@ -143,18 +143,18 @@
 
 **ElmID**: Een voor ieder vlak uniek ID. Deze kan vanuit de bronkartering komen, maar kan ook nieuw zijn gegenereerd. Dit gebeurt de als ElmID (of een ElmID equivalent zoals OBJECTID) in de bronkartering niet voor ieder vlak uniek is; als dit het geval is is hierover een warning gegeven.
 
 **_Samnvttng**: Weergave van hoeveel procent van het vlak bedekt is met welk habitattype. Dit is een combinatie van alle kolommen `Habtype{i}` en `Perc{i}`.
 
 **_LokVegTyp**: Het in de bronkartering opgegeven lokale vegetatietype, als er een lokaal vegetatietype kolom is opgegeven.
 
-**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan. 
+**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan.
 
 ### Complex-deel-specifieke kolommen
-**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel. 
+**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel.
 
 **Perc{i}**: Percentage van het gehele vlak wat door dit complex-deel wordt bedekt.
 
 **Opp{i}**: Oppervlakte van dit complex-deel in m2.
 
 **Kwal{i}**: Kwaliteit van dit complex-deel. Dit kan zijn G (goed), M (matig) of X (nvt).
```

### Comparing `veg2hab-0.2.1/pyproject.toml` & `veg2hab-0.2.2a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "veg2hab"
-version = "0.2.1"
+version = "0.2.2a0"
 description = "Package voor automatisch omzetten van vegetatiekarteringen naar habitatkaarten"
 authors = ["Spheer.ai <info@spheer.ai>"]
 readme = "README.md"
-license = "LGPLv3" 
+license = "LGPLv3"
 classifiers = [
   "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -16,23 +16,24 @@
 
 [project.urls]
 Homepage = "https://github.com/Spheer-ai/veg2hab"
 Issues = "https://github.com/Spheer-ai/veg2hab/issues"
 Source = "https://github.com/Spheer-ai/veg2hab"
 
 [tool.poetry.scripts]
-veg2hab = "veg2hab.__main__:main"
+veg2hab = "veg2hab.__main__:veg2hab"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-geopandas = ">=0.10.0"
-openpyxl = ">=3.0.0"
-xlrd = ">=2.0.1"
-pyodbc= ">=4.0.1"
-pydantic = ">=1.0,<2.0"
+python = ">=3.7.1,<4.0"
+pandas = "^1.3.0"
+geopandas = "^0.10.0"
+openpyxl = "^3.1.0"
+xlrd = "^2.0.1"
+pyodbc= "^4.0.1"
+pydantic = "^1.10.0"
 setuptools = "<60.0.0"
 pygeos = "^0.14"
 typing-extensions = "4.7.1"
 click = "^8.1.7"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = ">=6.0.0"
```

### Comparing `veg2hab-0.2.1/veg2hab/__main__.py` & `veg2hab-0.2.2a0/veg2hab/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import logging
-import subprocess
-from pathlib import Path
 
 import click
 
 import veg2hab
-from veg2hab import constants
-from veg2hab.definitietabel import opschonen_definitietabel
+from veg2hab import main
 from veg2hab.io.cli import CLIAccessDBInputs, CLIInterface, CLIShapefileInputs
-from veg2hab.waswordtlijst import opschonen_waswordtlijst
 
 
-@click.group(name="veg2hab")
+@click.group()
 @click.version_option(veg2hab.__version__)
-@click.option("-v", "--verbose", count=True)
-def main(verbose: int):
+@click.option(
+    "-v", "--verbose", count=True, help="Increase verbosity, use -vv for debug info"
+)
+def veg2hab(verbose: int):
     if verbose == 0:
         log_level = logging.WARNING
     elif verbose == 1:
         log_level = logging.INFO
     else:
         log_level = logging.DEBUG
 
     CLIInterface.get_instance().instantiate_loggers(log_level)
 
 
-@main.command(
+@veg2hab.command(
     name=CLIAccessDBInputs.label,
     help=CLIAccessDBInputs.get_argument_description(),
 )
 @CLIAccessDBInputs.click_decorator
 def digitale_standaard(**kwargs):
-    print(kwargs)
     params = CLIAccessDBInputs(**kwargs)
+    main.run(params)
 
 
-@main.command(
+@veg2hab.command(
     name=CLIShapefileInputs.label,
     help=CLIShapefileInputs.get_argument_description(),
 )
 @CLIShapefileInputs.click_decorator
 def vector_bestand(**kwargs):
     params = CLIShapefileInputs(**kwargs)
+    main.run(params)
 
 
 if __name__ == "__main__":
-    main()
+    veg2hab()
```

### Comparing `veg2hab-0.2.1/veg2hab/access_db.py` & `veg2hab-0.2.2a0/veg2hab/access_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     # the pyodb is not officially suppported by pandas, so we suppress that
     # warning:
     with warnings.catch_warnings():
         warnings.simplefilter(action="ignore", category=UserWarning)
         return pd.read_sql(
             f"SELECT {','.join(col_names.keys())} FROM {table_name.value}",
             conn,
-            dtype=col_names,
-        )
+            columns=col_names.keys(),
+        ).astype(col_names)
 
 
 @read_table.register
 def _(folder: Path, table_name: TableNames, col_names: Dict[str, Any]) -> pd.DataFrame:
     return pd.read_csv(
         folder / f"{table_name.value}.csv",
         usecols=list(col_names.keys()),
```

### Comparing `veg2hab-0.2.1/veg2hab/criteria.py` & `veg2hab-0.2.2a0/veg2hab/criteria.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,23 +75,24 @@
     def check(self, row: gpd.GeoSeries) -> None:
         self._evaluation = MaybeBoolean.TRUE
 
     def __str__(self):
         return "Geen mits (altijd waar)"
 
 
-class PlaceholderCriterium(BeperkendCriterium):
-    type: ClassVar[str] = "Placeholder"
+class NietGeautomatiseerdCriterium(BeperkendCriterium):
+    type: ClassVar[str] = "NietGeautomatiseerd"
+    toelichting: str
     _evaluation: Optional[MaybeBoolean] = PrivateAttr(default=None)
 
     def check(self, row: gpd.GeoSeries) -> None:
         self._evaluation = MaybeBoolean.CANNOT_BE_AUTOMATED
 
     def __str__(self):
-        return "Placeholder mits (nog niet geimplementeerd) (nooit waar)"
+        return f"(Niet geautomatiseerd: {self.toelichting})"
 
 
 class FGRCriterium(BeperkendCriterium):
     type: ClassVar[str] = "FGRCriterium"
     fgrtype: FGRType
     _evaluation: Optional[MaybeBoolean] = PrivateAttr(default=None)
```

### Comparing `veg2hab-0.2.1/veg2hab/definitietabel.py` & `veg2hab-0.2.2a0/veg2hab/definitietabel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import copy
+import json
 import logging
 from functools import lru_cache
 from pathlib import Path
 from typing import List, Union
 
 import pandas as pd
 
 from veg2hab.criteria import BeperkendCriterium
 from veg2hab.enums import Kwaliteit
 from veg2hab.habitat import HabitatVoorstel
+from veg2hab.io.common import Interface
 from veg2hab.mozaiek import (  # DummyMozaiekregel,; GeenMozaiekregel,
     MozaiekRegel,
     StandaardMozaiekregel,
 )
 from veg2hab.vegetatietypen import SBB, VvN
 from veg2hab.vegkartering import VegTypeInfo
 
@@ -90,15 +92,21 @@
             voorstel = copy.deepcopy(self._find_habtypes_for_code(code))
             for item in voorstel:
                 item.percentage = info.percentage
                 item.vegtypeinfo = info
             voorstellen += voorstel
 
         if len(voorstellen) == 0:
-            voorstellen.append(HabitatVoorstel.H0000_vegtype_not_in_dt(info))
+            niet_geautomatiseerde_sbb = (
+                Interface.get_instance().get_config().niet_geautomatiseerde_sbb
+            )
+            if len(info.SBB) > 0 and str(info.SBB[0]) in niet_geautomatiseerde_sbb:
+                voorstellen.append(HabitatVoorstel.HXXXX_niet_geautomatiseerd_SBB(info))
+            else:
+                voorstellen.append(HabitatVoorstel.H0000_vegtype_not_in_dt(info))
 
         return voorstellen
 
     @lru_cache(maxsize=256)
     def _find_habtypes_for_code(
         self, code: Union[SBB, VvN, None]
     ) -> List[HabitatVoorstel]:
@@ -146,16 +154,19 @@
 ) -> None:
     """
     Ontvangt een was-wordt lijst en output een opgeschoonde was-wordt lijst.
     Voegt ook json voor de mitsen toe vanuit path_in_json_def.
     """
     assert path_in_deftabel.suffix == ".xls", "Input deftabel file is not an xls file"
     assert (
-        path_in_mitsjson.suffix == ".csv"
-    ), "Input json definitions file is not an csv file"
+        path_in_mitsjson.suffix == ".json"
+    ), "Input json definitions file is not a json file"
+    assert (
+        path_in_mozaiekjson.suffix == ".json"
+    ), "Input mozaiek json definitions file is not a json file"
     assert path_out.suffix == ".xlsx", "Output file is not an xlsx file"
 
     ### Inladen
     dt = pd.read_excel(
         path_in_deftabel,
         engine="xlrd",
         usecols=[
@@ -199,27 +210,40 @@
         dt["VvN"], print_invalid=True
     ), "Niet alle VvN codes zijn valid"
 
     # Reorder
     dt = dt[["DT regel", "Habitattype", "Kwaliteit", "SBB", "VvN", "mits", "mozaiek"]]
 
     ### Mits json definities toevoegen
-    # TODO: .json van maken
-    mitsjson = pd.read_csv(path_in_mitsjson, sep="|")
+    with open(path_in_mitsjson, "r", encoding="utf-8") as file:
+        data = json.load(file)
+    mitsjson = pd.DataFrame(
+        [{"mits": key, "mitsjson": value} for key, value in data.items()]
+    )
 
     # Checken dat we alle mitsen in dt ook in mitsjson hebben
     for mits in dt.mits.dropna().unique():
         if mits not in mitsjson.mits.unique():
             raise ValueError(f"Mits {mits} is niet gevonden in mitsjson")
 
+    # NaN vervangen door lege strings zodat hier GeenCriteria vanuit mitsjson op matchen
+    dt.mits[dt.mits.isna()] = ""
     dt = dt.merge(mitsjson, on="mits", how="left")
+    dt["mitsjson"] = dt.mitsjson.apply(json.dumps)
 
     ### Mozaiek json definities toevoegen
-    mozaiekjson = pd.read_csv(path_in_mozaiekjson, sep="|")
+    with open(path_in_mozaiekjson, "r", encoding="utf-8") as file:
+        data = json.load(file)
+    mozaiekjson = pd.DataFrame(
+        [{"mozaiek": key, "mozaiekjson": value} for key, value in data.items()]
+    )
 
     for mozaiek in dt.mozaiek.dropna().unique():
         if mozaiek not in mozaiekjson.mozaiek.unique():
             raise ValueError(f"Mozaiek {mozaiek} is niet gevonden in mozaiekjson")
 
+    # NaN vervangen door lege strings zodat hier GeenMozaiek vanuit mozaiekjson op matchen
+    dt["mozaiek"] = dt["mozaiek"].fillna("")
     dt = dt.merge(mozaiekjson, on="mozaiek", how="left")
+    dt["mozaiekjson"] = dt.mozaiekjson.apply(json.dumps)
 
     dt.to_excel(path_out, index=False)
```

### Comparing `veg2hab-0.2.1/veg2hab/enums.py` & `veg2hab-0.2.2a0/veg2hab/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class MaybeBoolean(Enum):
     FALSE = 1
 
     # MAYBE = 2
 
-    # Voor dingen die niet geautomatiseerd kunnen worden (bijv. placeholder criteria)
+    # Voor dingen die niet geautomatiseerd kunnen worden (bijv. NietGeautomatiseerdCriterium)
     CANNOT_BE_AUTOMATED = 3
 
     # Voor als evaluatie later nog eens geprobeerd moet worden (bijv. mozaiekregels waar nog
     # onvoldoende omliggende vlakken een habitattype hebben)
     POSTPONE = 4
 
     TRUE = 5
@@ -112,42 +112,37 @@
 
     # Vlak heeft uit de kartering geen vegetatietypen
     GEEN_OPGEGEVEN_VEGTYPEN = auto()
 
     # Meerdere even specifieke habitatvoorstellen met kloppende mitsen
     MEERDERE_KLOPPENDE_MITSEN = auto()
 
-    # Er zijn PlaceholderCriteriums, dus handmatige controle
-    PLACEHOLDER = auto()
+    # Er zijn NietGeautomatiseerdCriteriums, dus handmatige controle
+    NIET_GEAUTOMATISEERD_CRITERIUM = auto()
 
-    # # Dit gaat Veg2Hab niet op kunnen lossen
-    # HANDMATIGE_CONTROLE = auto()
+    # Er is een vegetatietype dat we niet kunnen omzetten
+    NIET_GEAUTOMATISEERD_VEGTYPE = auto()
 
     # Er is meer dan threshold % HXXXX in de omliggende vlakken
     WACHTEN_OP_MOZAIEK = auto()
 
+    __toelichting = {
+        "DUIDELIJK": "Als alle regels gevolgd worden is er 1 duidelijke optie; er is maar 1 habitatvoorstel met kloppende mits/mozaiek.",
+        "GEEN_KLOPPENDE_MITSEN": "Er is geen habitatvoorstel met kloppende mits/mozaiek. Er kan dus geen habitattype toegekend worden.",
+        "VEGTYPEN_NIET_IN_DEFTABEL": "De vegetatietypen van het vlak zijn niet in de definitietabel gevonden en leiden dus niet tot een habitattype.",
+        "GEEN_OPGEGEVEN_VEGTYPEN": "Er zijn in de vegetatiekartering geen (habitatwaardige)vegetatietypen opgegeven voor dit vlak. Er is dus geen habitattype toe te kennen.",
+        "MEERDERE_KLOPPENDE_MITSEN": "Er zijn meerdere habitatvoorstellen met kloppende mits/mozaiek. Er is geen duidelijke keuze te maken.",
+        "NIET_GEAUTOMATISEERD_CRITERIUM": "Er zijn niet-geautomatiseerde mitsen/mozaiekregels gevonden; deze kunnen niet door Veg2Hab worden gecontroleerd.",
+        "NIET_GEAUTOMATISEERD_VEGTYPE": "Er is een vegetatietype dat niet geautomatiseerd kan worden omgezet naar een habitattype.",
+        "WACHTEN_OP_MOZAIEK": "Er is te weinig informatie over de habitattypen van omliggende vlakken (teveel HXXXX)",
+    }
+
+    @property
     def toelichting(self):
-        if self == KeuzeStatus.DUIDELIJK:
-            return "Als alle regels gevolgd worden is er 1 duidelijke optie; er is maar 1 habitatvoorstel met kloppende mits/mozaiek."
-        elif self == KeuzeStatus.GEEN_KLOPPENDE_MITSEN:
-            return "Er is geen habitatvoorstel met kloppende mits/mozaiek. Er kan dus geen habitattype toegekend worden."
-        elif self == KeuzeStatus.VEGTYPEN_NIET_IN_DEFTABEL:
-            return "De vegetatietypen van het vlak zijn niet in de definitietabel gevonden en leiden dus niet tot een habitattype."
-        elif self == KeuzeStatus.GEEN_OPGEGEVEN_VEGTYPEN:
-            return "Er zijn in de vegetatiekartering geen (habitatwaardige)vegetatietypen opgegeven voor dit vlak. Er is dus geen habitattype toe te kennen."
-        elif self == KeuzeStatus.MEERDERE_KLOPPENDE_MITSEN:
-            return "Er zijn meerdere habitatvoorstellen met kloppende mits/mozaiek. Er is geen duidelijke keuze te maken."
-        elif self == KeuzeStatus.PLACEHOLDER:
-            return "Er zijn placeholder mitsen/mozaiekregels gevonden; deze kunnen (nog) niet door Veg2Hab worden gecontroleerd."
-        # elif self == KeuzeStatus.HANDMATIGE_CONTROLE:
-        #     assert (
-        #         False
-        #     ), "Bij KeuzeStatus.HANDMATIGE_CONTROLE moet nog een mooie toelichting, maar ik weet nu nog niet hoe of wat precies, want deze KeuzeStatus is nog niet in gebruik."
-        elif self == KeuzeStatus.WACHTEN_OP_MOZAIEK:
-            return "Er is te weinig informatie over de habitattypen van omliggende vlakken (teveel HXXXX)"
+        return self.__toelichting.value[self.name]
 
 
 class FGRType(Enum):
     DU = "Duinen"
     GG = "Getijdengebied"
     HL = "Heuvelland"
     HZ = "Hogere Zandgronden"
```

### Comparing `veg2hab-0.2.1/veg2hab/fgr.py` & `veg2hab-0.2.2a0/veg2hab/fgr.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.1/veg2hab/habitat.py` & `veg2hab-0.2.2a0/veg2hab/habitat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import List, Optional, Tuple, Union
 
 from veg2hab.criteria import BeperkendCriterium, GeenCriterium
 from veg2hab.enums import KeuzeStatus, Kwaliteit, MatchLevel, MaybeBoolean
-from veg2hab.mozaiek import (
-    GeenMozaiekregel,
-    MozaiekRegel,
-    StandaardMozaiekregel,
-    is_mozaiek_type_present,
-)
+from veg2hab.io.common import Interface
+from veg2hab.mozaiek import GeenMozaiekregel, MozaiekRegel, is_mozaiek_type_present
 from veg2hab.vegetatietypen import SBB as _SBB
 from veg2hab.vegetatietypen import VvN as _VvN
 
 
 @dataclass
 class HabitatVoorstel:
     """
@@ -54,14 +50,28 @@
             kwaliteit=Kwaliteit.NVT,
             idx_in_dt=None,
             mits=GeenCriterium(),
             mozaiek=GeenMozaiekregel(),
             match_level=MatchLevel.NO_MATCH,
         )
 
+    @classmethod
+    def HXXXX_niet_geautomatiseerd_SBB(cls, info: "VegTypeInfo"):
+        assert len(info.SBB) > 0
+        return cls(
+            onderbouwend_vegtype=info.SBB[0],
+            vegtype_in_dt=None,
+            habtype="HXXXX",
+            kwaliteit=Kwaliteit.NVT,
+            idx_in_dt=None,
+            mits=GeenCriterium(),
+            mozaiek=GeenMozaiekregel(),
+            match_level=MatchLevel.NO_MATCH,
+        )
+
 
 @dataclass
 class HabitatKeuze:
     status: KeuzeStatus
     habtype: str  # format = "H1123"
     kwaliteit: Kwaliteit
     habitatvoorstellen: List[HabitatVoorstel]  # used as a refence
@@ -80,15 +90,15 @@
             KeuzeStatus.GEEN_KLOPPENDE_MITSEN,
             KeuzeStatus.VEGTYPEN_NIET_IN_DEFTABEL,
             KeuzeStatus.GEEN_OPGEGEVEN_VEGTYPEN,
         ]:
             assert self.habtype == "H0000"
         elif self.status in [
             KeuzeStatus.WACHTEN_OP_MOZAIEK,
-            KeuzeStatus.PLACEHOLDER,
+            KeuzeStatus.NIET_GEAUTOMATISEERD_CRITERIUM,
             KeuzeStatus.MEERDERE_KLOPPENDE_MITSEN,
         ]:
             assert self.habtype == "HXXXX"
 
         if self.habtype in ["H0000", "HXXXX"]:
             assert self.kwaliteit == Kwaliteit.NVT
 
@@ -181,14 +191,35 @@
             habitatvoorstellen=all_voorstellen,
             opmerking="Er zijn geen vegetatietypen opgegeven voor dit vlak.",
             mits_opmerking="",
             mozaiek_opmerking="",
             debug_info="",
         )
 
+    # Als er maar 1 habitatvoorstel is en dat is HXXXX, kan dat zijn omdat het vegetatietype niet geautomatiseerd is
+    if len(all_voorstellen) == 1 and all_voorstellen[0].habtype == "HXXXX":
+        voorstel = all_voorstellen[0]
+        niet_geautomatiseerde_sbb = (
+            Interface.get_instance().get_config().niet_geautomatiseerde_sbb
+        )
+        if str(voorstel.onderbouwend_vegtype) in niet_geautomatiseerde_sbb:
+            assert isinstance(voorstel.onderbouwend_vegtype, _SBB)
+            assert isinstance(voorstel.mits, GeenCriterium)
+            assert isinstance(voorstel.mozaiek, GeenMozaiekregel)
+            return HabitatKeuze(
+                status=KeuzeStatus.NIET_GEAUTOMATISEERD_VEGTYPE,
+                habtype="HXXXX",
+                kwaliteit=Kwaliteit.NVT,
+                habitatvoorstellen=all_voorstellen,
+                opmerking="Dit vegetatietype is niet geautomatiseerd. Handmatige omzetting is vereist.",
+                mits_opmerking="",
+                mozaiek_opmerking="",
+                debug_info="",
+            )
+
     sublisted_voorstellen = _sublist_per_match_level(all_voorstellen)
 
     # Per MatchLevel checken of er kloppende mitsen zijn
     for current_voorstellen in sublisted_voorstellen:
         truth_values_mits = [
             voorstel.mits.evaluation for voorstel in current_voorstellen
         ]
@@ -243,27 +274,27 @@
 
         # Als er een CANNOT_BE_AUTOMATED is...
         if MaybeBoolean.CANNOT_BE_AUTOMATED in truth_values:
             # ...dan kunnen we voor de huidige voorstellen geen keuze maken
 
             # We weten wel dat habitatvoorstellen met een specifieker matchniveau dan die van
             # de current_voorstellen allemaal FALSE waren, dus die hoeven we niet terug te geven
-            # We filteren ook mits&mozaiek eruit die FALSE zijn; die hangen nm toch niet van een placeholder af.
+            # We filteren ook mits&mozaiek eruit die FALSE zijn; die hangen nm toch niet van een NietGeautomatiseerdCriterium af.
             return_voorstellen = [
                 voorstel
                 for voorstel in all_voorstellen
                 if voorstel.match_level <= current_voorstellen[0].match_level
                 and (
                     voorstel.mits.evaluation & voorstel.mozaiek.evaluation
                     != MaybeBoolean.FALSE
                 )
             ]
 
             return HabitatKeuze(
-                status=KeuzeStatus.PLACEHOLDER,
+                status=KeuzeStatus.NIET_GEAUTOMATISEERD_CRITERIUM,
                 habtype="HXXXX",
                 kwaliteit=Kwaliteit.NVT,
                 habitatvoorstellen=return_voorstellen,
                 opmerking=f"Er zijn mitsen of mozaiekregels die nog niet geimplementeerde zijn. Zie mits/mozk_opm voor meer info in format [opgegeven vegtype, potentieel habtype, mits/mozaiek]",
                 mits_opmerking=f"Mitsen: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mits), str(voorstel.mits.evaluation)] for voorstel in return_voorstellen]}",
                 mozaiek_opmerking=f"Mozaiekregels: {[[str(voorstel.onderbouwend_vegtype), voorstel.habtype, str(voorstel.mozaiek), str(voorstel.mozaiek.evaluation)] for voorstel in return_voorstellen]}",
                 debug_info="",
@@ -271,15 +302,15 @@
 
         # Als er een POSTPONE is...
         if MaybeBoolean.POSTPONE in truth_values:
             # ...dan komt dat door een mozaiekregel waar nog te weinig info over omliggende vlakken voor is
 
             # We weten wel dat habitatvoorstellen met een specifieker matchniveau dan die van
             # de current_voorstellen allemaal FALSE waren, dus die hoeven we niet terug te geven
-            # We filteren ook mits&mozaiek eruit die FALSE zijn; die hangen nm toch niet van een placeholder af.
+            # We filteren ook mits&mozaiek eruit die FALSE zijn; die hangen nm toch niet van een NietGeautomatiseerdCriterium af.
             return_voorstellen = [
                 voorstel
                 for voorstel in all_voorstellen
                 if voorstel.match_level <= current_voorstellen[0].match_level
                 and (
                     voorstel.mits.evaluation & voorstel.mozaiek.evaluation
                     != MaybeBoolean.FALSE
```

### Comparing `veg2hab-0.2.1/veg2hab/io/cli.py` & `veg2hab-0.2.2a0/veg2hab/io/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,46 @@
 import logging
+from datetime import datetime, timezone
 from functools import wraps
-from typing import Callable, Dict
+from pathlib import Path
+from typing import Callable, Dict, Optional
 
 import click
 from geopandas.geodataframe import GeoDataFrame
 from typing_extensions import override
 
 from .common import AccessDBInputs, Interface, ShapefileInputs
 
 
 class CLIInterface(Interface):
     @override
-    def output_shapefile(self, shapefile_id: str, gdf: GeoDataFrame) -> None:
+    def output_shapefile(self, shapefile_id: Optional[Path], gdf: GeoDataFrame) -> None:
+        if shapefile_id is None:
+            shapefile_id = Path(
+                f"./habkart_{datetime.now(timezone.utc).strftime('%Y-%m-%dT%H-%M-%S')}.gpkg"
+            )
         gdf.to_file(shapefile_id, driver="GPKG", layer="main")
 
     @override
     def instantiate_loggers(self, log_level: int) -> None:
         logging.basicConfig(level=log_level)
 
 
 def _decorate_click(func: Callable, param_schema: Dict):
-    for field_name, field_info in reversed(param_schema["properties"].items()):
+    for field_name, field_info in reversed(list(param_schema["properties"].items())):
         is_required = field_name in param_schema["required"]
 
         if field_info.get("format", "") == "path":
-            param_type = click.Path(exists=True)
+            writable = field_name == "output"
+            param_type = click.Path(exists=False, writable=writable)
+        elif "enum" in field_info:
+            param_type = click.Choice(field_info["enum"])
         else:
             param_type = str
 
-        if "enum" in field_info:
-            param_type = click.Choice(field_info["enum"])
-
         if is_required:
             func = click.argument(
                 field_name,
                 type=param_type,
                 required=is_required,
             )(func)
         else:
@@ -45,19 +51,19 @@
                 required=is_required,
             )(func)
 
     return func
 
 
 def _get_argument_description(description: str, param_schema: Dict):
-    description += "\n\n"
+    description += "\n\nArguments:\n\n"
     for field_name, field_info in param_schema["properties"].items():
         if field_name in param_schema["required"]:
             description += (
-                f" - {field_name.upper()}: {field_info.get('description', '')}\n\n"
+                f"  {field_name.upper()}: {field_info.get('description', '')}\n\n"
             )
     return description
 
 
 class CLIAccessDBInputs(AccessDBInputs):
     @classmethod
     def click_decorator(cls, func):
```

### Comparing `veg2hab-0.2.1/veg2hab/io/common.py` & `veg2hab-0.2.2a0/veg2hab/io/common.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,117 @@
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from typing import ClassVar, Optional, Type
+from typing import ClassVar, List, Optional
 
 import geopandas as gpd
-from pydantic import BaseModel, Field
-from typing_extensions import Literal, Self
+from pydantic import BaseModel, BaseSettings, Field
+from typing_extensions import List, Literal, Union
 
 
 class AccessDBInputs(BaseModel):
+    class Config:
+        extra = "forbid"
+
     label: ClassVar[str] = "digitale_standaard"
     description: ClassVar[str] = "Draai veg2hab o.b.v. de digitale standaard"
     shapefile: str = Field(
         description="Locatie van de vegetatiekartering",
     )
     elmid_col: str = Field(
         description="De kolomnaam van de ElementID in de Shapefile; deze wordt gematched aan de Element tabel in de AccessDB",
     )
     access_mdb_path: Path = Field(
         description="Locatie van de .mdb file van de digitale standaard",
     )
-    opmerkingen_column: Optional[str] = Field(
+    datum_col: Optional[str] = Field(
+        default=None,
+        description="Datum kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
+    )
+    opmerking_col: Optional[str] = Field(
         default=None,
         description="Opmerking kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
-    datum_column: Optional[str] = Field(
+    output: Optional[Path] = Field(
         default=None,
-        description="Datum kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
+        description="Output bestand (optioneel), indien niet gegeven wordt er een bestandsnaam gegenereerd",
     )
 
 
 class ShapefileInputs(BaseModel):
+    class Config:
+        extra = "forbid"
+
     label: ClassVar[str] = "vector_bestand"
     description: ClassVar[str] = "Draai veg2hab o.b.v. een vector bestand"
     shapefile: str = Field(
         description="Locatie van de vegetatiekartering",
     )
-    elmid_col: str = Field(
+    elmid_col: Optional[str] = Field(
         description="De kolomnaam van de ElementID in de Shapefile; uniek per vlak",
     )
     vegtype_col_format: Literal["single", "multi"] = Field(
         description='"single" als complexen in 1 kolom zitten of "multi" als er meerdere kolommen zijn',
     )
-    sbb_of_vvn: Literal["VvN", "SBB", "beide"] = Field(
+    sbb_of_vvn: Literal["SBB", "VvN", "beide"] = Field(
         description='"VvN" als VvN de voorname vertaling is vanuit het lokale type, "SBB" voor SBB en "beide" als beide er zijn.'
     )
+    sbb_col: List[str] = Field(
+        default_factory=list,
+        description="SBB kolom(men) (verplicht wanneer het voorname type 'SBB' of 'beide' is)",
+    )
+    vvn_col: List[str] = Field(
+        default_factory=list,
+        description="VvN kolom(men) (verplicht wanneer het voorname type 'VvN' of 'beide' is)",
+    )
+    perc_col: List[str] = Field(
+        default_factory=list,
+        description="Percentage kolom(men) (optioneel)",
+    )
+    lok_vegtypen_col: List[str] = Field(
+        default_factory=list,
+        description="Lokale vegetatietypen kolom(men) (optioneel)",
+    )
+    split_char: Optional[str] = Field(
+        default="+",
+        description='Karakter waarop de complexe vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa"))',
+    )
     datum_col: Optional[str] = Field(
         default=None,
         description="Datum kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
     opmerking_col: Optional[str] = Field(
         default=None,
         description="Opmerking kolom (optioneel), deze wordt onveranderd aan de output meegegeven",
     )
-    SBB_col: Optional[str] = Field(
-        default=None,
-        description="kolomnaam van de SBB vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)",
-    )
-    VvN_col: Optional[str] = Field(
+    output: Optional[Path] = Field(
         default=None,
-        description="kolomnaam van de VvN vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)",
+        description="Output bestand (optioneel), indien niet gegeven wordt er een bestandsnaam gegenereerd",
     )
-    split_char: Optional[str] = Field(
-        default="+",
-        description='karakter waarop de vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa")) (wordt bij mutli_col gebruikt om de kolommen te scheiden)',
+
+
+class Veg2HabConfig(BaseSettings):
+    class Config:
+        env_prefix = "VEG2HAB_"
+
+    mozaiek_threshold: Union[int, float] = Field(
+        default=95.0,  # todo number/float
+        description="Threshold voor het bepalen of een vlak in het mozaiek ligt",
     )
-    perc_col: Optional[str] = Field(
-        default=None,
-        description="kolomnaam van de percentage als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))",
+    mozaiek_als_rand_langs_threshold: Union[int, float] = Field(
+        default=50.0,  # todo number/float
+        description="Threshold voor het bepalen of een vlak langs de rand van het mozaiek ligt",
     )
-    lok_vegtypen_col: Optional[str] = Field(
-        default=None,
-        description="kolomnaam van de lokale vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))",
+    niet_geautomatiseerde_sbb: List[str] = Field(
+        default=[
+            "100",
+            "200",
+            "300",
+            "400",
+        ],
+        description="SBB vegetatietypen die niet geautomatiseerd kunnen worden",
     )
 
 
 class Interface(metaclass=ABCMeta):
     """Singleton class that defines the interface for the different UI systems."""
 
     __instance = None
@@ -87,20 +124,25 @@
 
     @classmethod
     def get_instance(cls):
         if Interface.__instance is None:
             Interface.__instance = object.__new__(cls)
         return Interface.__instance
 
-    def shape_id_to_filename(self, shapefile_id: str) -> str:
+    def shape_id_to_filename(self, shapefile_id: str) -> Path:
         """Convert the shapefile id to a (temporary) file and returns the filename"""
-        return shapefile_id
+        return Path(shapefile_id)
 
     @abstractmethod
-    def output_shapefile(self, shapefile_id: str, gdf: gpd.GeoDataFrame) -> None:
+    def output_shapefile(
+        self, shapefile_id: Optional[Path], gdf: gpd.GeoDataFrame
+    ) -> None:
         """Output the shapefile with the given id.
         ID would either be a path to a shapefile or an identifier to a shapefile in ArcGIS or QGIS.
         """
 
     @abstractmethod
     def instantiate_loggers(self, log_level: int) -> None:
         """Instantiate the loggers for the module."""
+
+    def get_config(self) -> Veg2HabConfig:
+        return Veg2HabConfig()
```

### Comparing `veg2hab-0.2.1/veg2hab/main.py` & `veg2hab-0.2.2a0/veg2hab/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 from veg2hab.definitietabel import DefinitieTabel
 from veg2hab.fgr import FGR
 from veg2hab.io.common import AccessDBInputs, Interface, ShapefileInputs
 from veg2hab.vegkartering import Kartering
 from veg2hab.waswordtlijst import WasWordtLijst
 
 
-def installation_instructions():
+def installatie_instructies():
     print(
         dedent(
             f"""
-    To install the veg2hab toolbox, go to add Python toolbox in ArcGIS Pro and select the file at the following location:
+    Om veg2hab te kunnen draaien, moet de veg2hab toolbox geïnstalleerd worden in ArcGIS Pro.
+    Ga naar "add Python toolbox" in ArcGIS Pro en selecteer het bestand op de volgende locatie:
         {constants.TOOLBOX_PYT_PATH}
 """
         )
     )
 
 
 def run(params: Union[AccessDBInputs, ShapefileInputs]):
@@ -44,32 +45,33 @@
     if filename != params.shapefile:
         logging.info(
             f"Tijdelijke versie van {params.shapefile} is opgeslagen in {filename}"
         )
 
     if isinstance(params, AccessDBInputs):
         kartering = Kartering.from_access_db(
-            shape_path=Path(filename),
-            shape_elm_id_column=params.ElmID_col,
+            shape_path=filename,
+            shape_elm_id_column=params.elmid_col,
             access_mdb_path=params.access_mdb_path,
-            opmerkingen_column=params.opmerkingen_column,
-            datum_column=params.datum_column,
+            opmerkingen_column=params.opmerking_col,
+            datum_column=params.datum_col,
         )
     elif isinstance(params, ShapefileInputs):
         kartering = Kartering.from_shapefile(
-            shape_path=Path(filename),
-            ElmID_col=params.ElmID_col,
+            shape_path=filename,
+            ElmID_col=params.elmid_col,
             vegtype_col_format=params.vegtype_col_format,
             sbb_of_vvn=params.sbb_of_vvn,
             datum_col=params.datum_col,
             opmerking_col=params.opmerking_col,
-            SBB_col=params.SBB_col,
-            VvN_col=params.VvN_col,
+            SBB_col=params.sbb_col,
+            VvN_col=params.vvn_col,
             split_char=params.split_char,
             perc_col=params.perc_col,
+            lok_vegtypen_col=params.lok_vegtypen_col,
         )
     else:
         raise RuntimeError("Something went wrong with the input parameters")
 
     logging.info(f"Vegetatie kartering is succesvol ingelezen")
 
     kartering.apply_wwl(wwl)
@@ -82,10 +84,10 @@
 
     kartering.bepaal_habitatkeuzes(fgr)
 
     logging.info(f"Mitsen zijn gecheckt")
 
     final_format = kartering.as_final_format()
 
-    logging.info("Omzetting is successvol, wordt nu weggeschreven naar .gpkg")
+    logging.info("Omzetting is successvol, wordt nu weggeschreven naar een geopackage")
 
-    Interface.get_instance().output_shapefile("output_name", final_format)
+    Interface.get_instance().output_shapefile(params.output, final_format)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `veg2hab-0.2.1/veg2hab/mozaiek.py` & `veg2hab-0.2.2a0/veg2hab/mozaiek.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import json
 import warnings
 from collections import defaultdict
 from numbers import Number
 from typing import ClassVar, Dict, List, Optional, Tuple, Union
 
 import geopandas as gpd
-import pandas as pd
-from pydantic import BaseModel, PrivateAttr
+from pydantic import BaseModel, Field, PrivateAttr
 
 from veg2hab.enums import Kwaliteit, MaybeBoolean
+from veg2hab.io.common import Interface
 
 
 class MozaiekRegel(BaseModel):
     # NOTE: Mogelijk kunnen we in de toekomst van deze structuur af en met maar 1 type mozaiekregel werken
 
     type: ClassVar[Optional[str]] = None
     _subtypes_: ClassVar[dict] = dict()
-    mozaiek_threshold = 90
+    mozaiek_threshold: Union[int, float] = Field(
+        default_factory=lambda: Interface.get_instance().get_config().mozaiek_threshold
+    )
 
     def __init_subclass__(cls):
         # Vul de _subtypes_ dict met alle subclasses
         if cls.type is None:
             raise ValueError(
                 "You should specify the `type: ClassVar[str] = 'EnCritera'`"
             )
@@ -57,42 +59,29 @@
     def evaluation(self) -> MaybeBoolean:
         raise NotImplementedError()
 
     def __str__(self):
         raise NotImplementedError()
 
 
-class PlaceholderMozaiekregel(MozaiekRegel):
-    type: ClassVar[str] = "PlaceholderMozaiekregel"
+class NietGeimplementeerdeMozaiekregel(MozaiekRegel):
+    type: ClassVar[str] = "NietGeimplementeerdeMozaiekregel"
     _evaluation: Optional[MaybeBoolean] = PrivateAttr(default=None)
 
     def check(self, habtype_percentage_dict: Dict) -> None:
         self._evaluation = MaybeBoolean.CANNOT_BE_AUTOMATED
 
     @property
     def evaluation(self) -> MaybeBoolean:
         return self._evaluation
 
     def __str__(self):
         return "Placeholder mozaiekregel (nog niet geimplementeerd) (nooit waar)"
 
 
-# class DummyMozaiekregel(Mozaiekregel):
-#     # TODO: remove this once no longer needed
-#     type: ClassVar[str] = "DummyMozaiekregel"
-#     _evaluation: Optional[MaybeBoolean] = PrivateAttr(default=None)
-
-#     def check(self, habtype_percentage_dict: Dict) -> None:
-#         self._evaluation = MaybeBoolean.FALSE
-
-#     @property
-#     def evaluation(self) -> MaybeBoolean:
-#         return self._evaluation
-
-
 class GeenMozaiekregel(MozaiekRegel):
     type: ClassVar[str] = "GeenMozaiekregel"
     _evaluation: Optional[MaybeBoolean] = PrivateAttr(default=MaybeBoolean.TRUE)
 
     def check(self, habtype_percentage_dict: Dict) -> None:
         self._evaluation = MaybeBoolean.TRUE
 
@@ -136,24 +125,25 @@
 
             if not self.alleen_zelfstandig:
                 self.keys.append((self.habtype, False, Kwaliteit.MATIG))
 
     def check(self, habtype_percentage_dict: Dict) -> None:
         requested_habtype_percentage = 0
         for key in self.keys:
-            requested_habtype_percentage += habtype_percentage_dict[key]
+            requested_habtype_percentage += habtype_percentage_dict.get(key, 0)
 
         # Threshold is behaald, dus TRUE
         if requested_habtype_percentage >= self.mozaiek_threshold:
             self._evaluation = MaybeBoolean.TRUE
             return
 
-        unknown_habtype_percentage = habtype_percentage_dict[
-            ("HXXXX", True, Kwaliteit.NVT)
-        ]
+        unknown_habtype_percentage = habtype_percentage_dict.get(
+            ("HXXXX", True, Kwaliteit.NVT),
+            0,
+        )
         # Threshold kan nog behaald worden, dus POSTPONE
         if (
             requested_habtype_percentage + unknown_habtype_percentage
             >= self.mozaiek_threshold
         ):
             self._evaluation = MaybeBoolean.POSTPONE
             return
```

### Comparing `veg2hab-0.2.1/veg2hab/package_data/FGR.json` & `veg2hab-0.2.2a0/veg2hab/package_data/FGR.json`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.1/veg2hab/package_data/toolbox.pyt` & `veg2hab-0.2.2a0/veg2hab/package_data/veg2hab.pyt`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Type, Union
 
 import veg2hab.io.arcgis
 import veg2hab.main
 import veg2hab.constants
 import logging
 
-SUPPORTED_VERSIONS = ["0.1.0", "0.1.1", "0.2.1"]
+SUPPORTED_VERSIONS = ["0.1.0", "0.1.1", "0.2.1", "0.2.2a0"]
 
 # this instantiates the arcgis interface and configures the logging
 veg2hab.io.arcgis.ArcGISInterface.get_instance().instantiate_loggers()
 
 class Toolbox:
     def __init__(self):
         """Define the toolbox (the name of the toolbox is the name of the
@@ -42,37 +42,27 @@
         """Set whether the tool is licensed to execute."""
         return True
 
     def updateParameters(self, parameters):
         """Modify the values and properties of parameters before internal
         validation is performed.  This method is called whenever a parameter
         has been changed."""
-        # TODO: we could do some more validation here
-        # and or make some parameters dependent on others
-        # validate that the column exists
-        # if parameters[0].altered:
-        #     try:
-        #         layer = parameters[0].valueAsText
-        #         fields = [f.name for f in arcpy.ListFields(layer)]
-        #         parameters[1].filter.list = fields
-        #     except Exception as e:
-        #         # hmm, dit doet het nog niet helemaal..
-        #         logging.error(e)
+        return self.param_type.update_parameters(parameters)
 
     def updateMessages(self, parameters):
         """Modify the messages created by internal validation for each tool
         parameter. This method is called after internal validation."""
 
     def execute(self, parameters, messages):
         """The source code of the tool."""
         if veg2hab.__version__ not in SUPPORTED_VERSIONS:
             logging.warning(
                 "Deze versie van de toolbox is niet getest met deze versie van de software.\n"
                 "Gelieve de toolbox opnieuw toe te voegen aan ArcGIS, zie installatie instructies.\n"
-                f"De locatie van toolbox.pyt is: {veg2hab.constants.TOOLBOX_PYT_PATH}"
+                f"De locatie van veg2hab.pyt is: {veg2hab.constants.TOOLBOX_PYT_PATH}"
             )
 
         input_params = self.param_type.from_parameter_list(parameters)
         veg2hab.main.run(input_params)
 
     def postExecute(self, parameters):
         """This method takes place after outputs are processed and
```

### Comparing `veg2hab-0.2.1/veg2hab/validation.py` & `veg2hab-0.2.2a0/veg2hab/validation.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.1/veg2hab/vegetatietypen.py` & `veg2hab-0.2.2a0/veg2hab/vegetatietypen.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 from dataclasses import dataclass
 from typing import ClassVar, Optional, Union
 
 import pandas as pd
 
 from veg2hab.enums import MatchLevel
+from veg2hab.io.common import Interface
 
 
 @dataclass
 class SBB:
     """
     Format van SBB codes:
     ## is cijfer ('1', '5', '10', '32', zonder voorloopnul, dus geen '01' of '04')
@@ -34,16 +35,20 @@
     associatie: Optional[str] = None
     subassociatie: Optional[str] = None
     derivaatgemeenschap: Optional[str] = None
     rompgemeenschap: Optional[str] = None
 
     def __init__(self, code: str):
         assert isinstance(code, str), "Code is not a string"
-        if code in ["100", "200", "300", "400"]:
-            self.klasse = "niet habitattypewaardig"
+        # TODO: dit zou heel mooi naar een config kunnen later
+        niet_geautomatiseerde_sbb = (
+            Interface.get_instance().get_config().niet_geautomatiseerde_sbb
+        )
+        if code in niet_geautomatiseerde_sbb:
+            self.klasse = code
             return
 
         # Zet de gemeenschappen alvast op None zodat we ze kunnen overschrijven als het een gemeenschap is
         self.derivaatgemeenschap = None
         self.rompgemeenschap = None
 
         match = self.gemeenschap.search(code)
```

### Comparing `veg2hab-0.2.1/veg2hab/vegkartering.py` & `veg2hab-0.2.2a0/veg2hab/vegkartering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
-import warnings
 from collections import defaultdict
 from dataclasses import dataclass
 from numbers import Number
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import List, Optional, Tuple, Union
 
 import geopandas as gpd
 import pandas as pd
 from typing_extensions import Literal, Self
 
 from veg2hab.access_db import read_access_tables
 from veg2hab.criteria import FGRCriterium, is_criteria_type_present
@@ -108,39 +107,39 @@
 
     def __hash__(self):
         return hash((self.percentage, tuple(self.VvN), tuple(self.SBB)))
 
 
 def ingest_vegtype(
     gdf: gpd.GeoDataFrame,
-    sbb_cols: Optional[List[str]],
-    vvn_cols: Optional[List[str]],
+    sbb_cols: List[str],
+    vvn_cols: List[str],
     perc_cols: List[str],
 ) -> pd.Series:
     """
     Leest de vegetatietypen van een vlak in en maakt er een lijst van VegTypeInfo objecten van
     Vlakken zonder percentage
     """
     # Validatie
-    if sbb_cols is not None and len(sbb_cols) != len(perc_cols):
+    if len(sbb_cols) != 0 and len(sbb_cols) != len(perc_cols):
         raise ValueError(
             f"De lengte van sbb_cols ({len(sbb_cols)}) moet 0 zijn of gelijk zijn aan de lengte van perc_col ({len(perc_cols)})"
         )
 
-    if vvn_cols is not None and len(vvn_cols) != len(perc_cols):
+    if len(vvn_cols) != 0 and len(vvn_cols) != len(perc_cols):
         raise ValueError(
             f"De lengte van vvn_cols ({len(vvn_cols)}) moet 0 zijn of gelijk zijn aan de lengte van perc_col ({len(perc_cols)})"
         )
 
-    assert sbb_cols or vvn_cols, "Er moet een SBB of VvN kolom zijn"
+    assert len(sbb_cols) + len(vvn_cols) > 0, "Er moet een SBB of VvN kolom zijn"
 
     # Inlezen
-    if not sbb_cols:
+    if len(sbb_cols) == 0:
         sbb_cols = [None] * len(perc_cols)
-    if not vvn_cols:
+    if len(vvn_cols) == 0:
         vvn_cols = [None] * len(perc_cols)
 
     def _row_to_vegtypeinfo_list(row: gpd.GeoSeries) -> List[VegTypeInfo]:
         vegtype_list = []
         for sbb_col, vvn_col, perc_col in zip(sbb_cols, vvn_cols, perc_cols):
             # Als er geen percentage is, willen we ook geen VegTypeInfo,
             # dus slaan we deze over
@@ -248,35 +247,39 @@
     "70.00% goed zelfstandig H1234, 20.00% matig mozaiek H5678, 10.00% zelfstandig HXXXX"
 
     """
     # Als er nergens mozaiekregels zijn, is er ook geen dict
     if habtype_percentage_dict is None:
         return ""
 
+    assert all(
+        [v > 0 for v in habtype_percentage_dict.values()]
+    ), "Alle percentages moeten groter dan 0 zijn"
+
     return ", ".join(
         f"{v:.2f}% {'goed ' if k[2] == Kwaliteit.GOED else 'matig ' if k[2] == Kwaliteit.MATIG else ''}{'zelfstandig' if k[1] else 'mozaiek'} {k[0]}"
         for k, v in habtype_percentage_dict.items()
-        if v > 0
     )
 
 
 def hab_as_final_format(print_info: tuple, idx: int, opp: float) -> pd.Series:
     """ """
 
     keuze, vegtypeinfo = print_info
 
     # Er is 1 HabitatVoorstel
     if len(keuze.habitatvoorstellen) == 1:
         if keuze.status in [
             KeuzeStatus.DUIDELIJK,
             KeuzeStatus.VEGTYPEN_NIET_IN_DEFTABEL,
             KeuzeStatus.GEEN_KLOPPENDE_MITSEN,
-            KeuzeStatus.PLACEHOLDER,
+            KeuzeStatus.NIET_GEAUTOMATISEERD_CRITERIUM,
             KeuzeStatus.WACHTEN_OP_MOZAIEK,
             KeuzeStatus.GEEN_OPGEGEVEN_VEGTYPEN,
+            KeuzeStatus.NIET_GEAUTOMATISEERD_VEGTYPE,
         ]:
             voorstel = keuze.habitatvoorstellen[0]
             series_dict = {
                 f"Habtype{idx}": keuze.habtype,
                 f"Perc{idx}": vegtypeinfo.percentage,
                 f"Opp{idx}": opp * vegtypeinfo.percentage,
                 f"Kwal{idx}": keuze.kwaliteit.as_letter(),
@@ -295,15 +298,15 @@
                 f"SBB{idx}": (
                     str(voorstel.onderbouwend_vegtype)
                     if isinstance(voorstel.onderbouwend_vegtype, _SBB)
                     else None
                 ),
                 # f"VEGlok{idx}" TODO: Doen we voor nu nog even niet
                 f"_Status{idx}": str(keuze.status),
-                f"_Uitleg{idx}": keuze.status.toelichting(),
+                f"_Uitleg{idx}": keuze.status.toelichting,
                 f"_VvNdftbl{idx}": (
                     str(
                         [
                             str(voorstel.vegtype_in_dt),
                             voorstel.idx_in_dt,
                             voorstel.habtype,
                         ]
@@ -335,15 +338,15 @@
         assert (
             False
         ), f"Er is 1 habitatkeuze maar KeuzeStatus {keuze.status} is niet DUIDELIJK, VEGTYPEN_NIET_IN_DEFTABEL of GEEN_KLOPPENDE_MITSEN"
 
     if keuze.status in [
         KeuzeStatus.MEERDERE_KLOPPENDE_MITSEN,
         KeuzeStatus.GEEN_KLOPPENDE_MITSEN,
-        KeuzeStatus.PLACEHOLDER,
+        KeuzeStatus.NIET_GEAUTOMATISEERD_CRITERIUM,
         KeuzeStatus.WACHTEN_OP_MOZAIEK,
     ]:
         voorstellen = keuze.habitatvoorstellen
         # Als alle voorgestelde habtypen hetzelfde zijn kunnen we ze plat slaan
         # NOTE: Wordt keuzestatus dan ook weer duidelijk? Moet deze check dan al in habitatkeuze_obv_mitsen gedaan worden?
         voorgestelde_hab_en_kwal = [
             [voorstel.habtype, voorstel.kwaliteit] for voorstel in voorstellen
@@ -380,15 +383,15 @@
                         else None
                     )
                     for voorstel in voorstellen
                 ]
             ),
             # f"VEGlok{idx}" TODO: Doen we voor nu nog even niet
             f"_Status{idx}": str(keuze.status),
-            f"_Uitleg{idx}": keuze.status.toelichting(),
+            f"_Uitleg{idx}": keuze.status.toelichting,
             f"_VvNdftbl{idx}": str(
                 [
                     (
                         str(
                             [
                                 str(voorstel.vegtype_in_dt),
                                 voorstel.idx_in_dt,
@@ -499,24 +502,24 @@
     for i in range(1, n_habtype_blocks + 1):
         new_columns = new_columns + [
             f"Habtype{i}",
             f"Perc{i}",
             f"Opp{i}",
             f"Kwal{i}",
             f"Opm{i}",
-            f"VvN{i}",
             f"SBB{i}",
+            f"VvN{i}",
+            f"_VgTypInf{i}",
             f"_Status{i}",
             f"_Uitleg{i}",
-            f"_VgTypInf{i}",
+            f"_SBBdftbl{i}",
+            f"_VvNdftbl{i}",
             f"_Mits_opm{i}",
             f"_Mozk_opm{i}",
             f"_MozkPerc{i}",
-            f"_VvNdftbl{i}",
-            f"_SBBdftbl{i}",
         ]
     return gdf[new_columns]
 
 
 def fix_crs(
     gdf: gpd.GeoDataFrame, shape_path: Path = "onbekende locatie"
 ) -> gpd.GeoDataFrame:
@@ -552,15 +555,15 @@
 
 def _single_to_multi(
     gdf: gpd.GeoDataFrame,
     SBB_col: Optional[str] = None,
     VvN_col: Optional[str] = None,
     split_char: Optional[str] = None,
     perc_col: Optional[str] = None,
-) -> gpd.GeoDataFrame:
+) -> Tuple[gpd.GeoDataFrame, List[str], List[str], List[str]]:
     """
     Converteert een "single" kolomformat dataframe naar een "multi" kolomformat dataframe
     De nieuwe "multi" format kolommen heten SBB1/2/3/..., VvN1/2/3/... en perc1/2/3/...
     """
     # Uitvinden hoe veel kolommen er moeten komen
     assert SBB_col or VvN_col, "Er moet een SBB of VvN kolom zijn"
     if perc_col:
@@ -600,33 +603,39 @@
                     new_col_prefix=col,
                 )
             )
             gdf = gdf.join(new_columns)
 
     # Kolomnamen moeten geupdated worden.
     if SBB_col:
-        SBB_col = [f"{SBB_col}{idx+1}" for idx in range(n_cols_needed)]
+        SBB_out = [f"{SBB_col}{idx+1}" for idx in range(n_cols_needed)]
         # Stel dat er max 3 VvN zijn en max 2 SBB, dan moet de SBB3 nog wel bestaan
-        for col in SBB_col:
+        for col in SBB_out:
             if col not in gdf.columns:
                 gdf[col] = None
+    else:
+        SBB_out = []
 
     if VvN_col:
-        VvN_col = [f"{VvN_col}{idx+1}" for idx in range(n_cols_needed)]
-        for col in VvN_col:
+        VvN_out = [f"{VvN_col}{idx+1}" for idx in range(n_cols_needed)]
+        for col in VvN_out:
             if col not in gdf.columns:
                 gdf[col] = None
+    else:
+        VvN_out = []
 
     if perc_col:
-        perc_col = [f"{perc_col}{idx+1}" for idx in range(n_cols_needed)]
-        for col in perc_col:
+        perc_out = [f"{perc_col}{idx+1}" for idx in range(n_cols_needed)]
+        for col in perc_out:
             if col not in gdf.columns:
                 gdf[col] = None
+    else:
+        perc_out = []
 
-    return gdf, SBB_col, VvN_col, perc_col
+    return gdf, SBB_out, VvN_out, perc_out
 
 
 class Kartering:
     def __init__(self, gdf: gpd.GeoDataFrame):
         self.gdf = gdf
 
         # Alle VegTypeInfo sorteren op percentage van hoog naar laag
@@ -736,49 +745,93 @@
 
         return cls(gdf)
 
     @classmethod
     def from_shapefile(
         cls,
         shape_path: Path,
-        ElmID_col: str,
+        *,
         vegtype_col_format: Literal["single", "multi"],
         sbb_of_vvn: Literal["VvN", "SBB", "beide"],
+        ElmID_col: Optional[str] = None,
         datum_col: Optional[str] = None,
         opmerking_col: Optional[str] = None,
-        SBB_col: Optional[str] = None,
-        VvN_col: Optional[str] = None,
+        SBB_col: List[str],
+        VvN_col: List[str],
         split_char: Optional[str] = "+",
-        perc_col: Optional[str] = None,
-        lok_vegtypen_col: Optional[str] = None,
+        perc_col: List[str],
+        lok_vegtypen_col: List[str],
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
-        - VvN_col: kolomnaam van de VvN vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
-        - SBB_col: kolomnaam van de SBB vegetatietypen als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
+        - VvN_col: kolomnaam van de VvN vegetatietypen als deze er is (bij single_col mag deze list maximaal lengte 1 hebben)
+        - SBB_col: kolomnaam van de SBB vegetatietypen als deze er is (bij single_col mag deze list maximaal lengte 1 hebben)
         - split_char: karakter waarop de vegetatietypen gesplitst moeten worden (voor complexen (bv "16aa2+15aa")) (wordt bij mutli_col gebruikt om de kolommen te scheiden)
-        - perc_col: kolomnaam van de percentage als deze er is (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char))
-        - lok_vegtypen_col: kolomnaam van de lokale vegetatietypen als deze er zijn (bij multi_col: alle kolomnamen gesplitst door vegtype_split_char)
+        - perc_col: kolomnaam van de percentage als deze er is (bij single_col mag deze list maximaal lengte 1 hebben))
+        - lok_vegtypen_col: kolomnaam van de lokale vegetatietypen als deze er zijn (bij single_col mag deze list maximaal lengte 1 hebben)
         """
+        # CONTROLEREN VAN DE INPUT
+        if sbb_of_vvn == "VvN":
+            num_cols = len(VvN_col)
+            if len(VvN_col) == 0:
+                raise ValueError(
+                    "VvN_col moet worden opgegeven als sbb_of_vvn == 'VvN'"
+                )
+        elif sbb_of_vvn == "SBB":
+            num_cols = len(SBB_col)
+            if len(SBB_col) == 0:
+                raise ValueError(
+                    "SBB_col moet worden opgegeven als sbb_of_vvn == 'SBB'"
+                )
+        elif sbb_of_vvn == "beide":
+            num_cols = len(VvN_col)
+            if len(VvN_col) == 0 or len(SBB_col) == 0:
+                raise ValueError(
+                    "Zowel VvN_col als SBB_col moeten worden opgegeven als sbb_of_vvn == 'beide'"
+                )
+            if len(VvN_col) != len(SBB_col):
+                raise ValueError(
+                    "VvN_col en SBB_col moeten even lang zijn als sbb_of_vvn == 'beide'"
+                )
+        else:
+            raise ValueError("sbb_of_vvn moet ['VvN', 'SBB' of 'beide'] zijn")
 
-        ###############
-        ##### Valideren, opschonen en aanvullen van de shapefile
-        ###############
+        if vegtype_col_format == "single":
+            if num_cols != 1:
+                raise ValueError(
+                    "Aantal kolommen moet 1 zijn bij vegtype_col_format == 'single'"
+                )
+        elif vegtype_col_format == "multi":
+            if num_cols == 0:
+                raise ValueError(
+                    "Aantal kolommen moet groter dan 0 zijn bij vegtype_col_format == 'multi'"
+                )
+
+        if len(perc_col) != num_cols and len(perc_col) != 0:
+            raise ValueError(
+                "Aantal kolommen moet gelijk zijn tussen perc_col en SBB_col/VvN_col"
+            )
 
+        if len(lok_vegtypen_col) != num_cols and len(lok_vegtypen_col) != 0:
+            raise ValueError(
+                "Aantal kolommen moet gelijk zijn tussen perc_col en SBB_col/VvN_col"
+            )
+
+        # VALIDEREN, OPSCHONEN EN AANVULLEN VAN DE SHAPEFILE
         shapefile = gpd.read_file(shape_path)
 
         if ElmID_col and not shapefile[ElmID_col].is_unique:
-            warnings.warn(
+            logging.warn(
                 f"""De kolom {ElmID_col} bevat niet-unieke waarden in {shape_path}.
                 Eerste paar dubbele waarden:
                 {
                     shapefile[ElmID_col][shapefile[ElmID_col].duplicated()].head().to_list()
                 }
                 Er worden nieuwe waarden voor {ElmID_col} gemaakt en vanaf nu gebruikt.
                 """
@@ -791,94 +844,81 @@
             shapefile[ElmID_col] = range(len(shapefile))
 
         # Om niet bij splitten steeds "if split_char is not None:" te hoeven doen
         if split_char is None:
             split_char = "+"
 
         # Vastleggen lokale vegtypen voor in de output
-        if lok_vegtypen_col is not None:
+        if len(lok_vegtypen_col) > 0:
             shapefile["_LokVegTyp"] = shapefile.apply(
-                lambda row: ", ".join(
-                    [str(row[col]) for col in lok_vegtypen_col.split(split_char)]
-                ),
+                lambda row: ", ".join([str(row[col]) for col in lok_vegtypen_col]),
                 axis=1,
             )
         else:
             shapefile[
                 "_LokVegTyp"
             ] = "Geen kolommen opgegeven voor lokale vegetatietypen"
 
         # Selectie van de te bewaren kolommen
         cols = [
             col for col in [datum_col, opmerking_col] if col in shapefile.columns
         ] + [ElmID_col, "_LokVegTyp", "geometry"]
 
         # Uitvinden welke vegtype kolommen er mee moeten
-        if vegtype_col_format == "multi":
-            if SBB_col is not None:
-                SBB_col = SBB_col.split(split_char)
-                cols += SBB_col
-            if VvN_col is not None:
-                VvN_col = VvN_col.split(split_char)
-                cols += VvN_col
-            if perc_col is not None:
-                perc_col = perc_col.split(split_char)
-                cols += perc_col
-        else:
-            cols += [col for col in [VvN_col, SBB_col, perc_col] if col is not None]
+        cols += SBB_col + VvN_col + perc_col
         if not all(col in shapefile.columns for col in cols):
             raise ValueError(
                 f"Niet alle opgegeven kolommen ({cols}) gevonden in de shapefile kolommen ({shapefile.columns})"
             )
         gdf = shapefile[cols].copy()
 
         # Standardiseren van kolomnamen
+        # Als er geen datum of opmerking kolom is, dan maken we die en vullen we deze met None
+        if datum_col is None:
+            datum_col = "Datum"
+            gdf[datum_col] = None
+        if opmerking_col is None:
+            opmerking_col = "Opmerking"
+            gdf[opmerking_col] = None
+
         gdf = gdf.rename(
             columns={ElmID_col: "ElmID", opmerking_col: "Opmerking", datum_col: "Datum"}
         )
         ElmID_col = "ElmID"
         opmerking_col = "Opmerking"
         datum_col = "Datum"
 
         gdf = fix_crs(gdf, shape_path)
 
         if vegtype_col_format == "single":
             gdf, SBB_col, VvN_col, perc_col = _single_to_multi(
                 gdf=gdf,
-                SBB_col=SBB_col,
-                VvN_col=VvN_col,
+                SBB_col=None if len(SBB_col) == 0 else SBB_col[0],
+                VvN_col=None if len(VvN_col) == 0 else VvN_col[0],
                 split_char=split_char,
-                perc_col=perc_col,
+                perc_col=None if len(perc_col) == 0 else perc_col[0],
             )
             vegtype_col_format = "multi"
 
         # Opschonen
-        if SBB_col:
+        if len(SBB_col) > 0:
             gdf[SBB_col] = gdf[SBB_col].apply(_SBB.opschonen_series)
 
-        if VvN_col:
+        if len(VvN_col) > 0:
             gdf[VvN_col] = gdf[VvN_col].apply(_VvN.opschonen_series)
 
-        # Als er geen datum of opmerking kolom is, dan maken we die en vullen we deze met None
-        datum_col = "Datum" if datum_col is None else datum_col
-        opmerking_col = "Opmerking" if opmerking_col is None else opmerking_col
-        for col in [datum_col, opmerking_col]:
-            if col not in gdf.columns:
-                gdf[col] = None
-
         # Standardiseren van kolomnamen
-        gdf = gdf.rename(columns={datum_col: "Datum", opmerking_col: "Opmerking"})
         gdf["Opp"] = gdf["geometry"].area
         LokVrtNar_string = sbb_of_vvn if sbb_of_vvn != "beide" else "zowel SBB als VvN"
         gdf[
             "_LokVrtNar"
         ] = f"Lokale typologie is primair vertaald naar {LokVrtNar_string}"
 
         # Percentages invullen als die er niet zijn
-        if perc_col is None:
+        if len(perc_col) == 0:
             if vegtype_col_format == "multi":
                 perc_col = [
                     f"perc_{n}"
                     for n in range(
                         max([len(col) for col in [SBB_col, VvN_col] if col is not None])
                     )
                 ]
@@ -916,15 +956,15 @@
         # NOTE: Als dit te langzaam blijkt is een steekproef wss ook voldoende
         # NOTE NOTE: Als we zowel SBB en VvN uit de kartering hebben, willen we
         #            dan nog wwl doen voor de SBB zonder al meegegeven VvN?
         VvN_already_present = self.gdf["VegTypeInfo"].apply(
             lambda infos: any(len(info.VvN) > 0 for info in infos)
         )
         if VvN_already_present.any() and not override_existing_VvN:
-            warnings.warn(
+            logging.warn(
                 "Er zijn al VvN aanwezig in de kartering. De was-wordt lijst wordt niet toegepast."
             )
             return
 
         self.gdf["VegTypeInfo"] = self.gdf["VegTypeInfo"].apply(
             wwl.toevoegen_VvN_aan_List_VegTypeInfo
         )
@@ -1055,27 +1095,27 @@
 
             if (
                 n_keuzes_still_to_determine_pre == n_keuzes_still_to_determine_post
                 or n_keuzes_still_to_determine_post == 0
             ):
                 break
         else:
-            warnings.warn(
+            logging.warn(
                 f"Maximaal aantal iteraties ({max_iter}) bereikt voor het bepalen van de habitatkeuzes."
             )
 
         # Of we hebben overal een keuze, of we komen niet verder met nog meer iteraties,
         # of we hebben max_iter bereikt
 
         if n_keuzes_still_to_determine_post > 0:
             # NOTE
             # NOTE: @reviewer Moet dit een warning zijn vind je? Of gewoon een print?
             # NOTE: Het is iets wat niet alarmerend is maar wel nuttig om te weten.
             # NOTE
-            warnings.warn(
+            logging.warn(
                 f"Er zijn nog {n_keuzes_still_to_determine_post} habitatkeuzes die niet bepaald konden worden."
             )
 
         assert (
             self.gdf.HabitatKeuze.apply(lambda keuzes: keuzes.count(None)).sum() == 0
         ), "Er zijn nog habitatkeuzes die niet behandeld zijn en nog None zijn na bepaal_habitatkeuzes"
```

### Comparing `veg2hab-0.2.1/veg2hab/waswordtlijst.py` & `veg2hab-0.2.2a0/veg2hab/waswordtlijst.py`

 * *Files identical despite different names*

### Comparing `veg2hab-0.2.1/PKG-INFO` & `veg2hab-0.2.2a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: veg2hab
-Version: 0.2.1
+Version: 0.2.2a0
 Summary: Package voor automatisch omzetten van vegetatiekarteringen naar habitatkaarten
 License: LGPLv3
 Author: Spheer.ai
 Author-email: info@spheer.ai
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.7.1,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
 Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: geopandas (>=0.10.0)
-Requires-Dist: openpyxl (>=3.0.0)
-Requires-Dist: pydantic (>=1.0,<2.0)
+Requires-Dist: geopandas (>=0.10.0,<0.11.0)
+Requires-Dist: openpyxl (>=3.1.0,<4.0.0)
+Requires-Dist: pandas (>=1.3.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: pygeos (>=0.14,<0.15)
-Requires-Dist: pyodbc (>=4.0.1)
+Requires-Dist: pyodbc (>=4.0.1,<5.0.0)
 Requires-Dist: setuptools (<60.0.0)
 Requires-Dist: typing-extensions (==4.7.1)
-Requires-Dist: xlrd (>=2.0.1)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # veg2hab
 
 - [veg2hab](#veg2hab)
   - [Introductie](#introductie)
   - [Installatie instructies](#installatie-instructies)
@@ -51,35 +52,35 @@
 
 veg2hab wordt gedistribueerd via PyPI, waar alle toekomstige versies aan toe worden gevoegd.
 
 ## Installatie instructies
 
 ### Installatie binnen ArcGIS Pro
 
-Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger. 
-Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven: 
+Gebruik van veg2hab is ontwikkeld voor en getest in ArcGIS Pro versie 3.0 en hoger.
+Installatie vanaf PyPI is veruit het eenvoudigst, en wordt hieronder omschreven:
 
  1. Open ArcGIS Pro
- 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren): 
-    - Open de 'Package Manager'  
+ 2. Maak een nieuwe python environment aan voor veg2hab (de default conda environment is read-only en niet geschikt om veg2hab in te installeren):
+    - Open de 'Package Manager'
         <img src="./images/package_manager.png" alt="package manager" width="400"/>
-    - Klik op het tandwiel naast 'Active Environment'  
-    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.  
-        <img src="./images/new_environment.png" alt="new python environment" width="400"/>  
+    - Klik op het tandwiel naast 'Active Environment'
+    - Maak een nieuwe environment aan op een locatie naar keuze. Gebruik als 'Source' de default Environment.
+        <img src="./images/new_environment.png" alt="new python environment" width="400"/>
         <img src="./images/environment_location.png" alt="location of new environment" width="400"/>
     - Selecteer de environment en druk op 'OK'.
  3. Download en installeer veg2hab:
-    - Klik op 'New notebook'  
+    - Klik op 'New notebook'
         <img src="./images/new_notebook.png" alt="new notebook" width="400"/>
-    - Download veg2hab met het commando `!pip install --upgrade veg2hab`  
+    - Download veg2hab met het commando `!pip install --upgrade veg2hab`
         <img src="./images/notebook_prompts.png" alt="prompts in notebook to install veg2hab" width="400"/>
     - Installeer veg2hab met het commando `import veg2hab`
  4. Installeer de veg2hab Python Toolbox:
     - Gebruik het commando `veg2hab.installatie_instructies()` om de locatie van de toolbox te vinden
-    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie  
+    - Ga naar 'Add Toolbox (file)' en voeg de toolbox toe vanaf de locatie
         <img src="./images/add_toolbox.png" alt="adding the veg2hab Python Toolbox" width="400"/>
 
 Als het goed is, wordt de veg2hab toolbox nu getoond in de Geoprocessing tab:
 
 <img src="./images/geoprocessing_tab.png" alt="geoprocessing tab" width="400"/>
 
 
@@ -94,31 +95,31 @@
 
 ### Gebruik in ArcGIS Pro
 
 De omzetting van veg2hab van vegetatiekarteringen naar habitattypekaarten gebeurt in tools in de veg2hab Python Toolbox. Om de omzetting te doen, dient de gebruiker eerst de betreffende vegetatiekarteringen in te laden als kaart in ArcGIS Pro.
 
 De omzettool komt in twee smaken:
 1. `digitale_standaard`, voor het omzetten van vegetatiekarteringen die de landelijke digitale standaard gebruiken, die bestaat uit een shapefile gecombineerd met een access database. De gebruiker voert in welke vegetatiekarteringen omgezet moet worden en waar de bijhorende access database te vinden is.
-2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat. 
+2. `vector_bestand`, voor het omzetten van vegetatiekarteringen die alle benodigde informatie in de shapefile zelf bevatten. Omdat shapefiles geen standaard kolomnamen hebben, dient de gebruiker hier een handvol inputvelden in te vullen, bijvoorbeeld welke kolom de te gebruiken landelijke typologie bevat.
 
 Let op:
 - Wanneer de gebruiker beschikt over een access database, raden wij aan de  `digitale_standaard` omzetting te gebruiken, ook als de shapefile alle informatie bevat. Hierbij is de kans op handmatige fouten kleiner.
-- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN). 
+- Vegetatiekarteringen die omgezet worden met `vector_bestand` moeten beschikken over een landelijke typologie (SBB, VvN of rVvN).
 
 
 ### Bronbestanden die veg2hab gebruikt
 
-veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen. 
+veg2hab is afhankelijk van verschillende bronbestanden tijdens het omzetten van vegetatiekarteringen.
 
-Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker: 
+Sommige bestanden zijn landelijk beschikbaar. Deze bestanden worden automatisch mee geïnstalleerd met veg2hab en zijn niet aanpasbaar door de gebruiker:
 
  - [WasWordtLijst](./data/5.%20Was-wordt-lijst-vegetatietypen-en-habitattypen-09-02-2021.xlsx) (versie 09-feb-2021): dit bestand wordt gebruikt om landelijke vegetatietypologieën in elkaar om te zetten
  - [DefinitieTabel](./data/definitietabel%20habitattypen%20(versie%2024%20maart%202009)_0.xls) (versie 24 maart 2009): dit is een samenvatting van de profieldocumenten
  - [Fysisch-Geografische Regio kaart](./data/bronbestanden/FGR.json) (versie 2013, [link naar origineel op Nationaal georegister](https://nationaalgeoregister.nl/geonetwork/srv/dut/catalog.search#/metadata/c8b5668f-c354-42f3-aafc-d15ae54cf170))
-  
+
 Let op: bij volgende versies komen er waarschijnlijk meer bronbestanden bij.
 
 
 
 ## Handleiding voor ontwikkelaars
 ### Lokale ontwikkeling
 Download de git repository:
@@ -147,15 +148,15 @@
 poetry run pytest tests/
 ```
 
 ### Nieuwe release
 1. Zorg ervoor dat de laatste bronbestanden in package_data staan met `poetry run python release.py create-package-data`.
 2. Maak een nieuwe versie met poetry (major, minor, patch): `poetry version {{rule}}`
 3. Pas de [\_\_init\_\_.py](veg2hab/__init__.py) __version__ variabele aan zodat deze overeen komt met de nieuw poetry version
-4. Pas [toolbox.pyt](veg2hab/package_data/toolbox.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan toolbox.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
+4. Pas [veg2hab.pyt](veg2hab/package_data/veg2hab.pyt) zodat de nieuwe version in SUPPORTED_VERSIONS staat. Heb je aanpassingen gedaan aan veg2hab.pyt sinds de laatste release, zorg er dan voor dat de `SUPPORTED_VERSIONS = [{{new_version}}]` wordt gezet.
 5. Draai `python release.py check-versions` om te checken dat je geen fouten hebt gemaakt.
 6. Push nu eerst je nieuwe wijzigingen (mochten die er zijn), naar github. (`git add`, `git commit`, `git push`)
 7. Maak een nieuwe tag: `git tag v$(poetry version -s)`
 8. Push de tag naar git `git push origin tag v$(poetry version -s)`
 9. Github actions zal automatisch de nieuwe versie op PyPI zetten.
 
 
@@ -170,18 +171,18 @@
 
 **ElmID**: Een voor ieder vlak uniek ID. Deze kan vanuit de bronkartering komen, maar kan ook nieuw zijn gegenereerd. Dit gebeurt de als ElmID (of een ElmID equivalent zoals OBJECTID) in de bronkartering niet voor ieder vlak uniek is; als dit het geval is is hierover een warning gegeven.
 
 **_Samnvttng**: Weergave van hoeveel procent van het vlak bedekt is met welk habitattype. Dit is een combinatie van alle kolommen `Habtype{i}` en `Perc{i}`.
 
 **_LokVegTyp**: Het in de bronkartering opgegeven lokale vegetatietype, als er een lokaal vegetatietype kolom is opgegeven.
 
-**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan. 
+**_LokVrtNar**: Of de oorspronkelijk opgegeven lokale vegetatietypen in de bronkartering primair is vertaald naar SBB, VvN of beide. Als er naar SBB is vertaald, zijn er bijbehorende VvN uit de waswordtlijst gehaald. Als er naar VvN of naar beide is vertaald, is dit niet gedaan.
 
 ### Complex-deel-specifieke kolommen
-**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel. 
+**Habtype{i}**: Habitattype van het complex-deel. HXXXX hier betekend dat er menselijk oordeel nodig is over dit complex-deel.
 
 **Perc{i}**: Percentage van het gehele vlak wat door dit complex-deel wordt bedekt.
 
 **Opp{i}**: Oppervlakte van dit complex-deel in m2.
 
 **Kwal{i}**: Kwaliteit van dit complex-deel. Dit kan zijn G (goed), M (matig) of X (nvt).
```

