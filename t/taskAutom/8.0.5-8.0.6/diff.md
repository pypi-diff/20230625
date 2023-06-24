# Comparing `tmp/taskAutom-8.0.5.tar.gz` & `tmp/taskAutom-8.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-8.0.5.tar", last modified: Fri Jun 23 00:41:47 2023, max compression
+gzip compressed data, was "taskAutom-8.0.6.tar", last modified: Sat Jun 24 22:56:37 2023, max compression
```

## Comparing `taskAutom-8.0.5.tar` & `taskAutom-8.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-23 00:41:47.271654 taskAutom-8.0.5/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.5/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-23 00:41:47.271654 taskAutom-8.0.5/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.5/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-23 00:41:47.271654 taskAutom-8.0.5/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-06-23 00:41:22.000000 taskAutom-8.0.5/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-23 00:41:47.271654 taskAutom-8.0.5/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-23 00:41:47.271654 taskAutom-8.0.5/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-06-23 00:41:34.000000 taskAutom-8.0.5/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    68009 2023-06-22 22:55:36.000000 taskAutom-8.0.5/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-23 00:41:47.271654 taskAutom-8.0.5/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-23 00:41:47.000000 taskAutom-8.0.5/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-06-23 00:41:47.000000 taskAutom-8.0.5/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-23 00:41:47.000000 taskAutom-8.0.5/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-06-23 00:41:47.000000 taskAutom-8.0.5/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-06-23 00:41:47.000000 taskAutom-8.0.5/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-06-23 00:41:47.000000 taskAutom-8.0.5/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-24 22:56:37.957511 taskAutom-8.0.6/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.6/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-24 22:56:37.957511 taskAutom-8.0.6/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.6/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-24 22:56:37.957511 taskAutom-8.0.6/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-06-24 21:06:25.000000 taskAutom-8.0.6/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-24 22:56:37.953511 taskAutom-8.0.6/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-24 22:56:37.953511 taskAutom-8.0.6/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-06-24 21:06:28.000000 taskAutom-8.0.6/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    68307 2023-06-24 22:20:17.000000 taskAutom-8.0.6/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-24 22:56:37.957511 taskAutom-8.0.6/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-24 22:56:37.000000 taskAutom-8.0.6/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-06-24 22:56:37.000000 taskAutom-8.0.6/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-24 22:56:37.000000 taskAutom-8.0.6/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-06-24 22:56:37.000000 taskAutom-8.0.6/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-06-24 22:56:37.000000 taskAutom-8.0.6/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-06-24 22:56:37.000000 taskAutom-8.0.6/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-8.0.5/LICENSE` & `taskAutom-8.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.5/PKG-INFO` & `taskAutom-8.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.5
+Version: 8.0.6
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-8.0.5/README.md` & `taskAutom-8.0.6/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.5/setup.py` & `taskAutom-8.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='8.0.5',
+    version='8.0.6',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-8.0.5/src/taskAutom/taskAutom.py` & `taskAutom-8.0.6/src/taskAutom/taskAutom.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import yaml
 import docx
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
-LATEST_VERSION = '8.0.5'
+LATEST_VERSION = '8.0.6'
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
@@ -141,114 +141,115 @@
 
 def fncPrintResults(listOfRouters, timeTotalStart, dictParam):
 
 	separator = "\n------ * ------"
 
 	outTxt    = ""
 
-	outTxt = outTxt + separator + '\n'
+	outTxt += separator + '\n'
 
 	#### GLOBALS
 
-	outTxt = outTxt + "Global Parameters:\n"
+	outTxt += "Global Parameters:\n"
 
-	outTxt = outTxt + "  Template File:              " + str(dictParam['pluginFilename']) + '\n'
+	outTxt += f'  Template File:              {str(dictParam["pluginFilename"])}\n'
 	if bool(dictParam['pluginType']):
