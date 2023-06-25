# Comparing `tmp/py_assimilator-1.2.3.tar.gz` & `tmp/py_assimilator-1.2.4.tar.gz`

## Comparing `py_assimilator-1.2.3.tar` & `py_assimilator-1.2.4.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/__init__.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/__init__.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/error_wrapper.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/model_utils.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/repository.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/specifications/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/database/specifications/specifications.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/outbox_relay.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/database/__init__.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/alchemy/events/database/repository.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/exceptions.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/exceptions.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/models.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/repository.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/__init__.py
--rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/adaptive.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/specifications.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/database/specifications/types.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/__init__.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/events.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/events_bus.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/exceptions.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/events/outbox_relay.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/__init__.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/context_managers.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/error_wrapper.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/patterns/lazy_command.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/services/__init__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/services/base.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/core/services/crud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/error_wrapper.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/models_utils.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/repository.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/__init__.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/filter_specifications.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/internal_operator.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/specifications.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/database/specifications/utils.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/events/__init__.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/internal/events/events_bus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/kafka_/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/kafka_/events/__init__.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/kafka_/events/events_bus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/__init__.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/error_wrapper.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/models.py
--rw-r--r--   0        0        0     5642 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/repository.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/unit_of_work.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/specifications/__init__.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/specifications/filtering_options.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/mongo/database/specifications/specifications.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/__init__.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/models.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/repository.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/database/unit_of_work.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/events/__init__.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/assimilator/redis_/events/events_bus.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/LICENSE.md
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/README.md
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 py_assimilator-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/__init__.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/error_wrapper.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/model_utils.py
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/repository.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/specifications/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     5766 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/database/specifications/specifications.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/events/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/events/outbox_relay.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/events/database/__init__.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/alchemy/events/database/repository.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/exceptions.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/exceptions.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/models.py
+-rw-r--r--   0        0        0     6186 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/repository.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/specifications/__init__.py
+-rw-r--r--   0        0        0     3372 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/specifications/adaptive.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/specifications/specifications.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/database/specifications/types.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/events/__init__.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/events/events.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/events/events_bus.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/events/exceptions.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/events/outbox_relay.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/patterns/__init__.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/patterns/context_managers.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/patterns/error_wrapper.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/patterns/lazy_command.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/services/__init__.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/services/base.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/core/services/crud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/error_wrapper.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/models_utils.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/repository.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/specifications/__init__.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/specifications/filter_specifications.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/specifications/internal_operator.py
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/specifications/specifications.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/database/specifications/utils.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/events/__init__.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/internal/events/events_bus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/kafka_/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/kafka_/events/__init__.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/kafka_/events/events_bus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/__init__.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/error_wrapper.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/models.py
+-rw-r--r--   0        0        0     5983 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/repository.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/unit_of_work.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/specifications/__init__.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/specifications/filtering_options.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/specifications/specifications.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/mongo/database/specifications/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/redis_/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/redis_/database/__init__.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/redis_/database/models.py
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/redis_/database/repository.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/redis_/database/unit_of_work.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/redis_/events/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/assimilator/redis_/events/events_bus.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/LICENSE.md
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/README.md
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     7677 2020-02-02 00:00:00.000000 py_assimilator-1.2.4/PKG-INFO
```

### Comparing `py_assimilator-1.2.3/assimilator/__init__.py` & `py_assimilator-1.2.4/assimilator/__init__.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/database/error_wrapper.py` & `py_assimilator-1.2.4/assimilator/alchemy/database/error_wrapper.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/database/model_utils.py` & `py_assimilator-1.2.4/assimilator/alchemy/database/model_utils.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/database/repository.py` & `py_assimilator-1.2.4/assimilator/alchemy/database/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,31 +74,29 @@
                     "to the update() yet provided specifications"
                 )
 
             query = self._apply_specifications(
                 query=update(self.model),
                 specifications=specifications,
             )
-
             self.session.execute(
                 query.values(update_values).execution_options(synchronize_session=False)
             )
 
         elif obj is not None:
             if obj not in self.session:
                 obj = self.session.merge(obj)
