# Comparing `tmp/hddfancontrol-1.5.0.tar.gz` & `tmp/hddfancontrol-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hddfancontrol-1.5.0.tar", last modified: Sun Nov 14 14:28:43 2021, max compression
+gzip compressed data, was "hddfancontrol-1.5.1.tar", last modified: Sun Jun 25 13:28:22 2023, max compression
```

## Comparing `hddfancontrol-1.5.0.tar` & `hddfancontrol-1.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2021-11-14 14:28:43.234729 hddfancontrol-1.5.0/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    35147 2017-08-27 13:09:56.000000 hddfancontrol-1.5.0/LICENSE
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       43 2014-11-30 01:23:29.000000 hddfancontrol-1.5.0/MANIFEST.in
--rw-r--r--   0 maxime    (1000) maxime    (1000)    12093 2021-11-14 14:28:43.234729 hddfancontrol-1.5.0/PKG-INFO
--rw-r--r--   0 maxime    (1000) maxime    (1000)     9596 2021-11-14 14:25:07.000000 hddfancontrol-1.5.0/README.md
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2021-11-14 14:28:43.234729 hddfancontrol-1.5.0/hddfancontrol/
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)    52287 2021-11-14 14:25:36.000000 hddfancontrol-1.5.0/hddfancontrol/__init__.py
--rwxrwxr-x   0 maxime    (1000) maxime    (1000)      143 2021-03-01 22:46:44.000000 hddfancontrol-1.5.0/hddfancontrol/__main__.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)      273 2021-09-26 21:27:27.000000 hddfancontrol-1.5.0/hddfancontrol/bin_dep.py
--rw-r--r--   0 maxime    (1000) maxime    (1000)     1071 2021-09-26 21:27:27.000000 hddfancontrol-1.5.0/hddfancontrol/colored_logging.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2021-11-14 14:28:43.234729 hddfancontrol-1.5.0/hddfancontrol.egg-info/
--rw-rw-r--   0 maxime    (1000) maxime    (1000)    12093 2021-11-14 14:28:43.000000 hddfancontrol-1.5.0/hddfancontrol.egg-info/PKG-INFO
--rw-rw-r--   0 maxime    (1000) maxime    (1000)      407 2021-11-14 14:28:43.000000 hddfancontrol-1.5.0/hddfancontrol.egg-info/SOURCES.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2021-11-14 14:28:43.000000 hddfancontrol-1.5.0/hddfancontrol.egg-info/dependency_links.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       57 2021-11-14 14:28:43.000000 hddfancontrol-1.5.0/hddfancontrol.egg-info/entry_points.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       21 2021-11-14 14:28:43.000000 hddfancontrol-1.5.0/hddfancontrol.egg-info/requires.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       14 2021-11-14 14:28:43.000000 hddfancontrol-1.5.0/hddfancontrol.egg-info/top_level.txt
--rw-rw-r--   0 maxime    (1000) maxime    (1000)       21 2017-01-13 10:46:07.000000 hddfancontrol-1.5.0/requirements.txt
--rw-r--r--   0 maxime    (1000) maxime    (1000)       38 2021-11-14 14:28:43.234729 hddfancontrol-1.5.0/setup.cfg
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)     2169 2021-03-01 22:50:53.000000 hddfancontrol-1.5.0/setup.py
-drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2021-11-14 14:28:43.234729 hddfancontrol-1.5.0/tests/
--rwxr-xr-x   0 maxime    (1000) maxime    (1000)    39072 2021-11-14 14:25:07.000000 hddfancontrol-1.5.0/tests/__init__.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-25 13:28:22.289154 hddfancontrol-1.5.1/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    35147 2017-08-27 13:09:56.000000 hddfancontrol-1.5.1/LICENSE
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       43 2014-11-30 01:23:29.000000 hddfancontrol-1.5.1/MANIFEST.in
+-rw-r--r--   0 maxime    (1000) maxime    (1000)    11021 2023-06-25 13:28:22.289154 hddfancontrol-1.5.1/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     9714 2023-06-24 21:08:41.000000 hddfancontrol-1.5.1/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-25 13:28:22.289154 hddfancontrol-1.5.1/hddfancontrol/
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)    54500 2023-06-25 13:27:57.000000 hddfancontrol-1.5.1/hddfancontrol/__init__.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)      143 2021-03-01 22:46:44.000000 hddfancontrol-1.5.1/hddfancontrol/__main__.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      271 2022-04-27 19:11:03.000000 hddfancontrol-1.5.1/hddfancontrol/bin_dep.py
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     1067 2022-04-27 19:11:03.000000 hddfancontrol-1.5.1/hddfancontrol/colored_logging.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-25 13:28:22.289154 hddfancontrol-1.5.1/hddfancontrol.egg-info/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    11021 2023-06-25 13:28:22.000000 hddfancontrol-1.5.1/hddfancontrol.egg-info/PKG-INFO
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)      407 2023-06-25 13:28:22.000000 hddfancontrol-1.5.1/hddfancontrol.egg-info/SOURCES.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)        1 2023-06-25 13:28:22.000000 hddfancontrol-1.5.1/hddfancontrol.egg-info/dependency_links.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       56 2023-06-25 13:28:22.000000 hddfancontrol-1.5.1/hddfancontrol.egg-info/entry_points.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       21 2023-06-25 13:28:22.000000 hddfancontrol-1.5.1/hddfancontrol.egg-info/requires.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       14 2023-06-25 13:28:22.000000 hddfancontrol-1.5.1/hddfancontrol.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       21 2017-01-13 10:46:07.000000 hddfancontrol-1.5.1/requirements.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       38 2023-06-25 13:28:22.289154 hddfancontrol-1.5.1/setup.cfg
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)     2220 2023-06-24 21:08:41.000000 hddfancontrol-1.5.1/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-06-25 13:28:22.289154 hddfancontrol-1.5.1/tests/
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)    39138 2023-06-24 21:08:41.000000 hddfancontrol-1.5.1/tests/__init__.py
```

### Comparing `hddfancontrol-1.5.0/LICENSE` & `hddfancontrol-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hddfancontrol-1.5.0/PKG-INFO` & `hddfancontrol-1.5.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,182 +1,182 @@
 Metadata-Version: 2.1
 Name: hddfancontrol
-Version: 1.5.0
+Version: 1.5.1
 Summary: Control system fan speed by monitoring hard drive temperature
 Home-page: https://github.com/desbma/hddfancontrol
+Download-URL: https://github.com/desbma/hddfancontrol/archive/1.5.1.tar.gz
 Author: desbma
