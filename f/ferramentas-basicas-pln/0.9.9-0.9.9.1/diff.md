# Comparing `tmp/ferramentas-basicas-pln-0.9.9.tar.gz` & `tmp/ferramentas-basicas-pln-0.9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferramentas-basicas-pln-0.9.9.tar", last modified: Sun Mar 31 18:27:18 2024, max compression
+gzip compressed data, was "ferramentas-basicas-pln-0.9.9.1.tar", last modified: Thu Apr  4 00:38:05 2024, max compression
```

## Comparing `ferramentas-basicas-pln-0.9.9.tar` & `ferramentas-basicas-pln-0.9.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 18:27:18.478706 ferramentas-basicas-pln-0.9.9/
--rw-rw-rw-   0        0        0    13946 2024-03-31 18:27:18.477707 ferramentas-basicas-pln-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0    13600 2024-03-22 04:47:29.000000 ferramentas-basicas-pln-0.9.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 18:27:18.472701 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln/
--rw-rw-rw-   0        0        0     1052 2024-03-23 00:45:34.000000 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln/__init__.py
--rw-rw-rw-   0        0        0    43867 2024-03-31 18:26:13.000000 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln/main.py
-drwxrwxrwx   0        0        0        0 2024-03-31 18:27:18.476704 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln.egg-info/
--rw-rw-rw-   0        0        0    13946 2024-03-31 18:27:18.000000 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-03-31 18:27:18.000000 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 18:27:18.000000 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-31 18:27:18.000000 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-03-31 18:27:18.000000 ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 18:27:18.478706 ferramentas-basicas-pln-0.9.9/setup.cfg
--rw-rw-rw-   0        0        0      618 2024-03-31 18:26:53.000000 ferramentas-basicas-pln-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:38:05.859736 ferramentas-basicas-pln-0.9.9.1/
+-rw-rw-rw-   0        0        0    13948 2024-04-04 00:38:05.858734 ferramentas-basicas-pln-0.9.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0    13600 2024-04-04 00:37:59.000000 ferramentas-basicas-pln-0.9.9.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-04 00:38:05.853531 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/
+-rw-rw-rw-   0        0        0     1039 2024-04-04 00:37:19.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/__init__.py
+-rw-rw-rw-   0        0        0    43893 2024-04-04 00:34:47.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/main.py
+drwxrwxrwx   0        0        0        0 2024-04-04 00:38:05.857734 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/
+-rw-rw-rw-   0        0        0    13948 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-04 00:38:05.000000 ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 00:38:05.859736 ferramentas-basicas-pln-0.9.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-04-03 22:21:30.000000 ferramentas-basicas-pln-0.9.9.1/setup.py
```

### Comparing `ferramentas-basicas-pln-0.9.9/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9 Summary: Kit
-de ferramentas para processos bÃ¡sicos de Processamento de Linguagem Natural.
-Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.1 Summary:
+Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
+Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
     * _P_y_p_i_ _p_a_c_k_a_g_e_ _e_n_g_l_i_s_h_ _v_e_r_s_i_o_n
     * _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y_ _e_n_g_l_i_s_h_ _v_e_r_s_i_o_n
```

### Comparing `ferramentas-basicas-pln-0.9.9/README.md` & `ferramentas-basicas-pln-0.9.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln/__init__.py` & `ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 from .main import STRING_CARACTERES_ESPECIAIS_PADRAO,CARACTERES_NORMAIS
 from .main import LISTA_STOPWORDS_PADRAO_FREQUENCIA,LISTA_STOPWORDS_PADRAO_TOKENIZACAO,LISTA_PONTOS_FINAIS_PADRAO_FRASES,DICIONARIO_CONFIG_PADRAO_TOKENIZACAO
 from .main import DIGITO_DIA,DIGITO_MES,DIGITO_ANO,PADRAO_REGEX_DATA
 from .main import DDD_PAIS, DDD_ESTADO, DDD_CELULAR, PADRAO_REGEX_TELEFONE_CELULAR
 from .main import PADRAO_REGEX_EMAIL,PADRAO_REGEX_LINKS, PADRAO_REGEX_NUMEROS,PADRAO_REGEX_DINHEIRO,PADRAO_REGEX_CPF,PADRAO_REGEX_CEP,PADRAO_REGEX_RG