-		outTxt = outTxt + "  Template Type:              " + str(dictParam['pluginType']) + '\n'
-	outTxt = outTxt + "  DATA File:                  " + str(dictParam['dataFile']) + '\n'
-	outTxt = outTxt + "  DATA UseHeader:             " + str(dictParam['useHeader']) + '\n'
-	outTxt = outTxt + "  Folder logInfo:             " + dictParam['logInfo'] + '\n'
-	outTxt = outTxt + "  Log FileName:               " + dictParam['logFileName'] + '\n'
-	outTxt = outTxt + "  Text File:                  " + dictParam['logInfo'] + "/job0_" + str(dictParam['pluginFileAlone']) + ".txt" + '\n'
+		outTxt += f"  Template Type:              {str(dictParam['pluginType'])}\n"
+	outTxt += f"  DATA File:                  {str(dictParam['dataFile'])}\n"
+	outTxt += f"  DATA UseHeader:             {str(dictParam['useHeader'])}\n"
+	outTxt += f"  Folder logInfo:             {dictParam['logInfo']}\n"
+	outTxt += f"  Log FileName:               {dictParam['logFileName']}\n"
+	outTxt += f"  Text File:                  {dictParam['logInfo']}/job0_{str(dictParam['pluginFileAlone'])}.txt\n"
 
 	if dictParam['genMop'] is True:
-		outTxt = outTxt + "  MOP filename                " + dictParam['logInfo'] + "/job0_" + str(dictParam['pluginFileAlone']) + ".docx\n"
+		outTxt += f"  MOP filename                {dictParam['logInfo']}/job0_{str(dictParam['pluginFileAlone'])}.docx\n"
 
 	if bool(dictParam['inventoryFile']):
-		outTxt = outTxt + "  Inventory file              " + str(dictParam['inventoryFile']) + "\n"
+		outTxt += f"  Inventory file              {str(dictParam['inventoryFile'])}\n"
 
 
-	outTxt = outTxt + "  Verify Commands:            " + str(dictParam['cmdVerify']) + '\n'	
-	outTxt = outTxt + "  Strict Order:               " + str(dictParam['strictOrder']) + '\n'
-	outTxt = outTxt + "  Pass Data By Row:           " + str(dictParam['passByRow']) + '\n'
+	outTxt += f"  Verify Commands:            {str(dictParam['cmdVerify'])}\n"	
+	outTxt += f"  Strict Order:               {str(dictParam['strictOrder'])}\n"
+	outTxt += f"  Pass Data By Row:           {str(dictParam['passByRow'])}\n"
 
 	if dictParam['strictOrder'] is True:
-		outTxt = outTxt + "  Halt-on-Error:              " + str(dictParam['haltOnError']) + '\n'
+		outTxt += f"  Halt-on-Error:              {str(dictParam['haltOnError'])}\n"
 
 	if dictParam['cronTime']['type'] is not None:
-		outTxt = outTxt + "  CRON Config:                " + str(dictParam['cronTime']) + '\n'
+		outTxt += f"  CRON Config:                {str(dictParam['cronTime'])}\n"
 
 	if dictParam['strictOrder'] is False:
-		outTxt = outTxt + "  Total Routers:              " + str(len(listOfRouters)) + '\n'
+		outTxt += f"  Total Routers:              {str(len(listOfRouters))}\n"
 	else:
-		outTxt = outTxt + "  Total Lines:                " + str(len(listOfRouters)) + '\n'
+		outTxt += f"  Total Lines:                {str(len(listOfRouters))}\n"
 
 	#### CONNECTION
 
-	outTxt = outTxt + "\nDefault Connection Parameters:\n"
+	outTxt += f"\nDefault Connection Parameters:\n"
 
 	if dictParam['inventoryFile'] != None:
-		outTxt = outTxt + "(Override by inventory file: " + dictParam['inventoryFile'] + ")\n\n"
+		outTxt += f"(Override by inventory file: {dictParam['inventoryFile']})\n\n"
 	
 	if dictParam['useSSHTunnel'] is True:
-		outTxt = outTxt + "  Use SSH tunnel:             " + str(dictParam['useSSHTunnel']) +" ("+ str(len(dictParam['jumpHosts'])) +")" + '\n'
+		outTxt += f"  Use SSH tunnel:             {str(dictParam['useSSHTunnel'])}; Server: {str(len(dictParam['jumpHosts']))}; File: {dictParam['jumpHostsFile']}\n"
 	else:
-		outTxt = outTxt + "  Use SSH tunnel:             " + str(dictParam['useSSHTunnel']) + '\n'
+		outTxt += f"  Use SSH tunnel:             {str(dictParam['useSSHTunnel'])}\n"
 	
