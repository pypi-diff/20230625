# Comparing `tmp/jellyash-0.4.0.tar.gz` & `tmp/jellyash-0.4.1.tar.gz`

## Comparing `jellyash-0.4.0.tar` & `jellyash-0.4.1.tar`

### file list

```diff
@@ -1,307 +1,46 @@
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jellyash-0.4.0/tox.ini
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0   177663 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    52396 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    18223 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   170956 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0   111332 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_operator.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_operator.meta.json
--rw-r--r--   0        0        0    23358 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0   149720 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/argparse.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/argparse.meta.json
--rw-r--r--   0        0        0    60683 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1054946 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   123324 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   104156 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    57608 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0     4907 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    40359 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dis.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/dis.meta.json
--rw-r--r--   0        0        0    61016 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    22395 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/getpass.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/getpass.meta.json
--rw-r--r--   0        0        0   339721 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/inspect.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/inspect.meta.json
--rw-r--r--   0        0        0    85344 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0    28774 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    78978 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/opcode.data.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/opcode.meta.json
--rw-r--r--   0        0        0    46568 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/operator.data.json
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/operator.meta.json
--rw-r--r--   0        0        0    88250 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    44389 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    34948 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/platform.data.json
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/platform.meta.json
--rw-r--r--   0        0        0    75204 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0   167171 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    14127 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    28009 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    49438 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   157890 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   140040 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   228226 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   417108 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73945 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    33582 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/uuid.data.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/uuid.meta.json
--rw-r--r--   0        0        0    89061 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   407995 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   128990 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7434 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25069 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    79277 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    30853 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70171 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    64567 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    90273 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11931 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/jellyash/__init__.data.json
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/jellyash/__init__.meta.json
--rw-r--r--   0        0        0    15375 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/__init__.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/__init__.meta.json
--rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/decoder.data.json
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/decoder.meta.json
--rw-r--r--   0        0        0    10880 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/encoder.data.json
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/json/encoder.meta.json
--rw-r--r--   0        0        0   350174 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 jellyash-0.4.0/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1161349852a407df
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/11fe4e56a1a0998f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/12eed7b0df0436e1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/139b0884db11e1e8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/143665f5d7894aaf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1463469ef69bf78e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/16cb39ad3861193e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1919e19d29d7caa0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/19b2b937d1a7ab43
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1d70761d4d816b30
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1dd3bcd5629284a8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1efcba8af52f7427
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1f2e9a081c8f8f99
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/1fd53c5cd1e0cb59
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/208903efda15df61
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/20e749519f49b18e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2673cfaf4403e190
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/278d08fe3071dc9d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/27e6962f095a9afa
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2ce46804cb25434d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2dc240553e4605e6
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2f2e286f4d93fe12
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/2f8d01deff758aca
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/344663dba662e101
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/369321b91d77fd86
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3a082fd391280242
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3b0f5f3f4ca662f2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3c6eb77fc9daaf4b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/3ec68bfe2bd02760
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/411c11eda0979215
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/41528c30d4c7c82e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/41e7b66b53d2a24c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/422079b659902906
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/426cd6790b31a273
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/43e057b3dcc43e96
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/49a5af4645b42506
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/4c9e958d28374767
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/5001be39813f2835
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/5017eb9f3edaf502
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/521750f423c285e6
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/52b08a05f3469c2
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/53abdaef3ad7e08e
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/562cf0d217c2e526
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/563b1ff8799d6d2f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/58136763caf87fdc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/581c717c582cac6d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/59fa0f38996b9d60
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/5aa88ef31443a878
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6201111bf7b60a76
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/625181274b029d67
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/62b82a00fa7de2b5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/62ed103883955520
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/655a1e70b9bf2246
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/669a75b0670c256b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/68382171887c4592
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6a5d72074f987be1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6a6da80531cfbb45
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6c280475c487a449
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6ca710681f0db6fb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6d1f6902c744386f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6fb1dd7faeee0f98
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/6fd8649e4e08a08
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/72ebc4636e7ac7be
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/73f0aac8fb55b6ba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/77a336face0ec4f1
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/7d930974c8e253d8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/7dbd668b9f492d3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/7f4b4829ba20a516
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8117798897b9ed6d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8260832a118d10dc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8305556502d2ea45
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8475b82408d2ee54
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/855a7b58ef0544ec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/86c3273e51072d3c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/877853d4dc81f361
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/88dbf7a942a9da64
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/89d595309b4b7b68
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/8e8cefaabb8a4bb8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/95ca40290aa6c953
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/95fd5ea7b9e5dfb3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/9db82954adbe850b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/9f504d0ffc92dcfb
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a1142c359e181a9d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a1a41619be06ccb4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a24137a45a8743b1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a2f215bbc4cc0d40
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a4787245a21ffe63
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a4875c83cb7271f0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a54359630edfacd6
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a68ba8f5f87dc608
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/a924d16624f6adf
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/abf21f3f84ad1df4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ae41f6f26033f4bc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/af9b4ba2d0453cda
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b1152a95cbf2d4f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b16ef8eaf80b86ad
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b2fe59c75a454b7e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/b782bb5920ed7631
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ba44a3c3b3ac38d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c07ac676dcd21496
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c1d760c0cfb41438
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c276d1d063a64727
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c647c1c6c09ad625
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c85f693897ea918c
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c8c3aed8bad1198b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/c91989c6d2d7a8a4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cd137e47823314dd
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cdc22caf17ec54d3
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ce702570cde74416
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cef88f7047b583d7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/cf82bbe7c7c1adf9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/d1d46e5a18de7d3a
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/d446985a27be26f4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/d4fc514a2f18d78
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/dc6404189af0c24c
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/dc6c6508ff33b09a
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/de63806b2b73c0f6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/def645b0042e6c87
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e0fec072417f247c
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e3414fe664479570
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e63ec54ef0702676
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e762d40f1905c5a1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e8da77cd8ff6c797
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/e928828d422ec175
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ea455768c753b5d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/eb90c6985bd660dc
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ec8abef61a13d59f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/efab3295776f4a9d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f0214717fe422ca0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f2daa6f6d8a29e8d
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f378cd188d3b89c7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f44daa5adc10db55
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f45513d4e62e04c1
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f502d4daab623491
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f7c55dccb7414089
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/f9d56765099deab8
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/fc57508d0201a413
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/fd85a9498d4d4764
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/fdad3b8deea4269
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 jellyash-0.4.0/.ruff_cache/content/ffaf3bb26cb3b723
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/__init__.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/bundle.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/client.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/duration.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/nextup.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/search.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/token.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 jellyash-0.4.0/jellyash/unwatched.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_bundle.py
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_client.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_duration.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_nextup.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_search.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_token.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/test_unwatched.py
--rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_bundle/TestApiResponse.client.yaml
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml
--rw-r--r--   0        0        0     7518 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_client/TestAuthedClient.client.yaml
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.client.yaml
--rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml
--rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_single_term.yaml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_term_not_found.yaml
--rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.client.yaml
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jellyash-0.4.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jellyash-0.4.0/LICENSE
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 jellyash-0.4.0/README.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jellyash-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 jellyash-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 jellyash-0.4.1/tox.ini
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 jellyash-0.4.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/bundle.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/client.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/duration.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/nextup.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/search.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/token.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 jellyash-0.4.1/jellyash/unwatched.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/test_bundle.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/test_client.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/test_duration.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/test_nextup.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/test_search.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/test_token.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/test_unwatched.py
+-rw-r--r--   0        0        0     7508 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_bundle/TestApiResponse.client.yaml
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml
+-rw-r--r--   0        0        0     7600 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_bundle/TestUnwrappedApiResponse.client.yaml
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_bundle/TestUnwrappedApiResponse.test_unwrapped_response.yaml
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_client/TestAuthedClient.client.yaml
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_duration/TestDuration.client.yaml
+-rw-r--r--   0        0        0     9732 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_search/TestSearch.test_single_term.yaml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_search/TestSearch.test_term_not_found.yaml
+-rw-r--r--   0        0        0     7407 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.client.yaml
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jellyash-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jellyash-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 jellyash-0.4.1/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 jellyash-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 jellyash-0.4.1/PKG-INFO
```

