# Comparing `tmp/sqlalchemy_celery_beat-0.6.2.tar.gz` & `tmp/sqlalchemy_celery_beat-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.6.2.tar", last modified: Wed Jun 21 01:22:51 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.7.0.tar", last modified: Sun Jun 25 01:43:09 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.6.2.tar` & `sqlalchemy_celery_beat-0.7.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 01:22:51.622756 sqlalchemy_celery_beat-0.6.2/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.6.2/LICENSE
--rw-rw-rw-   0        0        0    10599 2023-06-21 01:22:51.621757 sqlalchemy_celery_beat-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     9627 2023-06-20 07:42:22.000000 sqlalchemy_celery_beat-0.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 01:22:51.622756 sqlalchemy_celery_beat-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0     3156 2023-06-21 01:21:08.000000 sqlalchemy_celery_beat-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:22:51.568759 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      455 2023-06-21 01:21:13.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/clockedschedule.py
--rw-rw-rw-   0        0        0    21047 2023-06-20 14:53:43.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16320 2023-06-21 01:20:03.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     4171 2023-06-19 07:50:11.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1323 2023-06-20 12:52:02.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-20 02:26:17.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-21 01:22:51.619758 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0    10599 2023-06-21 01:22:51.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-21 01:22:51.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 01:22:51.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-21 01:22:51.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-21 01:22:51.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-21 01:22:51.000000 sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 01:43:09.178242 sqlalchemy_celery_beat-0.7.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0    10603 2023-06-25 01:43:09.179242 sqlalchemy_celery_beat-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9631 2023-06-25 01:42:42.000000 sqlalchemy_celery_beat-0.7.0/README.md
+-rw-rw-rw-   0        0        0      281 2023-06-25 01:43:09.186242 sqlalchemy_celery_beat-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     3156 2023-06-25 01:42:29.000000 sqlalchemy_celery_beat-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 01:43:09.129241 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      455 2023-06-25 01:41:58.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    21730 2023-06-25 00:49:12.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16457 2023-06-24 07:29:31.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     4171 2023-06-23 00:16:53.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-20 12:52:02.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-25 00:49:06.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-25 01:43:09.168240 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0    10603 2023-06-25 01:43:09.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-06-25 01:43:09.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 01:43:09.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-25 01:43:09.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-25 01:43:08.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-25 01:43:09.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-25 01:43:09.000000 sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 01:43:09.177242 sqlalchemy_celery_beat-0.7.0/tests/
+-rw-rw-rw-   0        0        0    11613 2023-06-25 01:33:32.000000 sqlalchemy_celery_beat-0.7.0/tests/test_crontab.py
+-rw-rw-rw-   0        0        0     4663 2023-06-25 01:27:22.000000 sqlalchemy_celery_beat-0.7.0/tests/test_models.py
+-rw-rw-rw-   0        0        0    26112 2023-06-25 01:27:22.000000 sqlalchemy_celery_beat-0.7.0/tests/test_schedulers.py
+-rw-rw-rw-   0        0        0     4812 2023-06-25 01:24:38.000000 sqlalchemy_celery_beat-0.7.0/tests/test_session.py
```

### Comparing `sqlalchemy_celery_beat-0.6.2/LICENSE` & `sqlalchemy_celery_beat-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.2/PKG-INFO` & `sqlalchemy_celery_beat-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -292,16 +292,16 @@
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
 - ✅ Implement a generic foreign key
 - ✅ More robust attribute validation on models
+- ✅ Add Tests
 - Add more examples
-- Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
 Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
```

### Comparing `sqlalchemy_celery_beat-0.6.2/README.md` & `sqlalchemy_celery_beat-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -273,16 +273,16 @@
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
 - ✅ Implement a generic foreign key
 - ✅ More robust attribute validation on models
+- ✅ Add Tests
 - Add more examples
-- Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
 Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
```

### Comparing `sqlalchemy_celery_beat-0.6.2/setup.py` & `sqlalchemy_celery_beat-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.6.2",
+    version="0.7.0",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
```

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/clockedschedule.py` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,19 +84,19 @@
     def update_changed(cls, mapper, connection: Connection, target):
         """
         :param mapper: the Mapper which is the target of this event
         :param connection: the Connection being used
         :param target: the mapped instance being persisted
         """
         logger.info('Database last time set to now')
