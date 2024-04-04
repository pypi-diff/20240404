# Comparing `tmp/gisweb_jppa-0.1.tar.gz` & `tmp/gisweb_jppa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisweb_jppa-0.1.tar", max compression
+gzip compressed data, was "gisweb_jppa-0.1.1.tar", max compression
```

## Comparing `gisweb_jppa-0.1.tar` & `gisweb_jppa-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-10-19 11:18:25.772662 gisweb_jppa-0.1/LICENSE
--rw-r--r--   0        0        0      213 2024-03-01 10:13:36.979369 gisweb_jppa-0.1/README.md
--rw-r--r--   0        0        0        0 2023-10-19 11:12:03.652659 gisweb_jppa-0.1/gisweb_jppa/__init__.py
--rw-r--r--   0        0        0     6746 2024-04-03 16:49:02.340968 gisweb_jppa-0.1/gisweb_jppa/jppa.py
--rw-r--r--   0        0        0     2740 2024-04-03 12:07:50.986488 gisweb_jppa-0.1/gisweb_jppa/schema.py
--rw-r--r--   0        0        0      216 2024-04-03 16:42:34.772734 gisweb_jppa-0.1/gisweb_jppa/templates/CreaAvvisoPagamento.xml
--rw-r--r--   0        0        0     2419 2024-04-03 16:45:09.324854 gisweb_jppa-0.1/gisweb_jppa/templates/Debito.xml
--rw-r--r--   0        0        0      186 2024-04-02 07:52:40.750671 gisweb_jppa-0.1/gisweb_jppa/templates/EliminaAvvisoPagamento.xml
--rw-r--r--   0        0        0      216 2024-04-02 16:32:57.426652 gisweb_jppa-0.1/gisweb_jppa/templates/NotificaPagamentoDebito.xml
--rw-r--r--   0        0        0     1431 2024-04-02 07:06:27.513115 gisweb_jppa-0.1/gisweb_jppa/templates/PagaDebiti.xml
--rw-r--r--   0        0        0      585 2024-04-02 07:32:09.736559 gisweb_jppa-0.1/gisweb_jppa/templates/serviceCall.xml
--rw-r--r--   0        0        0      486 2024-04-03 08:42:03.178699 gisweb_jppa-0.1/pyproject.toml
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 gisweb_jppa-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-10-19 11:18:25.772662 gisweb_jppa-0.1.1/LICENSE
+-rw-r--r--   0        0        0      213 2024-03-01 10:13:36.979369 gisweb_jppa-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-10-19 11:12:03.652659 gisweb_jppa-0.1.1/gisweb_jppa/__init__.py
+-rw-r--r--   0        0        0     8511 2024-04-04 13:27:37.740166 gisweb_jppa-0.1.1/gisweb_jppa/jppa.py
+-rw-r--r--   0        0        0     1462 2024-04-04 12:45:25.072173 gisweb_jppa-0.1.1/gisweb_jppa/schema.py
+-rw-r--r--   0        0        0      216 2024-04-03 16:42:34.772734 gisweb_jppa-0.1.1/gisweb_jppa/templates/CreaAvvisoPagamento.xml
+-rw-r--r--   0        0        0     2425 2024-04-04 10:05:09.163719 gisweb_jppa-0.1.1/gisweb_jppa/templates/Debito.xml
+-rw-r--r--   0        0        0      186 2024-04-02 07:52:40.750671 gisweb_jppa-0.1.1/gisweb_jppa/templates/EliminaAvvisoPagamento.xml
+-rw-r--r--   0        0        0      216 2024-04-02 16:32:57.426652 gisweb_jppa-0.1.1/gisweb_jppa/templates/NotificaPagamentoDebito.xml
+-rw-r--r--   0        0        0     1339 2024-04-04 10:12:09.011723 gisweb_jppa-0.1.1/gisweb_jppa/templates/PagaDebiti.xml
+-rw-r--r--   0        0        0      606 2024-04-04 10:27:10.052173 gisweb_jppa-0.1.1/gisweb_jppa/templates/serviceCall.xml
+-rw-r--r--   0        0        0      445 2024-04-04 13:33:36.500182 gisweb_jppa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 gisweb_jppa-0.1.1/PKG-INFO
```

### Comparing `gisweb_jppa-0.1/LICENSE` & `gisweb_jppa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gisweb_jppa-0.1/gisweb_jppa/jppa.py` & `gisweb_jppa-0.1.1/gisweb_jppa/jppa.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 
 # type: ignore
 from calendar import c
 from typing import Any