### Comparing `jellyash-0.4.0/jellyash/bundle.py` & `jellyash-0.4.1/jellyash/bundle.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,9 +44,12 @@
 
     def __len__(self) -> int:
         return self.value["TotalRecordCount"] + self.value["StartIndex"]
 
 
 class WrappedAPI(API):
     def _get(self, handler, params=None):
-        return ApiResponse(super()._get(handler, params=params))
+        resp = super()._get(handler, params=params)
+        if set(("Items", "TotalRecordCount")) <= set(resp.keys()):
+            return ApiResponse(resp)
+        return resp
```

### Comparing `jellyash-0.4.0/jellyash/client.py` & `jellyash-0.4.1/jellyash/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import inspect
 import json
+from json.decoder import JSONDecodeError
 import pathlib
 import platform
 import sys
 from typing import Optional
 from uuid import uuid4
 
 from jellyfin_apiclient_python.client import JellyfinClient
+from jellyfin_apiclient_python.connection_manager import CONNECTION_STATE
 
 from . import __version__
 from .bundle import WrappedAPI
 
 CREDENTIALS_FILE = pathlib.Path.home() / ".jellyfin_creds"
 
 
@@ -30,23 +32,27 @@
 
 
 def auth_with_token(client) -> None:
     if not CREDENTIALS_FILE.is_file():
         raise ValueError(f"{sys.argv[0]}: Requires credential file.")
     with open(CREDENTIALS_FILE, "r") as f:
         credentials = json.load(f)
