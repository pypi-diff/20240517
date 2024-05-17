# Comparing `tmp/trsolucoes-6.1.0.tar.gz` & `tmp/trsolucoes-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trsolucoes-6.1.0.tar", last modified: Fri May 17 13:19:05 2024, max compression
+gzip compressed data, was "trsolucoes-6.1.1.tar", last modified: Fri May 17 14:03:58 2024, max compression
```

## Comparing `trsolucoes-6.1.0.tar` & `trsolucoes-6.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 13:19:05.930697 trsolucoes-6.1.0/
--rw-rw-rw-   0        0        0     1088 2024-05-17 11:25:36.000000 trsolucoes-6.1.0/LICENCE
--rw-rw-rw-   0        0        0     2445 2024-05-17 13:19:05.929695 trsolucoes-6.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2119 2024-05-17 13:11:20.000000 trsolucoes-6.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 13:19:05.922697 trsolucoes-6.1.0/selenium_helper/
--rw-rw-rw-   0        0        0       43 2024-05-17 12:22:33.000000 trsolucoes-6.1.0/selenium_helper/__init__.py
--rw-rw-rw-   0        0        0    12864 2024-05-17 12:46:36.000000 trsolucoes-6.1.0/selenium_helper/selenium_helper.py
--rw-rw-rw-   0        0        0       42 2024-05-17 13:19:05.930697 trsolucoes-6.1.0/setup.cfg
--rw-rw-rw-   0        0        0      543 2024-05-17 13:16:07.000000 trsolucoes-6.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:19:05.928697 trsolucoes-6.1.0/trsolucoes.egg-info/
--rw-rw-rw-   0        0        0     2445 2024-05-17 13:19:05.000000 trsolucoes-6.1.0/trsolucoes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-17 13:19:05.000000 trsolucoes-6.1.0/trsolucoes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 13:19:05.000000 trsolucoes-6.1.0/trsolucoes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-17 13:19:05.000000 trsolucoes-6.1.0/trsolucoes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 14:03:58.641626 trsolucoes-6.1.1/
+-rw-rw-rw-   0        0        0     1088 2024-05-17 11:25:36.000000 trsolucoes-6.1.1/LICENCE
+-rw-rw-rw-   0        0        0     2550 2024-05-17 14:03:58.639625 trsolucoes-6.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2224 2024-05-17 14:01:24.000000 trsolucoes-6.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 14:03:58.625595 trsolucoes-6.1.1/selenium_helper/
+-rw-rw-rw-   0        0        0       43 2024-05-17 12:22:33.000000 trsolucoes-6.1.1/selenium_helper/__init__.py
+-rw-rw-rw-   0        0        0    12924 2024-05-17 14:02:29.000000 trsolucoes-6.1.1/selenium_helper/selenium_helper.py
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:03:58.641626 trsolucoes-6.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      543 2024-05-17 14:03:55.000000 trsolucoes-6.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:03:58.638625 trsolucoes-6.1.1/trsolucoes.egg-info/
+-rw-rw-rw-   0        0        0     2550 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-17 14:03:58.000000 trsolucoes-6.1.1/trsolucoes.egg-info/top_level.txt
```

### Comparing `trsolucoes-6.1.0/LICENCE` & `trsolucoes-6.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `trsolucoes-6.1.0/PKG-INFO` & `trsolucoes-6.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 6.1.0
+Version: 6.1.1
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
@@ -59,15 +59,16 @@
 sh.wait_and_click(driver, locator)
 ```
 
 ### `wait_and_select`
 Aguarda a presença de um elemento select e seleciona uma opção pelo texto visível.
 ```python
 locator = (By.TAG_NAME, 'select')
-sh.wait_and_select(driver, locator, 'Option Text')
+tag_filter = [('ng-reflect-name', 'labelOption'), ('ngcontent-c2', 'xp789e687')]
+sh.wait_and_select(driver, locator, 'Option Text', tag_filter=tag_filter)
 ```
 
 ### `wait_and_click_in_text`
 Aguarda um breve período e clica em um elemento cujo texto corresponde ao texto fornecido.
 ```python
 locator = (By.TAG_NAME, 'button')
 sh.wait_and_click_in_text(driver, locator, 'Button Text')
```

### Comparing `trsolucoes-6.1.0/README.md` & `trsolucoes-6.1.1/trsolucoes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: trsolucoes
+Version: 6.1.1
+Summary: Um repositório não oficial de funções de auxilio para Selenium
+Author: Tainan Ramos
+Author-email: tainan@trsolucoes.com.br
+License: MIT License
+Keywords: trsolucoes
+Requires: selenium
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # Selenium Helper
 
 Este pacote fornece um conjunto de utilitários para facilitar a interação com o Selenium WebDriver, incluindo funcionalidades para esperar por elementos, enviar texto, clicar em elementos, selecionar opções e mover o cursor sobre elementos.
 
 ## Instalação
 
 Você pode instalar o pacote diretamente do PyPI usando `pip`:
@@ -47,15 +59,16 @@
 sh.wait_and_click(driver, locator)
 ```
 
 ### `wait_and_select`
 Aguarda a presença de um elemento select e seleciona uma opção pelo texto visível.
 ```python
 locator = (By.TAG_NAME, 'select')
-sh.wait_and_select(driver, locator, 'Option Text')
+tag_filter = [('ng-reflect-name', 'labelOption'), ('ngcontent-c2', 'xp789e687')]
+sh.wait_and_select(driver, locator, 'Option Text', tag_filter=tag_filter)
 ```
 
 ### `wait_and_click_in_text`
 Aguarda um breve período e clica em um elemento cujo texto corresponde ao texto fornecido.
 ```python
 locator = (By.TAG_NAME, 'button')
 sh.wait_and_click_in_text(driver, locator, 'Button Text')
