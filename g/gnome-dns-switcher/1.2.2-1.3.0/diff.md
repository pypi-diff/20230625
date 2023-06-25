# Comparing `tmp/gnome-dns-switcher-1.2.2.tar.gz` & `tmp/gnome-dns-switcher-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnome-dns-switcher-1.2.2.tar", last modified: Mon May  2 09:02:52 2022, max compression
+gzip compressed data, was "gnome-dns-switcher-1.3.0.tar", last modified: Sun Jun 25 12:05:10 2023, max compression
```

## Comparing `gnome-dns-switcher-1.2.2.tar` & `gnome-dns-switcher-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ahcvisser  (1000) ahcvisser  (1000)        0 2022-05-02 09:02:52.408603 gnome-dns-switcher-1.2.2/
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)    35148 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/LICENSE
--rw-rw-r--   0 ahcvisser  (1000) ahcvisser  (1000)     1953 2022-05-02 09:02:52.408603 gnome-dns-switcher-1.2.2/PKG-INFO
--rwxr-xr-x   0 ahcvisser  (1000) ahcvisser  (1000)     1114 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/README.md
-drwxrwxr-x   0 ahcvisser  (1000) ahcvisser  (1000)        0 2022-05-02 09:02:52.408603 gnome-dns-switcher-1.2.2/gnome_dns_switcher/
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)        0 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/__init__.py
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)     1622 2021-02-02 08:21:42.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/__main__.py
-drwxrwxr-x   0 ahcvisser  (1000) ahcvisser  (1000)        0 2022-05-02 09:02:52.408603 gnome-dns-switcher-1.2.2/gnome_dns_switcher/gnome_helpers/
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)      115 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/gnome_helpers/__init__.py
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)      436 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/gnome_helpers/async_call.py
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)     1884 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/gnome_helpers/indicator.py
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)     1672 2022-05-02 09:02:30.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/gnome_helpers/nmcli.py
-drwxrwxr-x   0 ahcvisser  (1000) ahcvisser  (1000)        0 2022-05-02 09:02:52.408603 gnome-dns-switcher-1.2.2/gnome_dns_switcher/switcher/
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)       64 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/switcher/__init__.py
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)     2821 2022-05-02 09:02:34.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/switcher/dnsswitcher.py
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)      206 2021-02-02 08:21:42.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher/switcher/server.py
-drwxrwxr-x   0 ahcvisser  (1000) ahcvisser  (1000)        0 2022-05-02 09:02:52.408603 gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/
--rw-rw-r--   0 ahcvisser  (1000) ahcvisser  (1000)     1953 2022-05-02 09:02:52.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/PKG-INFO
--rw-rw-r--   0 ahcvisser  (1000) ahcvisser  (1000)      653 2022-05-02 09:02:52.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/SOURCES.txt
--rw-rw-r--   0 ahcvisser  (1000) ahcvisser  (1000)        1 2022-05-02 09:02:52.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/dependency_links.txt
--rw-rw-r--   0 ahcvisser  (1000) ahcvisser  (1000)       73 2022-05-02 09:02:52.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/entry_points.txt
--rw-rw-r--   0 ahcvisser  (1000) ahcvisser  (1000)       10 2022-05-02 09:02:52.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/requires.txt
--rw-rw-r--   0 ahcvisser  (1000) ahcvisser  (1000)       19 2022-05-02 09:02:52.000000 gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/top_level.txt
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)     1060 2022-05-02 09:02:52.408603 gnome-dns-switcher-1.2.2/setup.cfg
--rw-r--r--   0 ahcvisser  (1000) ahcvisser  (1000)      125 2021-02-02 08:03:20.000000 gnome-dns-switcher-1.2.2/setup.py
+drwxrwxr-x   0 anner     (1000) anner     (1000)        0 2023-06-25 12:05:10.690016 gnome-dns-switcher-1.3.0/
+-rw-rw-r--   0 anner     (1000) anner     (1000)    35148 2023-06-25 08:26:14.000000 gnome-dns-switcher-1.3.0/LICENSE
+-rw-rw-r--   0 anner     (1000) anner     (1000)     4328 2023-06-25 12:05:10.690016 gnome-dns-switcher-1.3.0/PKG-INFO
+-rwxrwxr-x   0 anner     (1000) anner     (1000)     3494 2023-06-25 12:01:56.000000 gnome-dns-switcher-1.3.0/README.md
+drwxrwxr-x   0 anner     (1000) anner     (1000)        0 2023-06-25 12:05:10.686016 gnome-dns-switcher-1.3.0/gnome_dns_switcher/
+-rw-rw-r--   0 anner     (1000) anner     (1000)        0 2023-06-25 08:26:14.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/__init__.py
+-rw-rw-r--   0 anner     (1000) anner     (1000)     3201 2023-06-25 11:39:27.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/__main__.py
+drwxrwxr-x   0 anner     (1000) anner     (1000)        0 2023-06-25 12:05:10.690016 gnome-dns-switcher-1.3.0/gnome_dns_switcher/gnome_helpers/
+-rw-rw-r--   0 anner     (1000) anner     (1000)      115 2023-06-25 08:26:14.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/gnome_helpers/__init__.py
+-rw-rw-r--   0 anner     (1000) anner     (1000)      436 2023-06-25 08:26:14.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/gnome_helpers/async_call.py
+-rw-rw-r--   0 anner     (1000) anner     (1000)     2450 2023-06-25 10:30:16.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/gnome_helpers/indicator.py
+-rw-rw-r--   0 anner     (1000) anner     (1000)     1872 2023-06-25 10:29:12.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/gnome_helpers/nmcli.py
+drwxrwxr-x   0 anner     (1000) anner     (1000)        0 2023-06-25 12:05:10.690016 gnome-dns-switcher-1.3.0/gnome_dns_switcher/switcher/
+-rw-rw-r--   0 anner     (1000) anner     (1000)       64 2023-06-25 08:26:14.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/switcher/__init__.py
+-rw-rw-r--   0 anner     (1000) anner     (1000)     3446 2023-06-25 10:31:44.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/switcher/dnsswitcher.py
+-rw-rw-r--   0 anner     (1000) anner     (1000)      206 2023-06-25 08:26:14.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher/switcher/server.py
+drwxrwxr-x   0 anner     (1000) anner     (1000)        0 2023-06-25 12:05:10.686016 gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/
+-rw-rw-r--   0 anner     (1000) anner     (1000)     4328 2023-06-25 12:05:10.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/PKG-INFO
+-rw-rw-r--   0 anner     (1000) anner     (1000)      653 2023-06-25 12:05:10.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/SOURCES.txt
+-rw-rw-r--   0 anner     (1000) anner     (1000)        1 2023-06-25 12:05:10.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/dependency_links.txt
+-rw-rw-r--   0 anner     (1000) anner     (1000)       73 2023-06-25 12:05:10.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/entry_points.txt
+-rw-rw-r--   0 anner     (1000) anner     (1000)       58 2023-06-25 12:05:10.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/requires.txt
+-rw-rw-r--   0 anner     (1000) anner     (1000)       19 2023-06-25 12:05:10.000000 gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/top_level.txt
+-rw-rw-r--   0 anner     (1000) anner     (1000)     1037 2023-06-25 12:05:10.690016 gnome-dns-switcher-1.3.0/setup.cfg
+-rw-rw-r--   0 anner     (1000) anner     (1000)      125 2023-06-25 08:26:14.000000 gnome-dns-switcher-1.3.0/setup.py
```

### Comparing `gnome-dns-switcher-1.2.2/LICENSE` & `gnome-dns-switcher-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gnome-dns-switcher-1.2.2/gnome_dns_switcher/gnome_helpers/indicator.py` & `gnome-dns-switcher-1.3.0/gnome_dns_switcher/gnome_helpers/indicator.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,54 +11,75 @@
 gi.require_version("GLib", "2.0")
 
 gi.require_version('Notify', '0.7')
 from gi.repository import Notify
 
 
 class Indicator:
-    indicator: appindicator.Indicator
-    menu: Gtk.Menu
-    notifications: List[Notify.Notification] = []
+    _return_code: int = 0
+    _application_id: str
+    _indicator: appindicator.Indicator = None
+    _menu: Gtk.Menu = None
+    _notifications: List[Notify.Notification] = []
 
     def __init__(self, application_id: str):
-        # noinspection PyArgumentList
-        # Using appindicator.Indicator() results in SIGSEGV
-        self.indicator = appindicator.Indicator.new(application_id, 'server',
-                                                    appindicator.IndicatorCategory.COMMUNICATIONS)
-        self.indicator.set_status(appindicator.IndicatorStatus.ACTIVE)
-        Notify.init(application_id)
-        self.menu = Gtk.Menu()
+        self._application_id = application_id
 
-        # INIT
+    def open(self):
+        if self._indicator:
+            raise AssertionError('Already open')
+
+        self._indicator = appindicator.Indicator.new(
+            self._application_id,
+            'server',
+            appindicator.IndicatorCategory.COMMUNICATIONS,
+        )
+        self._indicator.set_status(appindicator.IndicatorStatus.ACTIVE)
+        Notify.init(self._application_id)
+        self._menu = Gtk.Menu()
+
+        # Allow child implementation to set up its menu
         self.init_indicator()
 
         self.add_menu_item('Quit', Gtk.main_quit)