-    client.authenticate({"Servers": [credentials]}, discover=False)
+    state = client.authenticate({"Servers": [credentials]}, discover=False)
+    if state["State"] != CONNECTION_STATE["SignedIn"]:
+        raise ConnectionError("Failed to establish connection")
 
 
 def authed_client():
     client = create_client(None)
     try:
         auth_with_token(client)
-    except (PermissionError, ValueError, json.decoder.JSONDecodeError) as e:
-        print(e)
+    except (
+        PermissionError, ValueError, JSONDecodeError, ConnectionError
+        ) as e:
+        print(f"{sys.argv[0]}: {e}")
         sys.exit(1)
     return client
 
 
 def determine_app_name() -> str:
     frame = inspect.stack()[-2]
     return f"jellyfin_{inspect.getmodulename(frame.filename)}"
```

### Comparing `jellyash-0.4.0/jellyash/duration.py` & `jellyash-0.4.1/jellyash/duration.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/jellyash/nextup.py` & `jellyash-0.4.1/jellyash/nextup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 
 from .bundle import Item
 from .client import authed_client
 
 
 def episode_str(episode: Item) -> str:
-    seasonindex = f"{episode.ParentIndexNumber}x{episode.IndexNumber:02}"
+    seasonindex = f"{episode.ParentIndexNumber}x{episode.IndexNumber:0>2}"
     return f"{episode.SeriesName} [{seasonindex}] {episode.Name}"
 
 
 def nextup() -> None:
     client = authed_client()
     parser = argparse.ArgumentParser()
     parser.add_argument("-l", "--limit", dest="limit", type=int, default=30)
```

### Comparing `jellyash-0.4.0/jellyash/token.py` & `jellyash-0.4.1/jellyash/token.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/jellyash/unwatched.py` & `jellyash-0.4.1/jellyash/unwatched.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 
 def all_unwatched(client) -> None:
     r = client.jellyfin.search_media_items(
         term="", media="Series", limit=300
     )
     total = 0
     for series in sorted(r, key=attrgetter("Name")):
-        if (count := series.UserData.UnplayedItemCount) > 0:
+        count = series.UserData.UnplayedItemCount
+        if count > 0:
             ending = "s" if count != 1 else ""
             print(f"{series.Name}: {count} unwatched episode{ending}")
             total += count
     ending = "s" if total != 1 else ""
     print(f"Total: {total} unwatched episode{ending}")
```

### Comparing `jellyash-0.4.0/tests/conftest.py` & `jellyash-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/test_bundle.py` & `jellyash-0.4.1/tests/test_bundle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import pytest
 
-from jellyash.bundle import Item
+from jellyash.bundle import ApiResponse, Item
 from .conftest import ClientTest
 
 
 class TestItem(unittest.TestCase):
     def test_item(self):
         item = {"User": "demo"}
         wrapped = Item(item)
@@ -56,7 +56,15 @@
             "18 - The Passenger of the 'Atlanta'",
             "14 - Pickaxe and Trowel",
             "31 - Part II, Chapter 26: Bow and Arrow",
             "22 - The New Citizen of the United States"
         ]
         self.assertSequenceEqual([m.Name for m in self.search_result], names)
 
+
+class TestUnwrappedApiResponse(ClientTest):
+    @pytest.mark.vcr
+    def test_unwrapped_response(self):
+        resp = self.test_client.jellyfin.try_server()
+        self.assertFalse(isinstance(resp, ApiResponse))
+        self.assertEqual(resp["ServerName"], "Stable Demo")
+
```

### Comparing `jellyash-0.4.0/tests/test_client.py` & `jellyash-0.4.1/tests/test_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import pathlib
 import platform
 import tempfile
 import unittest