-        s = connection.execute(select(PeriodicTaskChanged).
+        s = connection.scalar(select(PeriodicTaskChanged).
                                where(PeriodicTaskChanged.id == 1).limit(1))
         if not s:
-            s = connection.execute(insert(PeriodicTaskChanged),
-                                   last_update=maybe_make_aware(dt.datetime.utcnow()))
+            s = connection.execute(insert(PeriodicTaskChanged).
+                                   values(id=1, last_update=maybe_make_aware(dt.datetime.utcnow())))
         else:
             s = connection.execute(update(PeriodicTaskChanged).
                                    where(PeriodicTaskChanged.id == 1).
                                    values(last_update=maybe_make_aware(dt.datetime.utcnow())))
 
     @classmethod
     def update_from_session(cls, session: Session, commit: bool = True):
@@ -213,32 +213,46 @@
     """
     @property
     def schedule_model(self):
         """Provides in-Python access to the "parent" by choosing
         the appropriate relationship.
 
         """
-        return getattr(self, "model_%s" % self.discriminator)
+        if self.discriminator:
+            return getattr(self, "model_%s" % self.discriminator)
+        return None
 
     @schedule_model.setter
     def schedule_model(self, value):
         if value is not None:
             self.schedule_id = value.id
             self.discriminator = value.discriminator
+            for attribute, _ in self.__dict__.items():
+                if attribute.startswith('model_'):
+                    setattr(self, attribute, None)
             setattr(self, "model_%s" % value.discriminator, value)
+        else:
+            self.schedule_id = None
+            self.discriminator = None
+            for attribute, value in self.__dict__.items():
+                if attribute.startswith('model_'):
+                    setattr(self, attribute, None)
 
     @staticmethod
     def before_insert_or_update(mapper, connection, target):
         if target.enabled and isinstance(target.schedule_model, ClockedSchedule) and not target.one_off:
             raise ValueError("one_off must be True for clocked schedule")
         if target.expire_seconds is not None and target.expires:
             raise ValueError('Only one can be set, in expires and expire_seconds')
 
     def __repr__(self):
-        fmt = '{0.name}: {0.schedule_model}'
+        if self.schedule_model:
+            fmt = '{0.name}: {0.schedule_model}'
+        else:
+            fmt = '{0.name}: no schedule'
         return fmt.format(self)
 
     @property
     def expires_(self):
         return self.expires or self.expire_seconds
 
     @property
@@ -266,15 +280,16 @@
         primaryjoin=sa.and_(
             class_.id == foreign(remote(PeriodicTask.schedule_id)),
             PeriodicTask.discriminator == discriminator,
         ),
         backref=backref(
             "model_%s" % discriminator,
             primaryjoin=remote(class_.id) == foreign(PeriodicTask.schedule_id),
-            viewonly=True
+            viewonly=True,
+            lazy='selectin'
         ),
         overlaps='periodic_tasks',
         cascade="all, delete-orphan"
     )
 
     @event.listens_for(class_.periodic_tasks, "append")
     def append_periodic_tasks(target, value, initiator):
@@ -312,15 +327,15 @@
         doc='Interval Period',
         comment='The type of period between task runs (Example: days)'
     )
 
     def __repr__(self):
         if self.every == 1:
             return 'every {0}'.format(self.period_singular)
-        return 'every {0} {1}'.format(self.every, self.period)
+        return 'every {0} {1}'.format(self.every, Period(self.period).value)
 
     @property
     def schedule(self):
         return schedules.schedule(
             dt.timedelta(**{self.period: self.every}),
             # nowfun=lambda: make_aware(now())
             # nowfun=dt.datetime.now
@@ -335,15 +350,15 @@
             model = cls(every=every, period=period)
             session.add(model)
             session.commit()
         return model
 
     @property
     def period_singular(self):
-        return self.period[:-1]
+        return Period(self.period).value[:-1]
 
 
 class CrontabSchedule(ScheduleModel, ModelBase):
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
     minute = sa.Column(
         sa.String(60 * 4),
@@ -388,18 +403,21 @@
         nullable=False,
         default='UTC',
         doc='Cron Timezone',
         comment='Timezone to Run the Cron Schedule on. Default is UTC.'
     )
 
     def __repr__(self):
-        return '{0} {1} {2} {3} {4} (m/h/d/dM/MY) {5}'.format(
-            self.cronexp(self.minute), self.cronexp(self.hour),
-            self.cronexp(self.day_of_week), self.cronexp(self.day_of_month),
-            self.cronexp(self.month_of_year), str(self.timezone)
+        return '{0} {1} {2} {3} {4} (m/h/dM/MY/d) {5}'.format(
+            self.cronexp(self.minute),
+            self.cronexp(self.hour),
+            self.cronexp(self.day_of_month),
+            self.cronexp(self.month_of_year),
+            self.cronexp(self.day_of_week),
+            str(self.timezone)
         )
 
     @staticmethod
     def aware_crontab(obj):
         return TzAwareCrontab(
             minute=obj.minute,
             hour=obj.hour, day_of_week=obj.day_of_week,
@@ -410,15 +428,15 @@
 
     @property
     def schedule(self):
         return self.aware_crontab(self)
 
     @staticmethod
     def cronexp(value):
-        return value and re.sub(r"[\s\[\]\{\}]", '', str(value))
+        return (value and re.sub(r"[\s\[\]\{\}]", '', str(value))) or '*'
 
     @classmethod
     def from_schedule(cls, session, schedule):
         spec = {
             'minute': cls.cronexp(schedule._orig_minute),
             'hour': cls.cronexp(schedule._orig_hour),
             'day_of_week': cls.cronexp(schedule._orig_day_of_week),
@@ -434,30 +452,25 @@
             model = cls(**spec)
             session.add(model)
             session.commit()
         return model
 
     @staticmethod
     def before_insert_or_update(mapper, connection, target):
+        if not target.timezone:
+            target.timezone = 'UTC'
+        if target.timezone not in available_timezones():
+            raise ValueError(f'Timezone "{target.timezone}"  is not found in available timezones')
         try:
+            for k in ('minute', 'hour', 'day_of_week', 'day_of_month', 'month_of_year'):
+                setattr(target, k, CrontabSchedule.cronexp(getattr(target, k)))
             # Test the object to make sure it is valid before saving to DB
             CrontabSchedule.aware_crontab(target).remaining_estimate(dt.datetime.utcnow())
         except Exception as exc:
-            raise ValueError(f"Could not parse cron values: {str(exc)}") from exc
-
-    @validates('timezone')
-    def validate_crontab(self, key, value):
-        if value not in available_timezones():
-            raise ValueError(f'Timezone "{value}"  is not found in available timezones')
-        return value
-
-    @validates('minute', 'hour', 'day_of_week', 'day_of_month', 'month_of_year')
-    def validate_values(self, key, value):
-        value = self.cronexp(value)
-        return value
+            raise ValueError(f"Could not parse cron {target}: {str(exc)}") from exc
 
 
 class SolarSchedule(ScheduleModel, ModelBase):
 
     __table_args__ = (
         sa.UniqueConstraint('event', 'latitude', 'longitude'),
         sa.CheckConstraint(sa.column('latitude').between(-90, 90)),
@@ -510,15 +523,15 @@
             model = cls(**spec)
             session.add(model)
             session.commit()
         return model
 
     def __repr__(self):
         return '{0} ({1}, {2})'.format(
-            self.event,
+            self.event.replace('_', ' '),
             self.latitude,
             self.longitude
         )
 
 
 class ClockedSchedule(ScheduleModel, ModelBase):
```

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/schedulers.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,18 +362,21 @@
                     self.schedule[name].save()  # save to database
                     logger.debug(
                         '{name} save to database'.format(name=name))
                     _tried.add(name)
                 except (KeyError) as exc:
                     logger.error(exc)
                     _failed.add(name)
-        except sa.exc.IntegrityError as exc:
+        except sa.exc.DatabaseError as exc:
             logger.exception('Database error while sync: %r', exc)
-        except Exception as exc:
-            logger.exception(exc)
+        except sa.exc.InterfaceError as exc:
+            logger.warning(
+                'DatabaseScheduler: InterfaceError in sync(), '
+                'waiting to retry in next call...'
+            )
         finally:
             # retry later, only for the failed ones
             self._dirty |= _failed
 
     def update_from_dict(self, dict_):
         s = {}
         for name, entry_fields in dict_.items():
```

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/time_utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -292,16 +292,16 @@
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
 - ✅ Implement a generic foreign key
 - ✅ More robust attribute validation on models
+- ✅ Add Tests
 - Add more examples
-- Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
 Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
```

### Comparing `sqlalchemy_celery_beat-0.6.2/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.7.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 sqlalchemy_celery_beat/__init__.py
 sqlalchemy_celery_beat/clockedschedule.py
 sqlalchemy_celery_beat/models.py
 sqlalchemy_celery_beat/schedulers.py
 sqlalchemy_celery_beat/session.py
 sqlalchemy_celery_beat/time_utils.py
 sqlalchemy_celery_beat/tzcrontab.py
 sqlalchemy_celery_beat.egg-info/PKG-INFO
 sqlalchemy_celery_beat.egg-info/SOURCES.txt
 sqlalchemy_celery_beat.egg-info/dependency_links.txt
 sqlalchemy_celery_beat.egg-info/entry_points.txt
 sqlalchemy_celery_beat.egg-info/not-zip-safe
 sqlalchemy_celery_beat.egg-info/requires.txt
-sqlalchemy_celery_beat.egg-info/top_level.txt
+sqlalchemy_celery_beat.egg-info/top_level.txt
+tests/test_crontab.py
+tests/test_models.py
+tests/test_schedulers.py
+tests/test_session.py
```

