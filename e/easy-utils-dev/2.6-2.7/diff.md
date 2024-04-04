# Comparing `tmp/easy_utils_dev-2.6.tar.gz` & `tmp/easy_utils_dev-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.6.tar", last modified: Sun Mar 31 19:40:26 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.7.tar", last modified: Thu Apr  4 13:44:32 2024, max compression
```

## Comparing `easy_utils_dev-2.6.tar` & `easy_utils_dev-2.7.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 19:40:26.518016 easy_utils_dev-2.6/
--rw-rw-rw-   0        0        0      172 2024-03-31 19:40:26.513023 easy_utils_dev-2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-31 19:40:26.476016 easy_utils_dev-2.6/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.6/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.6/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      292 2024-03-11 21:27:23.000000 easy_utils_dev-2.6/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.6/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     4407 2024-03-21 23:01:23.000000 easy_utils_dev-2.6/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.6/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0    30914 2024-03-31 19:39:46.000000 easy_utils_dev-2.6/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.6/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.6/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2129 2024-03-09 10:58:14.000000 easy_utils_dev-2.6/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.6/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     6242 2024-03-15 01:22:07.000000 easy_utils_dev-2.6/easy_utils_dev/wsnoclib.py
-drwxrwxrwx   0        0        0        0 2024-03-31 19:40:26.509019 easy_utils_dev-2.6/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      172 2024-03-31 19:40:26.000000 easy_utils_dev-2.6/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2024-03-31 19:40:26.000000 easy_utils_dev-2.6/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 19:40:26.000000 easy_utils_dev-2.6/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-03-31 19:40:26.000000 easy_utils_dev-2.6/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-31 19:40:26.000000 easy_utils_dev-2.6/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 19:40:26.518016 easy_utils_dev-2.6/setup.cfg
--rw-rw-rw-   0        0        0      315 2024-03-31 19:40:22.000000 easy_utils_dev-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:44:32.902983 easy_utils_dev-2.7/
+-rw-rw-rw-   0        0        0      172 2024-04-04 13:44:32.894457 easy_utils_dev-2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 13:44:32.827167 easy_utils_dev-2.7/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.7/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.7/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      339 2024-04-04 13:44:23.000000 easy_utils_dev-2.7/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.7/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     4470 2024-04-02 04:10:27.000000 easy_utils_dev-2.7/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.7/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7440 2024-04-04 13:43:40.000000 easy_utils_dev-2.7/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33403 2024-03-31 20:13:50.000000 easy_utils_dev-2.7/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.7/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.7/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.7/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     1918 2024-03-12 13:27:35.000000 easy_utils_dev-2.7/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.7/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 11:55:23.000000 easy_utils_dev-2.7/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-04 13:44:32.886643 easy_utils_dev-2.7/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      172 2024-04-04 13:44:32.000000 easy_utils_dev-2.7/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2024-04-04 13:44:32.000000 easy_utils_dev-2.7/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 13:44:32.000000 easy_utils_dev-2.7/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 13:44:32.000000 easy_utils_dev-2.7/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-04 13:44:32.000000 easy_utils_dev-2.7/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 13:44:32.902983 easy_utils_dev-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      315 2024-04-04 13:43:44.000000 easy_utils_dev-2.7/setup.py
```

### Comparing `easy_utils_dev-2.6/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.7/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.6/easy_utils_dev/Events.py` & `easy_utils_dev-2.7/easy_utils_dev/Events.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.6/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.7/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.6/easy_utils_dev/debugger.py` & `easy_utils_dev-2.7/easy_utils_dev/debugger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging , os , inspect
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
 from .utils import getRandomKey
 from .custom_env import custom_env , setupEnvironment , insertKey
 import json
-from .uiserver import UISERVER
 
 def setGlobalHomePath( path ) :
     env = custom_env()
     env['debugger_homepath'] = path
     if not os.path.exists( path ) :
         print(f'Warning: Provided path does not exist. Path is {path}')
 
