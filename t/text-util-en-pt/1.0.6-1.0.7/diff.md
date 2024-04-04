# Comparing `tmp/text_util_en_pt-1.0.6.tar.gz` & `tmp/text_util_en_pt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text_util_en_pt-1.0.6.tar", last modified: Thu Apr  4 13:10:28 2024, max compression
+gzip compressed data, was "text_util_en_pt-1.0.7.tar", last modified: Thu Apr  4 13:23:35 2024, max compression
```

## Comparing `text_util_en_pt-1.0.6.tar` & `text_util_en_pt-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/
--rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-08 21:33:02.000000 text_util_en_pt-1.0.6/LICENSE
--rw-r--r--   0 moro      (1000) moro      (1000)      550 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/PKG-INFO
--rwxrwxrwx   0 moro      (1000) moro      (1000)      640 2024-04-04 13:07:07.000000 text_util_en_pt-1.0.6/pyproject.toml
--rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/setup.cfg
--rw-r--r--   0 moro      (1000) moro      (1000)      757 2024-04-04 13:07:07.000000 text_util_en_pt-1.0.6/setup.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/text_util_en_pt/
--rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-08 21:59:15.000000 text_util_en_pt-1.0.6/text_util_en_pt/__init__.py
--rw-r--r--   0 moro      (1000) moro      (1000)    22957 2024-04-04 13:06:45.000000 text_util_en_pt-1.0.6/text_util_en_pt/cleaner.py
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/text_util_en_pt/resources/
--rw-r--r--   0 moro      (1000) moro      (1000)   263066 2024-02-08 21:31:18.000000 text_util_en_pt-1.0.6/text_util_en_pt/resources/english_nltk_tokenizer.pkl
--rw-r--r--   0 moro      (1000) moro      (1000)   400695 2024-02-08 21:31:18.000000 text_util_en_pt-1.0.6/text_util_en_pt/resources/portuguese_nltk_tokenizer.pkl
-drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:10:28.182783 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/
--rw-r--r--   0 moro      (1000) moro      (1000)      550 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/PKG-INFO
--rw-r--r--   0 moro      (1000) moro      (1000)      389 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/SOURCES.txt
--rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/dependency_links.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       26 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/requires.txt
--rw-r--r--   0 moro      (1000) moro      (1000)       16 2024-04-04 13:10:28.000000 text_util_en_pt-1.0.6/text_util_en_pt.egg-info/top_level.txt
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:23:35.712631 text_util_en_pt-1.0.7/
+-rwxrwxrwx   0 moro      (1000) moro      (1000)     1067 2024-02-08 21:33:02.000000 text_util_en_pt-1.0.7/LICENSE
+-rw-r--r--   0 moro      (1000) moro      (1000)      576 2024-04-04 13:23:35.712631 text_util_en_pt-1.0.7/PKG-INFO
+-rwxrwxrwx   0 moro      (1000) moro      (1000)      619 2024-04-04 13:22:54.000000 text_util_en_pt-1.0.7/pyproject.toml
+-rw-r--r--   0 moro      (1000) moro      (1000)       38 2024-04-04 13:23:35.712631 text_util_en_pt-1.0.7/setup.cfg
+-rw-r--r--   0 moro      (1000) moro      (1000)      586 2024-04-04 13:22:49.000000 text_util_en_pt-1.0.7/setup.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:23:35.712631 text_util_en_pt-1.0.7/text_util_en_pt/
+-rw-r--r--   0 moro      (1000) moro      (1000)        0 2024-02-08 21:59:15.000000 text_util_en_pt-1.0.7/text_util_en_pt/__init__.py
+-rw-r--r--   0 moro      (1000) moro      (1000)    22370 2024-04-04 13:20:12.000000 text_util_en_pt-1.0.7/text_util_en_pt/cleaner.py
+drwxr-xr-x   0 moro      (1000) moro      (1000)        0 2024-04-04 13:23:35.712631 text_util_en_pt-1.0.7/text_util_en_pt.egg-info/
+-rw-r--r--   0 moro      (1000) moro      (1000)      576 2024-04-04 13:23:35.000000 text_util_en_pt-1.0.7/text_util_en_pt.egg-info/PKG-INFO
+-rw-r--r--   0 moro      (1000) moro      (1000)      280 2024-04-04 13:23:35.000000 text_util_en_pt-1.0.7/text_util_en_pt.egg-info/SOURCES.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)        1 2024-04-04 13:23:35.000000 text_util_en_pt-1.0.7/text_util_en_pt.egg-info/dependency_links.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       11 2024-04-04 13:23:35.000000 text_util_en_pt-1.0.7/text_util_en_pt.egg-info/requires.txt
+-rw-r--r--   0 moro      (1000) moro      (1000)       16 2024-04-04 13:23:35.000000 text_util_en_pt-1.0.7/text_util_en_pt.egg-info/top_level.txt
```

### Comparing `text_util_en_pt-1.0.6/LICENSE` & `text_util_en_pt-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `text_util_en_pt-1.0.6/PKG-INFO` & `text_util_en_pt-1.0.7/text_util_en_pt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
-Name: text_util_en_pt
-Version: 1.0.6
+Name: text-util-en-pt
+Version: 1.0.7
 Summary: Python project for text cleaning. Some specifics for English and Portuguese languages.
 Author: Carlo Moro
 Author-email: Carlo Moro <cnmoro@gmail.com>
 Project-URL: Homepage, https://github.com/cnmoro
 Project-URL: Bug Tracker, https://github.com/cnmoro
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: langdetect
```