-from gisweb_jppa.schema import IDebito, IDocumento, IConfig, IImporto, ILoginRet, IPersona, IResult, IPagoPa, ITipoEnum, IEsito
+from gisweb_jppa.schema import IDebito, IConfig, IImporto, IPersona, IPagoPa, ITipoEnum, IEsito
 import logging
 import os, base64, uuid
 import json
 from datetime import datetime, date
 from pydantic import BaseModel
 from jinja2 import Environment, PackageLoader, select_autoescape
 import time
 import httpx
 from bs4 import BeautifulSoup
+import base64
 
 
 _logger = logging.getLogger('gisweb-jppa')
 
 
 env = Environment(
     loader=PackageLoader("gisweb_jppa"),
@@ -23,95 +24,52 @@
 )
 
 class Jppa:
     
     config:IConfig
     data:IPagoPa
     wsClient:Any
-    wsError: IResult
   
     def __init__(self, config:IConfig, data:IPagoPa) -> None:
         self.data = data
         self.config = config
-
-    async def provaXML(self):
-        respOK='''
-<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
-    <soap:Body>
-        <PagaDebitiResponse xmlns="http://schemi.informatica.maggioli.it/ws/pagopa/ServiziInterni">
-            <CodiceIPA>c_h183</CodiceIPA>
-            <IDOperazione>PagaDebiti</IDOperazione>
-            <DataRisposta>2024-04-03T12:52:27.499+02:00</DataRisposta>
-            <EsitoOperazionedd>OK</EsitoOperazione>
-            <DatiDettaglioRisposta>&lt;RispostaPagaDebiti xmlns="http://schemi.informatica.maggioli.it/operations/jcgpagopa/1_2">
-    &lt;Url>https://pspagopa.comune-online.it/jcitygov-pagopa/web/webpagopa/pagaCarrello?identTransazione=9c03ce84-c46b-4771-a763-f6298093100e&amp;amp;token=427212cb-671b-4b37-8529-318e6503facd&lt;/Url>
-    &lt;IdentTransazione>9c03ce84-c46b-4771-a763-f6298093100e&lt;/IdentTransazione>
-    &lt;Esito>
-        &lt;Esito>OK&lt;/Esito>
-    &lt;/Esito>
-&lt;/RispostaPagaDebiti></DatiDettaglioRisposta>
-        </PagaDebitiResponse>
-    </soap:Body>
-</soap:Envelope>
-        '''
-        
-        respERRORE='''
-        <soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
-    <soap:Body>
-        <PagaDebitiResponse xmlns="http://schemi.informatica.maggioli.it/ws/pagopa/ServiziInterni">
-            <CodiceIPA>c_h183</CodiceIPA>
-            <IDOperazione>PagaDebiti</IDOperazione>
-            <DataRisposta>2024-04-03T13:29:30.775+02:00</DataRisposta>
-            <EsitoOperazione>OK</EsitoOperazione>
-            <DatiDettaglioRisposta>&lt;RispostaPagaDebiti xmlns="http://schemi.informatica.maggioli.it/operations/jcgpagopa/1_2">
-    &lt;Url>https://pspagopa.comune-online.it/jcitygov-pagopa/web/webpagopa/pagaCarrello?identTransazione=ND&amp;amp;token=e83df496-7752-4ba6-a594-3a0e3fbb471e&lt;/Url>
-    &lt;IdentTransazione>ND&lt;/IdentTransazione>
-    &lt;Esito>
-        &lt;Esito>Error&lt;/Esito>
-        &lt;Messaggio>[I193_ERR_DATI_ACCERTAMENTO_INCONSISTENTI] I dati di accertamento non sono coerenti. Verificare che la somma degli importi specificati nell'oggetto &amp;lt;DettagliImporto&amp;gt; coincida con il valore dell'importo specificato nell'oggetto &amp;lt;DettaglioDebito&amp;gt;.&lt;/Messaggio>
-    &lt;/Esito>
-&lt;/RispostaPagaDebiti></DatiDettaglioRisposta>
-        </PagaDebitiResponse>
-    </soap:Body>
-</soap:Envelope>
-        '''
-        
-        import pdb;pdb.set_trace()
-        Operazione = "PagaDebiti"
-        soup = BeautifulSoup(respOK, 'xml')
-        esito = soup.find("EsitoOperazione") and soup.find("EsitoOperazione").string
-        if esito == 'OK':
-            respXml = soup.find('DatiDettaglioRisposta').string
-            soupresp = BeautifulSoup(respXml, 'xml')
-            print(soupresp)
-        elif esito == 'ERROR':
-            print('ddddddd')
-            
-        
-
         