-	outTxt = outTxt + "  Total Threads:              " + str(dictParam['progNumThreads']) + '\n'
-	outTxt = outTxt + "  Read Timeout:               " + str(dictParam['readTimeOut']) + '\n'
-	outTxt = outTxt + "  Time Between Routers:       " + str(dictParam['timeBetweenRouters']) + 'ms\n'
-	outTxt = outTxt + "  Username:                   " + str(dictParam['username']) + '\n'
-	outTxt = outTxt + "  Password Filename:          " + str(dictParam['passwordFile']) + '\n'
-	outTxt = outTxt + "  Device Type:                " + str(dictParam['deviceType']) + '\n'
+	outTxt += f"  Total Threads:              {str(dictParam['progNumThreads'])}\n"
+	outTxt += f"  Read Timeout:               {str(dictParam['readTimeOut'])}\n"
+	outTxt += f"  Time Between Routers:       {str(dictParam['timeBetweenRouters'])}ms\n"
+	outTxt += f"  Username:                   {str(dictParam['username'])}\n"
+	outTxt += f"  Password Filename:          {str(dictParam['passwordFile'])}\n"
+	outTxt += f"  Device Type:                {str(dictParam['deviceType'])}\n"
 
 	if dictParam['outputJob'] > 0:
 
 		timeTotalEnd 	= time.time()
 		timeTotal 		= timeTotalEnd - timeTotalStart		
 
-		outTxt = outTxt + separator + '\n'
+		outTxt += f"{separator}\n"
 
 		df = pd.concat(LOG_GLOBAL)
 
-		outTxt = outTxt + "\nTiming:\n"
+		outTxt += f"\nTiming:\n"
 
-		outTxt = outTxt + "  timeMin                     " + fncFormatTime(df['time'].min()) + '\n'
-		outTxt = outTxt + "  timeAvg:                    " + fncFormatTime(df['time'].mean()) + '\n'
-		outTxt = outTxt + "  timeMax:                    " + fncFormatTime(df['time'].max()) + '\n'
-		outTxt = outTxt + "  timeTotal:                  " + fncFormatTime(timeTotal) + '\n'
-		outTxt = outTxt + "  timeTotal/totalRouters:     " + fncFormatTime(timeTotal/len(LOG_GLOBAL)) + '\n'
+		outTxt += f'  timeMin                     {fncFormatTime(df["time"].min())}\n'
+		outTxt += f'  timeAvg:                    {fncFormatTime(df["time"].mean())}\n'
+		outTxt += f'  timeMax:                    {fncFormatTime(df["time"].max())}\n'
+		outTxt += f'  timeTotal:                  {fncFormatTime(timeTotal)}\n'
+		outTxt += f'  timeTotal/totalRouters:     {fncFormatTime(timeTotal/len(LOG_GLOBAL))}\n'
 
-		outTxt = outTxt + separator + '\n'
+		outTxt += f"{separator}\n"
 
 		df['threads']     = dictParam['progNumThreads']
 
 		df.to_csv(dictParam['logsCsvFilename'],index=False)
 
 		dfFailed = df[~df['Reason'].isin(['sftpOk','SendSuccess'])]
 
 		if dictParam['strictOrder'] is False:
-			outTxt = outTxt + "\nFailed routers:             " + str(len(dfFailed)) + '\n'
+			outTxt += f"\nFailed routers:             {str(len(dfFailed))}\n"
 		else:
-			outTxt = outTxt + "\nFailed lines:               " + str(len(dfFailed)) + '\n'
+			outTxt += f"\nFailed lines:               {str(len(dfFailed))}\n"
 
 		if dictParam['strictOrder'] is True and dictParam['haltOnError'] is True and dictParam['aluLogReason'] not in ['SendSucces','ReadTimeout']:
-			outTxt = outTxt + "   --> HaltOnError: " + dictParam['aluLogReason'] + ' <--\n'
+			outTxt += f"   --> HaltOnError: " + {dictParam['aluLogReason']} + ' <--\n'
 
 		if len(dfFailed) > 0:
-			outTxt = outTxt + dfFailed.to_string(max_colwidth=20) + '\n'
+			outTxt += dfFailed.to_string(max_colwidth=20)
 