@@ -37,26 +36,30 @@
         # Add the file handler to the logger
         self.logger.addHandler(file_handler)
         # self.logger.addHandler(self.stream_handler)
         self.logger.addFilter(self.on_log )
         if onscreen : self.enable_print()
         elif not onscreen : self.disable_print()
 
+
     def addStreamService( self , socketio , streampath='/debugger/stream/log' ) :
         """
         This function takes a live socketio server. it emit the log message using default path which is /debugger/stream/log
         """
         self.stream_service = socketio
         self.streampath = streampath
         
+    def updateLogName( self , name ) :
+        self.name = name
 
     def on_log(self , record) :
         d = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         l = f"[{d}] - [{self.name}] - [{record.levelname}]: {record.getMessage()}"
-        open(self.homePath , 'a+').write(f"{l}\n")
+        with open(self.homePath , 'a+') as f :
+            f.write(f"{l}\n")
         if self.stream_service is not None :
             self.stream_service.emit( self.streampath , json.dumps({
                 'message' : l ,
                 'level' : record.levelname ,
                 'msg' : record.getMessage(),
                 'date' : d ,
                 'id' : self.id
```

### Comparing `easy_utils_dev-2.6/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.7/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.6/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.7/easy_utils_dev/ne1830PSS.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,33 +32,33 @@
         self.requireAknow=None
         self.pssRelease = None
         self.auto_enable_tcp_forward=auto_enable_tcp_forward
         self.tcpForwardStatus=None
         if self.auto_enable_tcp_forward :
             self.logger.info(f'WARNING : Auto enable tcp forwarding is enabled. This will allow tcp fowarding in target machine then restarting sshd service agent.')
 
+    def set_debug_level( self , level ) :
+        self.logger.set_level(level)
+
     def nfmtJumpServer(self, ip , usr , pw  ) :
         self.logger.info(f"""ssh to WSNOC VM nested/jumpserver ssh  [ IP => {ip} ]..""")
         try :
             self.jumpServerInSameInstance = True
             self.jumpserver  = paramiko.SSHClient()
             self.jumpserver.set_missing_host_key_policy(paramiko.AutoAddPolicy())
             self.logger.info(f'Connecting to VM jumpserver with {usr}@{ip} port=[{self.port}] ..')
             self.jumpserver.connect(ip  , self.port , usr , pw )
             self.isjumpserver = True
             self.nfmtip = ip 
             self.nfmtsshuser = usr
             self.nfmtsshpw = pw
             self.logger.debug(f"""check if tcpfowarding is allowed or not .. """)
-            stdin, stdout, stderr = self.jumpserver.exec_command("cat /etc/ssh/sshd_config | grep -i AllowTcpForwarding")
-            result = stdout.readlines()
+            isEnabled , result  = self.checkIfTcpForwardingEnabled()
             self.logger.debug(f"""check if tcpfowarding is allowed or not. Result : {result}""")
-            for line in result :
-                if "#" in line : continue 
-                if 'no' in line :
+            if not isEnabled :
                     self.logger.debug(f"""check if tcpfowarding is allowed or not. result is disallowed. fixing .. """)
                     self.fixTcpSSH()
                     self.jumpserver.close()
                     self.logger.debug(f"""re-establish the connection [ jumpserver ] after modifying the sshd file and restarting the sshd service ..""")
                     self.jumpserver  = paramiko.SSHClient()
                     self.jumpserver.set_missing_host_key_policy(paramiko.AutoAddPolicy())
                     self.jumpserver.connect(ip  , self.port , usr , pw )
@@ -233,18 +233,19 @@
             return self.client
         # getting the ne version.
         result = self.get_neversion()
         if '-' in result :
             self.logger.debug(f'partitioning release response as - in result .. ')
             self.pssRelease = float(result.partition('-')[2].partition('-')[0])
             self.logger.debug(f'paritioned release response as float is {self.pssRelease}')
-            if self.pssRelease < 23.6 :
+            isRequired = self.isRequireAknowledge(self.pssRelease)
+            if isRequired :
                 self.logger.debug(f'switching to require aknow mode as release is less than 23.6')
                 self.requireAknow = True
-            else :
+            elif not isRequired :
                 self.logger.debug(f'switching to NOT require aknow mode as release is not less than 23.6')
                 self.requireAknow = False
         else :
             self.logger.error(f'PSS release is undefined due to detection pattern is not found. no "-" char found in pss release result. result {result}')
             raise Exception('undefined PSS Release return output. check logs ')         
         self.channel = self.client.invoke_shell()
         self.logger.debug(f'set timeout in srv channel to {self.TIMEOUT}')
@@ -257,15 +258,24 @@
         self.logger.debug(f'Starting/Processing login window handler to enter username, password and aknowledge message if appears ...')
         self.enter_login_prompt()
         self.logger.debug(f'Starting/Processing to auto detect the NE prompt NE_NAME+# ...')
         self.determine_prompt()
         self.connected = True
         self.logger.debug(f'Processing handler to enter username, password completed. returning self.client object ')
         return self.client
-        
+    
+    def isRequireAknowledge(self , newRelease) : 
+        if '-' in str(newRelease) :
+            newRelease = float(newRelease.split('-')[0])
+        if int(newRelease) in range( 0 , 15 ) :
+            return True
+        elif int(newRelease) >= 23 :
+            return False
+        else  : 
+            return True
 
     def getTime(self) :
         now = datetime.now()
         dt_string = now.strftime("%d-%m-%Y_%H-%M-%S")
         return dt_string
 
     def get_neversion(self) :
@@ -588,14 +598,24 @@
                     profile= 'N/A'
                 data.append({'shelf' : shelf , 'slot' : slot ,  'shelf/slot' : shelfslot , 'card' : card , 'profile' : profile  })
             except :
                 continue
         self.logger.info('Getting NE firmware .. completed') 
         return data
 
+    def get_ec_type(self) :
+        self.logger.debug('retreiving EC type from all installed cards ...')
+        cards = self.get_allcards().get('all')
+        for key , value in cards.items() :
+            self.logger.debug(f'Searching for EC in {key} detail=> {value}')
+            if 'EC' in value.get('card' , '').upper() :
+                self.logger.debug(f'''EC card detected in {key} card={value.get('card')}''')
+                return value.get('card')
+
+
     def get_availableFW(self) :
         self.logger.info('Getting available firmware .. ')        
         cli = f"show firmware available"
         result = self.cli_execute(cli)
         self.logger.info(f'get_availableFW : command = {cli}')    
         self.logger.debug(f'{self.nodeName} - {cli} - {result}')
         result = result.splitlines()
@@ -618,14 +638,50 @@
                         current_fw = line.replace(' ', '').replace('\n' , '').replace('*' , '')
                         data[card] = {'profiles' : profiles , 'currentfw' :  current_fw}
             except : 
                 pass
         self.logger.debug(f'Getting available firmware completed. {data}') 
         return data
 
+    def enable_cli_user(self , user, exception_on_failure=True ):
+        """
+        Enable PSS login user status from disabled to enabled.
+        user : cli user : string
+        exception_on_failure : bool, default True. Raise exception if user not found.
+
+        return True if user is enabled
+        return False if error raised during the process.
+        """
+        self.logger.debug(f"enable pss cli user {user}")
+        cli = f'config admin users edit {user} status enabled'
+        result = self.cli_execute(cli)
+        if 'unknown username' in result or len(result) > 0 :
+            if exception_on_failure :
+                raise Exception(f'Username {user} is not found. PSS response is {result}')
+            return False
+        return True
+
+    def disable_cli_user(self , user, exception_on_failure=True ):
+        """
+        Disable PSS login user status from enabled to disabled.
+        user : cli user : string
+        exception_on_failure : bool, default True. Raise exception if user not found.
+
+        return True if user is disabled
+        return False if error raised during the process.
+        """
+        self.logger.debug(f"enable pss cli user {user}")
+        cli = f'config admin users edit {user} status disabled'
+        result = self.cli_execute(cli)
+        if 'unknown username' in result or len(result) > 0 :
+            if exception_on_failure :
+                raise Exception(f'Username {user} is not found. PSS response is {result}')
+            return False
+        return True
+
     def get_shelfs(self) :
         self.logger.info('Getting shelfs .. ')
         shelfsList = []
         cli = f"show shelf *"
         shelfs = self.cli_execute(cli).splitlines()
         for line in shelfs :
             try :
@@ -644,21 +700,26 @@
         return shelfsList
 
 
 if __name__ == '__main__' : 
     pass
 
         
-pss = PSS1830()
+pss = PSS1830(auto_enable_tcp_forward=True)
 pss.port = 322
+pss.set_debug_level('debug')
 jumpserver = pss.nfmtJumpServer('127.0.0.1' , 'root' , 'Nokia@2023')
-# pss = PSS1830()
-# x= pss.connect('ssh' , neip="10.10.20.1" , jumpserver=jumpserver )
+pss = PSS1830()
+pss.set_debug_level('debug')
+x= pss.connect('cli' , neip="10.10.40.167" , jumpserver=jumpserver )
 # x = pss.get_allcards()
-# print(x)
+# x = pss.get_ec_type()
+s = pss.enable_cli_user('admin')
+print(s)
+
 # s = pss.get_nefirmware()
 # print(s)
 # pss.get_mastershelf()
 # pss.disable_openagent()
 # pss.enable_openagent()
 # pss.openagent_status()
 # pss.get_version()
```

### Comparing `easy_utils_dev-2.6/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.7/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.6/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.7/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.6/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.7/easy_utils_dev/uiserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,18 @@
     def __init__(self ,id=getRandomKey(n=15),secretkey=generateToken(),address='localhost',port=5312,**kwargs) -> None:
         self.id = id
         self.app = app = Flask(self.id)
         app.config['SECRET_KEY'] = secretkey
         CORS(app,resources={r"/*":{"origins":"*"}})
         self.address= address 
         self.port = port
+        self.httpProtocol = 'http'
         self.socketio = SocketIO(app , cors_allowed_origins="*"  ,async_mode='threading' , engineio_logger=False , always_connect=True ,**kwargs )
         cenv[id] = self
-        self.fullAddress = f"http://{self.address}:{self.port}"
+        self.fullAddress = f"{self.httpProtocol}://{self.address}:{self.port}"
 
     def getInstance(self) :
         return self.getFlask() , self.getSocketio() , self.getWsgi()
     
     def getSocketio( self ):
         return self.socketio
     
@@ -52,13 +53,11 @@
             app = self.app )
         
         def _start() :
             print(f"web-socket: {self.fullAddress}")
             log = logging.getLogger('werkzeug')
             log.setLevel(logging.ERROR)
             wsgi_server.serve_forever()   
-
-
         
         self.flaskprocess = Thread(target=_start)
         self.flaskprocess.daemon = True
         self.flaskprocess.start()
```

### Comparing `easy_utils_dev-2.6/easy_utils_dev/utils.py` & `easy_utils_dev-2.7/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.6/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.7/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 setup.py
 easy_utils_dev/EasySsh.py
 easy_utils_dev/Events.py
 easy_utils_dev/__init__.py
 easy_utils_dev/custom_env.py
 easy_utils_dev/debugger.py
 easy_utils_dev/encryptor.py
+easy_utils_dev/lralib.py
 easy_utils_dev/ne1830PSS.py
 easy_utils_dev/optics_utils.py
 easy_utils_dev/simple_sqlite.py
 easy_utils_dev/uiserver.py
 easy_utils_dev/utils.py
 easy_utils_dev/wsnoclib.py
+easy_utils_dev/wsselib.py
 easy_utils_dev.egg-info/PKG-INFO
 easy_utils_dev.egg-info/SOURCES.txt
 easy_utils_dev.egg-info/dependency_links.txt
 easy_utils_dev.egg-info/requires.txt
 easy_utils_dev.egg-info/top_level.txt
```