-    async def serviceCall(self, Operazione:str, testXml=False) -> IEsito:
+    
+    async def serviceCall(self, Operazione:str, **kwargs) -> IEsito:
         """
         chiamata base al servizio JPPA
         """
 
         config = self.config
         data_richiesta =  datetime.now().strftime('%Y-%m-%dT%H:%M:%SZ') 
         
         template = env.get_template("Debito.xml")
-        self.data.debito_xml =  template.render(self.data)
-        
-        template = env.get_template(f"{Operazione}.xml")
-        datiDettaglioRichiesta =  template.render(self.data)
+        debito_xml =  template.render(self.data)
 
+        template = env.get_template(f"{Operazione}.xml")
+        datiDettaglioRichiesta =  template.render(
+            self.data, 
+            debito_xml=debito_xml, 
+            notifica_ko=config.notificaKO, 
+            notifica_ok=config.notificaOK, 
+            notifica_pagamento=config.notificaPagamento,
+            numero_avviso=kwargs.get("avviso")
+        )
+        
         template = env.get_template("serviceCall.xml")
-        xml = template.render({"content":datiDettaglioRichiesta, "operazione":Operazione, "data": data_richiesta})
+        xml = template.render(
+            content=datiDettaglioRichiesta, 
+            operazione=Operazione, 
+            data=data_richiesta, 
+            codice_ipa=config.codiceIpa, 
+            codice_servizio=config.codiceServizio
+        )
         headers = {'Content-type': 'text/xml; charset=utf-8'}  
         
-        if testXml:
+        if kwargs.get("testXml"):
             return xml
 
         async with httpx.AsyncClient() as client:
             
             #import pdb;pdb.set_trace()
             response = await client.post(config.wsUrl, content=xml, headers=headers)
             soup = BeautifulSoup(response.text, 'xml')
@@ -134,15 +92,14 @@
 
                         
                 
                 
     async def parseResponse(self, xml:str) -> IEsito:
         
         #import pdb;pdb.set_trace()
-        
         soup = BeautifulSoup(xml, 'xml')
         esito = soup.find("Esito")
         url = soup.find("Url") and soup.find("Url").string
         if soup.find("ChiaveDebito"):
             chiave = soup.find("ChiaveDebito") and soup.find("ChiaveDebito").string
         if soup.find("IdentTransazione"):
             chiave = soup.find("IdentTransazione") and soup.find("IdentTransazione").string
@@ -153,19 +110,113 @@
             stresito = esito.find('Esito') and esito.find('Esito').string
             if stresito == 'OK':
                 return {"esito":stresito, "chiave":chiave, "url":url, "avviso":avviso}
             elif stresito == 'Error':
                 if esito.find('Messaggio') :
                     return {"esito":stresito, "errore":esito.find('Messaggio').string}
                 