-		outTxt = outTxt + separator
+		outTxt += f"{separator}\n"
 
 		df['Reason'] = df['Reason'].str.replace('(\w+:\d+|\d+.\d+.\d+.\d+:\d{1,6}|\d+.\d+.\d+.\d+)','',regex=True)
 		df['Reason'] = df.apply(lambda x: x['Reason'].replace(x['HostName'],''), axis=1)
 		dfGroup = df.groupby(['Reason']).agg({'Reason':['count'],'time':['min','max']})
 
-		outTxt = outTxt + '\n' + dfGroup.to_string(max_colwidth=20) + '\n'
+		outTxt += dfGroup.to_string(max_colwidth=20)
 
+		### Final reports
 		with open(dictParam['logsDirectory'] + '00_report.txt','w') as f:
 			f.write(outTxt)
 			f.close()
 
 		with open(dictParam['logsDirectory'] + '00_log_console.txt','w') as f:
 			for k in LOG_CONSOLE:
 				f.write(k+'\n')
@@ -265,15 +266,23 @@
 					dictParam['jumpHosts'][srv]['password'] = '*****'
 			if len(dictParam['inventory']) > 0:
 				for ip in dictParam['inventory']:
 					dictParam['inventory'][ip]['password'] = '*****'
 			json.dump(dictParam, f)
 			f.close()
 
-	outTxt = outTxt + separator + '\n'
+		### Data File of failed routers
+		dataFile = pd.read_excel(dictParam['dataFile'],sheet_name=dictParam['xlsSheetName']) if dictParam['xlsSheetName'] is not None else pd.read_csv(dictParam['dataFile'])
+		grpCol   = dictParam['dataGroupColumn']
+		listFailed = dfFailed['IP'].to_list()
+		failedDataFile = dataFile[dataFile[grpCol].isin(listFailed)]
+		if len(failedDataFile)>0:
+			failedDataFile.to_csv(dictParam['logsDirectory'] + '00_failedDataFile.csv',index=False)
+
+	outTxt += f"{separator}\n"
 
 	print(outTxt)
 
 def fncFormatTime(timeFloat, adjust=True):
 
 	move = 100
 
@@ -1046,15 +1055,15 @@
 			if pluginType == 'config':
 
 				try:
 					outputTxt    = conn2rtr.send_config_set(config_commands=inText, enter_config_mode=False, cmd_verify=cmdVerify, read_timeout=readTimeOut)
 					aluLogReason = ""
 					runStatus    = 1
 				except Exception as e:
-					aluLogReason = str(e).replace('\n',' ')
+					aluLogReason = str(e).replace('\n',' ').lstrip()
 					runStatus    = -1						
 
 			elif pluginType == 'show':
 
 				try:
 
 					for cmd in inText:
@@ -1070,26 +1079,26 @@
 							outputTxt = outputTxt + '\n' + cmd + '\n' + rx				
 					
 					aluLogReason = ""
 					runStatus    = 1
 
 				except Exception as e:
 					outputTxt = outputTxt + '\n' + cmd + '\n' + rx
-					aluLogReason = str(e).replace('\n',' ')
+					aluLogReason = str(e).replace('\n',' ').lstrip()
 					runStatus    = -1
 
 		elif isinstance(inText,str):
 			
 			try:
 				outputTxt    = conn2rtr.send_command(inText, expect_string=expectString, cmd_verify=cmdVerify, read_timeout=readTimeOut)
 				aluLogReason = ""
 				runStatus    = 1					
 			except Exception as e:
 				outputTxt    = ''
-				aluLogReason = str(e).replace('\n',' ')
+				aluLogReason = str(e).replace('\n',' ').lstrip()
 				runStatus    = -1
 
 		return runStatus, aluLogReason, outputTxt, outputJson
 
 	def fncAuxGetVal(self, connInfo, what):
 
 		def _getData(inText,connInfo):
@@ -1308,42 +1317,40 @@
 
 		if sftp:
 			remotePort = connInfo['sftpPort']
 		else:
 			remotePort = connInfo['remotePort']
 
 		systemIP = connInfo['systemIP']
-
+		fncPrintConsole(connInfo['strConn'] + "Trying sshServer on IP: " + str(tempIp))
+		
 		try:
-
 			server = sshtunnel.SSHTunnelForwarder( 	(tempIp, tempPort), 
 												ssh_username = tempUser, 
 												ssh_password = tempPass, 
 												remote_bind_address = (systemIP, remotePort),
 												allow_agent = False,
 											)
-
 		except Exception as e:
-
-			aluLogReason = "Problems creating SSH server: " + str(e).replace('\n',' ')
+			aluLogReason = "Problems creating SSH server: " + str(e).replace('\n',' ').lstrip()
 			fncPrintConsole(connInfo['strConn'] + str(aluLogReason))
 			server.stop(force=True)
 			controlPlaneAccess = False
 			localPort          = None
 			server             = None
 
 		if server is not None:
 
 			try:
 				server.start()
 				localPort = server.local_bind_port
-				fncPrintConsole(connInfo['strConn'] + "Trying sshServerTunnel on port: " + str(localPort))			
+				fncPrintConsole(connInfo['strConn'] + "Trying sshServerTunnel on port: " + str(localPort))		
 			except Exception as e:
 				fncPrintConsole(connInfo['strConn'] + "Trying sshServerTunnel on port: " + str(localPort))
-				aluLogReason = "Problems starting SSH server: " + str(e).replace('\n',' ')
+				aluLogReason = "Problems starting SSH server: " + str(e).replace('\n',' ').lstrip()
 				fncPrintConsole(connInfo['strConn'] + aluLogReason)
 				server.stop(force=True)
 				controlPlaneAccess = False
 				localPort          = None
 				server             = None
 		
 		if server is not None:
@@ -1358,16 +1365,14 @@
 				server.stop(force=True)
 				controlPlaneAccess = False
 				localPort          = None
 				server             = None
 			else:
 				controlPlaneAccess = True
 
-
-
 		connInfo['aluLogReason']       = aluLogReason
 		connInfo['controlPlaneAccess'] = controlPlaneAccess
 		connInfo['localPort']          = localPort
 		connInfo['sshServer']          = server
 
 		return connInfo
 
@@ -1407,15 +1412,15 @@
 				aluLogged    = True
 				aluLogReason = "LoggedOk"
 				aluLogUser   = tempUser
 				aluPass      = tempPass
 			except Exception as e:
 				conn2rtr     = None
 				aluLogged 	 = False
-				aluLogReason = str(e).replace('\n',' ')				
+				aluLogReason = str(e).replace('\n',' ').lstrip()
 				aluLogUser   = tempUser
 				aluPass      = "PassN/A"
 				fncPrintConsole(connInfo['strConn'] + aluLogReason + ": " + systemIP)
 
 		connInfo['conn2rtr']     = conn2rtr
 		connInfo['aluLogged']    = aluLogged
 		connInfo['aluLogUser']   = aluLogUser
@@ -1440,15 +1445,15 @@
 		else:
 			datos = connInfo['pluginScript']
 			fncPrintConsole(connInfo['strConn'] + "Running script per line...", show=1)
 
 		datos = datos.split('\n')
 		runStatus, aluLogReason, outRx, outRxJson = self.fncWriteToConnection(datos, connInfo)
 
-		aluLogReason = aluLogReason.replace('\n',' ')
+		aluLogReason = aluLogReason.replace('\n',' ').lstrip()
 
 		tEnd  = time.time()
 		tDiff = tEnd - tStart
 
 		## Analizing output only if writing to connection was successfull
 		if aluLogReason == "":
 			
@@ -1752,15 +1757,15 @@
 
 def getDictParam():
 
 	parser = argparse.ArgumentParser(description='taskAutom Parameters.', prog='taskAutom', usage='%(prog)s [options]')
 	parser.add_argument('-v'  ,'--version',     help='Version', action='version', version='Lucas Aimaretto - (c)2023 - laimaretto@gmail.com - Version: '+LATEST_VERSION )
 
 	groupJobTypes = parser.add_argument_group('JobTypes')
-	groupJobTypes.add_argument('-j'  ,'--jobType',       type=int, choices=[0,2,3], default=0, help='Type of job. j=0 to check data and plugin; j=2, to execute. j=3, to upload files via SCP/SFTP. Default=0')
+	groupJobTypes.add_argument('-j'  ,'--jobType',       type=int, choices=[0,2,3], default=0, help='Type of job. j=0 to check data and plugin; j=2, to execute. j=3, to upload files via SCP/SFTP. When j=3, password must be entered manually. Default=0')
 
 	groupPugin = parser.add_argument_group('Plugin')
 	groupPugin.add_argument('-pt' ,'--pluginType',      type=str, help='Type of plugin.', default='show', choices=['show','config'])
 	groupPugin.add_argument('-py' ,'--pluginFilename' , type=str, help='PY Template File. Optional if jobType=3.')
 
 	groupData = parser.add_argument_group('Data Related')
 	groupData.add_argument('-d'  ,'--dataFile',        type=str, required=True, help='DATA File with parameters. Either CSV or XLSX. If XLSX, enable -xls option with sheet name.')