### Comparing `text_util_en_pt-1.0.6/pyproject.toml` & `text_util_en_pt-1.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "langdetect", "nltk", "langchain"]
+requires = ["setuptools>=61.0", "langdetect"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text_util_en_pt"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Carlo Moro", email="cnmoro@gmail.com" },
 ]
 description = "Python project for text cleaning. Some specifics for English and Portuguese languages."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `text_util_en_pt-1.0.6/text_util_en_pt/cleaner.py` & `text_util_en_pt-1.0.7/text_util_en_pt/cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from enum import Enum
-import re, copy, pickle
+import re, copy
 from langdetect import detect_langs
-import pkg_resources
 
 punctuations = re.escape('!"#%\'()*+,./:;<=>?@[\\]^_`{|}~')
 re_remove_brackets = re.compile(r'\{.*\}')
 re_remove_html = re.compile(r'<(\/|\\)?.+?>', re.UNICODE)
 re_transform_numbers = re.compile(r'\d', re.UNICODE)
 re_transform_emails = re.compile(r'[^\s]+@[^\s]+', re.UNICODE)
 re_transform_url = re.compile(r'(http|https)://[^\s]+', re.UNICODE)
@@ -20,16 +19,14 @@
 re_punkts_b = re.compile(r'([ %s])([%s])(\w+)' % (punctuations, punctuations), re.UNICODE)
 re_punkts_c = re.compile(r'(\w+)([%s])$' % (punctuations), re.UNICODE)
 re_changehyphen = re.compile(u'–')
 re_doublequotes_1 = re.compile(r'(\"\")')
 re_doublequotes_2 = re.compile(r'(\'\')')
 re_trim = re.compile(r' +', re.UNICODE)
 