-from unittest.mock import patch
+from unittest.mock import patch, Mock
 
 from jellyfin_apiclient_python.client import JellyfinClient
 import pytest
 
 from jellyash import __version__
 from jellyash.client import (
     authed_client, auth_with_password, auth_with_token, create_client,
@@ -29,18 +29,15 @@
     
     @pytest.mark.vcr
     def test_auth_with_password(self):
         server_url = "https://demo.jellyfin.org/stable"
         auth_result = auth_with_password(self.client, server_url, "demo", "")
         self.assertEqual(auth_result["User"]["Name"], "demo")
         self.assertEqual(auth_result["SessionInfo"]["UserName"], "demo")
-        self.assertEqual(
-            auth_result["SessionInfo"]["DeviceName"],
-            platform.node()
-        )
+        self.assertEqual(auth_result["SessionInfo"]["DeviceName"], "wrecked")
 
 
 class TestAuthWithToken(unittest.TestCase):
     def test_auth_with_token_credential_directory(self):
         with tempfile.TemporaryDirectory() as tempdir:
             ptd = pathlib.Path(tempdir)
             with patch("jellyash.client.CREDENTIALS_FILE", ptd):
@@ -55,42 +52,75 @@
                 with self.assertRaises(PermissionError):
                     auth_with_token(None)
             ptf.chmod(0o600)
 
     def test_auth_with_token_invalid_json(self):
         with tempfile.NamedTemporaryFile() as tmpfile:
             tmpfile.file.write(b"{{\n")
+            tmpfile.file.flush()
             ptf = pathlib.Path(tmpfile.name)
             with patch("jellyash.client.CREDENTIALS_FILE", ptf):
                 with self.assertRaises(json.decoder.JSONDecodeError):
                     auth_with_token(None)
 
     def test_auth_with_nonexistant_file(self):
         non_exist = pathlib.Path("/does/not/exist")
         with patch("jellyash.client.CREDENTIALS_FILE", non_exist):
             with self.assertRaises(ValueError):
                 auth_with_token(None)
 
+    def test_auth_with_state_zero(self):
+        with tempfile.NamedTemporaryFile() as tmpfile:
+            tmpfile.file.write(b"{\"User\": \"foo\"}\n")
+            tmpfile.file.flush()
+            ptf = pathlib.Path(tmpfile.name)
+            with patch("jellyash.client.CREDENTIALS_FILE", ptf):
+                client_mock = Mock()
+                client_mock.authenticate.return_value = {"State": 0}
+                with self.assertRaises(ConnectionError):
+                    auth_with_token(client_mock)
+                client_mock.authenticate.assert_called_once()
+
 
 class TestAuthedClient(ClientTest):
+    @pytest.fixture(autouse=True)
+    def capsys(self, capsys):
+        self.capsys = capsys
+
     @pytest.mark.vcr
     def test_authed_client(self):
         with tempfile.NamedTemporaryFile() as tmpfile:
             credentials = self.test_client.auth.credentials.get_credentials()
             with open(tmpfile.name, 'w') as f:
                 json.dump(credentials["Servers"][0], f)
             ptf = pathlib.Path(tmpfile.name)
             with patch("jellyash.client.CREDENTIALS_FILE", ptf):
                 client = authed_client()
                 self.assertTrue(isinstance(client, JellyfinClient))
 
+    @pytest.mark.vcr
+    def test_authed_client_offline(self):
+        with tempfile.NamedTemporaryFile() as tmpfile:
+            credentials = self.test_client.auth.credentials.get_credentials()
+            with open(tmpfile.name, 'w') as f:
+                json.dump(credentials["Servers"][0], f)
+            ptf = pathlib.Path(tmpfile.name)
+            with patch("jellyash.client.CREDENTIALS_FILE", ptf):
+                with patch("sys.argv", ["test_offline"]):
+                    with self.assertRaises(SystemExit):
+                        authed_client()
+        captured = self.capsys.readouterr()
+        self.assertEqual(
+            captured.out, "test_offline: Failed to establish connection\n"
+            )
+        self.assertEqual(captured.err, "")
+
     def test_authed_client_non_existant_file(self):
         non_exist = pathlib.Path("/does/not/exist")
         with patch("jellyash.client.CREDENTIALS_FILE", non_exist):
-            with patch("sys.exit", return_value=None) as mock_exit:
+            with self.assertRaises(SystemExit):
                 authed_client()
-                mock_exit.assert_called_once()
 
 
 class TestDetermineAppName(unittest.TestCase):
     def test_determine_app_name(self):
         self.assertEqual(determine_app_name(), "jellyfin___init__")
```

### Comparing `jellyash-0.4.0/tests/test_duration.py` & `jellyash-0.4.1/tests/test_duration.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/test_nextup.py` & `jellyash-0.4.1/tests/test_nextup.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/test_search.py` & `jellyash-0.4.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/test_token.py` & `jellyash-0.4.1/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/test_unwatched.py` & `jellyash-0.4.1/tests/test_unwatched.py`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_bundle/TestApiResponse.client.yaml` & `jellyash-0.4.1/tests/cassettes/test_bundle/TestApiResponse.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml` & `jellyash-0.4.1/tests/cassettes/test_bundle/TestApiResponse.setUp.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_client/TestAuthedClient.client.yaml` & `jellyash-0.4.1/tests/cassettes/test_client/TestAuthedClient.client.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -9,43 +9,43 @@
       Accept-encoding:
       - gzip
       Connection:
       - keep-alive
       Content-type:
       - application/x-www-form-urlencoded; charset=UTF-8
       User-Agent:
-      - jellyash_test_testauthedclient/0.3.4
+      - jellyash_test_testauthedclient/0.4.0
       X-Application:
-      - jellyash_test_testauthedclient/0.3.4
+      - jellyash_test_testauthedclient/0.4.0
       x-emby-authorization:
-      - MediaBrowser Client=jellyash_test_testauthedclient, Device=wrecked, DeviceId=a83dd3cd-21b6-47b7-aa58-33024978d5e4,
-        Version=0.3.4
+      - MediaBrowser Client=jellyash_test_testauthedclient, Device=wrecked, DeviceId=2c04707d-5fce-4c46-89ad-fd705a2187d9,
+        Version=0.4.0
     method: GET
     uri: https://demo.jellyfin.org/stable/system/info/public
   response:
     body:
       string: '{"LocalAddress":"http://172.17.0.2:8096/stable","ServerName":"Stable
         Demo","Version":"10.8.10","ProductName":"Jellyfin Server","OperatingSystem":"Linux","Id":"713dc3fe952b438fa70ed35e4ef0525a","StartupWizardCompleted":true}'
     headers:
       content-type:
       - application/json; charset=utf-8
       date:
-      - Sat, 13 May 2023 02:42:16 GMT
+      - Tue, 20 Jun 2023 10:30:26 GMT
       referrer-policy:
       - no-referrer,same-origin,strict-origin,strict-origin-when-cross-origin
       server:
       - Kestrel
       strict-transport-security:
       - max-age=31536000;includeSubDomains;preload
       transfer-encoding:
       - chunked
       x-content-type-options:
       - nosniff
       x-response-time-ms:
-      - '1'
+      - '2'
       x-xss-protection:
       - 1;mode=block
     status:
       code: 200
       message: OK
 - request:
     body: null
@@ -57,43 +57,43 @@
       Accept-encoding:
       - gzip
       Connection:
       - keep-alive
       Content-type:
       - application/x-www-form-urlencoded; charset=UTF-8
       User-Agent:
-      - jellyash_test_testauthedclient/0.3.4
+      - jellyash_test_testauthedclient/0.4.0
       X-Application:
-      - jellyash_test_testauthedclient/0.3.4
+      - jellyash_test_testauthedclient/0.4.0
       x-emby-authorization:
-      - MediaBrowser Client=jellyash_test_testauthedclient, Device=wrecked, DeviceId=a83dd3cd-21b6-47b7-aa58-33024978d5e4,
-        Version=0.3.4
+      - MediaBrowser Client=jellyash_test_testauthedclient, Device=wrecked, DeviceId=2c04707d-5fce-4c46-89ad-fd705a2187d9,
+        Version=0.4.0
     method: GET
     uri: https://demo.jellyfin.org/stable/system/info/public
   response:
     body:
       string: '{"LocalAddress":"http://172.17.0.2:8096/stable","ServerName":"Stable
         Demo","Version":"10.8.10","ProductName":"Jellyfin Server","OperatingSystem":"Linux","Id":"713dc3fe952b438fa70ed35e4ef0525a","StartupWizardCompleted":true}'
     headers:
       content-type:
       - application/json; charset=utf-8
       date:
-      - Sat, 13 May 2023 02:42:17 GMT
+      - Tue, 20 Jun 2023 10:30:26 GMT
       referrer-policy:
       - no-referrer,same-origin,strict-origin,strict-origin-when-cross-origin
       server:
       - Kestrel
       strict-transport-security:
       - max-age=31536000;includeSubDomains;preload
       transfer-encoding:
       - chunked
       x-content-type-options:
       - nosniff
       x-response-time-ms:
-      - '1'
+      - '0'
       x-xss-protection:
       - 1;mode=block
     status:
       code: 200
       message: OK
 - request:
     body: '{"username": "demo", "Pw": ""}'
@@ -107,41 +107,41 @@
       Connection:
       - keep-alive
       Content-Length:
       - '30'
       Content-type:
       - application/json
       User-Agent:
-      - jellyash_test_testauthedclient/0.3.4
+      - jellyash_test_testauthedclient/0.4.0
       X-Application:
-      - jellyash_test_testauthedclient/0.3.4
+      - jellyash_test_testauthedclient/0.4.0
       x-emby-authorization:
-      - MediaBrowser Client=jellyash_test_testauthedclient, Device=wrecked, DeviceId=a83dd3cd-21b6-47b7-aa58-33024978d5e4,
-        Version=0.3.4
+      - MediaBrowser Client=jellyash_test_testauthedclient, Device=wrecked, DeviceId=2c04707d-5fce-4c46-89ad-fd705a2187d9,
+        Version=0.4.0
     method: POST
     uri: https://demo.jellyfin.org/stable/Users/AuthenticateByName
   response:
     body:
-      string: '{"User":{"Name":"demo","ServerId":"713dc3fe952b438fa70ed35e4ef0525a","Id":"a076a5bfc9034f379f5889bc6dafc77b","HasPassword":false,"HasConfiguredPassword":false,"HasConfiguredEasyPassword":true,"EnableAutoLogin":false,"LastLoginDate":"2023-05-13T02:42:18.9307019Z","LastActivityDate":"2023-05-13T02:42:18.9307019Z","Configuration":{"AudioLanguagePreference":"","PlayDefaultAudioTrack":true,"SubtitleLanguagePreference":"dut","DisplayMissingEpisodes":true,"GroupedFolders":["f137a2dd21bbc1b99aa5c0f6bf02a805","767bffe4f11c93ef34b805451a696a4e"],"SubtitleMode":"Always","DisplayCollectionsView":false,"EnableLocalPassword":true,"OrderedViews":["b6239cb8a74ff47b07bbf770d40a8e56","f137a2dd21bbc1b99aa5c0f6bf02a805","7e64e319657a9516ec78490da03edccb","767bffe4f11c93ef34b805451a696a4e","9d7ad6afe9afa2dab1a2f6e00ad28fa6"],"LatestItemsExcludes":[],"MyMediaExcludes":["9d7ad6afe9afa2dab1a2f6e00ad28fa6"],"HidePlayedInLatest":false,"RememberAudioSelections":true,"RememberSubtitleSelections":true,"EnableNextEpisodeAutoPlay":true},"Policy":{"IsAdministrator":false,"IsHidden":true,"IsDisabled":false,"BlockedTags":[],"EnableUserPreferenceAccess":true,"AccessSchedules":[],"BlockUnratedItems":[],"EnableRemoteControlOfOtherUsers":false,"EnableSharedDeviceControl":false,"EnableRemoteAccess":true,"EnableLiveTvManagement":false,"EnableLiveTvAccess":true,"EnableMediaPlayback":true,"EnableAudioPlaybackTranscoding":true,"EnableVideoPlaybackTranscoding":true,"EnablePlaybackRemuxing":true,"ForceRemoteSourceTranscoding":false,"EnableContentDeletion":false,"EnableContentDeletionFromFolders":[],"EnableContentDownloading":true,"EnableSyncTranscoding":true,"EnableMediaConversion":true,"EnabledDevices":[],"EnableAllDevices":true,"EnabledChannels":[],"EnableAllChannels":true,"EnabledFolders":[],"EnableAllFolders":true,"InvalidLoginAttemptCount":0,"LoginAttemptsBeforeLockout":-1,"MaxActiveSessions":0,"EnablePublicSharing":false,"BlockedMediaFolders":[],"BlockedChannels":[],"RemoteClientBitrateLimit":0,"AuthenticationProviderId":"Jellyfin.Server.Implementations.Users.DefaultAuthenticationProvider","PasswordResetProviderId":"Jellyfin.Server.Implementations.Users.DefaultPasswordResetProvider","SyncPlayAccess":"CreateAndJoinGroups"}},"SessionInfo":{"PlayState":{"CanSeek":false,"IsPaused":false,"IsMuted":false,"RepeatMode":"RepeatNone"},"AdditionalUsers":[],"Capabilities":{"PlayableMediaTypes":[],"SupportedCommands":[],"SupportsMediaControl":false,"SupportsContentUploading":false,"SupportsPersistentIdentifier":true,"SupportsSync":false},"RemoteEndPoint":"2403:5807:3a:0:1e79:6f72:cc02:5647","PlayableMediaTypes":[],"Id":"2bb007d80776989f500f158f94b29c54","UserId":"a076a5bfc9034f379f5889bc6dafc77b","UserName":"demo","Client":"jellyash_test_testauthedclient","LastActivityDate":"2023-05-13T02:42:18.9633434Z","LastPlaybackCheckIn":"0001-01-01T00:00:00.0000000Z","DeviceName":"wrecked","DeviceId":"a83dd3cd-21b6-47b7-aa58-33024978d5e4","ApplicationVersion":"0.3.4","IsActive":true,"SupportsMediaControl":false,"SupportsRemoteControl":false,"NowPlayingQueue":[],"NowPlayingQueueFullItems":[],"HasCustomDeviceName":false,"ServerId":"713dc3fe952b438fa70ed35e4ef0525a","SupportedCommands":[]},"AccessToken":"d1912d06a0e146d4bb4dc2244df9287c","ServerId":"713dc3fe952b438fa70ed35e4ef0525a"}'
+      string: '{"User":{"Name":"demo","ServerId":"713dc3fe952b438fa70ed35e4ef0525a","Id":"a076a5bfc9034f379f5889bc6dafc77b","HasPassword":false,"HasConfiguredPassword":false,"HasConfiguredEasyPassword":true,"EnableAutoLogin":false,"LastLoginDate":"2023-06-20T10:30:27.9183696Z","LastActivityDate":"2023-06-20T10:30:27.9183696Z","Configuration":{"AudioLanguagePreference":"","PlayDefaultAudioTrack":true,"SubtitleLanguagePreference":"dut","DisplayMissingEpisodes":true,"GroupedFolders":["f137a2dd21bbc1b99aa5c0f6bf02a805","767bffe4f11c93ef34b805451a696a4e"],"SubtitleMode":"Always","DisplayCollectionsView":false,"EnableLocalPassword":true,"OrderedViews":["b6239cb8a74ff47b07bbf770d40a8e56","f137a2dd21bbc1b99aa5c0f6bf02a805","7e64e319657a9516ec78490da03edccb","767bffe4f11c93ef34b805451a696a4e","9d7ad6afe9afa2dab1a2f6e00ad28fa6"],"LatestItemsExcludes":[],"MyMediaExcludes":["9d7ad6afe9afa2dab1a2f6e00ad28fa6"],"HidePlayedInLatest":false,"RememberAudioSelections":true,"RememberSubtitleSelections":true,"EnableNextEpisodeAutoPlay":true},"Policy":{"IsAdministrator":false,"IsHidden":true,"IsDisabled":false,"BlockedTags":[],"EnableUserPreferenceAccess":true,"AccessSchedules":[],"BlockUnratedItems":[],"EnableRemoteControlOfOtherUsers":false,"EnableSharedDeviceControl":false,"EnableRemoteAccess":true,"EnableLiveTvManagement":false,"EnableLiveTvAccess":true,"EnableMediaPlayback":true,"EnableAudioPlaybackTranscoding":true,"EnableVideoPlaybackTranscoding":true,"EnablePlaybackRemuxing":true,"ForceRemoteSourceTranscoding":false,"EnableContentDeletion":false,"EnableContentDeletionFromFolders":[],"EnableContentDownloading":true,"EnableSyncTranscoding":true,"EnableMediaConversion":true,"EnabledDevices":[],"EnableAllDevices":true,"EnabledChannels":[],"EnableAllChannels":true,"EnabledFolders":[],"EnableAllFolders":true,"InvalidLoginAttemptCount":0,"LoginAttemptsBeforeLockout":-1,"MaxActiveSessions":0,"EnablePublicSharing":false,"BlockedMediaFolders":[],"BlockedChannels":[],"RemoteClientBitrateLimit":0,"AuthenticationProviderId":"Jellyfin.Server.Implementations.Users.DefaultAuthenticationProvider","PasswordResetProviderId":"Jellyfin.Server.Implementations.Users.DefaultPasswordResetProvider","SyncPlayAccess":"CreateAndJoinGroups"}},"SessionInfo":{"PlayState":{"CanSeek":false,"IsPaused":false,"IsMuted":false,"RepeatMode":"RepeatNone"},"AdditionalUsers":[],"Capabilities":{"PlayableMediaTypes":[],"SupportedCommands":[],"SupportsMediaControl":false,"SupportsContentUploading":false,"SupportsPersistentIdentifier":true,"SupportsSync":false},"RemoteEndPoint":"103.246.103.99","PlayableMediaTypes":[],"Id":"b7d79ef2a71a561bbb97e28de9ea4ae7","UserId":"a076a5bfc9034f379f5889bc6dafc77b","UserName":"demo","Client":"jellyash_test_testauthedclient","LastActivityDate":"2023-06-20T10:30:27.9496472Z","LastPlaybackCheckIn":"0001-01-01T00:00:00.0000000Z","DeviceName":"wrecked","DeviceId":"2c04707d-5fce-4c46-89ad-fd705a2187d9","ApplicationVersion":"0.4.0","IsActive":true,"SupportsMediaControl":false,"SupportsRemoteControl":false,"NowPlayingQueue":[],"NowPlayingQueueFullItems":[],"HasCustomDeviceName":false,"ServerId":"713dc3fe952b438fa70ed35e4ef0525a","SupportedCommands":[]},"AccessToken":"efb1cef07e9c42edbc4eb622bc13beff","ServerId":"713dc3fe952b438fa70ed35e4ef0525a"}'
     headers:
       content-type:
       - application/json; charset=utf-8
       date:
-      - Sat, 13 May 2023 02:42:18 GMT
+      - Tue, 20 Jun 2023 10:30:27 GMT
       referrer-policy:
       - no-referrer,same-origin,strict-origin,strict-origin-when-cross-origin
       server:
       - Kestrel
       strict-transport-security:
       - max-age=31536000;includeSubDomains;preload
       transfer-encoding:
       - chunked
       x-content-type-options:
       - nosniff
       x-response-time-ms:
-      - '41'
+      - '38'
       x-xss-protection:
       - 1;mode=block
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `jellyash-0.4.0/tests/cassettes/test_client/TestAuthedClient.test_authed_client.yaml` & `jellyash-0.4.1/tests/cassettes/test_client/TestAuthedClient.test_authed_client_offline.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml` & `jellyash-0.4.1/tests/cassettes/test_client/TestClient.test_auth_with_password.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.client.yaml` & `jellyash-0.4.1/tests/cassettes/test_duration/TestDuration.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml` & `jellyash-0.4.1/tests/cassettes/test_duration/TestDuration.test_calculate_duration.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml` & `jellyash-0.4.1/tests/cassettes/test_duration/TestDuration.test_calculate_duration_not_found.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml` & `jellyash-0.4.1/tests/cassettes/test_nextup/TestEpisodeStr.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml` & `jellyash-0.4.1/tests/cassettes/test_nextup/TestEpisodeStr.test_episode_str.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml` & `jellyash-0.4.1/tests/cassettes/test_search/TestSearch.test_multiple_terms_exact.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml` & `jellyash-0.4.1/tests/cassettes/test_search/TestSearch.test_multiple_terms_not_exact.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_search/TestSearch.test_single_term.yaml` & `jellyash-0.4.1/tests/cassettes/test_search/TestSearch.test_single_term.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml` & `jellyash-0.4.1/tests/cassettes/test_token/TestCreateJellyfinToken.test_create_token.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.client.yaml` & `jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.client.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml` & `jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.test_all_unwatched.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml` & `jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml` & `jellyash-0.4.1/tests/cassettes/test_unwatched/TestUnwatched.test_specific_unwatched_not_found.yaml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/LICENSE` & `jellyash-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/pyproject.toml` & `jellyash-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jellyash-0.4.0/PKG-INFO` & `jellyash-0.4.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jellyash
-Version: 0.4.0
+Version: 0.4.1
 License: Copyright 2023 Steve Kowalik <steven@wedontsleep.org>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
@@ -14,14 +14,16 @@
 Requires-Python: >=3.7
 Requires-Dist: jellyfin-apiclient-python
 Requires-Dist: typing-extensions; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # Jellyash
 
+[![PyPI Version](https://badge.fury.io/py/jellyash.svg)](https://badge.fury.io/py/jellyash)[![Build](https://github.com/s-t-e-v-e-n-k/jellyash/actions/workflows/ci.yml/badge.svg)](https://github.com/s-t-e-v-e-n-k/jellyash/actions/workflows/ci.yml)[![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/s-t-e-v-e-n-k/0926cbcb886804fa2c0fdb68212a367d/raw/coverage-badge.json)](https://gist.github.com/s-t-e-v-e-n-k/0926cbcb886804fa2c0fdb68212a367d/raw/coverage-badge.json)
+
 Jelly **A**eroplane **S**hark **H**elper
 
 Wrapper around jellyfin-apiclient-python to provide convenience functions:
 
 Create an unauthenticated client:
 
 ```
```