-        self.menu.show_all()
-        self.indicator.set_menu(self.menu)
+        self._menu.show_all()
+        self._indicator.set_menu(self._menu)
 
-        self.menu.connect('destroy', self.__cleanup)
+        self._menu.connect('destroy', self.__cleanup)  # This doesn't trigger when we quit ourselves
         Gtk.main()
+        self.__cleanup()
+        return self._return_code
 
     def init_indicator(self):
         raise NotImplementedError
 
     def add_menu_item(self, label: str, on_activate=None, *args):
-        item = Gtk.MenuItem()
-        item.set_label(label)
+        item = Gtk.MenuItem.new_with_label(label)
+
         if on_activate:
             item.connect('activate', lambda source, *a: on_activate(*a), *args)
-        self.menu.append(item)
-        return item
+        self._menu.append(item)
+
+    def add_separator(self):
+        self._menu.append(Gtk.SeparatorMenuItem.new())
+
+    def set_label(self, label: str):
+        self._indicator.set_label(label, label)
 
     def notify(self, title: str, message: str, icon: str = 'server'):
         self.__clear_notifications()
         n = Notify.Notification().new(title, message, icon)
         n.show()
-        self.notifications.append(n)
+        self._notifications.append(n)
+
+    def close(self, return_code: int = 0):
+        self._return_code = return_code
+        Gtk.main_quit()
 
     def __clear_notifications(self):
-        for n in self.notifications:
+        for n in self._notifications:
             n.close()
 
     def __cleanup(self):
+        self._indicator.run_dispose()
         self.__clear_notifications()
         Notify.uninit()
```

### Comparing `gnome-dns-switcher-1.2.2/gnome_dns_switcher/gnome_helpers/nmcli.py` & `gnome-dns-switcher-1.3.0/gnome_dns_switcher/gnome_helpers/nmcli.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     def set_dns_auto_mode(self, auto: bool):
         run_command('nmcli connection modify {} ipv4.ignore-auto-dns {}'
                     .format(self.uuid, 'no' if auto else 'yes'))  # invert cause its ignore
 
     def reload_connection(self):
         run_command('nmcli connection up {}'.format(self.uuid))
 
+    def reload_dns(self):
+        """
+        This is a clean way to reload DNS, but it requires root privileges
+        """
+        run_command('nmcli general reload dns-full {}'.format(self.uuid))
+
 
 def run_command(command: str, split_lines=False) -> str:
     cmd = subprocess.Popen(command, shell=True, stdout=subprocess.PIPE)
     output = cmd.stdout.read().decode('utf8').strip('\n')
     return output.split('\n') if split_lines else output
```

### Comparing `gnome-dns-switcher-1.2.2/gnome_dns_switcher/switcher/dnsswitcher.py` & `gnome-dns-switcher-1.3.0/gnome_dns_switcher/switcher/dnsswitcher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from typing import List
 
 from gnome_dns_switcher.gnome_helpers import Indicator, Connection, async_call
 # from gnome_dns_switcher.gnome_helpers import Indicator, Connection, async_call
 from .server import Server
 
 