+                self.session.add(obj)
 
-            self.session.add(obj)
-
-    def dict_to_models(self, data: dict) -> dict:
-        return dict_to_alchemy_models(data=data, model=self.model)
+    def dict_to_models(self, data: dict) -> AlchemyModelT:
+        return self.model(**dict_to_alchemy_models(data=data, model=self.model))
 
     def save(self, obj: Optional[AlchemyModelT] = None, **data) -> AlchemyModelT:
         if obj is None:
-            obj = self.model(**self.dict_to_models(data))
+            obj = self.dict_to_models(data)
 
         self.session.add(obj)
         return obj
 
     def refresh(self, obj: AlchemyModelT) -> None:
         if obj not in self.session:
             obj = self.session.merge(obj)
```

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/database/unit_of_work.py` & `py_assimilator-1.2.4/assimilator/alchemy/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/database/specifications/filtering_options.py` & `py_assimilator-1.2.4/assimilator/alchemy/database/specifications/filtering_options.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/database/specifications/specifications.py` & `py_assimilator-1.2.4/assimilator/alchemy/database/specifications/specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/events/outbox_relay.py` & `py_assimilator-1.2.4/assimilator/alchemy/events/outbox_relay.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/alchemy/events/database/repository.py` & `py_assimilator-1.2.4/assimilator/alchemy/events/database/repository.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/database/models.py` & `py_assimilator-1.2.4/assimilator/core/database/models.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/database/repository.py` & `py_assimilator-1.2.4/assimilator/core/database/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         else:
             raise NotImplementedError("You must either pass the initial query or define get_initial_query()")
 
     def _get_specifications_context(self) -> Dict[str, Any]:
         return {"model": self.model, "repository": self}
 
     @abstractmethod
-    def dict_to_models(self, data: dict) -> dict:
+    def dict_to_models(self, data: dict) -> ModelT:
         """
         Converts data from Python dictionaries to models that Repository uses.
         You don't need to use that function directly 99% of the times.
         """
         raise NotImplementedError()
 
     @final
```

### Comparing `py_assimilator-1.2.3/assimilator/core/database/unit_of_work.py` & `py_assimilator-1.2.4/assimilator/core/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/database/specifications/adaptive.py` & `py_assimilator-1.2.4/assimilator/core/database/specifications/adaptive.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/database/specifications/filtering_options.py` & `py_assimilator-1.2.4/assimilator/core/database/specifications/filtering_options.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/database/specifications/specifications.py` & `py_assimilator-1.2.4/assimilator/core/database/specifications/specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/database/specifications/types.py` & `py_assimilator-1.2.4/assimilator/core/database/specifications/types.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/events/events.py` & `py_assimilator-1.2.4/assimilator/core/events/events.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/events/events_bus.py` & `py_assimilator-1.2.4/assimilator/core/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/events/outbox_relay.py` & `py_assimilator-1.2.4/assimilator/core/events/outbox_relay.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/patterns/context_managers.py` & `py_assimilator-1.2.4/assimilator/core/patterns/context_managers.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/patterns/error_wrapper.py` & `py_assimilator-1.2.4/assimilator/core/patterns/error_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,19 @@
             *self.error_mappings.values(),  # we want to skip all the mapped values as they are already fixed
         }
 
     def __enter__(self):
         return self
 
     def is_already_wrapped(self, exc_type: Type[Exception]) -> bool:
-        return any(issubclass(exc_type, error) for error in self.skipped_errors)
+        return any(
+            issubclass(exc_type, error)
+            for error in self.skipped_errors
+            if issubclass(error, Exception)
+        )
 
     def create_error(self, original_error: Exception, wrapped_error_type: Type[Exception]):
         _, _, tb = sys.exc_info()
         raise wrapped_error_type(original_error).with_traceback(tb)
 
     def __exit__(self, exc_type: Type[Exception], exc_val: Exception, exc_tb):
         if exc_val is None:
```

### Comparing `py_assimilator-1.2.3/assimilator/core/patterns/lazy_command.py` & `py_assimilator-1.2.4/assimilator/core/patterns/lazy_command.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/core/services/crud.py` & `py_assimilator-1.2.4/assimilator/core/services/crud.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,34 +21,33 @@
                 obj = self.uow.repository.save(obj_data)
 
             self.uow.commit()
 
         self.uow.repository.refresh(obj)
         return obj
 
-    def update(self, update_obj: Union[dict, ModelT], *filters, **kwargs_filters) -> ModelT:
+    def update(self, obj_data: Union[dict, ModelT], *filters, **kwargs_filters) -> ModelT:
         with self.uow:
-            if isinstance(update_obj, dict):
-                obj = self.get(*filters, **kwargs_filters)
+            if isinstance(obj_data, dict):
+                old_obj = self.get(*filters, **kwargs_filters)
+                parsed_obj = self.uow.repository.dict_to_models(obj_data)
 
-                update_obj = self.uow.repository.update(
-                    
-                )
+                for updated_key in obj_data:
+                    setattr(old_obj, updated_key, getattr(parsed_obj, updated_key))
 
-                obj.__dict__.update(update_obj.__dict__)
-                update_obj = obj
+                update_obj = old_obj
 
             self.uow.repository.update(update_obj)
             self.uow.commit()
 
         self.uow.repository.refresh(update_obj)
         return update_obj
 
     def list(
-        self, *filters, lazy: bool = False, **kwargs_filters,
+        self, *filters, lazy: bool = False, **kwargs_filters
     ) -> Union[Iterable[ModelT], LazyCommand[Iterable[ModelT]]]:
         return self.uow.repository.filter(self._specs.filter(*filters, **kwargs_filters), lazy=lazy)
 
     def get(self, *filters, lazy: bool = False, **kwargs_filters) -> Union[ModelT, LazyCommand[ModelT]]:
         return self.uow.repository.get(self._specs.filter(*filters, **kwargs_filters), lazy=lazy)
 
     def delete(self, *filters, **kwargs_filters) -> None:
```

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/models_utils.py` & `py_assimilator-1.2.4/assimilator/internal/database/models_utils.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/repository.py` & `py_assimilator-1.2.4/assimilator/internal/database/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,20 +70,20 @@
         initial_query: Optional[str] = None,
     ) -> Union[LazyCommand[List[ModelT]], List[ModelT]]:
         return list(self._apply_specifications(
             query=self.session.values(),
             specifications=specifications,
         ))
 
-    def dict_to_models(self, data: dict) -> dict:
-        return dict_to_internal_models(data=data, model=self.model)
+    def dict_to_models(self, data: dict) -> ModelT:
+        return self.model(**dict_to_internal_models(data=data, model=self.model))
 
     def save(self, obj: Optional[ModelT] = None, **obj_data) -> ModelT:
         if obj is None:
-            obj = self.model(**self.dict_to_models(obj_data))
+            obj = self.dict_to_models(obj_data)
 
         self.session[obj.id] = obj
         return obj
 
     def delete(self, obj: Optional[ModelT] = None, *specifications: SpecificationType) -> None:
         obj, specifications = self._check_obj_is_specification(obj, specifications)
```

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/unit_of_work.py` & `py_assimilator-1.2.4/assimilator/internal/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/specifications/filter_specifications.py` & `py_assimilator-1.2.4/assimilator/internal/database/specifications/filter_specifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         super(InternalFilter, self).__init__(
             *(set(filters) - set(self.text_filters)),
             **named_filters,
         )
 
     def __call__(self, query: QueryT, **context) -> Union[str, Generator[BaseModel, Any, None]]:
         if isinstance(query, str):
-            return f'{query}{"".join(self.text_filters)}'
+            return f'{query}{"".join(str(filter_) for filter_ in self.text_filters)}'
         elif not self.filters:
             return query
 
         return (
             model for model in query
             if all(filter_func(model) for filter_func in self.filters)
         )
