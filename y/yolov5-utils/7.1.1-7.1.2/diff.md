# Comparing `tmp/yolov5-utils-7.1.1.tar.gz` & `tmp/yolov5-utils-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolov5-utils-7.1.1.tar", last modified: Fri Jun 16 02:34:20 2023, max compression
+gzip compressed data, was "yolov5-utils-7.1.2.tar", last modified: Sun Jun 25 07:10:30 2023, max compression
```

## Comparing `yolov5-utils-7.1.1.tar` & `yolov5-utils-7.1.2.tar`

### file list

```diff
@@ -1,173 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/workflows/package_testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)    35126 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/yolov5_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-16 02:34:02.000000 yolov5-utils-7.1.1/yolov5_utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/yolov5_utils/yolov5/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41308 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    40334 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/README.zh-CN.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/benchmarks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/train.py
--rw-r--r--   0 runner    (1001) docker     (123)   103620 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Argoverse.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/GlobalWheat2020.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/ImageNet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/SKU-110K.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VisDrone.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/
--rw-r--r--   0 runner    (1001) docker     (123)   487438 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/bus.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   168949 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/zidane.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.969872 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/download_weights.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco128.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_imagenet.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/data/xView.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    39168 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/hubconf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41530 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/anchors.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5l6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5m6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5n6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s6.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5x6.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5l.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5n.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5s.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5x.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.973872 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    34744 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23993 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/val.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    40908 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autoanchor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autobatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/mime.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/userdata.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/dataloaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/example_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    45439 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/general.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/additional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/app.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/
--rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.977872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.981872 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/augmentations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/dataloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    19642 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-06-16 02:34:03.000000 yolov5-utils-7.1.1/yolov5_utils/yolov5/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:34:20.965872 yolov5-utils-7.1.1/yolov5_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 02:34:20.000000 yolov5-utils-7.1.1/yolov5_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.649483 yolov5-utils-7.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.613482 yolov5-utils-7.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.613482 yolov5-utils-7.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/.github/workflows/package_testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)    35126 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-25 07:10:30.649483 yolov5-utils-7.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 07:10:30.649483 yolov5-utils-7.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.613482 yolov5-utils-7.1.2/yolov5_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/yolov5_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/yolov5_utils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/yolov5_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/yolov5_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-25 07:10:17.000000 yolov5-utils-7.1.2/yolov5_utils/import_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.617482 yolov5-utils-7.1.2/yolov5_utils/yolov5/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41308 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    40334 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/README.zh-CN.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.617482 yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16395 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103620 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.621482 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/Argoverse.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/GlobalWheat2020.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/ImageNet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/SKU-110K.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/VisDrone.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/coco.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/coco128-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/coco128.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.621482 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.621482 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   487438 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/images/bus.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   168949 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/images/zidane.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.625482 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/download_weights.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/get_coco.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/get_coco128.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1672 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/get_imagenet.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/data/xView.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14320 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39168 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/hubconf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.625482 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41530 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.633483 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/anchors.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5l6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5m6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5n6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s6.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5x6.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.633483 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    27019 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17767 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5l.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5s.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5x.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.637483 yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34744 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43389 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23993 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/val.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    33767 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40908 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.641482 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17031 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/autoanchor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/autobatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.641482 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/mime.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/userdata.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/dataloaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.641482 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.641482 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/flask_rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/flask_rest_api/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/flask_rest_api/example_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45439 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.645483 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/google_app_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/google_app_engine/additional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/google_app_engine/app.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.645483 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.645483 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8034 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.645483 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18731 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.649483 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/wandb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24671 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.649483 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/dataloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19642 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-06-25 07:10:18.000000 yolov5-utils-7.1.2/yolov5_utils/yolov5/val.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:10:30.613482 yolov5-utils-7.1.2/yolov5_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-25 07:10:30.000000 yolov5-utils-7.1.2/yolov5_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-25 07:10:30.000000 yolov5-utils-7.1.2/yolov5_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 07:10:30.000000 yolov5-utils-7.1.2/yolov5_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 07:10:30.000000 yolov5-utils-7.1.2/yolov5_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-25 07:10:30.000000 yolov5-utils-7.1.2/yolov5_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-25 07:10:30.000000 yolov5-utils-7.1.2/yolov5_utils.egg-info/top_level.txt
```

### Comparing `yolov5-utils-7.1.1/.github/workflows/ci.yml` & `yolov5-utils-7.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/.github/workflows/package_testing.yml` & `yolov5-utils-7.1.2/.github/workflows/package_testing.yml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/.github/workflows/python-publish.yml` & `yolov5-utils-7.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/.gitignore` & `yolov5-utils-7.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/LICENSE` & `yolov5-utils-7.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/PKG-INFO` & `yolov5-utils-7.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-utils
-Version: 7.1.1
+Version: 7.1.2
 Summary: Packaged version of the Yolov5 object detector
 License: GPL
 Project-URL: Documentation, https://github.com/msclock/yolov5-utils
 Project-URL: Source, https://github.com/msclock/yolov5-utils
 Project-URL: Tracker, https://github.com/msclock/yolov5-utils/issues
 Keywords: machine-learning,deep-learning,ml,triton,inference,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yolov5-utils-7.1.1/README.md` & `yolov5-utils-7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/pyproject.toml` & `yolov5-utils-7.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -101,20 +101,14 @@
 license-files = ["LICENSE"]
 
 [tool.distutils.bdist_wheel]
 python_tag = "py37.py38.py39.py310"
 
 [tool.setuptools.packages.find]
 namespaces = false