-from .main import padronizarRG,padronizarCPF,padronizarCEP,padronizarDatas,padronizarDinheiros,padronizarEmails,padronizarLinks,padronizarNumeros,padronizarParaFormaCanonica,padronizarTelefoneCelular,padronizarTextoParaMinuscula
-from .main import coletarTextoDeArquivoTxt,removerCaracteresEspeciais,removerCaracteresMaisQueEspeciais,removerEspacosEmBrancoExtras,transformarTextoSubstituindoCaracteres,verificarExistenciaDeElemento,contarFrequenciaDePalavras,formatarTexto, tokenizarTexto,organizaTextoPelasLinhas
+from .main import padronizarRG,padronizarCPF,padronizarCEP,padronizarDatas,padronizarDinheiros,padronizarEmails,padronizarLinks,padronizarNumeros,normalizarTexto,padronizarTelefoneCelular,padronizarTextoParaMinuscula
+from .main import coletarTextoDeArquivoTxt,removerCaracteresEspeciais,removerCaracteresMaisQueEspeciais,removerEspacosEmBrancoExtras,transformarTextoSubstituindoCaracteres,verificarExistenciaDeElemento,contarFrequenciaDePalavras,formatarTexto,tokenizarTexto,organizaTextoPelasLinhas
```

### Comparing `ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln/main.py` & `ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,16 @@
     ### Parâmetros:
     - :parâmetro texto: String contendo o texto que você quer limpar.
 
     ### Retornos:
     - :retorno: String limpa dos caracteres "mais que especiais" (emojis, dígitos estranhos, 
     formas que não se encontram no teclado, etc).
     """
-    for c in texto:
-        if c not in CARACTERES_NORMAIS:
-            texto = texto.replace(c,'')
+    for caracter_estranho in [c for c in texto if c not in CARACTERES_NORMAIS]:
+        texto = texto.replace(caracter_estranho,'')
     return texto
 
 def removerEspacosEmBrancoExtras(texto : str) -> str:
     """
     ### Objetivo
     Remover espaços em branco em excesso (dois ou mais em sequência) no texto fornecido como entrada.
 
@@ -286,14 +285,16 @@
         else:
             return False
     if encontrar_dinheiro:
         if re.search(PADRAO_REGEX_DINHEIRO,texto):
             return True
         else:
             return False
+         
+
 
 def padronizarRG(texto: str,
                  padrao_rg : str = 'RG') -> str:
     """
     ### Objetivo
     Função destinada à padronizar os elementos no texto que se caracterizem em RG do tipo "0.000.000"
     ### Parâmetros:
@@ -409,56 +410,42 @@
     - texto: String fornecida de entrada, para alterar os caracteres que contém o padrão de DINHEIRO.
     - padrao_dinheiro: String que ocupará o lugar dos caracteres referentes aos DINHEIROS, mascarando-os.
     ### Retornos:
     - return: String do texto modificado, caso encontre caracteres no padrão de dinheiro.
     """ 
     return re.sub(PADRAO_REGEX_DINHEIRO,padrao_dinheiro,texto)
 
-def padronizarParaFormaCanonica(texto : str) -> str:
+
+def normalizarTexto(texto : str) -> str:
     """
     ### Objetivo
     Função destinada à padronizar os elementos no texto que se caracterizem por possuir acentos, "ç", etc, passando-os para a forma mais "normal" destes.
     Exemplo: "ação" padronizado para a forma canonica ficaria "acao".
     ### Parâmetros:
     - texto: String fornecida de entrada, para alterar os caracteres que não estão na forma canônica.
     ### Retornos:
     - return: String do texto modificado, caso encontre caracteres que não estão na forma canônica.
     """
     return ''.join(c for c in (d for char in texto for d in unicodedata.normalize('NFD', char) if unicodedata.category(d) != 'Mn'))
 
+
 def padronizarTextoParaMinuscula(texto : str) -> str:
     """
     ### Objetivo
     Função destinada à padronizar os caracteres nos texto para minúscula.
     Exemplo: "PrograMaR" padronizado para minúsculas ficaria "programar".
     ### Parâmetros:
     - texto: String fornecida de entrada, para alterar os caracteres que não estão em minúscula.
     ### Retornos:
     - return: String do texto modificado, caso encontre caracteres que não estão em minúscula.
     """
     return texto.lower()
 