-License: UNKNOWN
-Download-URL: https://github.com/desbma/hddfancontrol/archive/1.5.0.tar.gz
-Description: # HDD Fan control
-        
-        [![PyPI version](https://img.shields.io/pypi/v/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
-        [![AUR version](https://img.shields.io/aur/version/hddfancontrol.svg?style=flat)](https://aur.archlinux.org/packages/hddfancontrol/)
-        [![Tests status](https://github.com/desbma/hddfancontrol/actions/workflows/ci.yml/badge.svg)](https://github.com/desbma/hddfancontrol/actions/)
-        [![Coverage](https://img.shields.io/coveralls/desbma/hddfancontrol/master.svg?style=flat)](https://coveralls.io/github/desbma/hddfancontrol?branch=master)
-        [![Lines of code](https://tokei.rs/b1/github/desbma/hddfancontrol)](https://github.com/desbma/hddfancontrol)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
-        [![License](https://img.shields.io/github/license/desbma/hddfancontrol.svg?style=flat)](https://github.com/desbma/hddfancontrol/blob/master/LICENSE)
-        
-        HDD Fan control is a command line tool to dynamically control fan speed according to hard drive temperature on Linux.
-        
-        This has 3 benefits:
-        
-        - it allows maintaining your hard drives in the ideal temperature range to have maximum longevity and avoid overheating
-        
-        Because fans will slow down or stop when not needed:
-        
-        - it minimizes noise generated by the fans
-        - it also minimizes power consumption at the same time
-        
-        ## When is this useful?
-        
-        HDD Fan control is useful when you have one or several hard drives with one or several fans close to them, and do not want to let the motherboard control the fan speed, because it does so either statically, or using a temperature sensor unrelated to the real drive temperature (either on the CPU or on some other place on the motherboard).
-        
-        The ideal use case is for a NAS with several hard drives, a low power CPU (ie. ARM or Intel Atom) with passive cooling (no fans), and a chassis with fans close to the hard drive. It that case the CPU will generate less heat than the hard drives and it makes sense to control fan speed according to the main heat source.
-        
-        ## Features
-        
-        - Can run in daemon mode
-        - Can control several fans and/or several drives with a single invocation
-        - Supports 6 different ways of querying temperature:
-          - `hddtemp` invocation
-          - `hddtemp` daemon query
-          - `hdparm` invocation
-          - `smartctl` invocation (SCT)
-          - `smartctl` invocation (SMART attributes)
-          - `drivetemp` native kernel hwmon
-        - Can automatically spin down drives after a customizable period of inactivity
-        - Can adapt to different fan characteristics
-        - Can be set to stop fans or run them at full speed at customizable temperatures
-        - Can be configured to never set the fans below a certain speed (useful if the fans controlled by HDD Fan control are the only ones available in the chassis)
-        - Can also optionally monitor CPU temperature, and control fan speed accordingly
-        
-        ## Prerequisites
-        
-        - A Linux distribution
-        - A least one SATA hard drive, that supports:
-          - Temperature querying
-          - Power state querying
-        - A motherboard which:
-          - exposes to the OS a PWM to control fan speed
-          - exposes to the OS a sensor to query fan speed
-        
-        Most motherboards and SATA drives fit these requirements.
-        
-        ## Installation
-        
-        HDD Fan control requires [Python](https://www.python.org/downloads/) >= 3.6.
-        
-        ### Distribution packages
-        
-        Some Linux distributions have a hddfancontrol package available in their repository:
-        
-        - Arch Linux (AUR): [hddfancontrol](https://aur.archlinux.org/packages/hddfancontrol/)
-        - Fedora: [hddfancontrol](https://apps.fedoraproject.org/packages/hddfancontrol) (thanks to [TC01](https://github.com/TC01))
-        
-        ### From PyPI (with PIP)
-        
-        1. If you don't already have it, [install pip](https://pip.pypa.io/en/stable/installing/) for Python 3
-        2. Install HDD Fan control: `pip3 install hddfancontrol`
-        3. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php).
-           On Ubuntu and other Debian derivatives: `sudo apt-get install hdparm hddtemp`.
-        
-        ### From source
-        
-        1. If you don't already have it, [install setuptools](https://pypi.python.org/pypi/setuptools#installation-instructions) for Python 3
-        2. Clone this repository: `git clone https://github.com/desbma/hddfancontrol`
-        3. Install HDD Fan control: `python3 setup.py install`
-        4. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php).
-           On Ubuntu and other Debian derivatives: `sudo apt-get install hdparm hddtemp`.
-        
-        To query fan characteristics, you may also need pwmconfig. On Ubuntu and other Debian derivatives, it is part of the fancontrol package, that you can install with `sudo apt-get install fancontrol`. HDD fancontrol and fancontrol are unrelated. The fancontrol daemon is **not** needed for HDD fan control to operate. If you use both fancontrol and HDD fancontrol, be careful not to make them control the same fans.
-        
-        ## Configuration
-        
-        ### A word of caution
-        
-        The default parameters will run fans at 100% speed at temperatures > 50°C, and run them a 20% speed if < 30°C, which corresponds to the usual recommended drive operating temperature. If you are sure that there are no other components in your system that generate significant heat, if you have other fans to cool down your system, or if you have a case optimized for passive cooling, you can set minimum speed to 0%, which will stop the fans if temperature is below the minimum threshold.
-        
-        **Be aware that a misconfiguration of this tool can lead to a failure to cool down your system properly which can damage components or reduce their lifetime.**
-        
-        Before using HDD Fan control unmonitored for long period of time, I recommend keeping a minimum fan speed for security, and checking that the temperature of your system stays in reasonable range as expected.
-        
-        ### Fan configuration
-        
-        To get the value for the `--pwm`, `--pwm-start-value` and `--pwm-stop-value` parameters, you can either:
-        
-        - Use the `-t` or `--test` parameter, which will run some tests and detect the values at which the fans start and stop. However you need to have previously identified the PWM file (the `--pwm` parameter)
-        - use the [pwmconfig tool](http://www.lm-sensors.org/wiki/man/pwmconfig).
-        
-        ### Drive auto spin down
-        
-        SATA drives can be configured to automatically spin down after a certain period of inactivity, which saves power. If your drives are configured to do so, you may notice that they do not spin down when HDD Fan control is running.
-        This is due to the fact that HDD Fan control will query temperature at fixed interval, which the drive will consider an activity and reset the spin down timeout.
-        To fix that, you can either:
-        
-        - Use a value for the `-i`/`--interval` parameter higher than your SATA spin down time (not recommended unless your spin down time is very low, ie < 2 min). In that case you do not need to use hddfancontrol's `--spin-down-time` switch, because the builtin SATA drive timeout (that you can set for example with [`hdparm -S XXX` command](https://linux.die.net/man/8/hdparm)) should take effect.
-        - Use the `--spin-down-time` parameter that will monitor drive activity and spin it down if inactive, independantly of the SATA feature (recommended)
-        
-        **Keep in mind that spinning down and up a drive repeatedly wears it prematurly, so unless you are in a power constrained environement (ie. laptop), do not set the spin down time too low.**
-        
-        Reading temperature while a drive is in low power state will make it spin up, so HDD Fan control will stop querying temperature in that case, and wait for the drive (which will be cooling down in low power state anyway) to spin up.
-        
-        Some HGST (previously Hitachi) drives support a special way of querying temperature that does not spin up drives, which HDD Fan control will detect and use, however it still prevents them from spinning down, so the above instructions still apply.
-        
-        ## Command line usage
-        
-        Run `hddfancontrol -h` to get full command line reference.
-        
-        As an example, the command line below will instruct HDD Fan control to:
-        
-        - monitor temperature of drives `/dev/sda` and `/dev/sdb`
-        - control fan speed using PWM 2 and 3 in `/sys/class/hwmon/hwmon1/device/`
-        - start both fans using PWM value 200
-        - consider the fans will stop with PWM value 75
-        - never run the fans below 10% of their maximum speed
-        - check temperature at least every minute
-        - automatically spin down drives if they are inactive for 2 hours (7200 seconds)
-        - run in daemon mode
-        - log what is going on to `/var/log/hddfancontrol.log`
-        
-        `hddfancontrol -d /dev/sda /dev/sdb -p /sys/class/hwmon/hwmon1/device/pwm2 /sys/class/hwmon/hwmon1/device/pwm3 --pwm-start-value 200 200 --pwm-stop-value 75 75 --min-fan-speed-prct 10 -i 60 --spin-down-time 7200 -b -l /var/log/hddfancontrol.log`
-        
-        ## Systemd service
-        
-        A systemd service file is provided to control the daemon easily.
-        If you installed hddfancontrol from a distribution package, you likely already have it installed, otherwise you can install it from the sources of this repository with:
-        
-        ```
-        sudo cp ./systemd/hddfancontrol.service /etc/systemd/system/
-        sudo mkdir -p /etc/conf.d
-        sudo cp ./systemd/hddfancontrol.conf /etc/conf.d/hddfancontrol
-        ```
-        
-        Then you need to edit the `HDDFANCONTROL_ARGS` variable in `/etc/conf.d/hddfancontrol` to set the parameters (drives, temperature range...).
-        
-        You can then start the daemon with `sudo systemctl start hddfancontrol`, see its status with `sudo systemctl status hddfancontrol` and enable automatic startup at boot time with `sudo systemctl enable hddfancontrol`.
-        
-        ## License
-        
-        [GPLv3](https://www.gnu.org/licenses/gpl-3.0-standalone.html)
-        
 Keywords: hdd,drive,temperature,fan,control,speed
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HDD Fan control
+
+[![PyPI version](https://img.shields.io/pypi/v/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
+[![AUR version](https://img.shields.io/aur/version/hddfancontrol.svg?style=flat)](https://aur.archlinux.org/packages/hddfancontrol/)
+[![Tests status](https://github.com/desbma/hddfancontrol/actions/workflows/ci.yml/badge.svg)](https://github.com/desbma/hddfancontrol/actions/)
+[![Coverage](https://img.shields.io/coveralls/desbma/hddfancontrol/master.svg?style=flat)](https://coveralls.io/github/desbma/hddfancontrol?branch=master)
+[![Lines of code](https://tokei.rs/b1/github/desbma/hddfancontrol)](https://github.com/desbma/hddfancontrol)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
+[![License](https://img.shields.io/github/license/desbma/hddfancontrol.svg?style=flat)](https://github.com/desbma/hddfancontrol/blob/master/LICENSE)
+
+HDD Fan control is a command line tool to dynamically control fan speed according to hard drive temperature on Linux.
+
+This has 3 benefits:
+
+- it allows maintaining your hard drives in the ideal temperature range to have maximum longevity and avoid overheating
+
+Because fans will slow down or stop when not needed:
+
+- it minimizes noise generated by the fans
+- it also minimizes power consumption at the same time
+
+## When is this useful?
+
+HDD Fan control is useful when you have one or several hard drives with one or several fans close to them, and do not want to let the motherboard control the fan speed, because it does so either statically, or using a temperature sensor unrelated to the real drive temperature (either on the CPU or on some other place on the motherboard).
+
+The ideal use case is for a NAS with several hard drives, a low power CPU (ie. ARM or Intel Atom) with passive cooling (no fans), and a chassis with fans close to the hard drive. It that case the CPU will generate less heat than the hard drives and it makes sense to control fan speed according to the main heat source.
+
+## Features
+
+- Can run in daemon mode
+- Can control several fans and/or several drives with a single invocation
+- Supports 6 different ways of querying temperature:
+  - `hddtemp` invocation
+  - `hddtemp` daemon query
+  - `hdparm` invocation
+  - `smartctl` invocation (SCT)
+  - `smartctl` invocation (SMART attributes)
+  - `drivetemp` native kernel hwmon
+- Can automatically spin down drives after a customizable period of inactivity
+- Can adapt to different fan characteristics
+- Can be set to stop fans or run them at full speed at customizable temperatures
+- Can be configured to never set the fans below a certain speed (useful if the fans controlled by HDD Fan control are the only ones available in the chassis)
+- Can also optionally monitor CPU temperature, and control fan speed accordingly
+
+## Prerequisites
+
+- A Linux distribution
+- A least one SATA hard drive, that supports:
+  - Temperature querying
+  - Power state querying
+- A motherboard which:
+  - exposes to the OS a PWM to control fan speed
+  - exposes to the OS a sensor to query fan speed
+
+Most motherboards and SATA drives fit these requirements.
+
+## Installation
+
+HDD Fan control requires [Python](https://www.python.org/downloads/) >= 3.6.
+
+### Distribution packages
+
+Some Linux distributions have a hddfancontrol package available in their repository:
+
+- Arch Linux (AUR): [hddfancontrol](https://aur.archlinux.org/packages/hddfancontrol/)
+- Fedora: [hddfancontrol](https://apps.fedoraproject.org/packages/hddfancontrol) (thanks to [TC01](https://github.com/TC01))
+
+### From PyPI (with PIP)
+
+1. If you don't already have it, [install pip](https://pip.pypa.io/en/stable/installing/) for Python 3
+2. Install HDD Fan control: `pip3 install hddfancontrol`
+3. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php) or [smartctl](https://www.smartmontools.org/).
+   On recent Ubuntu and other Debian derivatives: `sudo apt-get install hdparm smartmontools`.
+
+### From source
+
+1. If you don't already have it, [install setuptools](https://pypi.python.org/pypi/setuptools#installation-instructions) for Python 3
+2. Clone this repository: `git clone https://github.com/desbma/hddfancontrol`
+3. Install HDD Fan control: `python3 setup.py install`
+4. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php) or [smartctl](https://www.smartmontools.org/).
+   On recent Ubuntu and other Debian derivatives: `sudo apt-get install hdparm smartmontools`.
+
+To query fan characteristics, you may also need pwmconfig. On Ubuntu and other Debian derivatives, it is part of the fancontrol package, that you can install with `sudo apt-get install fancontrol`. HDD fancontrol and fancontrol are unrelated. The fancontrol daemon is **not** needed for HDD fan control to operate. If you use both fancontrol and HDD fancontrol, be careful not to make them control the same fans.
+
+## Configuration
+
+### A word of caution
+
+The default parameters will run fans at 100% speed at temperatures > 50°C, and run them a 20% speed if < 30°C, which corresponds to the usual recommended drive operating temperature. If you are sure that there are no other components in your system that generate significant heat, if you have other fans to cool down your system, or if you have a case optimized for passive cooling, you can set minimum speed to 0%, which will stop the fans if temperature is below the minimum threshold.
+
+**Be aware that a misconfiguration of this tool can lead to a failure to cool down your system properly which can damage components or reduce their lifetime.**
+
+Before using HDD Fan control unmonitored for long period of time, I recommend keeping a minimum fan speed for security, and checking that the temperature of your system stays in reasonable range as expected.
+
+### Fan configuration
+
+To get the value for the `--pwm`, `--pwm-start-value` and `--pwm-stop-value` parameters, you can either:
+
+- Use the `-t` or `--test` parameter, which will run some tests and detect the values at which the fans start and stop. However you need to have previously identified the PWM file (the `--pwm` parameter)
+- use the [pwmconfig tool](http://www.lm-sensors.org/wiki/man/pwmconfig).
+
+### Drive auto spin down
+
+SATA drives can be configured to automatically spin down after a certain period of inactivity, which saves power. If your drives are configured to do so, you may notice that they do not spin down when HDD Fan control is running.
+This is due to the fact that HDD Fan control will query temperature at fixed interval, which the drive will consider an activity and reset the spin down timeout.
+To fix that, you can either:
+
+- Use a value for the `-i`/`--interval` parameter higher than your SATA spin down time (not recommended unless your spin down time is very low, ie < 2 min). In that case you do not need to use hddfancontrol's `--spin-down-time` switch, because the builtin SATA drive timeout (that you can set for example with [`hdparm -S XXX` command](https://linux.die.net/man/8/hdparm)) should take effect.
+- Use the `--spin-down-time` parameter that will monitor drive activity and spin it down if inactive, independantly of the SATA feature (recommended)
+
+**Keep in mind that spinning down and up a drive repeatedly wears it prematurly, so unless you are in a power constrained environement (ie. laptop), do not set the spin down time too low.**
+
+Reading temperature while a drive is in low power state will make it spin up, so HDD Fan control will stop querying temperature in that case, and wait for the drive (which will be cooling down in low power state anyway) to spin up.
+
+Some HGST (previously Hitachi) drives support a special way of querying temperature that does not spin up drives, which HDD Fan control will detect and use, however it still prevents them from spinning down, so the above instructions still apply.
+
+## Command line usage
+
+Run `hddfancontrol -h` to get full command line reference.
+
+As an example, the command line below will instruct HDD Fan control to:
+
+- monitor temperature of drives `/dev/sda` and `/dev/sdb`
+- control fan speed using PWM 2 and 3 in `/sys/class/hwmon/hwmon1/device/`
+- start both fans using PWM value 200
+- consider the fans will stop with PWM value 75
+- never run the fans below 10% of their maximum speed
+- check temperature at least every minute
+- automatically spin down drives if they are inactive for 2 hours (7200 seconds)
+- run in daemon mode
+- log what is going on to `/var/log/hddfancontrol.log`
+
+`hddfancontrol -d /dev/sda /dev/sdb -p /sys/class/hwmon/hwmon1/device/pwm2 /sys/class/hwmon/hwmon1/device/pwm3 --pwm-start-value 200 200 --pwm-stop-value 75 75 --min-fan-speed-prct 10 -i 60 --spin-down-time 7200 -b -l /var/log/hddfancontrol.log`
+
+## Systemd service
+
+A systemd service file is provided to control the daemon easily.
+If you installed hddfancontrol from a distribution package, you likely already have it installed, otherwise you can install it from the sources of this repository with:
+
+```
+sudo cp ./systemd/hddfancontrol.service /etc/systemd/system/
+sudo mkdir -p /etc/conf.d
+sudo cp ./systemd/hddfancontrol.conf /etc/conf.d/hddfancontrol
+```
+
+Then you need to edit the `HDDFANCONTROL_ARGS` variable in `/etc/conf.d/hddfancontrol` to set the parameters (drives, temperature range...).
+
+You can then start the daemon with `sudo systemctl start hddfancontrol`, see its status with `sudo systemctl status hddfancontrol` and enable automatic startup at boot time with `sudo systemctl enable hddfancontrol`.
+
+## License
+
+[GPLv3](https://www.gnu.org/licenses/gpl-3.0-standalone.html)
```

### Comparing `hddfancontrol-1.5.0/README.md` & `hddfancontrol-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,24 +65,24 @@
 - Arch Linux (AUR): [hddfancontrol](https://aur.archlinux.org/packages/hddfancontrol/)
 - Fedora: [hddfancontrol](https://apps.fedoraproject.org/packages/hddfancontrol) (thanks to [TC01](https://github.com/TC01))
 
 ### From PyPI (with PIP)
 
 1. If you don't already have it, [install pip](https://pip.pypa.io/en/stable/installing/) for Python 3
 2. Install HDD Fan control: `pip3 install hddfancontrol`
-3. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php).
-   On Ubuntu and other Debian derivatives: `sudo apt-get install hdparm hddtemp`.
+3. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php) or [smartctl](https://www.smartmontools.org/).
+   On recent Ubuntu and other Debian derivatives: `sudo apt-get install hdparm smartmontools`.
 
 ### From source
 
 1. If you don't already have it, [install setuptools](https://pypi.python.org/pypi/setuptools#installation-instructions) for Python 3
 2. Clone this repository: `git clone https://github.com/desbma/hddfancontrol`
 3. Install HDD Fan control: `python3 setup.py install`
-4. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php).
-   On Ubuntu and other Debian derivatives: `sudo apt-get install hdparm hddtemp`.
+4. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php) or [smartctl](https://www.smartmontools.org/).
+   On recent Ubuntu and other Debian derivatives: `sudo apt-get install hdparm smartmontools`.
 
 To query fan characteristics, you may also need pwmconfig. On Ubuntu and other Debian derivatives, it is part of the fancontrol package, that you can install with `sudo apt-get install fancontrol`. HDD fancontrol and fancontrol are unrelated. The fancontrol daemon is **not** needed for HDD fan control to operate. If you use both fancontrol and HDD fancontrol, be careful not to make them control the same fans.
 
 ## Configuration
 
 ### A word of caution
```

### Comparing `hddfancontrol-1.5.0/hddfancontrol/__init__.py` & `hddfancontrol-1.5.1/hddfancontrol/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 """ Dynamically control fan speed according to hard drive temperature. """
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 __author__ = "desbma"
 __license__ = "GPLv3"
 
 import abc
 import argparse
 import collections
 import contextlib
@@ -39,80 +39,80 @@
 
 
 exit_evt = threading.Event()
 
 
 class DriveAsleepError(Exception):
 
-    """ Exception raised when getTemperature fails because drive is asleep. """
+    """Exception raised when getTemperature fails because drive is asleep."""
 
     pass
 
 
 class HddtempDaemonQueryFailed(Exception):
 
-    """ Exception raised when hddtemp daemon fails to return temperature for a drive. """
+    """Exception raised when hddtemp daemon fails to return temperature for a drive."""
 
     pass
 
 
 class LoggingSysLogHandler(logging.Handler):
 
-    """ Class similar in goal to logging.handlers.SysLogHandler, but uses the syslog call instead of socket. """
+    """Class similar in goal to logging.handlers.SysLogHandler, but uses the syslog call instead of socket."""
 
     def __init__(self, facility, options=syslog.LOG_PID):
         syslog.openlog(logoption=options, facility=facility)
         super().__init__()
 
     def emit(self, record):
-        """ See logging.Handler.emit. """
+        """See logging.Handler.emit."""
         msg = self.format(record)
         h = logging.handlers.SysLogHandler
         level = h.priority_names[h.priority_map[record.levelname]]
         syslog.syslog(level, msg)
 
     def close(self):
-        """ See logging.Handler.close. """
+        """See logging.Handler.close."""
         syslog.closelog()
         super().close()
 
 
 class HotDevice:
 
-    """ Base class for devices generating heat. """
+    """Base class for devices generating heat."""
 
     @abc.abstractmethod
     def getTemperature(self) -> float:
-        """ Get device temperature as int or float. """
+        """Get device temperature as int or float."""
         pass
 
     @abc.abstractmethod
     def getTemperatureRange(self) -> Tuple[float, float]:
         """
         Get min/max target temperatures.
 
         Fans should be at minimum speed below min, and blow at full speed above max.
         """
         pass
 
 
 class Drive(HotDevice):
 
-    """ Drive represented by a device file like /dev/sdX. """
+    """Drive represented by a device file like /dev/sdX."""
 
     DriveState = enum.Enum("DriveState", ("UNKNOWN", "ACTIVE_IDLE", "STANDBY", "SLEEPING"))
 
     HDPARM_GET_TEMP_HITACHI_REGEX = re.compile(r"drive temperature \(celsius\) is:\s*([0-9]*)")
     HDPARM_GET_TEMP_HITACHI_ERROR_REGEX = re.compile("^SG_IO: .* sense data", re.MULTILINE)
     HDPARM_GET_MODEL_REGEX = re.compile(r"Model Number:\s*(.*)")
     HDDTEMP_SLEEPING_SUFFIX = ": drive is sleeping\n"
 
     class TempProbingMethod(enum.Enum):
 
-        """ Method used to query drive temperature, depending on what the drive/system support. """
+        """Method used to query drive temperature, depending on what the drive/system support."""
 
         HDDTEMP_INVOCATION = enum.auto()
         HDDTEMP_DAEMON = enum.auto()
         HDPARM_INVOCATION = enum.auto()
         SMARTCTL_ATTRIB_INVOCATION = enum.auto()
         SMARTCTL_SCT_INVOCATION = enum.auto()
         DRIVETEMP = enum.auto()
@@ -169,31 +169,31 @@
         if self.__class__.isPartition(device_filepath):
             self.logger.warning(
                 f"{device_filepath!r} is a partition, "
                 f"parent device {self.device_filepath!r} will be used except for activity stats"
             )
 
     def __str__(self):
-        """ Return a pretty drive name. """
+        """Return a pretty drive name."""
         return self.pretty_name
 
     def getPrettyName(self) -> str:
-        """ Return a pretty drive name. """
+        """Return a pretty drive name."""
         # get device metadata to grab model string
         cmd = ("hdparm", "-I", self.device_filepath)
         output = subprocess.check_output(
             cmd, stdin=subprocess.DEVNULL, stderr=subprocess.DEVNULL, universal_newlines=True
         )
         model_match = self.__class__.HDPARM_GET_MODEL_REGEX.search(output)
         assert model_match is not None
         model = model_match.group(1).strip()
         return f"{os.path.basename(self.device_filepath)} {model}"
 
     def getDrivetempInputFilepath(self) -> Optional[str]:
-        """ Return sysfs drivetemp input filepath if supported, None instead. """
+        """Return sysfs drivetemp input filepath if supported, None instead."""
         try:
             sysfs_bus_dir = f"/sys/block/{os.path.basename(self.device_filepath)}"
             sysfs_bus_dir = os.path.normpath(
                 os.path.join(os.path.dirname(sysfs_bus_dir), os.readlink(sysfs_bus_dir), "..", "..")
             )
             with os.scandir(f"{sysfs_bus_dir}/hwmon") as dir_it:
                 for entry in filter(operator.methodcaller("is_dir"), dir_it):
@@ -204,15 +204,15 @@
                         return f"{hwmon_dir}/temp1_input"
         except FileNotFoundError:
             pass
         self.logger.info("Drive does not support native drivetemp temp query")
         return None
 
     def supportsHitachiTempQuery(self) -> bool:
-        """ Test if drive supports hdparm -H. """
+        """Test if drive supports hdparm -H."""
         supported = True
         cmd = ("hdparm", "-H", self.device_filepath)
         try:
             output = subprocess.check_output(
                 cmd, stdin=subprocess.DEVNULL, stderr=subprocess.STDOUT, universal_newlines=True
             )
         except subprocess.CalledProcessError:
@@ -223,15 +223,15 @@
             if self.__class__.HDPARM_GET_TEMP_HITACHI_ERROR_REGEX.search(output) is not None:
                 supported = False
         if not supported:
             self.logger.warning("Drive does not support HGST temp query")
         return supported
 
     def supportsSctTempQuery(self) -> bool:
-        """ Test if drive supports smartctl -l scttempsts. """
+        """Test if drive supports smartctl -l scttempsts."""
         supported = True
         cmd = ("smartctl", "-l", "scttempsts", self.device_filepath)
         output = subprocess.check_output(
             cmd, stdin=subprocess.DEVNULL, stderr=subprocess.DEVNULL, universal_newlines=True
         )
         try:
             temp_line = next(filter(lambda x: x.lstrip().startswith("Current Temperature: "), output.splitlines()))
@@ -241,21 +241,23 @@
         else:
             supported = True
         if not supported:
             self.logger.warning("Drive does not support SCT temp query")
         return supported
 
     def supportsProbingWhileAsleep(self) -> bool:
-        """ Return True if drive can be probed while asleep, without waking up, False instead. """
+        """Return True if drive can be probed while asleep, without waking up, False instead."""
         return self.temp_query_method in (Drive.TempProbingMethod.HDPARM_INVOCATION, Drive.TempProbingMethod.DRIVETEMP)
 
     def getState(self) -> DriveState:
-        """ Get drive power state, as a DriveState enum. """
+        """Get drive power state, as a DriveState enum."""
         states = {
             "unknown": self.__class__.DriveState.UNKNOWN,
+            "active": self.__class__.DriveState.ACTIVE_IDLE,
+            "idle": self.__class__.DriveState.ACTIVE_IDLE,
             "active/idle": self.__class__.DriveState.ACTIVE_IDLE,
             "standby": self.__class__.DriveState.STANDBY,
             "sleeping": self.__class__.DriveState.SLEEPING,
         }
         cmd = ("hdparm", "-C", self.device_filepath)
         with self.get_state_lock:
             output = subprocess.check_output(
@@ -264,23 +266,23 @@
             self.get_state_count += 1
         str_state = output.rsplit(" ", 1)[-1].strip()
         state = states[str_state]
         self.logger.debug(f"Drive state: {state.name}")
         return state
 
     def isSleeping(self) -> bool:
-        """ Return True if drive is in low power state, False otherwise. """
+        """Return True if drive is in low power state, False otherwise."""
         return self.getState() in (Drive.DriveState.STANDBY, Drive.DriveState.SLEEPING)
 
     def getTemperatureRange(self) -> Tuple[float, float]:
-        """ See HotDevice.getTemperatureRange. """
+        """See HotDevice.getTemperatureRange."""
         return self.min_temp, self.max_temp
 
     def getTemperature(self) -> float:
-        """ Get drive temperature in Celcius. """
+        """Get drive temperature in Celcius."""
         methods = {
             Drive.TempProbingMethod.HDDTEMP_INVOCATION: self.getTemperatureWithHddtempInvocation,
             Drive.TempProbingMethod.HDDTEMP_DAEMON: self.getTemperatureWithHddtempDaemon,
             Drive.TempProbingMethod.HDPARM_INVOCATION: self.getTemperatureWithHdparmInvocation,
             Drive.TempProbingMethod.SMARTCTL_ATTRIB_INVOCATION: self.getTemperatureWithSmartctlAttribInvocation,
             Drive.TempProbingMethod.SMARTCTL_SCT_INVOCATION: self.getTemperatureWithSmartctlSctInvocation,
             Drive.TempProbingMethod.DRIVETEMP: self.getTemperatureWithDrivetemp,
@@ -299,15 +301,15 @@
 
             self.probe_count += 1
 
         self.logger.debug(f"Drive temperature: {temp} °C")
         return temp
 
     def getTemperatureWithHddtempDaemon(self) -> int:
-        """ Get drive temperature in Celcius using hddtemp daemon. """
+        """Get drive temperature in Celcius using hddtemp daemon."""
         # get temp from daemon
         daemon_data = bytearray()
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as sckt:
             sckt.connect(("127.0.0.1", self.hddtemp_daemon_port))
             while True:
                 new_daemon_data = sckt.recv(4096)
                 if not new_daemon_data:
@@ -336,37 +338,37 @@
                 break
 
         if not found:
             raise RuntimeError(f"Unable to get temperature from hddtemp daemon for drive {self}")
         return temp
 
     def getTemperatureWithHddtempInvocation(self) -> int:
-        """ Get drive temperature in Celcius using a one shot hddtemp invocation. """
+        """Get drive temperature in Celcius using a one shot hddtemp invocation."""
         cmd = ("hddtemp", "-u", "C", "-n", self.device_filepath)
         cmd_env = dict(os.environ)
         cmd_env["LANG"] = "C"
         output = subprocess.check_output(
             cmd, stdin=subprocess.DEVNULL, stderr=subprocess.DEVNULL, env=cmd_env, universal_newlines=True
         )
         if output.endswith(self.__class__.HDDTEMP_SLEEPING_SUFFIX):
             raise DriveAsleepError
         return int(output.strip())
 
     def getTemperatureWithHdparmInvocation(self) -> int:
-        """ Get drive temperature in Celcius using hdparm. """
+        """Get drive temperature in Celcius using hdparm."""
         cmd = ("hdparm", "-H", self.device_filepath)
         output = subprocess.check_output(
             cmd, stdin=subprocess.DEVNULL, stderr=subprocess.DEVNULL, universal_newlines=True
         )
         temp_match = self.__class__.HDPARM_GET_TEMP_HITACHI_REGEX.search(output)
         assert temp_match is not None
         return int(temp_match.group(1))
 
     def getTemperatureWithSmartctlAttribInvocation(self) -> int:
-        """ Get drive temperature in Celcius using smartctl SMART attribute. """
+        """Get drive temperature in Celcius using smartctl SMART attribute."""
         cmd = ("smartctl", "-A", self.device_filepath)
         output = subprocess.check_output(
             cmd, stdin=subprocess.DEVNULL, stderr=subprocess.DEVNULL, universal_newlines=True
         )
         output_lines = output.splitlines()
 
         prefixes = collections.OrderedDict(
@@ -389,36 +391,36 @@
             except StopIteration:
                 continue
             break
 
         return int(temp_line.split()[token_index])
 
     def getTemperatureWithSmartctlSctInvocation(self) -> int:
-        """ Get drive temperature in Celcius using smartctl SCT reading. """
+        """Get drive temperature in Celcius using smartctl SCT reading."""
         cmd = ("smartctl", "-l", "scttempsts", self.device_filepath)
         output = subprocess.check_output(
             cmd, stdin=subprocess.DEVNULL, stderr=subprocess.DEVNULL, universal_newlines=True
         )
         temp_line = next(filter(lambda x: x.lstrip().startswith("Current Temperature: "), output.splitlines()))
         return int(temp_line.split()[2])
 
     def getTemperatureWithDrivetemp(self) -> int:
-        """ Get drive temperature in Celcius using drivetemp sysfs. """
+        """Get drive temperature in Celcius using drivetemp sysfs."""
         assert self.drivetemp_input_filepath is not None
         with open(self.drivetemp_input_filepath, "rt") as f:
             return int(f.read().rstrip()) // 1000
 
     def spinDown(self) -> None:
-        """ Spin down a drive, effectively setting it to DriveState.STANDBY state. """
+        """Spin down a drive, effectively setting it to DriveState.STANDBY state."""
         self.logger.info(f"Spinning down drive {self}")
         cmd = ("hdparm", "-y", self.device_filepath)
         subprocess.check_call(cmd, stdin=subprocess.DEVNULL, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
     def getActivityStats(self) -> Tuple[int, ...]:
-        """ Return drive stats as in /proc/diskstats, as a tuple of integer. """
+        """Return drive stats as in /proc/diskstats, as a tuple of integer."""
         with open(self.stat_filepath, "rt") as stat_file:
             stat_data = stat_file.read()
         stats = tuple(map(int, filter(None, map(str.strip, stat_data.strip().split(" ")))))
         if not stats:
             raise RuntimeError(f"Unable to get stats for drive {self}")
         return stats
 
@@ -492,68 +494,68 @@
         # )
 
         return not (
             (current[0] - prev[0] == expected_read_io_delta) and (current[2] - prev[2] == expected_read_sectors_delta)
         )
 
     def getTempProbeLock(self) -> threading.Lock:
-        """ Return the mutex to protect the temp probe count. """
+        """Return the mutex to protect the temp probe count."""
         return self.probe_lock
 
     def getTempProbeCount(self) -> int:
         """
         Return current temp probe count.
 
         The caller must hold the lock returned by getTempProbeLock.
         """
         return self.probe_count
 
     def getStateProbeLock(self) -> threading.Lock:
-        """ Return the mutex to protect the state probe count. """
+        """Return the mutex to protect the state probe count."""
         return self.get_state_lock
 
     def getStateProbeCount(self) -> int:
         """
         Return current state probe count.
 
         The caller must hold the lock returned by getStateProbeLock.
         """
         return self.get_state_count
 
     @staticmethod
     def normalizeDrivePath(path: str) -> str:
-        """ Normalize filepath by following symbolic links, and making it absolute. """
+        """Normalize filepath by following symbolic links, and making it absolute."""
         if os.path.islink(path):
             r = os.readlink(path)
             if not os.path.isabs(r):
                 r = os.path.join(os.path.dirname(path), r)
         else:
             r = path
         return os.path.abspath(r)
 
     @staticmethod
     def isPartition(device_filepath: str) -> bool:
-        """ Return True if device is a partition, False otherwise. """
+        """Return True if device is a partition, False otherwise."""
         # https://github.com/python/mypy/issues/4177
         assert __class__.normalizeDrivePath(device_filepath) == device_filepath  # type: ignore
         return os.path.isfile(f"/sys/class/block/{os.path.basename(device_filepath)}/partition")
 
     @staticmethod
     def getParentDevice(device_filepath: str) -> str:
-        """ Get parent device from a partition device filepath. """
+        """Get parent device from a partition device filepath."""
         # https://github.com/python/mypy/issues/4177
         assert __class__.normalizeDrivePath(device_filepath) == device_filepath  # type: ignore
         sysfs_dev = os.readlink(f"/sys/class/block/{os.path.basename(device_filepath)}")
         parent_dev = os.path.basename(os.path.dirname(sysfs_dev))
         return f"/dev/{parent_dev}"
 
 
 class CPU(HotDevice):
 
-    """ CPU device with a sysfs temp sensor. """
+    """CPU device with a sysfs temp sensor."""
 
     SENSOR_DIGITS_REGEX = re.compile("temp([0-9])*_input$")
     DEFAULT_MIN_TEMP = 30
 
     def __init__(self, cpu_sensor: str, temp_range: Tuple[float, float]):
         self.cpu_sensor_input_filepath = cpu_sensor
         self.logger = logging.getLogger(self.__class__.__name__)
@@ -561,26 +563,26 @@
         if self.min_temp is None:
             self.min_temp = self.__class__.DEFAULT_MIN_TEMP
         if self.max_temp is None:
             self.max_temp = self.getDefaultMaxTemp()
         assert 0 < self.min_temp < self.max_temp
 
     def getSysfsTempValue(self, filepath: str) -> float:
-        """ Get temperature value from a sysfs file as a float. """
+        """Get temperature value from a sysfs file as a float."""
         with open(filepath, "rt") as f:
             return int(f.read()) / 1000
 
     def getTemperature(self) -> float:
-        """ See HotDevice.getTemperature. """
+        """See HotDevice.getTemperature."""
         r = self.getSysfsTempValue(self.cpu_sensor_input_filepath)
         self.logger.debug(f"CPU temperature: {r} °C")
         return r
 
     def getDefaultMaxTemp(self) -> float:
-        """ Compute maximum temperature. """
+        """Compute maximum temperature."""
         # first compute filepath for max and crit sysfs files
         sensor_match = self.__class__.SENSOR_DIGITS_REGEX.search(self.cpu_sensor_input_filepath)
         assert sensor_match is not None
         sensor_num = int(sensor_match.group(1))
         max_filepath = os.path.join(os.path.dirname(self.cpu_sensor_input_filepath), f"temp{sensor_num}_max")
         crit_filepath = os.path.join(os.path.dirname(self.cpu_sensor_input_filepath), f"temp{sensor_num}_crit")
 
@@ -597,32 +599,32 @@
         max_temp, crit_temp = min(max_temp, crit_temp), max(max_temp, crit_temp)
 
         # keep a safety margin
         r = max_temp - (crit_temp - max_temp)
         return r
 
     def getTemperatureRange(self) -> Tuple[float, float]:
-        """ See HotDevice.getTemperatureRange. """
+        """See HotDevice.getTemperatureRange."""
         return self.min_temp, self.max_temp
 
 
 class DriveSpinDownThread(threading.Thread):
 
-    """ Thread responsible for spinning down a drive when it is not active for a certain amount of time. """
+    """Thread responsible for spinning down a drive when it is not active for a certain amount of time."""
 
     LOOP_SLEEP_DELAY_S = 60
 
     def __init__(self, drive: Drive, spin_down_time_s: int):
         super().__init__(name=f"{self.__class__.__name__}-{drive}")
         self.drive = drive
         self.spin_down_time_s = spin_down_time_s
         self.logger = logging.getLogger(self.name)
 
     def run(self):
-        """ Thread loop. """
+        """Thread loop."""
         try:
             previous_stats = None
             while not exit_evt.is_set():
                 if self.drive.isSleeping():
                     self.logger.debug("Drive is already sleeping")
                     self.sleep(__class__.LOOP_SLEEP_DELAY_S)
                     continue
@@ -663,24 +665,24 @@
 
             self.logger.info("Exiting")
 
         except Exception as e:
             self.logger.error(f"{e.__class__.__qualname__}: {e}")
 
     def sleep(self, s: int) -> None:
-        """ Sleep for s seconds, or less if exit event occurs. """
+        """Sleep for s seconds, or less if exit event occurs."""
         self.logger.debug(f"Sleeping for {s} seconds")
         interrupted = exit_evt.wait(timeout=s)
         if interrupted:
             self.logger.debug("Sleep interrupted")
 
 
 class Fan:
 
-    """ Represent a fan associated with a PWM file to control its speed. """
+    """Represent a fan associated with a PWM file to control its speed."""
 
     LAST_DIGITS_REGEX = re.compile("[^0-9]*([0-9]*)$")
 
     def __init__(self, id: int, pwm_filepath: str, start_value: int, stop_value: int):
         assert 0 <= start_value <= 255
         assert 0 <= stop_value <= 255
         self.id = id
@@ -689,33 +691,35 @@
             # we don't want to write to a block device in setPwmValue
             # command line parameters have probably been mixed up
             raise RuntimeError(f"{self.pwm_filepath!r} is a block device, PWM /sys file expected")
         pwm_num_match = self.__class__.LAST_DIGITS_REGEX.search(self.pwm_filepath)
         assert pwm_num_match is not None
         pwm_num = int(pwm_num_match.group(1))
         self.fan_input_filepath = os.path.join(os.path.dirname(self.pwm_filepath), f"fan{pwm_num}_input")
-        self.enable_filepath = f"{self.pwm_filepath}_enable"
+        self.enable_filepath: Optional[str] = f"{self.pwm_filepath}_enable"
         self.start_value = start_value
         self.stop_value = stop_value
         self.startup = False
         self.logger = logging.getLogger(f"Fan #{self.id}")
+        self.enable_restore = self.getEnabledValue()
+        self.pwm_restore = self.getPwmValue()
 
     def getRpm(self) -> int:
-        """ Read fan speed in revolutions per minute. """
+        """Read fan speed in revolutions per minute."""
         with open(self.fan_input_filepath, "rt") as fan_input_file:
             rpm = int(fan_input_file.read().strip())
         self.logger.debug(f"Rotation speed is currently {rpm} RPM")
         return rpm
 
     def isRunning(self) -> bool:
-        """ Return True if fan is moving, False instead. """
+        """Return True if fan is moving, False instead."""
         return self.getRpm() > 0
 
     def isStartingUp(self) -> bool:
-        """ Return True if fan is starting up, False instead. """
+        """Return True if fan is starting up, False instead."""
         return self.startup
 
     def waitStabilize(self) -> None:
         """
         Wait for the fan to have a stable rotational speed.
 
         The algorithm only works if the fan is either slowing down, accelerating, or steady during the test, not if its
@@ -728,15 +732,15 @@
             rpm = self.getRpm()
             if min_rpm <= rpm <= max_rpm:
                 break
             min_rpm = min(min_rpm, rpm)
             max_rpm = max(max_rpm, rpm)
 
     def setSpeed(self, target_prct: int) -> None:
-        """ Set fan speed to a percentage of its maximum speed. """
+        """Set fan speed to a percentage of its maximum speed."""
         # preconditions
         assert 0 <= target_prct <= 100
 
         self.logger.info(f"Setting fan speed to {target_prct}%")
 
         # calculate target PWM value
         if target_prct == 0:
@@ -751,40 +755,82 @@
         else:
             self.startup = False
 
         # set speed
         self.setPwmValue(target_value)
 
     def setPwmValue(self, value: int) -> None:
-        """ Set fan PWM value. """
+        """Set fan PWM value."""
         assert 0 <= value <= 255
-        with open(self.enable_filepath, "r+t") as enable_file:
-            enabled_val = int(enable_file.read().strip())
-            if enabled_val != 1:
-                self.logger.warning(f"{self.enable_filepath} was {enabled_val}, setting it to 1")
-                enable_file.seek(0)
-                enable_file.write("1")
+        self.setEnabledValue(1)
         self.logger.debug(f"Setting PWM value to {value}")
         with open(self.pwm_filepath, "wt") as pwm_file:
             pwm_file.write(str(value))
 
+    def getEnabledValue(self) -> Optional[int]:
+        """Read the enabled value of the fan."""
+        if self.enable_filepath is not None:
+            try:
+                with open(self.enable_filepath, "rt") as enable_file:
+                    enabled_val = int(enable_file.read().strip())
+                    self.logger.debug(f"Fan is in enabled state {enabled_val}")
+                    return enabled_val
+            except FileNotFoundError:
+                self.enable_filepath = None
+        return None
+
+    def setEnabledValue(self, value: int) -> None:
+        """
+        Set fan enabled value.
+
+        0: no fan speed control (i.e. fan at full speed)
+        1: manual fan speed control enabled
+        2+: automatic fan speed control enabled
+        """
+        assert 0 <= value
+        if self.enable_filepath is not None:
+            try:
+                with open(self.enable_filepath, "r+t") as enable_file:
+                    enabled_val = int(enable_file.read().strip())
+                    if enabled_val != value:
+                        self.logger.warning(f"{self.enable_filepath} was {enabled_val}, setting it to {value}")
+                        enable_file.seek(0)
+                        enable_file.write(str(value))
+            except FileNotFoundError:
+                self.enable_filepath = None
+
+    def getPwmValue(self) -> int:
+        """Read pwm value of the fan."""
+        with open(self.pwm_filepath, "rt") as pwm_file:
+            pwm = int(pwm_file.read().strip())
+        self.logger.debug(f"PWM value is currently {pwm}")
+        return pwm
+
+    def restoreFanSettings(self) -> None:
+        """Restore fan settings."""
+        self.logger.debug(f"Fan PWM is restored to {self.pwm_restore}")
+        self.setPwmValue(self.pwm_restore)
+        if self.enable_restore is not None:
+            self.setEnabledValue(self.enable_restore)
+            self.logger.debug(f"Fan enabled state is restored to {self.enable_restore}")
+
 
 class TestHardware:
 
-    """ Run basic drive tests, and analyze fan start/stop behaviour. """
+    """Run basic drive tests, and analyze fan start/stop behaviour."""
 
     def __init__(self, drives: Sequence[Drive], fans: Sequence[Fan]):
         self.drives = drives
         self.fans = fans
         self.ok_count = 0
         self.ko_count = 0
         self.logger = logging.getLogger(self.__class__.__name__)
 
     def run(self) -> None:
-        """ Run tests on drives and PWMs to recommend parameter values. """
+        """Run tests on drives and PWMs to recommend parameter values."""
         self.logger.info("Running hardware tests, this may take a few minutes")
         self.testDrives()
         start_stop_values = self.testPwms()
         if self.ko_count > 0:
             print(f"{self.ko_count}/{self.ko_count + self.ok_count} tests failed!")
         else:
             print(f"{self.ok_count}/{self.ok_count} tests OK, all good :)")
@@ -793,15 +839,15 @@
             % (
                 " ".join(str(min(255, x[0] + 32)) for x in start_stop_values),
                 " ".join(str(x[1]) for x in start_stop_values),
             )
         )
 
     def testDrives(self) -> None:
-        """ Run tests on hard disc drives. """
+        """Run tests on hard disc drives."""
         for drive in self.drives:
             self.reportTestGroupStart(f"Test of drive {drive}")
 
             test_desc = "Getting drive power state"
             self.reportTestStart(test_desc)
             try:
                 state = drive.getState()
@@ -825,15 +871,15 @@
                 stats = drive.getActivityStats()
                 test_ok = isinstance(stats, tuple)
             except Exception:
                 test_ok = False
             self.reportTestResult(test_desc, test_ok)
 
     def testPwms(self) -> Sequence[Tuple[int, int]]:
-        """ Run tests on PWMs. """
+        """Run tests on PWMs."""
         start_stop_values = []
         pwm_vals = (255,) + tuple(range(240, -1, -16))
         for fan in self.fans:
             self.reportTestGroupStart(f"Test of fan #{fan.id}")
             start_value, stop_value = 255, 0
 
             test_desc = "Stopping fan"
@@ -887,48 +933,48 @@
             self.reportTestResult(test_desc, test_ok)
 
             start_stop_values.append((start_value, stop_value))
 
         return start_stop_values
 
     def reportTestGroupStart(self, desc: str) -> None:
-        """ Output text when starting a group of tests. """
+        """Output text when starting a group of tests."""
         print("%s %s" % (desc, "-" * (shutil.get_terminal_size()[0] - len(desc) - 1)))
 
     def reportTestStart(self, desc: str) -> None:
-        """ Output text when starting a test. """
+        """Output text when starting a test."""
         print(desc, end=" ", flush=True)
 
     def reportTestResult(self, desc: str, ok: bool) -> None:
-        """ Output text when ending a test. """
+        """Output text when ending a test."""
         if ok:
             self.ok_count += 1
         else:
             self.ko_count += 1
         print(("[ %s ]" % ("OK" if ok else "KO")).rjust(shutil.get_terminal_size()[0] - len(desc) - 1))
 
 
 def test(drive_filepaths: Sequence[str], fan_pwm_filepaths: Sequence[str], hddtemp_daemon_port: int):
-    """ Entry point to run hardware tests. """
+    """Entry point to run hardware tests."""
     fans = [Fan(i, fan_pwm_filepath, 0, 0) for i, fan_pwm_filepath in enumerate(fan_pwm_filepaths, 1)]
     drives = [Drive(drive_filepath, hddtemp_daemon_port, 0, 0, False) for drive_filepath in drive_filepaths]
 
     tester = TestHardware(drives, fans)
     tester.run()
 
 
 def signal_handler(sig, frame):
-    """ Signal handler for clean exit. """
+    """Signal handler for clean exit."""
     logging.getLogger("Signal handler").info(f"Catched signal {sig}")
     global exit_evt
     exit_evt.set()
 
 
 def set_high_priority(logger: logging.Logger) -> None:
-    """ Change process scheduler and priority. """
+    """Change process scheduler and priority."""
     # use "real time" scheduler
     done = False
     sched = os.SCHED_RR
     if os.sched_getscheduler(0) == sched:
         # already running with RR scheduler, likely set from init system, don't touch priority
         done = True
     else:
@@ -967,16 +1013,17 @@
     min_drive_temp: int,
     max_drive_temp: int,
     cpu_temp_range: Tuple[float, float],
     interval_s: int,
     spin_down_time_s: int,
     hddtemp_daemon_port: Optional[int],
     use_smartctl: bool,
+    restore_fan_settings: bool,
 ):
-    """ Run main program logic, after handling command line specific stuff. """
+    """Run main program logic, after handling command line specific stuff."""
     logger = logging.getLogger("Main")
     fans = []
     try:
         # change process priority
         set_high_priority(logger)
 
         # register signal handler
@@ -1080,21 +1127,24 @@
         for thread in spin_down_threads:
             thread.join()
 
     except Exception as e:
         logger.error(f"{e.__class__.__qualname__}: {e}")
         exit_evt.set()
 
-    # run fans at full speed at exit
+    # restore fan settings or run fans at full speed at exit
     for fan in fans:
-        fan.setSpeed(100)
+        if restore_fan_settings:
+            fan.restoreFanSettings()
+        else:
+            fan.setSpeed(100)
 
 
 def cl_main():  # noqa: C901
-    """ Command line entry point. """
+    """Command line entry point."""
     # parse args
     arg_parser = argparse.ArgumentParser(
         description=f"HDD Fan Control v{__version__}.{__doc__}",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
     arg_parser.add_argument(
         "-d",
@@ -1230,14 +1280,20 @@
     )
     arg_parser.add_argument(
         "--smartctl",
         action="store_true",
         default=False,
         help="""Probe temperature using smartctl instead of hddtemp/hdparm/drivetemp (EXPERIMENTAL)""",
     )
+    arg_parser.add_argument(
+        "--restore-fan-settings",
+        action="store_true",
+        default=False,
+        help="""Restore fan settings on exit, otherwise the fans are run with full speed on exit""",
+    )
     args = arg_parser.parse_args()
     if ((args.fan_start_value is not None) and (len(args.fan_pwm_filepath) != len(args.fan_start_value))) or (
         (args.fan_stop_value is not None) and (len(args.fan_pwm_filepath) != len(args.fan_stop_value))
     ):
         print("Invalid parameter count")
         exit(os.EX_USAGE)
     if args.interval_s is None:
@@ -1277,14 +1333,17 @@
     logging.getLogger().addHandler(logging_handler)
 
     # check if root
     if os.geteuid() != 0:
         logging.getLogger("Startup").error("You need to run this script as root")
         exit(1)
 
+    # check mandatory deps
+    bin_dep.check_bin_dependency(("hdparm",))
+
     if args.test_mode or (args.fan_start_value is None) or (args.fan_stop_value is None):
         if (args.fan_start_value is None) or (args.fan_stop_value is None):
             logging.getLogger("Startup").warning(
                 "Missing --pwm-start-value or --pwm-stop-value argument, running hardware test to find values"
             )
         test(args.drive_filepaths, args.fan_pwm_filepath, args.hddtemp_daemon_port if args.hddtemp_daemon else None)
 
@@ -1313,16 +1372,13 @@
                 args.min_temp,
                 args.max_temp,
                 args.cpu_temp_range,
                 args.interval_s,
                 args.spin_down_time_s,
                 args.hddtemp_daemon_port if args.hddtemp_daemon else None,
                 args.smartctl,
+                args.restore_fan_settings,
             )
 
 
-# check deps
-bin_dep.check_bin_dependency(("hddtemp", "hdparm"))
-
-
 if __name__ == "__main__":
     cl_main()
```

### Comparing `hddfancontrol-1.5.0/hddfancontrol/colored_logging.py` & `hddfancontrol-1.5.1/hddfancontrol/colored_logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 LEVEL_COLOR_MAPPING = {logging.WARNING: Colors.YELLOW, logging.ERROR: Colors.RED, logging.CRITICAL: Colors.RED}
 LEVEL_BOLD_MAPPING = {logging.WARNING: False, logging.ERROR: False, logging.CRITICAL: True}
 
 
 class ColoredFormatter(logging.Formatter):
 
-    """ Formatter for the logging module, coloring terminal output according to error criticity. """
+    """Formatter for the logging module, coloring terminal output according to error criticity."""
 
     def format(self, record):
-        """ See logging.Formatter.format. """
+        """See logging.Formatter.format."""
         message = super().format(record)
         if sys.stderr.isatty() and not sys.platform.startswith("win32"):
             try:
                 color_code = LEVEL_COLOR_MAPPING[record.levelno].value
                 bold = LEVEL_BOLD_MAPPING[record.levelno]
             except KeyError:
                 pass
```

### Comparing `hddfancontrol-1.5.0/hddfancontrol.egg-info/PKG-INFO` & `hddfancontrol-1.5.1/hddfancontrol.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,182 +1,182 @@
 Metadata-Version: 2.1
 Name: hddfancontrol
-Version: 1.5.0
+Version: 1.5.1
 Summary: Control system fan speed by monitoring hard drive temperature
 Home-page: https://github.com/desbma/hddfancontrol
+Download-URL: https://github.com/desbma/hddfancontrol/archive/1.5.1.tar.gz
 Author: desbma
-License: UNKNOWN
-Download-URL: https://github.com/desbma/hddfancontrol/archive/1.5.0.tar.gz
-Description: # HDD Fan control
-        
-        [![PyPI version](https://img.shields.io/pypi/v/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
-        [![AUR version](https://img.shields.io/aur/version/hddfancontrol.svg?style=flat)](https://aur.archlinux.org/packages/hddfancontrol/)
-        [![Tests status](https://github.com/desbma/hddfancontrol/actions/workflows/ci.yml/badge.svg)](https://github.com/desbma/hddfancontrol/actions/)
-        [![Coverage](https://img.shields.io/coveralls/desbma/hddfancontrol/master.svg?style=flat)](https://coveralls.io/github/desbma/hddfancontrol?branch=master)
-        [![Lines of code](https://tokei.rs/b1/github/desbma/hddfancontrol)](https://github.com/desbma/hddfancontrol)
-        [![Supported Python versions](https://img.shields.io/pypi/pyversions/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
-        [![License](https://img.shields.io/github/license/desbma/hddfancontrol.svg?style=flat)](https://github.com/desbma/hddfancontrol/blob/master/LICENSE)
-        
-        HDD Fan control is a command line tool to dynamically control fan speed according to hard drive temperature on Linux.
-        
-        This has 3 benefits:
-        
-        - it allows maintaining your hard drives in the ideal temperature range to have maximum longevity and avoid overheating
-        
-        Because fans will slow down or stop when not needed:
-        
-        - it minimizes noise generated by the fans
-        - it also minimizes power consumption at the same time
-        
-        ## When is this useful?
-        
-        HDD Fan control is useful when you have one or several hard drives with one or several fans close to them, and do not want to let the motherboard control the fan speed, because it does so either statically, or using a temperature sensor unrelated to the real drive temperature (either on the CPU or on some other place on the motherboard).
-        
-        The ideal use case is for a NAS with several hard drives, a low power CPU (ie. ARM or Intel Atom) with passive cooling (no fans), and a chassis with fans close to the hard drive. It that case the CPU will generate less heat than the hard drives and it makes sense to control fan speed according to the main heat source.
-        
-        ## Features
-        
-        - Can run in daemon mode
-        - Can control several fans and/or several drives with a single invocation
-        - Supports 6 different ways of querying temperature:
-          - `hddtemp` invocation
-          - `hddtemp` daemon query
-          - `hdparm` invocation
-          - `smartctl` invocation (SCT)
-          - `smartctl` invocation (SMART attributes)
-          - `drivetemp` native kernel hwmon
-        - Can automatically spin down drives after a customizable period of inactivity
-        - Can adapt to different fan characteristics
-        - Can be set to stop fans or run them at full speed at customizable temperatures
-        - Can be configured to never set the fans below a certain speed (useful if the fans controlled by HDD Fan control are the only ones available in the chassis)
-        - Can also optionally monitor CPU temperature, and control fan speed accordingly
-        
-        ## Prerequisites
-        
-        - A Linux distribution
-        - A least one SATA hard drive, that supports:
-          - Temperature querying
-          - Power state querying
-        - A motherboard which:
-          - exposes to the OS a PWM to control fan speed
-          - exposes to the OS a sensor to query fan speed
-        
-        Most motherboards and SATA drives fit these requirements.
-        
-        ## Installation
-        
-        HDD Fan control requires [Python](https://www.python.org/downloads/) >= 3.6.
-        
-        ### Distribution packages
-        
-        Some Linux distributions have a hddfancontrol package available in their repository:
-        
-        - Arch Linux (AUR): [hddfancontrol](https://aur.archlinux.org/packages/hddfancontrol/)
-        - Fedora: [hddfancontrol](https://apps.fedoraproject.org/packages/hddfancontrol) (thanks to [TC01](https://github.com/TC01))
-        
-        ### From PyPI (with PIP)
-        
-        1. If you don't already have it, [install pip](https://pip.pypa.io/en/stable/installing/) for Python 3
-        2. Install HDD Fan control: `pip3 install hddfancontrol`
-        3. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php).
-           On Ubuntu and other Debian derivatives: `sudo apt-get install hdparm hddtemp`.
-        
-        ### From source
-        
-        1. If you don't already have it, [install setuptools](https://pypi.python.org/pypi/setuptools#installation-instructions) for Python 3
-        2. Clone this repository: `git clone https://github.com/desbma/hddfancontrol`
-        3. Install HDD Fan control: `python3 setup.py install`
-        4. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php).
-           On Ubuntu and other Debian derivatives: `sudo apt-get install hdparm hddtemp`.
-        
-        To query fan characteristics, you may also need pwmconfig. On Ubuntu and other Debian derivatives, it is part of the fancontrol package, that you can install with `sudo apt-get install fancontrol`. HDD fancontrol and fancontrol are unrelated. The fancontrol daemon is **not** needed for HDD fan control to operate. If you use both fancontrol and HDD fancontrol, be careful not to make them control the same fans.
-        
-        ## Configuration
-        
-        ### A word of caution
-        
-        The default parameters will run fans at 100% speed at temperatures > 50°C, and run them a 20% speed if < 30°C, which corresponds to the usual recommended drive operating temperature. If you are sure that there are no other components in your system that generate significant heat, if you have other fans to cool down your system, or if you have a case optimized for passive cooling, you can set minimum speed to 0%, which will stop the fans if temperature is below the minimum threshold.
-        
-        **Be aware that a misconfiguration of this tool can lead to a failure to cool down your system properly which can damage components or reduce their lifetime.**
-        
-        Before using HDD Fan control unmonitored for long period of time, I recommend keeping a minimum fan speed for security, and checking that the temperature of your system stays in reasonable range as expected.
-        
-        ### Fan configuration
-        
-        To get the value for the `--pwm`, `--pwm-start-value` and `--pwm-stop-value` parameters, you can either:
-        
-        - Use the `-t` or `--test` parameter, which will run some tests and detect the values at which the fans start and stop. However you need to have previously identified the PWM file (the `--pwm` parameter)
-        - use the [pwmconfig tool](http://www.lm-sensors.org/wiki/man/pwmconfig).
-        
-        ### Drive auto spin down
-        
-        SATA drives can be configured to automatically spin down after a certain period of inactivity, which saves power. If your drives are configured to do so, you may notice that they do not spin down when HDD Fan control is running.
-        This is due to the fact that HDD Fan control will query temperature at fixed interval, which the drive will consider an activity and reset the spin down timeout.
-        To fix that, you can either:
-        
-        - Use a value for the `-i`/`--interval` parameter higher than your SATA spin down time (not recommended unless your spin down time is very low, ie < 2 min). In that case you do not need to use hddfancontrol's `--spin-down-time` switch, because the builtin SATA drive timeout (that you can set for example with [`hdparm -S XXX` command](https://linux.die.net/man/8/hdparm)) should take effect.
-        - Use the `--spin-down-time` parameter that will monitor drive activity and spin it down if inactive, independantly of the SATA feature (recommended)
-        
-        **Keep in mind that spinning down and up a drive repeatedly wears it prematurly, so unless you are in a power constrained environement (ie. laptop), do not set the spin down time too low.**
-        
-        Reading temperature while a drive is in low power state will make it spin up, so HDD Fan control will stop querying temperature in that case, and wait for the drive (which will be cooling down in low power state anyway) to spin up.
-        
-        Some HGST (previously Hitachi) drives support a special way of querying temperature that does not spin up drives, which HDD Fan control will detect and use, however it still prevents them from spinning down, so the above instructions still apply.
-        
-        ## Command line usage
-        
-        Run `hddfancontrol -h` to get full command line reference.
-        
-        As an example, the command line below will instruct HDD Fan control to:
-        
-        - monitor temperature of drives `/dev/sda` and `/dev/sdb`
-        - control fan speed using PWM 2 and 3 in `/sys/class/hwmon/hwmon1/device/`
-        - start both fans using PWM value 200
-        - consider the fans will stop with PWM value 75
-        - never run the fans below 10% of their maximum speed
-        - check temperature at least every minute
-        - automatically spin down drives if they are inactive for 2 hours (7200 seconds)
-        - run in daemon mode
-        - log what is going on to `/var/log/hddfancontrol.log`
-        
-        `hddfancontrol -d /dev/sda /dev/sdb -p /sys/class/hwmon/hwmon1/device/pwm2 /sys/class/hwmon/hwmon1/device/pwm3 --pwm-start-value 200 200 --pwm-stop-value 75 75 --min-fan-speed-prct 10 -i 60 --spin-down-time 7200 -b -l /var/log/hddfancontrol.log`
-        
-        ## Systemd service
-        
-        A systemd service file is provided to control the daemon easily.
-        If you installed hddfancontrol from a distribution package, you likely already have it installed, otherwise you can install it from the sources of this repository with:
-        
-        ```
-        sudo cp ./systemd/hddfancontrol.service /etc/systemd/system/
-        sudo mkdir -p /etc/conf.d
-        sudo cp ./systemd/hddfancontrol.conf /etc/conf.d/hddfancontrol
-        ```
-        
-        Then you need to edit the `HDDFANCONTROL_ARGS` variable in `/etc/conf.d/hddfancontrol` to set the parameters (drives, temperature range...).
-        
-        You can then start the daemon with `sudo systemctl start hddfancontrol`, see its status with `sudo systemctl status hddfancontrol` and enable automatic startup at boot time with `sudo systemctl enable hddfancontrol`.
-        
-        ## License
-        
-        [GPLv3](https://www.gnu.org/licenses/gpl-3.0-standalone.html)
-        
 Keywords: hdd,drive,temperature,fan,control,speed
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HDD Fan control
+
+[![PyPI version](https://img.shields.io/pypi/v/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
+[![AUR version](https://img.shields.io/aur/version/hddfancontrol.svg?style=flat)](https://aur.archlinux.org/packages/hddfancontrol/)
+[![Tests status](https://github.com/desbma/hddfancontrol/actions/workflows/ci.yml/badge.svg)](https://github.com/desbma/hddfancontrol/actions/)
+[![Coverage](https://img.shields.io/coveralls/desbma/hddfancontrol/master.svg?style=flat)](https://coveralls.io/github/desbma/hddfancontrol?branch=master)
+[![Lines of code](https://tokei.rs/b1/github/desbma/hddfancontrol)](https://github.com/desbma/hddfancontrol)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/hddfancontrol.svg?style=flat)](https://pypi.python.org/pypi/hddfancontrol/)
+[![License](https://img.shields.io/github/license/desbma/hddfancontrol.svg?style=flat)](https://github.com/desbma/hddfancontrol/blob/master/LICENSE)
+
+HDD Fan control is a command line tool to dynamically control fan speed according to hard drive temperature on Linux.
+
+This has 3 benefits:
+
+- it allows maintaining your hard drives in the ideal temperature range to have maximum longevity and avoid overheating
+
+Because fans will slow down or stop when not needed:
+
+- it minimizes noise generated by the fans
+- it also minimizes power consumption at the same time
+
+## When is this useful?
+
+HDD Fan control is useful when you have one or several hard drives with one or several fans close to them, and do not want to let the motherboard control the fan speed, because it does so either statically, or using a temperature sensor unrelated to the real drive temperature (either on the CPU or on some other place on the motherboard).
+
+The ideal use case is for a NAS with several hard drives, a low power CPU (ie. ARM or Intel Atom) with passive cooling (no fans), and a chassis with fans close to the hard drive. It that case the CPU will generate less heat than the hard drives and it makes sense to control fan speed according to the main heat source.
+
+## Features
+
+- Can run in daemon mode
+- Can control several fans and/or several drives with a single invocation
+- Supports 6 different ways of querying temperature:
+  - `hddtemp` invocation
+  - `hddtemp` daemon query
+  - `hdparm` invocation
+  - `smartctl` invocation (SCT)
+  - `smartctl` invocation (SMART attributes)
+  - `drivetemp` native kernel hwmon
+- Can automatically spin down drives after a customizable period of inactivity
+- Can adapt to different fan characteristics
+- Can be set to stop fans or run them at full speed at customizable temperatures
+- Can be configured to never set the fans below a certain speed (useful if the fans controlled by HDD Fan control are the only ones available in the chassis)
+- Can also optionally monitor CPU temperature, and control fan speed accordingly
+
+## Prerequisites
+
+- A Linux distribution
+- A least one SATA hard drive, that supports:
+  - Temperature querying
+  - Power state querying
+- A motherboard which:
+  - exposes to the OS a PWM to control fan speed
+  - exposes to the OS a sensor to query fan speed
+
+Most motherboards and SATA drives fit these requirements.
+
+## Installation
+
+HDD Fan control requires [Python](https://www.python.org/downloads/) >= 3.6.
+
+### Distribution packages
+
+Some Linux distributions have a hddfancontrol package available in their repository:
+
+- Arch Linux (AUR): [hddfancontrol](https://aur.archlinux.org/packages/hddfancontrol/)
+- Fedora: [hddfancontrol](https://apps.fedoraproject.org/packages/hddfancontrol) (thanks to [TC01](https://github.com/TC01))
+
+### From PyPI (with PIP)
+
+1. If you don't already have it, [install pip](https://pip.pypa.io/en/stable/installing/) for Python 3
+2. Install HDD Fan control: `pip3 install hddfancontrol`
+3. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php) or [smartctl](https://www.smartmontools.org/).
+   On recent Ubuntu and other Debian derivatives: `sudo apt-get install hdparm smartmontools`.
+
+### From source
+
+1. If you don't already have it, [install setuptools](https://pypi.python.org/pypi/setuptools#installation-instructions) for Python 3
+2. Clone this repository: `git clone https://github.com/desbma/hddfancontrol`
+3. Install HDD Fan control: `python3 setup.py install`
+4. Install [hdparm](http://sourceforge.net/projects/hdparm/) and [hddtemp](http://www.guzu.net/linux/hddtemp.php) or [smartctl](https://www.smartmontools.org/).
+   On recent Ubuntu and other Debian derivatives: `sudo apt-get install hdparm smartmontools`.
+
+To query fan characteristics, you may also need pwmconfig. On Ubuntu and other Debian derivatives, it is part of the fancontrol package, that you can install with `sudo apt-get install fancontrol`. HDD fancontrol and fancontrol are unrelated. The fancontrol daemon is **not** needed for HDD fan control to operate. If you use both fancontrol and HDD fancontrol, be careful not to make them control the same fans.
+
+## Configuration
+
+### A word of caution
+
+The default parameters will run fans at 100% speed at temperatures > 50°C, and run them a 20% speed if < 30°C, which corresponds to the usual recommended drive operating temperature. If you are sure that there are no other components in your system that generate significant heat, if you have other fans to cool down your system, or if you have a case optimized for passive cooling, you can set minimum speed to 0%, which will stop the fans if temperature is below the minimum threshold.
+
+**Be aware that a misconfiguration of this tool can lead to a failure to cool down your system properly which can damage components or reduce their lifetime.**
+
+Before using HDD Fan control unmonitored for long period of time, I recommend keeping a minimum fan speed for security, and checking that the temperature of your system stays in reasonable range as expected.
+
+### Fan configuration
+
+To get the value for the `--pwm`, `--pwm-start-value` and `--pwm-stop-value` parameters, you can either:
+
+- Use the `-t` or `--test` parameter, which will run some tests and detect the values at which the fans start and stop. However you need to have previously identified the PWM file (the `--pwm` parameter)
+- use the [pwmconfig tool](http://www.lm-sensors.org/wiki/man/pwmconfig).
+
+### Drive auto spin down
+
+SATA drives can be configured to automatically spin down after a certain period of inactivity, which saves power. If your drives are configured to do so, you may notice that they do not spin down when HDD Fan control is running.
+This is due to the fact that HDD Fan control will query temperature at fixed interval, which the drive will consider an activity and reset the spin down timeout.
+To fix that, you can either:
+
+- Use a value for the `-i`/`--interval` parameter higher than your SATA spin down time (not recommended unless your spin down time is very low, ie < 2 min). In that case you do not need to use hddfancontrol's `--spin-down-time` switch, because the builtin SATA drive timeout (that you can set for example with [`hdparm -S XXX` command](https://linux.die.net/man/8/hdparm)) should take effect.
+- Use the `--spin-down-time` parameter that will monitor drive activity and spin it down if inactive, independantly of the SATA feature (recommended)
+
+**Keep in mind that spinning down and up a drive repeatedly wears it prematurly, so unless you are in a power constrained environement (ie. laptop), do not set the spin down time too low.**
+
+Reading temperature while a drive is in low power state will make it spin up, so HDD Fan control will stop querying temperature in that case, and wait for the drive (which will be cooling down in low power state anyway) to spin up.
+
+Some HGST (previously Hitachi) drives support a special way of querying temperature that does not spin up drives, which HDD Fan control will detect and use, however it still prevents them from spinning down, so the above instructions still apply.
+
+## Command line usage
+
+Run `hddfancontrol -h` to get full command line reference.
+
+As an example, the command line below will instruct HDD Fan control to:
+
+- monitor temperature of drives `/dev/sda` and `/dev/sdb`
+- control fan speed using PWM 2 and 3 in `/sys/class/hwmon/hwmon1/device/`
+- start both fans using PWM value 200
+- consider the fans will stop with PWM value 75
+- never run the fans below 10% of their maximum speed
+- check temperature at least every minute
+- automatically spin down drives if they are inactive for 2 hours (7200 seconds)
+- run in daemon mode
+- log what is going on to `/var/log/hddfancontrol.log`
+
+`hddfancontrol -d /dev/sda /dev/sdb -p /sys/class/hwmon/hwmon1/device/pwm2 /sys/class/hwmon/hwmon1/device/pwm3 --pwm-start-value 200 200 --pwm-stop-value 75 75 --min-fan-speed-prct 10 -i 60 --spin-down-time 7200 -b -l /var/log/hddfancontrol.log`
+
+## Systemd service
+
+A systemd service file is provided to control the daemon easily.
+If you installed hddfancontrol from a distribution package, you likely already have it installed, otherwise you can install it from the sources of this repository with:
+
+```
+sudo cp ./systemd/hddfancontrol.service /etc/systemd/system/
+sudo mkdir -p /etc/conf.d
+sudo cp ./systemd/hddfancontrol.conf /etc/conf.d/hddfancontrol
+```
+
+Then you need to edit the `HDDFANCONTROL_ARGS` variable in `/etc/conf.d/hddfancontrol` to set the parameters (drives, temperature range...).
+
+You can then start the daemon with `sudo systemctl start hddfancontrol`, see its status with `sudo systemctl status hddfancontrol` and enable automatic startup at boot time with `sudo systemctl enable hddfancontrol`.
+
+## License
+
+[GPLv3](https://www.gnu.org/licenses/gpl-3.0-standalone.html)
```

### Comparing `hddfancontrol-1.5.0/setup.py` & `hddfancontrol-1.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import os
 import re
 import sys
 
 from setuptools import find_packages, setup
 
-if sys.hexversion < 0x3060000:
-    print("Python version %s is unsupported, >= 3.6.0 is needed" % (".".join(map(str, sys.version_info[:3]))))
+if sys.hexversion < 0x3070000:
+    print("Python version %s is unsupported, >= 3.7.0 is needed" % (".".join(map(str, sys.version_info[:3]))))
     exit(1)
 
 with open(os.path.join("hddfancontrol", "__init__.py"), "rt") as f:
     version_match = re.search('__version__ = "([^"]+)"', f.read())
     assert version_match is not None
     version = version_match.group(1)
 
@@ -45,16 +45,17 @@
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: System :: Hardware",
         "Topic :: System :: Monitoring",
         "Topic :: Utilities",
     ],
 )
```

### Comparing `hddfancontrol-1.5.0/tests/__init__.py` & `hddfancontrol-1.5.1/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,43 +12,43 @@
 import unittest.mock
 
 import hddfancontrol
 
 
 class FakeHddtempDaemon(threading.Thread):
 
-    """ Mock hddtemp daemon. """
+    """Mock hddtemp daemon."""
 
     outgoing = b""
 
     def __init__(self, port):
         socketserver.TCPServer.allow_reuse_address = True
         self.server = socketserver.TCPServer(("127.0.0.1", port), FakeHddtempDaemonHandler)
         super().__init__()
 
     def run(self):
-        """ Thread entry point. """
+        """Thread entry point."""
         self.server.serve_forever()
 
 
 class FakeHddtempDaemonHandler(socketserver.StreamRequestHandler):
 
-    """ Mock hddtemp daemon connection handler. """
+    """Mock hddtemp daemon connection handler."""
 
     def handle(self):
-        """ See socketserver.StreamRequestHandler.handle. """
+        """See socketserver.StreamRequestHandler.handle."""
         self.wfile.write(FakeHddtempDaemon.outgoing)
 
 
 class TestDrive(unittest.TestCase):
 
-    """ Main tests class. """
+    """Main tests class."""
 
     def setUp(self):
-        """ Setups test specific stuff. """
+        """Setups test specific stuff."""
         with unittest.mock.patch("hddfancontrol.os.stat") as os_stat_mock, unittest.mock.patch(
             "hddfancontrol.stat"
         ) as stat_mock, unittest.mock.patch(
             "hddfancontrol.subprocess.check_output"
         ) as subprocess_check_output_mock, unittest.mock.patch(
             "hddfancontrol.Drive.getPrettyName"
         ) as drive_getPrettyName, unittest.mock.patch(
@@ -59,34 +59,34 @@
             subprocess_check_output_mock.return_value = ""
             drive_getPrettyName.return_value = "drive_name"
             isfile_mock.return_value = False
             self.drive = hddfancontrol.Drive("/dev/_sdz", None, 30, 50, False)
         self.hddtemp_daemon = None
 
     def tearDown(self):
-        """ Cleanup test specific stuff. """
+        """Cleanup test specific stuff."""
         if self.hddtemp_daemon is not None:
             self.hddtemp_daemon.server.shutdown()
             self.hddtemp_daemon.server.server_close()
             self.hddtemp_daemon.join()
 
     def test_getPrettyName(self):
-        """ Test generation of pretty drive name. """
+        """Test generation of pretty drive name."""
         with unittest.mock.patch("hddfancontrol.subprocess.check_output") as subprocess_check_output_mock:
             subprocess_check_output_mock.return_value = "\n/dev/_sdz:\n\nATA device, with non-removable media\n\tModel Number:       WDC WD4003FZEX-00Z4SA0                  \n\tSerial Number:      WD-WMC5D0D4YY1K\n\tFirmware Revision:  01.01A01\n\tTransport:          Serial, SATA 1.0a, SATA II Extensions, SATA Rev 2.5, SATA Rev 2.6, SATA Rev 3.0\nStandards:\n\tSupported: 9 8 7 6 5 \n\tLikely used: 9\nConfiguration:\n\tLogical\t\tmax\tcurrent\n\tcylinders\t16383\t16383\n\theads\t\t16\t16\n\tsectors/track\t63\t63\n\t--\n\tCHS current addressable sectors:   16514064\n\tLBA    user addressable sectors:  268435455\n\tLBA48  user addressable sectors: 7814037168\n\tLogical  Sector size:                   512 bytes\n\tPhysical Sector size:                  4096 bytes\n\tLogical Sector-0 offset:                  0 bytes\n\tdevice size with M = 1024*1024:     3815447 MBytes\n\tdevice size with M = 1000*1000:     4000787 MBytes (4000 GB)\n\tcache/buffer size  = unknown\n\tNominal Media Rotation Rate: 7200\nCapabilities:\n\tLBA, IORDY(can be disabled)\n\tQueue depth: 32\n\tStandby timer values: spec'd by Standard, with device specific minimum\n\tR/W multiple sector transfer: Max = 16\tCurrent = 0\n\tDMA: mdma0 mdma1 mdma2 udma0 udma1 udma2 udma3 udma4 udma5 *udma6 \n\t     Cycle time: min=120ns recommended=120ns\n\tPIO: pio0 pio1 pio2 pio3 pio4 \n\t     Cycle time: no flow control=120ns  IORDY flow control=120ns\nCommands/features:\n\tEnabled\tSupported:\n\t   *\tSMART feature set\n\t    \tSecurity Mode feature set\n\t   *\tPower Management feature set\n\t   *\tWrite cache\n\t   *\tLook-ahead\n\t   *\tHost Protected Area feature set\n\t   *\tWRITE_BUFFER command\n\t   *\tREAD_BUFFER command\n\t   *\tNOP cmd\n\t   *\tDOWNLOAD_MICROCODE\n\t    \tPower-Up In Standby feature set\n\t   *\tSET_FEATURES required to spinup after power up\n\t    \tSET_MAX security extension\n\t   *\t48-bit Address feature set\n\t   *\tMandatory FLUSH_CACHE\n\t   *\tFLUSH_CACHE_EXT\n\t   *\tSMART error logging\n\t   *\tSMART self-test\n\t   *\tGeneral Purpose Logging feature set\n\t   *\t64-bit World wide name\n\t   *\t{READ,WRITE}_DMA_EXT_GPL commands\n\t   *\tSegmented DOWNLOAD_MICROCODE\n\t   *\tGen1 signaling speed (1.5Gb/s)\n\t   *\tGen2 signaling speed (3.0Gb/s)\n\t   *\tGen3 signaling speed (6.0Gb/s)\n\t   *\tNative Command Queueing (NCQ)\n\t   *\tHost-initiated interface power management\n\t   *\tPhy event counters\n\t   *\tNCQ priority information\n\t   *\tREAD_LOG_DMA_EXT equivalent to READ_LOG_EXT\n\t   *\tDMA Setup Auto-Activate optimization\n\t   *\tSoftware settings preservation\n\t   *\tSMART Command Transport (SCT) feature set\n\t   *\tSCT Write Same (AC2)\n\t   *\tSCT Features Control (AC4)\n\t   *\tSCT Data Tables (AC5)\n\t    \tunknown 206[12] (vendor specific)\n\t    \tunknown 206[13] (vendor specific)\n\t    \tunknown 206[14] (vendor specific)\nSecurity: \n\tMaster password revision code = 65534\n\t\tsupported\n\tnot\tenabled\n\tnot\tlocked\n\tnot\tfrozen\n\tnot\texpired: security count\n\t\tsupported: enhanced erase\n\t424min for SECURITY ERASE UNIT. 424min for ENHANCED SECURITY ERASE UNIT. \nLogical Unit WWN Device Identifier: 50014ee0593d4632\n\tNAA\t\t: 5\n\tIEEE OUI\t: 0014ee\n\tUnique ID\t: 0593d4632\nChecksum: correct\n"  # noqa: E501
             self.assertEqual(self.drive.getPrettyName(), "_sdz WDC WD4003FZEX-00Z4SA0")
             subprocess_check_output_mock.assert_called_once_with(
                 ("hdparm", "-I", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
 
     def test_supportsHitachiTempQuery(self):
-        """ Test detection for "Hitachi" temp query. """
+        """Test detection for "Hitachi" temp query."""
         with unittest.mock.patch("hddfancontrol.subprocess.check_output") as subprocess_check_output_mock:
             subprocess_check_output_mock.return_value = (
                 "\n/dev/_sdz:\n drive temperature (celsius) is:  30\n drive temperature in range:  yes"
             )
             self.assertTrue(self.drive.supportsHitachiTempQuery())
             subprocess_check_output_mock.assert_called_once_with(
                 ("hdparm", "-H", "/dev/_sdz"),
@@ -119,15 +119,15 @@
                 ("hdparm", "-H", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.STDOUT,
                 universal_newlines=True,
             )
 
     def test_supportsSctTempQuery(self):
-        """ Test detection for "SCT" temp query. """
+        """Test detection for "SCT" temp query."""
         with unittest.mock.patch("hddfancontrol.subprocess.check_output") as subprocess_check_output_mock:
             subprocess_check_output_mock.return_value = """smartctl 7.0 2018-12-30 r4883 [x86_64-linux-4.19.36-1-lts] (local build)
 Copyright (C) 2002-18, Bruce Allen, Christian Franke, www.smartmontools.org
 
 === START OF READ SMART DATA SECTION ===
 SCT Status Version:                  3
 SCT Version (vendor specific):       258 (0x0102)
@@ -136,40 +136,40 @@
 Power Cycle Min/Max Temperature:     18/39 Celsius
 Lifetime    Min/Max Temperature:      0/56 Celsius
 Under/Over Temperature Limit Count:   0/0
 Vendor specific:
 01 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 
-"""
+"""  # noqa: E501
             self.assertTrue(self.drive.supportsSctTempQuery())
             subprocess_check_output_mock.assert_called_once_with(
                 ("smartctl", "-l", "scttempsts", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
         with unittest.mock.patch("hddfancontrol.subprocess.check_output") as subprocess_check_output_mock:
             subprocess_check_output_mock.return_value = """smartctl 7.0 2018-12-30 r4883 [x86_64-linux-4.19.36-1-lts] (local build)
 Copyright (C) 2002-18, Bruce Allen, Christian Franke, www.smartmontools.org
 
 === START OF READ SMART DATA SECTION ===
 SCT Commands not supported
 
-"""
+"""  # noqa: E501
             self.assertFalse(self.drive.supportsSctTempQuery())
             subprocess_check_output_mock.assert_called_once_with(
                 ("smartctl", "-l", "scttempsts", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
 
     def test_getState(self):
-        """ Test drive state identification. """
+        """Test drive state identification."""
         with unittest.mock.patch("hddfancontrol.subprocess.check_output") as subprocess_check_output_mock:
             subprocess_check_output_mock.return_value = "\n/dev/_sdz:\n drive state is:  active/idle\n"
             self.assertEqual(self.drive.getState(), hddfancontrol.Drive.DriveState.ACTIVE_IDLE)
             subprocess_check_output_mock.assert_called_once_with(
                 ("hdparm", "-C", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
@@ -211,15 +211,15 @@
                 ("hdparm", "-C", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
 
     def test_isSleeping(self):
-        """ Test sleeping device identification. """
+        """Test sleeping device identification."""
         with unittest.mock.patch("hddfancontrol.subprocess.check_output") as subprocess_check_output_mock:
             subprocess_check_output_mock.return_value = "\n/dev/_sdz:\n drive state is:  active/idle\n"
             self.assertFalse(self.drive.isSleeping())
             subprocess_check_output_mock.assert_called_once_with(
                 ("hdparm", "-C", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
@@ -261,15 +261,15 @@
                 ("hdparm", "-C", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
 
     def test_getTemperature(self):
-        """ Test device temperature probing. """
+        """Test device temperature probing."""
 
         # smartctl -l scttempsts call
         self.drive.temp_query_method = hddfancontrol.Drive.TempProbingMethod.SMARTCTL_SCT_INVOCATION
         with unittest.mock.patch("hddfancontrol.subprocess.check_output") as subprocess_check_output_mock:
             subprocess_check_output_mock.return_value = """smartctl 7.0 2018-12-30 r4883 [x86_64-linux-4.19.36-1-lts] (local build)
 Copyright (C) 2002-18, Bruce Allen, Christian Franke, www.smartmontools.org
 
@@ -281,15 +281,15 @@
 Power Cycle Min/Max Temperature:     18/40 Celsius
 Lifetime    Min/Max Temperature:      0/56 Celsius
 Under/Over Temperature Limit Count:   0/0
 Vendor specific:
 01 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00 00
 
-"""
+"""  # noqa: E501
             self.assertEqual(self.drive.getTemperature(), 30)
             subprocess_check_output_mock.assert_called_once_with(
                 ("smartctl", "-l", "scttempsts", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
@@ -318,15 +318,15 @@
 193 Load_Cycle_Count        0x0012   100   100   000    Old_age   Always       -       571
 194 Temperature_Celsius     0x0002   171   171   000    Old_age   Always       -       35 (Min/Max 13/45)
 196 Reallocated_Event_Count 0x0032   100   100   000    Old_age   Always       -       0
 197 Current_Pending_Sector  0x0022   100   100   000    Old_age   Always       -       0
 198 Offline_Uncorrectable   0x0008   100   100   000    Old_age   Offline      -       0
 199 UDMA_CRC_Error_Count    0x000a   200   200   000    Old_age   Always       -       0
 
-"""
+"""  # noqa: E501
             self.assertEqual(self.drive.getTemperature(), 35)
             subprocess_check_output_mock.assert_called_once_with(
                 ("smartctl", "-A", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
@@ -357,15 +357,15 @@
 195 Hardware_ECC_Recovered  0x001a   048   048   000    Old_age   Always       -       80662606
 197 Current_Pending_Sector  0x0012   070   069   000    Old_age   Always       -       614
 198 Offline_Uncorrectable   0x0010   070   069   000    Old_age   Offline      -       614
 199 UDMA_CRC_Error_Count    0x003e   200   200   000    Old_age   Always       -       0
 200 Multi_Zone_Error_Rate   0x0000   100   253   000    Old_age   Offline      -       0
 202 TA_Increase_Count       0x0032   100   253   000    Old_age   Always       -       0
 
-"""
+"""  # noqa: E501
             self.assertEqual(self.drive.getTemperature(), 44)
             subprocess_check_output_mock.assert_called_once_with(
                 ("smartctl", "-A", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
@@ -391,15 +391,15 @@
 Power On Hours: 2
 Unsafe Shutdowns: 4
 Media and Data Integrity Errors: 0
 Error Information Log Entries: 0
 Warning Comp. Temperature Time: 0
 Critical Comp. Temperature Time: 0
 
-"""
+"""  # noqa: E501
             self.assertEqual(self.drive.getTemperature(), 37)
             subprocess_check_output_mock.assert_called_once_with(
                 ("smartctl", "-A", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
@@ -418,15 +418,15 @@
   Blocks read from cache and sent to initiator = 384030649
   Number of read and write commands whose size <= segment size = 21193148
   Number of read and write commands whose size > segment size = 1278317
 Vendor (Seagate/Hitachi) factory information
   number of hours powered up = 19.86
   number of minutes until next internal SMART test = 108
 
-"""
+"""  # noqa: E501
             self.assertEqual(self.drive.getTemperature(), 42)
             subprocess_check_output_mock.assert_called_once_with(
                 ("smartctl", "-A", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
                 universal_newlines=True,
             )
@@ -557,26 +557,26 @@
         with self.assertRaises(RuntimeError):
             self.drive.getTemperature()
         FakeHddtempDaemon.outgoing = b""
         with self.assertRaises(Exception):
             self.drive.getTemperature()
 
     def test_spinDown(self):
-        """ Test HDD spin down. """
+        """Test HDD spin down."""
         with unittest.mock.patch("hddfancontrol.subprocess.check_call") as subprocess_check_call_mock:
             self.drive.spinDown()
             subprocess_check_call_mock.assert_called_once_with(
                 ("hdparm", "-y", "/dev/_sdz"),
                 stdin=subprocess.DEVNULL,
                 stdout=subprocess.DEVNULL,
                 stderr=subprocess.DEVNULL,
             )
 
     def test_getActivityStats(self):
-        """ Test drive stats fetching. """
+        """Test drive stats fetching."""
         with self.assertRaises(Exception):
             self.drive.getActivityStats()
         with tempfile.NamedTemporaryFile("wt") as stat_file:
             self.drive.stat_filepath = stat_file.name
             with self.assertRaises(Exception):
                 self.drive.getActivityStats()
             stat_file.write(
@@ -585,15 +585,15 @@
             stat_file.flush()
             self.assertEqual(
                 self.drive.getActivityStats(),
                 (21695, 7718, 2913268, 95136, 13986, 754, 932032, 55820, 0, 19032, 150940),
             )
 
     def test_compareActivityStats(self):
-        """ Test drive stat analysis to detect activity. """
+        """Test drive stat analysis to detect activity."""
         self.drive.temp_query_method = hddfancontrol.Drive.TempProbingMethod.HDDTEMP_INVOCATION
         only_hddtemp_probe_stats = (
             (
                 (
                     3368700,
                     14189,
                     1667115340,
```

