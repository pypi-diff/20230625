# Comparing `tmp/so_vits_svc_fork-4.0.3.tar.gz` & `tmp/so_vits_svc_fork-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-4.0.3.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.1.0.tar", max compression
```

## Comparing `so_vits_svc_fork-4.0.3.tar` & `so_vits_svc_fork-4.1.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    12463 2023-06-25 08:21:53.946872 so_vits_svc_fork-4.0.3/LICENSE
--rw-r--r--   0        0        0    28059 2023-06-25 08:21:53.946872 so_vits_svc_fork-4.0.3/README.md
--rw-r--r--   0        0        0     3093 2023-06-25 08:21:54.926886 so_vits_svc_fork-4.0.3/pyproject.toml
--rw-r--r--   0        0        0       70 2023-06-25 08:21:54.874885 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    24434 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2875 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2599 2023-06-25 08:21:53.950872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    30617 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24605 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     9418 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1169 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1463 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     2051 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1705 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1862 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2975 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
--rw-r--r--   0        0        0     2710 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4667 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4447 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    21359 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    14797 2023-06-25 08:21:53.954872 so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    29867 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-06-25 14:18:35.879591 so_vits_svc_fork-4.1.0/LICENSE
+-rw-r--r--   0        0        0    28911 2023-06-25 14:18:35.879591 so_vits_svc_fork-4.1.0/README.md
+-rw-r--r--   0        0        0     3093 2023-06-25 14:18:36.895603 so_vits_svc_fork-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-06-25 14:18:36.843603 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24947 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     4914 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    30617 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24605 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9418 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-06-25 14:18:35.883592 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     2206 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    14797 2023-06-25 14:18:35.887591 so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    30719 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.1.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-4.0.3/LICENSE` & `so_vits_svc_fork-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/README.md` & `so_vits_svc_fork-4.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -289,14 +289,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/acekagami"><img src="https://avatars.githubusercontent.com/u/127201056?v=4?s=80" width="80px;" alt="acekagami"/><br /><sub><b>acekagami</b></sub></a><br /><a href="#translation-acekagami" title="Translation">🌍</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Highupech"><img src="https://avatars.githubusercontent.com/u/114140670?v=4?s=80" width="80px;" alt="Highupech"/><br /><sub><b>Highupech</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AHighupech" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Scorpi"><img src="https://avatars.githubusercontent.com/u/969654?v=4?s=80" width="80px;" alt="Scorpi"/><br /><sub><b>Scorpi</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Scorpi" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ph0rk0z"><img src="https://avatars.githubusercontent.com/u/59298527?v=4?s=80" width="80px;" alt="Forkoz"/><br /><sub><b>Forkoz</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3APh0rk0z" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Ph0rk0z" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zerui18"><img src="https://avatars.githubusercontent.com/u/34794550?v=4?s=80" width="80px;" alt="Zerui Chen"/><br /><sub><b>Zerui Chen</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Zerui18" title="Code">💻</a> <a href="#ideas-Zerui18" title="Ideas, Planning, & Feedback">🤔</a></td>
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
-                                                                   [Maximxls]                                      [Star3Lord]
-                                                                    Maximxls                                        Star3Lord
-                                                                      ð»                                      ð ð»
+                                                                   [Maximxls]                                      [Star3Lord]                          [Forkoz]                 [Zerui_Chen]
+                                                                    Maximxls                                        Star3Lord                            Forkoz                   Zerui_Chen
+                                                                      ð»                                      ð ð»                   ð ð»         ð» ð¤
     This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `so_vits_svc_fork-4.0.3/pyproject.toml` & `so_vits_svc_fork-4.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "4.0.3"
+version = "4.1.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -714,35 +714,44 @@
 @click.option(
     "-n",
     "--n-jobs",
     type=int,
     default=-1,
     help="number of jobs (optimal value may depend on your RAM capacity and audio duration per file)",
 )
+@click.option(
+    "-l",
+    "--max-length",
+    type=float,
+    default=10,
+    help="max length of each split in seconds",
+)
 @click.option("-d", "--top-db", type=float, default=30, help="top db")
 @click.option("-f", "--frame-seconds", type=float, default=1, help="frame seconds")
 @click.option(
     "-ho", "-hop", "--hop-seconds", type=float, default=0.3, help="hop seconds"
 )
 @click.option("-s", "--sr", type=int, default=44100, help="sample rate")
 def pre_split(
     input_dir: Path | str,
     output_dir: Path | str,
+    max_length: float,
     top_db: int,
     frame_seconds: float,
     hop_seconds: float,
     n_jobs: int,
     sr: int,
 ):
     """Split audio files into multiple files"""
     from so_vits_svc_fork.preprocessing.preprocess_split import preprocess_split
 
     preprocess_split(
         input_dir=input_dir,
         output_dir=output_dir,
+        max_length=max_length,
         top_db=top_db,
         frame_seconds=frame_seconds,
         hop_seconds=hop_seconds,
         n_jobs=n_jobs,
         sr=sr,
     )
 
@@ -871,25 +880,38 @@
     help="model path to save",
     default=Path("./logs/44k/kmeans.pt"),
 )
 @click.option("-n", "--n-clusters", type=int, help="number of clusters", default=2000)
 @click.option(
     "-m/-nm", "--minibatch/--no-minibatch", default=True, help="use minibatch k-means"
 )
+@click.option(
+    "-b", "--batch-size", type=int, default=4096, help="batch size for minibatch kmeans"
+)
+@click.option(
+    "-p/-np", "--partial-fit", default=False, help="use partial fit (only use with -m)"
+)
 def train_cluster(
-    input_dir: Path, output_path: Path, n_clusters: int, minibatch: bool
+    input_dir: Path,
+    output_path: Path,
+    n_clusters: int,
+    minibatch: bool,
+    batch_size: int,
+    partial_fit: bool,
 ) -> None:
     """Train k-means clustering"""
     from .cluster.train_cluster import main
 
     main(
         input_dir=input_dir,
         output_path=output_path,
         n_clusters=n_clusters,
         verbose=True,
         use_minibatch=minibatch,
+        batch_size=batch_size,
+        partial_fit=partial_fit,
     )
 
 
 if __name__ == "__main__":
     freeze_support()
     cli()
```

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_classify.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 def _process_one(
     input_path: Path,
     output_dir: Path,
     sr: int,
     *,
+    max_length: float = 10.0,
     top_db: int = 30,
     frame_seconds: float = 0.5,
     hop_seconds: float = 0.1,
 ):
     try:
         audio, sr = librosa.load(input_path, sr=sr, mono=True)
     except Exception as e:
@@ -30,27 +31,33 @@
         audio,
         top_db=top_db,
         frame_length=int(sr * frame_seconds),
         hop_length=int(sr * hop_seconds),
     )
     output_dir.mkdir(parents=True, exist_ok=True)
     for start, end in tqdm(intervals, desc=f"Writing {input_path}"):
-        audio_cut = audio[start:end]
-        sf.write(
-            (output_dir / f"{input_path.stem}_{start / sr:.3f}_{end / sr:.3f}.wav"),
-            audio_cut,
-            sr,
-        )
+        for sub_start in range(start, end, int(sr * max_length)):
+            sub_end = min(sub_start + int(sr * max_length), end)
+            audio_cut = audio[sub_start:sub_end]
+            sf.write(
+                (
+                    output_dir
+                    / f"{input_path.stem}_{sub_start / sr:.3f}_{sub_end / sr:.3f}.wav"
+                ),
+                audio_cut,
+                sr,
+            )
 
 
 def preprocess_split(
     input_dir: Path | str,
     output_dir: Path | str,
     sr: int,
     *,
+    max_length: float = 10.0,
     top_db: int = 30,
     frame_seconds: float = 0.5,
     hop_seconds: float = 0.1,
     n_jobs: int = -1,
 ):
     input_dir = Path(input_dir)
     output_dir = Path(output_dir)