```

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/specifications/filtering_options.py` & `py_assimilator-1.2.4/assimilator/internal/database/specifications/filtering_options.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/specifications/internal_operator.py` & `py_assimilator-1.2.4/assimilator/internal/database/specifications/internal_operator.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/specifications/specifications.py` & `py_assimilator-1.2.4/assimilator/internal/database/specifications/specifications.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/internal/database/specifications/utils.py` & `py_assimilator-1.2.4/assimilator/internal/database/specifications/utils.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/internal/events/events_bus.py` & `py_assimilator-1.2.4/assimilator/internal/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/kafka_/events/events_bus.py` & `py_assimilator-1.2.4/assimilator/kafka_/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/mongo/database/error_wrapper.py` & `py_assimilator-1.2.4/assimilator/mongo/database/error_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
         super(MongoErrorWrapper, self).__init__(
             error_mappings={
                 BSONError: ParsingError,
                 DuplicateKeyError: InvalidQueryError,
                 InvalidOperation: InvalidQueryError,
                 WriteError: InvalidQueryError,
             },
-            skipped_errors={NotFoundError},
+            skipped_errors={NotFoundError, DataLayerError},
             default_error=DataLayerError,
         )
 
 
 __all__ = ['MongoErrorWrapper']
```

### Comparing `py_assimilator-1.2.3/assimilator/mongo/database/repository.py` & `py_assimilator-1.2.4/assimilator/mongo/database/repository.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Optional, Collection, Type, TypeVar
+from typing import Union, Optional, Collection, Type, TypeVar, Any
 
 from pymongo import MongoClient
 
 from assimilator.mongo.database.models import MongoModel
 from assimilator.core.patterns import LazyCommand, ErrorWrapper
 from assimilator.mongo.database.error_wrapper import MongoErrorWrapper
 from assimilator.core.database import Repository, SpecificationType, \
@@ -10,14 +10,15 @@
 from assimilator.mongo.database.specifications.specifications import MongoSpecificationList
 from assimilator.internal.database.models_utils import dict_to_internal_models
 
 ModelT = TypeVar("ModelT", bound=MongoModel)
 
 
 class MongoRepository(Repository):
+    id: str = "_id"
     session: MongoClient
     model: Type[MongoModel]
 
     def __init__(
         self,
         session: MongoClient,
         model: Type[MongoModel],
@@ -34,16 +35,21 @@
             error_wrapper=error_wrapper or MongoErrorWrapper(),
         )
         self.database = database
 
     def get_initial_query(self, override_query: Optional[dict] = None) -> dict:
         return dict(super(MongoRepository, self).get_initial_query(override_query))
 
-    def dict_to_models(self, data: dict) -> dict:
-        return dict_to_internal_models(data, model=self.model)
+    def dict_to_models(self, data: dict) -> ModelT:
+        return self.model(**dict_to_internal_models(data, model=self.model))
+
+    @property
+    def _model_id_name(self):
+        config = getattr(self.model, 'AssimilatorConfig', None)
+        return "_id" if config is None else config.id_name
 
     @property
     def _collection_name(self):
         config = getattr(self.model, 'AssimilatorConfig', None)
         if config is not None:
             return self.model.AssimilatorConfig.collection
 
@@ -73,61 +79,63 @@
 
     def filter(
         self,
         *specifications: SpecificationType,
         lazy: bool = False,
         initial_query: dict = None
     ) -> Union[Collection[ModelT], LazyCommand[Collection[ModelT]]]:
-        query = self._apply_specifications(
-            query=initial_query,
-            specifications=specifications,
-        )
+        query = self._apply_specifications(query=initial_query, specifications=specifications)
         return [self.model(**data) for data in self._collection.find(**query)]
 
     def save(self, obj: Optional[ModelT] = None, **obj_data) -> ModelT:
         if obj is None:
-            obj = self.model(**self.dict_to_models(data=obj_data))
+            obj = self.dict_to_models(data=obj_data)
 
         self._collection.insert_one(obj.dict())
         return obj
 
     def delete(self, obj: Optional[ModelT] = None, *specifications: SpecificationType) -> None:
         obj, specifications = self._check_obj_is_specification(obj, specifications)
 
         if specifications:
+            id_name = self._model_id_name
             results = self._collection.find(**self._apply_specifications(
                 query=self.get_initial_query(),
-                specifications=(*specifications, self.specs.only('_id')),
+                specifications=(*specifications, self.specs.only(id_name)),
             ))
 
-            self._collection.delete_many({"_id": {"$in": [result['_id'] for result in results]}})
+            self._collection.delete_many({
+                id_name: {"$in": [result[id_name] for result in results]}
+            })
         elif obj is not None:
             self._collection.delete_one(obj.dict())
 
     def update(
         self,
         obj: Optional[ModelT] = None,
         *specifications: SpecificationType,
         **update_values,
     ) -> None:
         obj, specifications = self._check_obj_is_specification(obj, specifications)
 
         if specifications:
             results = self._collection.find(**self._apply_specifications(
                 query=self.get_initial_query(),
-                specifications=(*specifications, self.specs.only('_id')),
+                specifications=(*specifications, self.specs.only(self._model_id_name)),
             ))
 
             self._collection.update_many(
-                filter={"_id": {"$in": [result['_id'] for result in results]}},
+                filter={self._model_id_name: {"$in": [
+                    result[self._model_id_name] for result in results
+                ]}},
                 update={'$set': update_values},
             )
         elif obj is not None:
             self._collection.update_one(
-                {"id": obj.id},
+                {self._model_id_name: obj.id},
                 update={'$set': obj.dict()},
                 upsert=getattr('obj', 'upsert', False),
             )
 
     def is_modified(self, obj: ModelT) -> bool:
         return self.get(self.specs.filter(id=obj.id)) == obj
```

### Comparing `py_assimilator-1.2.3/assimilator/mongo/database/unit_of_work.py` & `py_assimilator-1.2.4/assimilator/mongo/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/mongo/database/specifications/specifications.py` & `py_assimilator-1.2.4/assimilator/mongo/database/specifications/specifications.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Optional, Collection
 
+from assimilator.mongo.database.specifications.utils import rename_mongo_id
 from assimilator.mongo.database.specifications.filtering_options import MongoFilteringOptions
 from assimilator.core.database import SpecificationList, FilterSpecification, specification, AdaptiveFilter
 
 
 class MongoFilter(FilterSpecification):
     filters: dict
     filtering_options_cls = MongoFilteringOptions