+        #nel caso di EliminaAvvisoPagamento non mette esito!!!
+        elif avviso:
+            return {"esito":"OK", "avviso":avviso}
+                
         with open("./jppa_resp.xml", "a") as f:
             f.write(xml)
         return {"esito":"ERRORE NON GESTITO"}
+    
+    async def stampaAvvisoPagamento(self):
+        
+        with open("logo.png", "rb") as f:
+            logo = base64.b64encode(f.read()).decode("latin1")
+        
+        xx=dict(
+            codiceIpaEnte=self.config.codiceIpa,
+            codiceServizio=self.config.codiceServizio,
+            codiceTipoDebito=self.data.debito.codice,
+            idDebito=self.data.debito.iddeb,
+            idPosizione=self.data.debito.idpos,
+        )
+        
+        data = dict(
+            authKeyDto = dict(username=self.config.wsUser,password=self.config.wsPassword),
+            base64FileLogoEnte = logo,
+            numeroAvviso = self.data.debito.iuv,
+            testoInformativaCanaliDigitali="ff sf asdf asdf asd fasdf asd f",
+            chiaviDebito=xx
+        )
+        
+        async with httpx.AsyncClient() as client:
+            response = await client.post(self.config.wsPrintUrl, data = json.dumps(data), headers = {'Content-type': 'application/json; charset=utf-8'})
+            if response.status_code == httpx.codes.OK:
+                try:
+                    return response.json()
+                except:
+                    return {"errore":"SSSSSSSSSSSS"}
+            else:
+                return {"errore":"SSSSSSSSSSSS"}
+        
+
+    
+    
+    
 
+    async def provaXML(self):
+        respOK='''
+<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
+    <soap:Body>
+        <PagaDebitiResponse xmlns="http://schemi.informatica.maggioli.it/ws/pagopa/ServiziInterni">
+            <CodiceIPA>c_h183</CodiceIPA>
+            <IDOperazione>PagaDebiti</IDOperazione>
+            <DataRisposta>2024-04-03T12:52:27.499+02:00</DataRisposta>
+            <EsitoOperazionedd>OK</EsitoOperazione>
+            <DatiDettaglioRisposta>&lt;RispostaPagaDebiti xmlns="http://schemi.informatica.maggioli.it/operations/jcgpagopa/1_2">
+    &lt;Url>https://pspagopa.comune-online.it/jcitygov-pagopa/web/webpagopa/pagaCarrello?identTransazione=9c03ce84-c46b-4771-a763-f6298093100e&amp;amp;token=427212cb-671b-4b37-8529-318e6503facd&lt;/Url>
+    &lt;IdentTransazione>9c03ce84-c46b-4771-a763-f6298093100e&lt;/IdentTransazione>
+    &lt;Esito>
+        &lt;Esito>OK&lt;/Esito>
+    &lt;/Esito>
+&lt;/RispostaPagaDebiti></DatiDettaglioRisposta>
+        </PagaDebitiResponse>
+    </soap:Body>
+</soap:Envelope>
+        '''
+        
+        respERRORE='''
+        <soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
+    <soap:Body>
+        <PagaDebitiResponse xmlns="http://schemi.informatica.maggioli.it/ws/pagopa/ServiziInterni">
+            <CodiceIPA>c_h183</CodiceIPA>
+            <IDOperazione>PagaDebiti</IDOperazione>
+            <DataRisposta>2024-04-03T13:29:30.775+02:00</DataRisposta>
+            <EsitoOperazione>OK</EsitoOperazione>
+            <DatiDettaglioRisposta>&lt;RispostaPagaDebiti xmlns="http://schemi.informatica.maggioli.it/operations/jcgpagopa/1_2">
+    &lt;Url>https://pspagopa.comune-online.it/jcitygov-pagopa/web/webpagopa/pagaCarrello?identTransazione=ND&amp;amp;token=e83df496-7752-4ba6-a594-3a0e3fbb471e&lt;/Url>
+    &lt;IdentTransazione>ND&lt;/IdentTransazione>
+    &lt;Esito>
+        &lt;Esito>Error&lt;/Esito>
+        &lt;Messaggio>[I193_ERR_DATI_ACCERTAMENTO_INCONSISTENTI] I dati di accertamento non sono coerenti. Verificare che la somma degli importi specificati nell'oggetto &amp;lt;DettagliImporto&amp;gt; coincida con il valore dell'importo specificato nell'oggetto &amp;lt;DettaglioDebito&amp;gt;.&lt;/Messaggio>
+    &lt;/Esito>
+&lt;/RispostaPagaDebiti></DatiDettaglioRisposta>
+        </PagaDebitiResponse>
+    </soap:Body>
+</soap:Envelope>
+        '''
+        
+        import pdb;pdb.set_trace()
+        Operazione = "PagaDebiti"
+        soup = BeautifulSoup(respOK, 'xml')
+        esito = soup.find("EsitoOperazione") and soup.find("EsitoOperazione").string
+        if esito == 'OK':
+            respXml = soup.find('DatiDettaglioRisposta').string
+            soupresp = BeautifulSoup(respXml, 'xml')
+            print(soupresp)
+        elif esito == 'ERROR':
+            print('ddddddd')
             