-def verificarFinalDeLinha(primeira_linha : str,
-                          segunda_linha : str,
-                          lista_de_pontos_finais : list = LISTA_PONTOS_FINAIS_PADRAO_FRASES) -> tuple[bool, str]:
-    primeira_linha = primeira_linha.strip()
-    segunda_linha = segunda_linha.strip()
-    for ptos_final in lista_de_pontos_finais:
-        if primeira_linha.strip().endswith(ptos_final):
-            if ptos_final == '.':
-                if not (verificaAbreviacao(primeira_linha[-4:]) and segunda_linha[0].islower()): # Terminação em abreviação de nome e próxima linha com caracter minúsculo (continuação de frase)
-                    return True, segunda_linha
-                else:
-                    return False, primeira_linha+' '+segunda_linha 
-            else:
-                return True, segunda_linha
-    if primeira_linha.endswith('-') and not (segunda_linha.startswith(' ')):
-        return False, primeira_linha+segunda_linha        
-    else:
-        return False, primeira_linha+' '+segunda_linha
+
+
 
 def contarFrequenciaDePalavras(texto : str | list,
                                palavras_especificas : list[str] | None = None,
                                n_top : int = -1,
                                remover_palavras_de_escape : bool = True,
                                lista_stopwords : list = LISTA_STOPWORDS_PADRAO_FREQUENCIA,
                                tratamento_padrao : bool = True) -> list:    
@@ -525,14 +512,16 @@
                   padronizar_emails : bool = False,
                   padrao_email : str = 'EMAIL',
                   padronizar_telefone_celular : bool = False,
                   padrao_tel : str = 'TEL',
                   padronizar_forma_canonica : bool = False) -> str:
     if remover_caracteres_mais_que_especiais:
         texto = removerCaracteresMaisQueEspeciais(texto)
+    if remover_espacos_em_branco_em_excesso:
+        texto = removerEspacosEmBrancoExtras(texto)
     if padronizar_dinheiros:
         for caracter_padrao_dinheiro in padrao_dinheiro:
             if caracter_padrao_dinheiro in string_caracteres_especiais:
                 caracteres_especiais_impacta_padrao_dinheiro = True
                 texto = padronizarDinheiros(texto=texto,padrao_dinheiro='codpdintzzqaio')
                 break
         else:
@@ -610,20 +599,19 @@
         else:
             caracteres_especiais_impacta_padrao_numero = False
             texto = padronizarNumeros(texto=texto,padrao_numeros=padrao_numero)
 
     if remover_caracteres_especiais:
         texto = removerCaracteresEspeciais(texto=texto,
                                            string_caracteres_especiais=string_caracteres_especiais)
-    if padronizar_forma_canonica:
-        texto = padronizarParaFormaCanonica(texto)
-    if remover_espacos_em_branco_em_excesso:
-        texto = removerEspacosEmBrancoExtras(texto)
+       
     if padronizar_texto_para_minuscula:
         texto = padronizarTextoParaMinuscula(texto)
+    if padronizar_forma_canonica:
+        texto = normalizarTexto(texto) 
     if padronizar_dinheiros and caracteres_especiais_impacta_padrao_dinheiro:
         texto = transformarTextoSubstituindoCaracteres(texto=texto,caracteres='codpdintzzqaio',substituir_por=padrao_dinheiro)
     if padronizar_links and caracteres_especiais_impacta_padrao_link:
         texto = transformarTextoSubstituindoCaracteres(texto=texto,caracteres='codpltzzqaio',substituir_por=padrao_link)
     if padronizar_numeros and caracteres_especiais_impacta_padrao_numero: 
         texto = transformarTextoSubstituindoCaracteres(texto=texto,caracteres='codpntzzqaio',substituir_por=padrao_numero)
     if padronizar_datas and caracteres_especiais_impacta_padrao_data:
@@ -639,14 +627,32 @@
     if padronizar_rg and caracteres_especiais_impacta_padrao_rg: 
         texto = transformarTextoSubstituindoCaracteres(texto=texto,caracteres='codprgtzzqaio',substituir_por=padrao_rg)
 
     return texto
 
 
 