```

### Comparing `trsolucoes-6.1.0/selenium_helper/selenium_helper.py` & `trsolucoes-6.1.1/selenium_helper/selenium_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def wait_element(self, driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, return_element:bool = False, max_result:bool = False) -> bool | WebElement:
         """
         Aguarda a presença de um elemento na página, opcionalmente retornando o próprio elemento.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
-            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (tag_name, attribute). Default é None.
+            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após a busca pelo elemento. Default é 0.3 segundos.
             * return_element (bool, opcional): Se True, retorna o próprio elemento encontrado. Se False, retorna um booleano indicando se o elemento foi encontrado. Default é False.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
 
         Returns:
@@ -47,15 +47,15 @@
         """
         Aguarda a presença de um elemento na página e envia um texto para ele, com opções para limpar o campo e clicar no elemento antes de enviar o texto.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * text (str): Texto a ser enviado para o elemento.
-            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (tag_name, attribute). Default é None.
+            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após enviar o texto para o elemento. Default é 0.3 segundos.
             * clear_form (bool, opcional): Se True, limpa o campo de texto antes de enviar o novo texto. Default é True.
             * click_before (bool, opcional): Se True, clica no elemento antes de enviar o texto. Default é False.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
@@ -72,15 +72,15 @@
     def wait_and_click(self, driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
         """
         Aguarda a presença de um elemento na página e clica nele.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
-            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (tag_name, attribute). Default é None.
+            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após clicar no elemento. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
@@ -92,15 +92,15 @@
         """
         Aguarda a presença de um elemento na página e seleciona uma opção por texto visível em um elemento <select>.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
             * text (str): Texto visível da opção a ser selecionada no elemento <select>.
-            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (tag_name, attribute). Default é None.
+            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após selecionar a opção. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
@@ -131,15 +131,15 @@
     def wait_and_hover(self, driver: WebDriver, locator: tuple[By, str], tag_filter: list[tuple[str, str]] = None, timeout: int = 30, delay_before: float = 0.3, delay_after: float = 0.3, max_result: bool = False) -> None:
         """
         Aguarda a presença de um elemento na página e passa o cursor do mouse sobre ele.
 
         Args:
             * driver (WebDriver): Instância do WebDriver usada para interagir com o navegador.
             * locator (tuple[By, str]): Localizador do elemento na forma (By, value), onde By é a estratégia de localização e value é o seletor.
-            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (tag_name, attribute). Default é None.
+            * tag_filter (list[tuple[str, str]], opcional): Filtro de tags para refinar a busca do elemento. Cada filtro é uma tupla (attribute_name, attribute_value). Default é None.
             * timeout (int, opcional): Tempo máximo de espera pelo elemento em segundos. Default é 30 segundos.
             * delay_before (float, opcional): Tempo em segundos para esperar antes de iniciar a busca pelo elemento. Default é 0.3 segundos.
             * delay_after (float, opcional): Tempo em segundos para esperar após passar o cursor sobre o elemento. Default é 0.3 segundos.
             * max_result (bool, opcional): Se True, aplica o filtro tag_filter ao resultado para retornar o elemento mais relevante. Default é False.
         """
         sleep(delay_before)
         element: WebElement
```

### Comparing `trsolucoes-6.1.0/setup.py` & `trsolucoes-6.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="UTF-8") as arq:
     readme = arq.read()
 
 setup(name="trsolucoes",
-      version="6.1.0",
+      version="6.1.1",
       license="MIT License",
       author="Tainan Ramos",
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email="tainan@trsolucoes.com.br",
       keywords="trsolucoes",
       description="Um repositório não oficial de funções de auxilio para Selenium",
```

### Comparing `trsolucoes-6.1.0/trsolucoes.egg-info/PKG-INFO` & `trsolucoes-6.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: trsolucoes
-Version: 6.1.0
-Summary: Um repositório não oficial de funções de auxilio para Selenium
-Author: Tainan Ramos
-Author-email: tainan@trsolucoes.com.br
-License: MIT License
-Keywords: trsolucoes
-Requires: selenium
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # Selenium Helper
 
 Este pacote fornece um conjunto de utilitários para facilitar a interação com o Selenium WebDriver, incluindo funcionalidades para esperar por elementos, enviar texto, clicar em elementos, selecionar opções e mover o cursor sobre elementos.
 
 ## Instalação
 
 Você pode instalar o pacote diretamente do PyPI usando `pip`:
@@ -59,15 +47,16 @@
 sh.wait_and_click(driver, locator)
 ```
 
 ### `wait_and_select`
 Aguarda a presença de um elemento select e seleciona uma opção pelo texto visível.
 ```python
 locator = (By.TAG_NAME, 'select')
-sh.wait_and_select(driver, locator, 'Option Text')
+tag_filter = [('ng-reflect-name', 'labelOption'), ('ngcontent-c2', 'xp789e687')]
+sh.wait_and_select(driver, locator, 'Option Text', tag_filter=tag_filter)
 ```
 
 ### `wait_and_click_in_text`
 Aguarda um breve período e clica em um elemento cujo texto corresponde ao texto fornecido.
 ```python
 locator = (By.TAG_NAME, 'button')
 sh.wait_and_click_in_text(driver, locator, 'Button Text')
```