@@ -24,32 +25,50 @@
                 self.add_menu_item(f'{conn.name} ({conn.device})')
                 for server in self.servers:
                     if server.ips and ''.join(server.ips) == ''.join(conn.get_dns()):
                         indicator_label = server.name
 
                     self.add_menu_item(' - ' + server.name, self.switch_dns, conn, server)
 
+                self.add_separator()
+
                 if conn.get_dns_auto_mode():
                     indicator_label = 'DHCP'
 
             if len(self.connections) > 1:
                 indicator_label = 'Multiple connections'
 
         if not indicator_label:
             indicator_label = '???'
 
-        self.indicator.set_label(indicator_label, indicator_label)
+        self.set_label(indicator_label)
 
-        self.add_menu_item('Debug', self.debug)
+        self.add_separator()
+        self.add_menu_item('Reload', self.reload)
+        self.add_menu_item('Restart NW Manager', self.restart_nw_manager)
+
+    def restart_nw_manager(self):
+        from gnome_dns_switcher.gnome_helpers.nmcli import run_command
+        self.set_label('Restarting...')
+
+        def reload_call():
+            run_command('systemctl restart NetworkManager')
+            self.set_label('Reloading...')
+            time.sleep(5)
 
-    def debug(self):
-        pass
+        async_call(
+            reload_call,
+            lambda r, e: self.reload()
+        )
+
+    def reload(self):
+        self.close(42)
 
     def switch_dns(self, conn: Connection, server: Server):
-        self.indicator.set_label('...', '...')
+        self.set_label('...')
 
         def set_call():
             if server.dhcp:
                 conn.set_dns([])
                 conn.set_dns_auto_mode(True)
                 conn.reload_connection()
             else:
@@ -71,9 +90,12 @@
                 "DNS Switcher",
                 "Error switching, DHCP status doesn't match. Result: " + str(result_dhcp),
                 "error"
             )
         elif not server.dhcp and result_dns_ips != ', '.join(server.ips):
             self.notify("DNS Switcher", "Error switching, result doesn't match. Result: " + result_dns_ips, 'error')
         else:
-            self.indicator.set_label(server.name, server.name)
+            label = server.name
+            if len(self.connections) > 1:
+                label = "{0}: {1}".format(conn.name, label)
+            self.set_label(label)
             self.notify("DNS Switcher", f"Switched server to: [{server.name}] {result_dns_ips}", 'network-wired')
```

### Comparing `gnome-dns-switcher-1.2.2/gnome_dns_switcher.egg-info/SOURCES.txt` & `gnome-dns-switcher-1.3.0/gnome_dns_switcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gnome-dns-switcher-1.2.2/setup.cfg` & `gnome-dns-switcher-1.3.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 [metadata]
 name = gnome-dns-switcher
-version = 1.2.2
+version = 1.3.0
 description = DNS Switcher for Ubuntu Gnome
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Anner Visser
-author_email = annervisser@gmail.com
+author_email = mail@annervisser.nl
 maintainer = Anner Visser
-maintainer_email = annervisser@gmail.com
+maintainer_email = mail@annervisser.nl
 license = GPLv3
 license_file = LICENSE
 classifiers = 
 	Intended Audience :: Information Technology
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python :: 3
 	Topic :: Utilities
 keywords = gnome, ubuntu, dns, appindicator
 project_urls = 
 	Source=https://github.com/annervisser/gnome-appindicator-dns-switcher/
-	Tracker=https://github.com/annervisser/gnome-appindicator-dns-switcher/issues
+	Issues=https://github.com/annervisser/gnome-appindicator-dns-switcher/issues
 
 [options]
 packages = find:
 install_requires = 
 	pyyaml>=5
-extra_requires = 
 	PyGObject>=3.36.0
 	pycairo>=1.16.0
 	six>=1.9.0,<2
 python_requires = >=3.6
 
 [options.entry_points]
 console_scripts =
```