-include = [
-    "yolov5_utils",
-    "yolov5_utils.yolov5.utils",
-    "yolov5_utils.yolov5.classify",
-    "yolov5_utils.yolov5.segment",
-]
 
 [tool.setuptools.package-data]
 yolov5_utils = ["**/*"]
 
 [tool.setuptools.dynamic]
 version = { attr = "yolov5_utils.__version__.__version__" }
 
@@ -136,17 +130,7 @@
   )/
 )
 '''
 
 [tool.isort]
 profile = "black"
 line_length = 120
-
-[tool.vulture]
-exclude = []
-ignore_decorators = []
-ignore_names = []
-make_whitelist = true
-min_confidence = 80
-paths = ["model_navigator"]
-sort_by_size = true
-verbose = false
```

### Comparing `yolov5-utils-7.1.1/yolov5_utils/cli.py` & `yolov5-utils-7.1.2/yolov5_utils/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import fire
 
+from yolov5_utils.import_hook import *
+
 from .yolov5.benchmarks import run as benchmarks
 from .yolov5.classify.predict import run as classify_predict
 from .yolov5.classify.train import run as classify_train
 from .yolov5.classify.val import run as classify_val
 from .yolov5.detect import run as detect
 from .yolov5.export import run as export
 from .yolov5.segment.predict import run as segment_predict
```

### Comparing `yolov5-utils-7.1.1/yolov5_utils/helpers.py` & `yolov5-utils-7.1.2/yolov5_utils/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from yolov5_utils.import_hook import *
+
 from .yolov5.models.common import AutoShape, DetectMultiBackend
 from .yolov5.models.experimental import attempt_load
 from .yolov5.models.yolo import ClassificationModel, SegmentationModel
 from .yolov5.utils.general import LOGGER, logging
 from .yolov5.utils.torch_utils import select_device
```

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/CONTRIBUTING.md` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/LICENSE` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/LICENSE`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/README.md` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/README.zh-CN.md` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/README.zh-CN.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/benchmarks.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/benchmarks.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/predict.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/predict.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/train.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/tutorial.ipynb` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/classify/val.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/classify/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Argoverse.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/Argoverse.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/GlobalWheat2020.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/GlobalWheat2020.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/ImageNet.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/ImageNet.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/Objects365.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/SKU-110K.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/SKU-110K.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VOC.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/VisDrone.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/VisDrone.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/coco.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128-seg.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/coco128-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/coco128.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/coco128.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.Objects365.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.VOC.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.no-augmentation.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.scratch-high.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.scratch-low.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/hyps/hyp.scratch-med.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/bus.jpg` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/images/bus.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/images/zidane.jpg` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/images/zidane.jpg`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/download_weights.sh` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/download_weights.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco.sh` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/get_coco.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_coco128.sh` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/get_coco128.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/scripts/get_imagenet.sh` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/scripts/get_imagenet.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/data/xView.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/data/xView.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/detect.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/detect.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/export.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/export.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/hubconf.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/hubconf.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/common.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/common.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/experimental.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/experimental.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/anchors.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/anchors.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov3-spp.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov3-tiny.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov3.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov3.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-bifpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-fpn.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p2.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p34.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-p7.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5-panet.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5l6.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5l6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5m6.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5m6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5n6.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5n6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s-LeakyReLU.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s-ghost.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s-transformer.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5s6.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5s6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/hub/yolov5x6.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/hub/yolov5x6.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5l-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5m-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5n-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5s-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/segment/yolov5x-seg.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/tf.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/tf.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolo.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolo.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5l.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5l.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5m.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5m.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5n.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5n.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5s.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5s.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/models/yolov5x.yaml` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/models/yolov5x.yaml`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/requirements.txt` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/requirements.txt`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/predict.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/predict.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/train.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/tutorial.ipynb` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/segment/val.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/segment/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/setup.cfg` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/setup.cfg`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/train.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/train.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/tutorial.ipynb` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/__init__.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/activations.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/activations.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/augmentations.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autoanchor.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/autobatch.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/autobatch.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/mime.sh` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/mime.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/resume.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/resume.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/aws/userdata.sh` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/aws/userdata.sh`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/callbacks.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/dataloaders.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/dataloaders.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/docker/Dockerfile-arm64`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/docker/Dockerfile-cpu`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/downloads.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/downloads.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/README.md` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/flask_rest_api/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/flask_rest_api/restapi.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/general.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/general.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/google_app_engine/Dockerfile`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/__init__.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/README.md` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/clearml_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/clearml/hpo.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/README.md` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/README.md`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/__init__.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/__init__.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/comet_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/hpo.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/hpo.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/comet/optimizer_config.json`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loggers/wandb/wandb_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/loss.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/metrics.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/plots.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/augmentations.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/augmentations.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/dataloaders.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/dataloaders.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/general.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/general.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/loss.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/loss.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/metrics.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/metrics.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/segment/plots.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/segment/plots.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/torch_utils.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/utils/triton.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/utils/triton.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils/yolov5/val.py` & `yolov5-utils-7.1.2/yolov5_utils/yolov5/val.py`

 * *Files identical despite different names*

### Comparing `yolov5-utils-7.1.1/yolov5_utils.egg-info/PKG-INFO` & `yolov5-utils-7.1.2/yolov5_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yolov5-utils
-Version: 7.1.1
+Version: 7.1.2
 Summary: Packaged version of the Yolov5 object detector
 License: GPL
 Project-URL: Documentation, https://github.com/msclock/yolov5-utils
 Project-URL: Source, https://github.com/msclock/yolov5-utils
 Project-URL: Tracker, https://github.com/msclock/yolov5-utils/issues
 Keywords: machine-learning,deep-learning,ml,triton,inference,pytorch,YOLO,object-detection,vision,YOLOv5,YOLOv7
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `yolov5-utils-7.1.1/yolov5_utils.egg-info/SOURCES.txt` & `yolov5-utils-7.1.2/yolov5_utils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 .github/workflows/ci.yml
 .github/workflows/package_testing.yml
 .github/workflows/python-publish.yml
 yolov5_utils/__init__.py
 yolov5_utils/__version__.py
 yolov5_utils/cli.py
 yolov5_utils/helpers.py
+yolov5_utils/import_hook.py
 yolov5_utils.egg-info/PKG-INFO
 yolov5_utils.egg-info/SOURCES.txt
 yolov5_utils.egg-info/dependency_links.txt
 yolov5_utils.egg-info/entry_points.txt
 yolov5_utils.egg-info/requires.txt
 yolov5_utils.egg-info/top_level.txt
 yolov5_utils/yolov5/CITATION.cff
```

### Comparing `yolov5-utils-7.1.1/yolov5_utils.egg-info/requires.txt` & `yolov5-utils-7.1.2/yolov5_utils.egg-info/requires.txt`

 * *Files identical despite different names*