+        
+
```

### Comparing `gisweb_jppa-0.1/gisweb_jppa/schema.py` & `gisweb_jppa-0.1.1/gisweb_jppa/schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,107 +28,39 @@
     capitolo: str | None = None
     
 class IDebito(BaseModel):
     idpos: str #max 256
     codice: str | None = None
     dettaglio: str #max 1000
     iddeb: str #univoco max 256
+    iuv: str | None = None
     gruppo: str | None = None
     ordinamento: int | None = None
     data_inizio: str
     data_fine: str | None = None
     data_limite: str | None = None
     importo: float
     causale: str # max 140 
     importi: list[IImporto]
     
 class IPagoPa(BaseModel):
     soggetto: IPersona
     debito: IDebito
-    debito_xml:str | None = None
-    numero_avviso: str | None = None
-    
+
 class IEsito(BaseModel):
     esito: str
     errore: str | None = None
     descrizione: str | None = None
 
-    
-
-    
 class IConfig(BaseModel):
     wsUrl: str
     wsUser: str
     wsPassword: str
+    wsPrintUrl: str
     codiceIpa: str
     codiceServizio: str
-    codiceTipoDebito: str
-    FAKE: bool = False
-    FAKE_ERROR: str = ""
-    
-class BaseRet(BaseModel):
-    lngErrNumber: int = 0
-    strErrString: str = ''
-
-class ILoginRet(BaseRet):
-    strDST: str | None
-    
-class IResult(BaseRet):
-    lngNumPG: int = 0
-    lngAnnoPG: int = 0
-    strDataPG: str = ''
-    lngDocID: int = 0
-
-    
-
-
-class IDocumento(BaseModel):
-    id: int | None
-    descrizione: str
-    tipo: str
-    nome: str
-    content: Any
-    size: int
-    mimetype: str
-    ext: str
-
-
-class IUser(BaseModel):
-    username: str
-    password: str
-
-class IAmministrazione(BaseModel):
-    Denominazione: str
-    CodiceAOO: str
-    CodiceEnte: str
-    IndirizzoTelematico: EmailStr
-
-class IFascicolo(BaseModel):
-    numero: str
-    anno:str
-    
-class IParametro(BaseModel):
-    nome: str
-    valore: str
-
-class IProtocolloBase(BaseModel):
-    Soggetto: List[IPersona]
-    Flusso: str = 'E'
-    Oggetto: str | None
-    Titolario: str | None
-    UO: str   | None
-    Fascicolo: IFascicolo | None
-    NumeroRegistrazione: str = '0'
-    DataRegistrazione: str = '0'
-    Parametri: List[IParametro]
-
-class IProtocollo(IProtocolloBase):
-    Amministrazione: IAmministrazione
-    Principale: IDocumento
-    Allegati: List[IDocumento]
-    Applicativo: str = 'AGSPR'
-
+    notificaOK: str
+    notificaKO: str
+    notificaPagamento: str
 