-tokenizer_ptbr = pickle.load(open(pkg_resources.resource_filename('text_util_en_pt', 'resources/portuguese_nltk_tokenizer.pkl'), 'rb'))
-tokenizer_enus = pickle.load(open(pkg_resources.resource_filename('text_util_en_pt', 'resources/english_nltk_tokenizer.pkl'), 'rb'))
 stopwords_ptbr = list(set(['clt1148028', 'bmetrack', 'nan','coluna', 'tentar', 'iniciar', 'ono', 'pronto', 'id', 'rá', 'ré', 'it', 'az', 'primeiro', 'segundo', 'terceiro', 'quarto', 'quinto', 'sexto', 'sétimo', 'oitavo', 'nono', 'décimo', 'senhor', 'senhora', 'falsar', 'clique', 'sebraepr', 'jan', 'fev', 'mar', 'abr', 'mai', 'jun', 'jul', 'ago', 'set', 'out', 'nov', 'dez', 'jananeiro', 'fevereiro', 'março', 'abril', 'maio', 'junho', 'julho', 'agosto', 'setembro', 'outubro', 'novembro', 'dezembro', 'ltda', 'sebrae', 'neste', 'novos', 'per', 'bastante', 'bem', 'devendo', 'houvermos', 'talvez', 'houvéssemos', 'certamente', 'entre', 'lhes', 'estiveste', 'amplas', 'grandes', 'estejamos', 'umas', 'ali', 'sem', 'tivéssemos', 'podiam', 'faz', 'desse', 'tivera', 'nenhum', 'todos', 'obrigada', 'outro', 'tiveram', 'dizer', 'questão', 'boas', 'não', 'perto', 'serão', 'feitas', 'pelas', 'mal', 'ainda', 'és', 'só', 'deveria', 'cá', 'ampla', 'nove', 'disso', 'tivéramos', 'enquanto', 'houveram', 'aquele', 'minha', 'apoio', 'mim', 'forem', 'às', 'meio', 'tinha', 'estes', 'catorze', 'primeira', 'fazemos', 'vais', 'segunda', 'teria', 'devia', 'vão', 'geral', 'dele', 'seria', 'estivessem', 'dez', 'poucos', 'hajam', 'tão', 'nunca', 'deverá', 'noite', 'na', 'estadoadeus', 'momento', 'um', 'sexta', 'máximo', 'relação', 'nesta', 'logo', 'é', 'houveríamos', 'dia', 'estivesse', 'tal', 'quarta', 'lá', 'meses', 'quatro', 'dos', 'mas', 'oito', 'fora', 'sei', 'tivessem', 'porém', 'muitas', 'hajamos', 'quinta', 'poderiam', 'estavam', 'nome', 'trabalho', 'naquele', 'porque', 'tu', 'estivéramos', 'houveria', 'todavia', 'tivermos', 'pequenos', 'fomos', 'sobre', 'poucas', 'nossas', 'hoje', 'mesmas', 'perante', 'houvera', 'são', 'mês', 'daquela', 'hora', 'aquelas', 'próximo', 'nossos', 'num', 'naquelas', 'vários', 'pude', 'uns', 'área', 'mesmos', 'ter', 'sendo', 'obrigado', 'nos', 'estive', 'foram', 'desses', 'esse', 'deste', 'treze', 'terão', 'próximas', 'antes', 'seríamos', 'contra', 'nestes', 'ponto', 'ele', 'lado', 'em', 'tivemos', 'naquela', 'cinco', 'terceira', 'cento', 'dar', 'hão', 'dessa', 'zero', 'dizem', 'vosso', 'dito', 'estão', 'nesses', 'dever', 'final', 'mais', 'até', 'mil', 'quê', 'vossos', 'coisas', 'desta', 'conselho', 'fui', 'fazeis', 'posição', 'tens', 'brasil', 'próximos', 'maior', 'com', 'nova', 'certeza', 'ou', 'tampouco', 'quando', 'vem', 'sétimo', 'cima', 'seremos', 'nenhuma', 'fostes', 'nessas', 'algum', 'sistema', 'https', 'feitos', 'nós', 'deviam', 'si', 'vens', 'nem', 'essas', 'querem', 'tua', 'viagem', 'seis', 'foste', 'assim', 'à', 'nessa', 'te', 'podendo', 'depois', 'pequeno', 'tido', 'naqueles', 'pelo', 'local', 'tenham', 'www', 'quer', 'queres', 'nível', 'tenha', 'aí', 'tiverem', 'feita', 'primeiras', 'todas', 'última', 'meus', 'poder', 'aquela', 'falta', 'fôramos', 'teus', 'dezesseis', 'estás', 'tantas', 'alguém', 'disto', 'novas', 'novo', 'quem', 'teriam', 'estar', 'eram', 'teve', 'este', 'possivelmente', 'próprias', 'algumas', 'tenho', 'vossa', 'estou', 'houverão', 'suas', 'fazem', 'lo', 'esses', 'para', 'menos', 'há', 'tendes', 'dúvida', 'nada', 'deles', 'tive', 'vós', 'muito', 'temos', 'último', 'sua', 'seu', 'embora', 'grande', 'três', 'isto', 'pelos', 'foi', 'paucas', 'se', 'tivesse', 'houvéramos', 'eles', 'esteja', 'breve', 'pouca', 'quanto', 'serei', 'ah', 'fez', 'primeiro', 'demais', 'deveriam', 'deverão', 'custa', 'destas', 'quereis', 'sejamos', 'aquilo', 'ao', 'quais', 'houve', 'nosso', 'deve', 'sete', 'tendo', 'últimas', 'posso', 'quinto', 'pequenas', 'os', 'menor', 'sexto', 'têm', 'teríamos', 'uma', 'põem', 'estivermos', 'estivera', 'http', 'ontem', 'sabem', 'oitavo', 'esta', 'aos', 'podia', 'ela', 'tiver', 'daquele', 'daqueles', 'da', 'duas', 'nestas', 'teremos', 'ver', 'podem', 'a', 'oitava', 'onze', 'nas', 'mesma', 'parte', 'la', 'outros', 'pouco', 'houverem', 'haja', 'vos', 'pequena', 'desde', 'tarde', 'diante', 'outras', 'dela', 'boa', 'maioria', 'partir', 'elas', 'vêm', 'põe', 'dentro', 'fossem', 'toda', 'forma', 'algo', 'fazendo', 'quero', 'própria', 'outra', 'éramos', 'seriam', 'favor', 'tiveste', 'tivestes', 'houvessem', 'fazes', 'ai', 'houvesse', 'ti', 'isso', 'tenhamos', 'nesse', 'tanto', 'estamos', 'longe', 'fôssemos', 'está', 'pontos', 'muitos', 'devem', 'número', 'próprio', 'parece', 'o', 'segundo', 'ano', 'dezessete', 'seja', 'vendo', 'atrás', 'meu', 'alguns', 'teu', 'no', 'feito', 'do', 'agora', 'dezoito', 'me', 'era', 'as', 'sois', 'tanta', 'debaixo', 'pela', 'também', 'estávamos', 'sejam', 'sido', 'através', 'grupo', 'quantos', 'estiver', 'já', 'estiveram', 'quarto', 'disse', 'somos', 'sou', 'queremos', 'dão', 'estivestes', 'estas', 'tuas', 'esteve', 'terei', 'cada', 'todo', 'doze', 'houver', 'tinham', 'alguma', 'dessas', 'ó', 'estivemos', 'tudo', 'tem', 'for', 'vir', 'houveriam', 'lugar', 'aqui', 'houverei', 'coisa', 'das', 'estava', 'sempre', 'estiverem', 'vez', 'essa', 'houverá', 'fim', 'puderam', 'vai', 'nossa', 'será', 'como', 'porquê', 'vezes', 'vinte', 'ninguém', 'poderia', 'exemplo', 'cedo', 'eu', 'qual', 'diz', 'sétima', 'estejam', 'após', 'fazer', 'próxima', 'sob', 'pois', 'houveremos', 'minhas', 'amplo', 'possível', 'delas', 'terá', 'havemos', 'tínhamos', 'daquelas', 'bons', 'sim', 'fosse', 'hei', 'destes', 'numa', 'dá', 'houvemos', 'aqueles', 'por', 'primeiros', 'além', 'lhe', 'dezenove', 'horas', 'próprios', 'baixo', 'seus', 'vocês', 'últimos', 'ser', 'faço', 'que', 'havia', 'quinze', 'e', 'amplos', 'de', 'onde', 'obra', 'pode', 'bom', 'apenas', 'muita', 'mesmo', 'contudo', 'anos', 'vossas', 'sabe', 'vindo', 'você', 'pôde', 'dois', 'tém', 'formos', 'ante', 'estivéssemos', 'ano', 'área', 'baixo', 'dar', 'dia', 'grupo', 'local', 'maior', 'máximo', 'noite', 'número', 'obra', 'questão', 'relação', 'viagem', 'capitar', 'industriar' , 'includeeditpanificar', 'caminho', 'estado', 'tempo', 'tipo', 'valor', 'verdade', 'x', 'h', 'www', 'inc', 'http', 'https', 'apontar', 'inciar', 'ligado', 'saber', 'trabalhar', 'usar']))
 stopwords_enus = list(set(["trademark","nan", "i", "me", "my", "myself", "we", "our", "ours", "ourselves", "you", "your", "yours", "yourself", "yourselves", "he", "him", "his", "himself", "she", "her", "hers", "herself", "it", "its", "itself", "they", "them", "their", "theirs", "themselves", "what", "which", "who", "whom", "this", "that", "these", "those", "am", "is", "are", "was", "were", "be", "been", "being", "have", "has", "had", "having", "do", "does", "did", "doing", "a", "an", "the", "and", "but", "if", "or", "because", "as", "until", "while", "of", "at", "by", "for", "with", "about", "against", "between", "into", "through", "during", "before", "after", "above", "below", "to", "from", "up", "down", "in", "out", "on", "off", "over", "under", "again", "further", "then", "once", "here", "there", "when", "where", "why", "how", "all", "any", "both", "each", "few", "more", "most", "other", "some", "such", "no", "nor", "not", "only", "own", "same", "so", "than", "too", "very", "s", "t", "can", "will", "just", "don", "should", "now", "aren't", "can't", "cannot", "could", "couldn't", "didn't", "doesn't", "don't", "hadn't", "hasn't", "haven't", "he'd", "he'll", "he's", "here's", "how's", "i'd", "i'll", "i'm", "i've", "isn't", "it's", "let's", "mustn't", "ought", "shan't", "she'd", "she'll", "she's", "shouldn't", "that's", "there's", "they'd", "they'll", "they're", "they've", "wasn't", "we'd", "we'll", "we're", "we've", "weren't", "what's", "when's", "where's", "who's", "why's", "won't", "would", "wouldn't", "you'd", "you'll", "you're", "you've"]))
 
 class Language(Enum):
     ptbr = 'ptbr'
     enus = 'enus'
 