+def verificarFinalDeLinha(primeira_linha : str,
+                          segunda_linha : str,
+                          lista_de_pontos_finais : list = LISTA_PONTOS_FINAIS_PADRAO_FRASES) -> tuple[bool, str]:
+    primeira_linha = primeira_linha.strip()
+    segunda_linha = segunda_linha.strip()
+    for ptos_final in lista_de_pontos_finais:
+        if primeira_linha.strip().endswith(ptos_final):
+            if ptos_final == '.':
+                if not (verificaAbreviacao(primeira_linha[-4:]) and segunda_linha[0].islower()): # Terminação em abreviação de nome e próxima linha com caracter minúsculo (continuação de frase)
+                    return True, segunda_linha
+                else:
+                    return False, primeira_linha+' '+segunda_linha 
+            else:
+                return True, segunda_linha
+    if primeira_linha.endswith('-') and not (segunda_linha.startswith(' ')):
+        return False, primeira_linha+segunda_linha        
+    else:
+        return False, primeira_linha+' '+segunda_linha
 
 
 def organizaTextoPelasLinhas(texto_completo : str) -> list:
     textos_separados_por_quebra_de_linha = texto_completo.split('\n')
     frases_completas_por_linha = []
     
     if textos_separados_por_quebra_de_linha:
@@ -794,15 +800,15 @@
                    remover_stopwords : bool = False,
                    lista_stopwords : list = LISTA_STOPWORDS_PADRAO_TOKENIZACAO,
                    desconsiderar_acentuacao_nas_stopwords : bool = False,
                    tratamento_padrao : bool = True,
                    config_tratamento_padrao : dict = DICIONARIO_CONFIG_PADRAO_TOKENIZACAO,
                    retorno_como_gerador : bool = False) -> list | Generator:
     if desconsiderar_acentuacao_nas_stopwords:
-        lista_stopwords = [padronizarParaFormaCanonica(elemento) for elemento in lista_stopwords]
+        lista_stopwords = [normalizarTexto(elemento) for elemento in lista_stopwords]
     if tratamento_padrao:
         try:
             if config_tratamento_padrao['removerCaracteresMaisQueEspeciais']:
                 texto = removerCaracteresMaisQueEspeciais(texto)
             if config_tratamento_padrao['removerCaracteresEspeciais'][0]:
                 # texto = removerCaracteresEspeciais(texto=texto,string_caracteres_especiais=config_tratamento_padrao['removerCaracteresEspeciais'][1])
                 remover_caracteres_especiais = True
```

### Comparing `ferramentas-basicas-pln-0.9.9/ferramentas_basicas_pln.egg-info/PKG-INFO` & `ferramentas-basicas-pln-0.9.9.1/ferramentas_basicas_pln.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferramentas-basicas-pln
-Version: 0.9.9
+Version: 0.9.9.1
 Summary: Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.
 Author: Igor Caetano de Souza
 Project-URL: GitHub Repository, https://github.com/IgorCaetano/ferramentas_basicas_pln
 Description-Content-Type: text/markdown
 Requires-Dist: regex
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9 Summary: Kit
-de ferramentas para processos bÃ¡sicos de Processamento de Linguagem Natural.
-Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
+Metadata-Version: 2.1 Name: ferramentas-basicas-pln Version: 0.9.9.1 Summary:
+Kit de ferramentas para processos bÃ¡sicos de Processamento de Linguagem
+Natural. Author: Igor Caetano de Souza Project-URL: GitHub Repository, https://
 github.com/IgorCaetano/ferramentas_basicas_pln Description-Content-Type: text/
 markdown Requires-Dist: regex # Ferramentas bÃ¡sicas para Processamento de
 Linguagem Natural Este pacote Ã© um kit de ferramentas (variadas funÃ§Ãµes)
 para execuÃ§Ã£o de processos bÃ¡sicos relacionados as etapas iniciais de
 processamento de linguagem natural. VVeerrss?Ã?£oo eemm iinnggll?Ã?ªss ((cclliiqquuee ppaarraa eexxppaannddiirr))
     * _P_y_p_i_ _p_a_c_k_a_g_e_ _e_n_g_l_i_s_h_ _v_e_r_s_i_o_n
     * _G_i_t_H_u_b_ _r_e_p_o_s_i_t_o_r_y_ _e_n_g_l_i_s_h_ _v_e_r_s_i_o_n
```

### Comparing `ferramentas-basicas-pln-0.9.9/setup.py` & `ferramentas-basicas-pln-0.9.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open(r'README.md','r',encoding='utf-8') as f:
     descricao_longa = f.read()
 
 setup(
     name='ferramentas-basicas-pln',
-    version='0.9.9',
+    version='0.9.9.1',
     packages=find_packages(),
     install_requires = ['regex'],
     description='Kit de ferramentas para processos básicos de Processamento de Linguagem Natural.',
     long_description=descricao_longa,
     long_description_content_type="text/markdown",
     author='Igor Caetano de Souza',
     project_urls={
```