@@ -1898,68 +1903,50 @@
 
 	return dictParam
 
 def checkCredentials(dictParam):
 
 	if dictParam['outputJob'] == 0:
 
-		#fncRun(dictParam)
 		pass
 
-	elif (	
-		dictParam['outputJob'] == 2 and 
-		dictParam['username'] and 
-		dictParam['passwordFile'] is None and 
-		dictParam['logInfo'] and 
-		(
-			dictParam['pluginType'] or dictParam['cronTime']
-		)
-		):
-
-		print("\n#######################################")
-		print("# About to run. Ctrl+C if not sure... #")
-		print("#######################################\n")
-		dictParam['password'] = getpass("### -> PASSWORD (default user: " + dictParam['username'] + "): ")
+	elif dictParam['outputJob'] == 2:
+		
+		if dictParam['username'] and dictParam['logInfo'] and (dictParam['pluginType'] or dictParam['cronTime']):
+		
+			if dictParam['passwordFile'] is None:
 
-		#fncRun(dictParam)
-		pass
+				print("\n#######################################")
+				print("# About to run. Ctrl+C if not sure... #")
+				print("#######################################\n")
+				dictParam['password'] = getpass("### -> PASSWORD (default user: " + dictParam['username'] + "): ")
 
-	elif (
-		dictParam['outputJob'] == 2 and 
-		dictParam['username'] and 
-		dictParam['passwordFile'] is not None and 
-		dictParam['logInfo'] and 
-		(
-			dictParam['pluginType'] or dictParam['cronTime']
-		)		
-	):	
-
-		# Trying to open the password file to obtain the password
-		with open(dictParam['passwordFile']) as pf:
-			dictParam['password'] = pf.readlines()[0].rstrip()
-			pf.close()
-		
-		#fncRun(dictParam)
-		pass
+			else:
+				# Trying to open the password file to obtain the password
+				with open(dictParam['passwordFile']) as pf:
+					dictParam['password'] = pf.readlines()[0].rstrip()
+					pf.close()
 
-	elif (	
-		dictParam['outputJob'] == 3 and 
-		dictParam['username'] and 
-		dictParam['passwordFile'] is None and 
-		dictParam['logInfo']
-		):
-
-		print("\n#############################################################")
-		print("# You are about to do massive upload of files vía SCP/SFTP  #")
-		print("# About to run. Ctrl+C if not sure...                       #")
-		print("#############################################################\n")
-		dictParam['password'] = getpass("### -> PASSWORD (default user: " + dictParam['username'] + "): ")
+		else:
+			print("Your type of Job is 2, which means you are about to execute scripts on routers.\nAt least define --username, --logInfo and --pluginType.\nRun: taskAutom -h for help.\nQuitting...")
+			quit()			
 
-		#fncRun(dictParam)
-		pass
+	elif dictParam['outputJob'] == 3:
+
+		if dictParam['username'] and dictParam['passwordFile'] is None and dictParam['logInfo']:
+
+			print("\n#############################################################")
+			print("# You are about to do massive upload of files vía SCP/SFTP  #")
+			print("# About to run. Ctrl+C if not sure...                       #")
+			print("#############################################################\n")
+			dictParam['password'] = getpass("### -> PASSWORD (default user: " + dictParam['username'] + "): ")
+
+		else:
+			print("Your type of Job is 3, which means you are about to send files to routers via SCP/SFTP.\nAt least define --username, --logInfo. Password must be enterd manually.\nRun: taskAutom -h for help.\nQuitting...")
+			quit()	
 
 	else:
 
 		print("Not enough paramteres.\nAt least define --username, --logInfo, depending on the jobType.\nRun: taskAutom -h for help.\nQuitting...")
 		quit()
 
 	return dictParam
```

### Comparing `taskAutom-8.0.5/taskAutom.egg-info/PKG-INFO` & `taskAutom-8.0.6/taskAutom.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.5
+Version: 8.0.6
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

