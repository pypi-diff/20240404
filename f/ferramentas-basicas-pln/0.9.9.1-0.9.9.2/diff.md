# Comparing `tmp/ferramentas-basicas-pln-0.9.9.1.tar.gz` & `tmp/ferramentas-basicas-pln-0.9.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferramentas-basicas-pln-0.9.9.1.tar", last modified: Thu Apr  4 00:38:05 2024, max compression
+gzip compressed data, was "ferramentas-basicas-pln-0.9.9.2.tar", last modified: Thu Apr  4 01:09:10 2024, max compression
```

## Comparing `ferramentas-basicas-pln-0.9.9.1.tar` & `ferramentas-basicas-pln-0.9.9.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 00:38:05.859736 ferramentas-basicas-pln-0.9.9.1/
--rw-rw-rw-   0        0        0    13948 2024-04-04 00:38:05.858734 ferramentas-basicas-pln-0.9.9.1/PKG-INFO
--rw-rw-rw-   0        0        0    13600 2024-04-04 00:37:59.000000 ferramentas-basicas-pln-0.9.9.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 00:38:05.853531 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/
--rw-rw-rw-   0        0        0     1039 2024-04-04 00:37:19.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/__init__.py
--rw-rw-rw-   0        0        0    43893 2024-04-04 00:34:47.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/main.py
-drwxrwxrwx   0        0        0        0 2024-04-04 00:38:05.857734 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/
--rw-rw-rw-   0        0        0    13948 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 00:38:05.859736 ferramentas-basicas-pln-0.9.9.1/setup.cfg
--rw-rw-rw-   0        0        0      620 2024-04-03 22:21:30.000000 ferramentas-basicas-pln-0.9.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:10.707299 ferramentas-basicas-pln-0.9.9.2/
+-rw-rw-rw-   0        0        0    13948 2024-04-04 01:09:10.706298 ferramentas-basicas-pln-0.9.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13600 2024-04-04 00:37:59.000000 ferramentas-basicas-pln-0.9.9.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:10.700269 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln/
+-rw-rw-rw-   0        0        0     1039 2024-04-04 00:37:19.000000 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln/__init__.py
+-rw-rw-rw-   0        0        0    43863 2024-04-04 01:08:45.000000 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln/main.py
+drwxrwxrwx   0        0        0        0 2024-04-04 01:09:10.705297 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln.egg-info/
+-rw-rw-rw-   0        0        0    13948 2024-04-04 01:09:10.000000 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-04 01:09:10.000000 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 01:09:10.000000 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 01:09:10.000000 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-04 01:09:10.000000 ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 01:09:10.707299 ferramentas-basicas-pln-0.9.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-04-04 01:08:59.000000 ferramentas-basicas-pln-0.9.9.2/setup.py
```

### Comparing `ferramentas-basicas-pln-0.9.9.1/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9.1
+Version: 0.9.9.2
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.1 Summary:
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.2 Summary:
 Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
 Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
```

### Comparing `ferramentas-basicas-pln-0.9.9.1/README.md` & `ferramentas-basicas-pln-0.9.9.2/README.md`

 * *Files identical despite different names*

### Comparing `ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/__init__.py` & `ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln/__init__.py`

 * *Files identical despite different names*

### Comparing `ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/main.py` & `ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
                   padrao_dinheiro : str = '$',
                   padronizar_datas : bool = False,
                   padrao_data : str = 'DATA',
                   padronizar_emails : bool = False,
                   padrao_email : str = 'EMAIL',
                   padronizar_telefone_celular : bool = False,
                   padrao_tel : str = 'TEL',
-                  padronizar_forma_canonica : bool = False) -> str:
+                  normalizar : bool = False) -> str:
     if remover_caracteres_mais_que_especiais:
         texto = removerCaracteresMaisQueEspeciais(texto)
     if remover_espacos_em_branco_em_excesso:
         texto = removerEspacosEmBrancoExtras(texto)
     if padronizar_dinheiros:
         for caracter_padrao_dinheiro in padrao_dinheiro:
             if caracter_padrao_dinheiro in string_caracteres_especiais:
@@ -602,15 +602,15 @@
 
     if remover_caracteres_especiais:
         texto = removerCaracteresEspeciais(texto=texto,
                                            string_caracteres_especiais=string_caracteres_especiais)
        
     if padronizar_texto_para_minuscula:
         texto = padronizarTextoParaMinuscula(texto)
-    if padronizar_forma_canonica:
+    if normalizar:
         texto = normalizarTexto(texto) 
     if padronizar_dinheiros and caracteres_especiais_impacta_padrao_dinheiro:
         texto = transformarTextoSubstituindoCaracteres(texto=texto,caracteres='codpdintzzqaio',substituir_por=padrao_dinheiro)
     if padronizar_links and caracteres_especiais_impacta_padrao_link:
         texto = transformarTextoSubstituindoCaracteres(texto=texto,caracteres='codpltzzqaio',substituir_por=padrao_link)
     if padronizar_numeros and caracteres_especiais_impacta_padrao_numero: 
         texto = transformarTextoSubstituindoCaracteres(texto=texto,caracteres='codpntzzqaio',substituir_por=padrao_numero)
```

### Comparing `ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.2/ferramentas_basicas_pln.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9.1
+Version: 0.9.9.2
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.1 Summary:
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.2 Summary:
 Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
 Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
```

### Comparing `ferramentas-basicas-pln-0.9.9.1/setup.py` & `ferramentas-basicas-pln-0.9.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open(r'README.md','r',encoding='utf-8') as f:
     descricao_longa = f.read()
 
 setup(
     name='ferramentas-basicas-pln',
-    version='0.9.9.1',
+    version='0.9.9.2',
     packages=find_packages(),
     install_requires = ['regex'],
     description='Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.',
     long_description=descricao_longa,
     long_description_content_type="text/markdown",
     author='Igor Caetano de Souza',
     project_urls={
```