@@ -146,17 +143,14 @@
 
 def replace_escaped_unicode(input_string):
     def decode_match(match):
         return bytes(match.group(), 'latin1').decode('unicode_escape')
 
     return re.sub(r'\\u00[0-9a-fA-F]{2}', decode_match, input_string)
 
-def apply_tokenization(text, lang):
-    return tokenizer_ptbr.tokenize(text) if lang == Language.ptbr else tokenizer_enus.tokenize(text)
-
 def split_string_into_sentences(text, sentence_length):
     words = text.split()
     sentences = []
     current_sentence = []
 
     for word in words:
         current_sentence.append(word)
@@ -280,19 +274,16 @@
     sentences = [item for index, item in enumerate(sentences) if index not in removed_indexes]
     return sentences, removed_indexes
 
 def get_sentences_from_raw_text(raw_text, sentence_length):
     raw_text = raw_text.replace('\\', '').replace('-\n', '').replace('\n', ' ')
     raw_text = preprocessing(raw_text)
 
-    detected_language = detect_language(raw_text)
-    sentences = apply_tokenization(raw_text, detected_language)
-    sentences = ' '.join(sentences)
     # Create sentences from text. Each sentence is a string and should have 'sentence_length' words
-    sentences = split_string_into_sentences(sentences, sentence_length)
+    sentences = split_string_into_sentences(raw_text, sentence_length)
     sentences, _ = remove_empty_sentences(sentences)
 
     # Check sentences that are too long and split if needed
     final_sentences = []
     for s in sentences:
         try:
             if len(s.split()) > sentence_length:
```