-class IMessageData(BaseModel):
-    pass
```

### Comparing `gisweb_jppa-0.1/gisweb_jppa/templates/Debito.xml` & `gisweb_jppa-0.1.1/gisweb_jppa/templates/Debito.xml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             <IDDeb>{{debito.iddeb}}</IDDeb>
             <Gruppo>{{debito.gruppo}}</Gruppo>
             {%- if debito.ordinamento %}<Ordinamento>{{debito.ordinamento}}</Ordinamento>{% endif %}
             <DataInizioValidita>{{debito.data_inizio}}</DataInizioValidita>
             {%- if debito.data_fine %}<DataFineValidita>{{debito.data_fine}}</DataFineValidita>{% endif %}
             {%- if debito.data_limite %}<DataLimitePagabilita>{{debito.data_limite}}</DataLimitePagabilita>{% endif %}
             <ImportoDebito>{{debito.importo}}</ImportoDebito>
-            <CausaleDebito>{{debito.causale}}</CausaleDebito>
+            <CausaleDebito>{{debito.causale[:140]}}</CausaleDebito>
             <DettagliImporto>{% for importo in debito.importi %}
                 <dettaglioImporto>
                     <codice>{{importo.codice}}</codice>
                     <descrizione>{{importo.descrizione}}</descrizione>
                     <importo>{{importo.importo}}</importo>
                     <capitoloBilancio>{{importo.capitolo}}</capitoloBilancio>
                 </dettaglioImporto>{% endfor %}
```

### Comparing `gisweb_jppa-0.1/gisweb_jppa/templates/PagaDebiti.xml` & `gisweb_jppa-0.1.1/gisweb_jppa/templates/PagaDebiti.xml`

 * *Files 21% similar despite different names*

#### Comparing `gisweb_jppa-0.1/gisweb_jppa/templates/PagaDebiti.xml` & `gisweb_jppa-0.1.1/gisweb_jppa/templates/PagaDebiti.xml`

```diff
@@ -26,12 +26,12 @@
         {%- if soggetto.nazione %}
     <Nazione>{{soggetto.nazione}}</Nazione>
     {% endif %}
     <Email>{{soggetto.email}}</Email>
   </Versante>
   <Debito>{{debito_xml|safe}}</Debito>
   <BackUrl>
-    <BackUrlOK>https://sue.comune.rapallo.ge.it/iol-PagoPaEsito</BackUrlOK>
-    <BackUrlKO>https://sue.comune.rapallo.ge.it/iol-PagoPaEsito</BackUrlKO>
-    <BackUrlNotify>https://sue.comune.rapallo.ge.it/iol-PagoPaEsito</BackUrlNotify>
+    <BackUrlOK>{{notifica_ok}}</BackUrlOK>
+    <BackUrlKO>{{notifica_ko}}</BackUrlKO>
+    <BackUrlNotify>{{notifica_pagamento}}</BackUrlNotify>
   </BackUrl>
 </RichiestaPagaDebiti>
```

### Comparing `gisweb_jppa-0.1/PKG-INFO` & `gisweb_jppa-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: gisweb-jppa
-Version: 0.1
+Version: 0.1.1
 Summary: 
 Author: Roberto Starnini
 Author-email: roberto.starnini@gmail.com
 Requires-Python: >3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: httpx (>=0.25.2,<0.26.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: pydantic[dotenv,email] (>=2.3.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Example Package
 
 This is a simple example package. You can use
```

