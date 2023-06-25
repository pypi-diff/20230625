# Comparing `tmp/so_vits_svc_fork-4.0.2.tar.gz` & `tmp/so_vits_svc_fork-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-4.0.2.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.0.3.tar", max compression
```

## Comparing `so_vits_svc_fork-4.0.2.tar` & `so_vits_svc_fork-4.0.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12463 2023-06-14 12:58:53.153535 so_vits_svc_fork-4.0.2/LICENSE
--rw-r--r--   0        0        0    27605 2023-06-14 12:58:53.153535 so_vits_svc_fork-4.0.2/README.md
--rw-r--r--   0        0        0     3091 2023-06-14 12:58:54.057548 so_vits_svc_fork-4.0.2/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-14 12:58:54.009548 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    24434 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2875 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2599 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    30617 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24605 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9408 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1169 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1463 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2051 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1705 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1862 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2975 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2710 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4667 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4447 2023-06-14 12:58:53.161535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-06-14 12:58:53.165535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-06-14 12:58:53.165535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-06-14 12:58:53.165535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-06-14 12:58:53.165535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21359 2023-06-14 12:58:53.165535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    14797 2023-06-14 12:58:53.165535 so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    29411 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-06-25 08:21:53.946872 so_vits_svc_fork-4.0.3/LICENSE
+-rw-r--r--   0        0        0    28059 2023-06-25 08:21:53.946872 so_vits_svc_fork-4.0.3/README.md
+-rw-r--r--   0        0        0     3093 2023-06-25 08:21:54.926886 so_vits_svc_fork-4.0.3/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-25 08:21:54.874885 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24434 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    30617 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24605 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9418 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    14797 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    29867 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.0.3/PKG-INFO
```

### Comparing `so_vits_svc_fork-4.0.2/LICENSE` & `so_vits_svc_fork-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/README.md` & `so_vits_svc_fork-4.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -288,14 +288,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/alexanderkoumis"><img src="https://avatars.githubusercontent.com/u/5108856?v=4?s=80" width="80px;" alt="Alexander Koumis"/><br /><sub><b>Alexander Koumis</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=alexanderkoumis" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/acekagami"><img src="https://avatars.githubusercontent.com/u/127201056?v=4?s=80" width="80px;" alt="acekagami"/><br /><sub><b>acekagami</b></sub></a><br /><a href="#translation-acekagami" title="Translation">🌍</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Highupech"><img src="https://avatars.githubusercontent.com/u/114140670?v=4?s=80" width="80px;" alt="Highupech"/><br /><sub><b>Highupech</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AHighupech" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Scorpi"><img src="https://avatars.githubusercontent.com/u/969654?v=4?s=80" width="80px;" alt="Scorpi"/><br /><sub><b>Scorpi</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Scorpi" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -129,13 +129,13 @@
                                                                                                                                                                                                                                                                            ð
                                                                 [Xianglong_He]                                          [75aosu]                           [tonyco82]              [yxlllc]        [outhipped]                        [escoolioinglesias]              [Blacksingh]
                                                                  Xianglong_He                                            75aosu                             tonyco82                yxlllc          outhipped                          escoolioinglesias                Blacksingh
                                                                      ð                                             ð                            ð            ð¤ ð�     ð                         ð ð ð¹         ð
                                                        [Mgs._M._Thoyib_Antarnusa]                                  [Exosfeer]                         [guranon]               [Alexander_Koumis]   [acekagami]                                  [Highupech]              [Scorpi]
                                                         Mgs._M._Thoyib_Antarnusa                                    Exosfeer                           guranon                 Alexander_Koumis     acekagami                                    Highupech                Scorpi
                                                                   ð                                          ð ð»              ð ð¤ ð»        ð»          ð                                    ð                ð»
-                                                                   [Maximxls]
-                                                                    Maximxls
-                                                                      ð»
+                                                                   [Maximxls]                                      [Star3Lord]
+                                                                    Maximxls                                        Star3Lord
+                                                                      ð»                                      ð ð»
     This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `so_vits_svc_fork-4.0.2/pyproject.toml` & `so_vits_svc_fork-4.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "4.0.2"
+version = "4.0.3"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
@@ -51,15 +51,15 @@
 tqdm-joblib = "*"
 tensorboardx = "*"
 cm-time = ">=0.1.2"
 pysimplegui = ">=4.6"
 pebble = ">=5.0"
 torchcrepe = ">=0.0.17"
 lightning = "^2.0.1"
-fastapi = "==0.88"
+fastapi = "==0.98.0"
 transformers = "^4.28.1"
 matplotlib = "^3.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
```

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     )
 
     try:
         pbar = tqdm(list(zip(input_paths, output_paths)), disable=len(input_paths) == 1)
         for input_path, output_path in pbar:
             pbar.set_description(f"{input_path}")
             try:
-                audio, _ = librosa.load(input_path, sr=svc_model.target_sample)
+                audio, _ = librosa.load(str(input_path), sr=svc_model.target_sample)
             except Exception as e:
                 LOG.error(f"Failed to load {input_path}")
                 LOG.exception(e)
                 continue
             output_path.parent.mkdir(parents=True, exist_ok=True)
             audio = svc_model.infer_silence(
                 audio.astype(np.float32),
@@ -102,15 +102,15 @@
                 f0_method=f0_method,
                 db_thresh=db_thresh,
                 pad_seconds=pad_seconds,
                 chunk_seconds=chunk_seconds,
                 absolute_thresh=absolute_thresh,
                 max_chunk_seconds=max_chunk_seconds,
             )
-            soundfile.write(output_path, audio, svc_model.target_sample)
+            soundfile.write(str(output_path), audio, svc_model.target_sample)
     finally:
         del svc_model
         torch.cuda.empty_cache()
 
 
 def realtime(
     *,
```

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.2/PKG-INFO` & `so_vits_svc_fork-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 4.0.2
+Version: 4.0.3
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: SoundFile
 Requires-Dist: cm-time (>=0.1.2)
-Requires-Dist: fastapi (==0.88)
+Requires-Dist: fastapi (==0.98.0)
 Requires-Dist: librosa
 Requires-Dist: lightning (>=2.0.1,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: onnx
 Requires-Dist: onnxoptimizer
 Requires-Dist: onnxsim
@@ -339,14 +339,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/alexanderkoumis"><img src="https://avatars.githubusercontent.com/u/5108856?v=4?s=80" width="80px;" alt="Alexander Koumis"/><br /><sub><b>Alexander Koumis</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=alexanderkoumis" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/acekagami"><img src="https://avatars.githubusercontent.com/u/127201056?v=4?s=80" width="80px;" alt="acekagami"/><br /><sub><b>acekagami</b></sub></a><br /><a href="#translation-acekagami" title="Translation">🌍</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Highupech"><img src="https://avatars.githubusercontent.com/u/114140670?v=4?s=80" width="80px;" alt="Highupech"/><br /><sub><b>Highupech</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AHighupech" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Scorpi"><img src="https://avatars.githubusercontent.com/u/969654?v=4?s=80" width="80px;" alt="Scorpi"/><br /><sub><b>Scorpi</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Scorpi" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.0.2 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.0.3 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Software Development :: Libraries Requires-Dist: SoundFile Requires-
-Dist: cm-time (>=0.1.2) Requires-Dist: fastapi (==0.88) Requires-Dist: librosa
-Requires-Dist: lightning (>=2.0.1,<3.0.0) Requires-Dist: matplotlib
+Dist: cm-time (>=0.1.2) Requires-Dist: fastapi (==0.98.0) Requires-Dist:
+librosa Requires-Dist: lightning (>=2.0.1,<3.0.0) Requires-Dist: matplotlib
 (>=3.7.1,<4.0.0) Requires-Dist: numpy (>=1.23,<2.0) Requires-Dist: onnx
 Requires-Dist: onnxoptimizer Requires-Dist: onnxsim Requires-Dist: pebble
 (>=5.0) Requires-Dist: praat-parselmouth Requires-Dist: pysimplegui (>=4.6)
 Requires-Dist: pyworld Requires-Dist: requests Requires-Dist: rich Requires-
 Dist: scipy Requires-Dist: sounddevice Requires-Dist: tensorboard Requires-
 Dist: tensorboardx Requires-Dist: torch Requires-Dist: torchaudio Requires-
 Dist: torchcrepe (>=0.0.17) Requires-Dist: tqdm Requires-Dist: tqdm-joblib
@@ -153,13 +153,13 @@
                                                                                                                                                                                                                                                                            ð
                                                                 [Xianglong_He]                                          [75aosu]                           [tonyco82]              [yxlllc]        [outhipped]                        [escoolioinglesias]              [Blacksingh]
                                                                  Xianglong_He                                            75aosu                             tonyco82                yxlllc          outhipped                          escoolioinglesias                Blacksingh
                                                                      ð                                             ð                            ð            ð¤ ð�     ð                         ð ð ð¹         ð
                                                        [Mgs._M._Thoyib_Antarnusa]                                  [Exosfeer]                         [guranon]               [Alexander_Koumis]   [acekagami]                                  [Highupech]              [Scorpi]
                                                         Mgs._M._Thoyib_Antarnusa                                    Exosfeer                           guranon                 Alexander_Koumis     acekagami                                    Highupech                Scorpi
                                                                   ð                                          ð ð»              ð ð¤ ð»        ð»          ð                                    ð                ð»
-                                                                   [Maximxls]
-                                                                    Maximxls
-                                                                      ð»
+                                                                   [Maximxls]                                      [Star3Lord]
+                                                                    Maximxls                                        Star3Lord
+                                                                      ð»                                      ð ð»
     This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