@@ -58,13 +65,14 @@
     input_paths = list(input_dir.rglob("*.*"))
     with tqdm_joblib(desc="Splitting", total=len(input_paths)):
         Parallel(n_jobs=n_jobs)(
             delayed(_process_one)(
                 input_path,
                 output_dir / input_path.relative_to(input_dir).parent,
                 sr,
+                max_length=max_length,
                 top_db=top_db,
                 frame_seconds=frame_seconds,
                 hop_seconds=hop_seconds,
             )
             for input_path in input_paths
         )
```

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/train.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.1.0/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-4.0.3/PKG-INFO` & `so_vits_svc_fork-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 4.0.3
+Version: 4.1.0
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -340,14 +340,16 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/acekagami"><img src="https://avatars.githubusercontent.com/u/127201056?v=4?s=80" width="80px;" alt="acekagami"/><br /><sub><b>acekagami</b></sub></a><br /><a href="#translation-acekagami" title="Translation">🌍</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Highupech"><img src="https://avatars.githubusercontent.com/u/114140670?v=4?s=80" width="80px;" alt="Highupech"/><br /><sub><b>Highupech</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AHighupech" title="Bug reports">🐛</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Scorpi"><img src="https://avatars.githubusercontent.com/u/969654?v=4?s=80" width="80px;" alt="Scorpi"/><br /><sub><b>Scorpi</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Scorpi" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="http://maximxlss.github.io"><img src="https://avatars.githubusercontent.com/u/29152154?v=4?s=80" width="80px;" alt="Maximxls"/><br /><sub><b>Maximxls</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=maximxlss" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Star3Lord"><img src="https://avatars.githubusercontent.com/u/57606931?v=4?s=80" width="80px;" alt="Star3Lord"/><br /><sub><b>Star3Lord</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3AStar3Lord" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Star3Lord" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ph0rk0z"><img src="https://avatars.githubusercontent.com/u/59298527?v=4?s=80" width="80px;" alt="Forkoz"/><br /><sub><b>Forkoz</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/issues?q=author%3APh0rk0z" title="Bug reports">🐛</a> <a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Ph0rk0z" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Zerui18"><img src="https://avatars.githubusercontent.com/u/34794550?v=4?s=80" width="80px;" alt="Zerui Chen"/><br /><sub><b>Zerui Chen</b></sub></a><br /><a href="https://github.com/voicepaw/so-vits-svc-fork/commits?author=Zerui18" title="Code">💻</a> <a href="#ideas-Zerui18" title="Ideas, Planning, & Feedback">🤔</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.0.3 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 4.1.0 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
@@ -153,13 +153,13 @@
                                                                                                                                                                                                                                                                            ð
                                                                 [Xianglong_He]                                          [75aosu]                           [tonyco82]              [yxlllc]        [outhipped]                        [escoolioinglesias]              [Blacksingh]
                                                                  Xianglong_He                                            75aosu                             tonyco82                yxlllc          outhipped                          escoolioinglesias                Blacksingh
                                                                      ð                                             ð                            ð            ð¤ ð�     ð                         ð ð ð¹         ð
                                                        [Mgs._M._Thoyib_Antarnusa]                                  [Exosfeer]                         [guranon]               [Alexander_Koumis]   [acekagami]                                  [Highupech]              [Scorpi]
                                                         Mgs._M._Thoyib_Antarnusa                                    Exosfeer                           guranon                 Alexander_Koumis     acekagami                                    Highupech                Scorpi
                                                                   ð                                          ð ð»              ð ð¤ ð»        ð»          ð                                    ð                ð»
-                                                                   [Maximxls]                                      [Star3Lord]
-                                                                    Maximxls                                        Star3Lord
-                                                                      ð»                                      ð ð»
+                                                                   [Maximxls]                                      [Star3Lord]                          [Forkoz]                 [Zerui_Chen]
+                                                                    Maximxls                                        Star3Lord                            Forkoz                   Zerui_Chen
+                                                                      ð»                                      ð ð»                   ð ð»         ð» ð¤
     This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