@@ -47,15 +48,15 @@
 mongo_filter = MongoFilter
 
 
 @specification
 def mongo_order(*clauses: str, query: dict, **_) -> dict:
     query['sort'] = query.get('sort', []) + [
         (column, -1 if column.startswith("-") else 1)
-        for column in clauses
+        for column in map(rename_mongo_id, clauses)
     ]
     return query
 
 
 @specification
 def mongo_paginate(
     *,
@@ -75,15 +76,15 @@
 @specification
 def mongo_join(*targets: Collection, query: dict, **join_args: dict) -> dict:
     return query
 
 
 @specification
 def mongo_only(*only_fields: str, query: dict, **_) -> dict:
-    query['projection'] = only_fields
+    query['projection'] = list(map(rename_mongo_id, only_fields))
     return query
 
 
 class MongoSpecificationList(SpecificationList):
     filter = MongoFilter
     order = mongo_order
     paginate = mongo_paginate
```

### Comparing `py_assimilator-1.2.3/assimilator/redis_/database/models.py` & `py_assimilator-1.2.4/assimilator/redis_/database/models.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/redis_/database/repository.py` & `py_assimilator-1.2.4/assimilator/redis_/database/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,31 +53,28 @@
 
     def get(
         self,
         *specifications: SpecificationType,
         lazy: bool = False,
         initial_query: Optional[str] = None,
     ) -> Union[LazyCommand[RedisModelT], RedisModelT]:
-        query = self._apply_specifications(
-            query=initial_query,
-            specifications=specifications,
-        ) or '*'
-
+        query = self._apply_specifications(query=initial_query, specifications=specifications) or '*'
         found_objects = self.session.mget(self.session.keys(query))
 
         if not all(found_objects):
             raise NotFoundError(f"{self} repository get() did not find any results with this query: {query}")
 
         parsed_objects = list(self._apply_specifications(
             query=[self.model.loads(found_object) for found_object in found_objects],
             specifications=specifications,
         ))
 
         if not parsed_objects:
-            raise NotFoundError(f"{self} repository get() did not find any results with this query: {query}")
+            raise NotFoundError(f"{self} repository get() did not find "
+                                f"any results with this query: {query}")
         elif len(parsed_objects) != 1:
             raise MultipleResultsError(f"{self} repository get() did not"
                                        f" find any results with this query: {query}")
 
         return parsed_objects[0]
 
     def filter(
@@ -99,20 +96,20 @@
         if isinstance(self.model, BaseModel):
             query = [self.model.loads(value) for value in models]
         else:
             query = [self.model(**json.loads(value)) for value in models]
 
         return list(self._apply_specifications(specifications=specifications, query=query))
 
-    def dict_to_models(self, data: dict) -> dict:
-        return dict_to_internal_models(data=data, model=self.model)
+    def dict_to_models(self, data: dict) -> RedisModelT:
+        return self.model(**dict_to_internal_models(data=data, model=self.model))
 
     def save(self, obj: Optional[RedisModelT] = None, **obj_data) -> RedisModelT:
         if obj is None:
-            obj = self.model(**self.dict_to_models(data=obj_data))
+            obj = self.dict_to_models(data=obj_data)
 
         self.transaction.set(
             name=obj.id,
             value=obj.json(),
             ex=getattr(obj, 'expire_in', None),     # for Pydantic model compatability
             px=getattr(obj, 'expire_in_px', None),
             nx=getattr(obj, 'only_create', False),
```

### Comparing `py_assimilator-1.2.3/assimilator/redis_/database/unit_of_work.py` & `py_assimilator-1.2.4/assimilator/redis_/database/unit_of_work.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/assimilator/redis_/events/events_bus.py` & `py_assimilator-1.2.4/assimilator/redis_/events/events_bus.py`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/.gitignore` & `py_assimilator-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/LICENSE.md` & `py_assimilator-1.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/README.md` & `py_assimilator-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `py_assimilator-1.2.3/pyproject.toml` & `py_assimilator-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ignore-vcs = true
 include = [
     "assimilator"
 ]
 
 [project]
 name = "py_assimilator"
-version = "1.2.3"
+version = "1.2.4"
 authors = [
   { name="Andrey Ivanov", email="python.on.papyrus@gmail.com" },
 ]
 maintainers = [
   { name="Andrey Ivanov", email="python.on.papyrus@gmail.com" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "Events", "Architecture", "Patterns", "Backend"]
```

### Comparing `py_assimilator-1.2.3/PKG-INFO` & `py_assimilator-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_assimilator
-Version: 1.2.3
+Version: 1.2.4
 Summary: The best Domain-driven design patterns for your projects
 Project-URL: Documentation, https://knucklesuganda.github.io/py_assimilator/
 Project-URL: Github, https://github.com/knucklesuganda/py_assimilator/
 Project-URL: Youtube RU, https://www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw
 Project-URL: Youtube ENG, https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA
 Author-email: Andrey Ivanov <python.on.papyrus@gmail.com>
 Maintainer-email: Andrey Ivanov <python.on.papyrus@gmail.com>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py_assimilator Version: 1.2.3 Summary: The best
+Metadata-Version: 2.1 Name: py_assimilator Version: 1.2.4 Summary: The best
 Domain-driven design patterns for your projects Project-URL: Documentation,
 https://knucklesuganda.github.io/py_assimilator/ Project-URL: Github, https://
 github.com/knucklesuganda/py_assimilator/ Project-URL: Youtube RU, https://
 www.youtube.com/channel/UCSNpJHMOU7FqjD4Ttux0uuw Project-URL: Youtube ENG,
 https://www.youtube.com/channel/UCeC9LNDwRP9OfjyOFHaSikA Author-email: Andrey
 Ivanov
 on.papyrus@gmail.com> Maintainer-email: Andrey Ivanov
```

