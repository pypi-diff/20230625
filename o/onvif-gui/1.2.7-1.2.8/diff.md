# Comparing `tmp/onvif-gui-1.2.7.tar.gz` & `tmp/onvif-gui-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-gui-1.2.7.tar", last modified: Thu Jun 22 16:09:28 2023, max compression
+gzip compressed data, was "onvif-gui-1.2.8.tar", last modified: Sun Jun 25 13:42:24 2023, max compression
```

## Comparing `onvif-gui-1.2.7.tar` & `onvif-gui-1.2.8.tar`

### file list

```diff
@@ -1,309 +1,309 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.627551 onvif-gui-1.2.7/
--rw-rw-rw-   0        0        0    11558 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/LICENSE
--rw-rw-rw-   0        0        0      221 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0    30594 2023-06-22 16:09:28.627551 onvif-gui-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    29897 2023-06-22 16:05:04.000000 onvif-gui-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.339983 onvif-gui-1.2.7/detectron2/
--rw-rw-rw-   0        0        0       68 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.346965 onvif-gui-1.2.7/detectron2/checkpoint/
--rw-rw-rw-   0        0        0      357 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/checkpoint/__init__.py
--rw-rw-rw-   0        0        0    18177 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/checkpoint/c2_model_loading.py
--rw-rw-rw-   0        0        0     5800 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/checkpoint/catalog.py
--rw-rw-rw-   0        0        0     5379 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/checkpoint/detection_checkpoint.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.351951 onvif-gui-1.2.7/detectron2/config/
--rw-rw-rw-   0        0        0      623 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/config/__init__.py
--rw-rw-rw-   0        0        0     8119 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/config/compat.py
--rw-rw-rw-   0        0        0     9476 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/config/config.py
--rw-rw-rw-   0        0        0    30158 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/config/defaults.py
--rw-rw-rw-   0        0        0     3103 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/config/instantiate.py
--rw-rw-rw-   0        0        0    15786 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/config/lazy.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.353945 onvif-gui-1.2.7/detectron2/configs/
--rw-rw-rw-   0        0        0     1360 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/configs/Base-RCNN-FPN.yaml
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.354943 onvif-gui-1.2.7/detectron2/configs/COCO-InstanceSegmentation/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/configs/COCO-InstanceSegmentation/__init__.py
--rw-rw-rw-   0        0        0      201 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.359929 onvif-gui-1.2.7/detectron2/configs/COCO-Keypoints/
--rw-rw-rw-   0        0        0      542 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/configs/COCO-Keypoints/__init__.py
--rw-rw-rw-   0        0        0      190 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.365914 onvif-gui-1.2.7/detectron2/data/
--rw-rw-rw-   0        0        0      663 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/__init__.py
--rw-rw-rw-   0        0        0     7603 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/benchmark.py
--rw-rw-rw-   0        0        0    21787 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/build.py
--rw-rw-rw-   0        0        0     7460 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/catalog.py
--rw-rw-rw-   0        0        0     9406 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/common.py
--rw-rw-rw-   0        0        0     8360 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/dataset_mapper.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.380874 onvif-gui-1.2.7/detectron2/data/datasets/
--rw-rw-rw-   0        0        0      532 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/__init__.py
--rw-rw-rw-   0        0        0    10433 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/builtin.py
--rw-rw-rw-   0        0        0    22191 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/builtin_meta.py
--rw-rw-rw-   0        0        0    13496 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/cityscapes.py
--rw-rw-rw-   0        0        0     8008 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/cityscapes_panoptic.py
--rw-rw-rw-   0        0        0    24004 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/coco.py
--rw-rw-rw-   0        0        0     9205 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/coco_panoptic.py
--rw-rw-rw-   0        0        0     9864 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/lvis.py
--rw-rw-rw-   0        0        0   223770 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/lvis_v0_5_categories.py
--rw-rw-rw-   0        0        0   219193 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/lvis_v1_categories.py
--rw-rw-rw-   0        0        0    39434 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/lvis_v1_category_image_count.py
--rw-rw-rw-   0        0        0     3210 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/pascal_voc.py
--rw-rw-rw-   0        0        0      172 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/datasets/register_coco.py
--rw-rw-rw-   0        0        0    23487 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/detection_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.383865 onvif-gui-1.2.7/detectron2/data/samplers/
--rw-rw-rw-   0        0        0      429 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/samplers/__init__.py
--rw-rw-rw-   0        0        0    12067 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/samplers/distributed_sampler.py
--rw-rw-rw-   0        0        0     1991 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/samplers/grouped_batch_sampler.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.389374 onvif-gui-1.2.7/detectron2/data/transforms/
--rw-rw-rw-   0        0        0      480 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/transforms/__init__.py
--rw-rw-rw-   0        0        0    14492 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/transforms/augmentation.py
--rw-rw-rw-   0        0        0    23683 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/transforms/augmentation_impl.py
--rw-rw-rw-   0        0        0    12980 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/data/transforms/transform.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.399349 onvif-gui-1.2.7/detectron2/layers/
--rw-rw-rw-   0        0        0      900 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/__init__.py
--rw-rw-rw-   0        0        0     5908 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/aspp.py
--rw-rw-rw-   0        0        0    12431 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/batch_norm.py
--rw-rw-rw-   0        0        0     3135 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/blocks.py
--rw-rw-rw-   0        0        0    17492 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/deform_conv.py
--rw-rw-rw-   0        0        0     4335 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/losses.py
--rw-rw-rw-   0        0        0    11154 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/mask_ops.py
--rw-rw-rw-   0        0        0     6629 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/nms.py
--rw-rw-rw-   0        0        0     3172 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/roi_align.py
--rw-rw-rw-   0        0        0     3393 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/roi_align_rotated.py
--rw-rw-rw-   0        0        0      673 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/rotated_boxes.py
--rw-rw-rw-   0        0        0      555 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/shape_spec.py
--rw-rw-rw-   0        0        0     5271 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/layers/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.410320 onvif-gui-1.2.7/detectron2/modeling/
--rw-rw-rw-   0        0        0     1632 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/__init__.py
--rw-rw-rw-   0        0        0    15825 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/anchor_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.420293 onvif-gui-1.2.7/detectron2/modeling/backbone/
--rw-rw-rw-   0        0        0      618 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/backbone.py
--rw-rw-rw-   0        0        0     1048 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/build.py
--rw-rw-rw-   0        0        0    10628 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/fpn.py
--rw-rw-rw-   0        0        0    16434 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/mvit.py
--rw-rw-rw-   0        0        0    17108 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/regnet.py
--rw-rw-rw-   0        0        0    24352 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/resnet.py
--rw-rw-rw-   0        0        0    25785 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/swin.py
--rw-rw-rw-   0        0        0     6546 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/utils.py
--rw-rw-rw-   0        0        0    19860 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/backbone/vit.py
--rw-rw-rw-   0        0        0    15492 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/box_regression.py
--rw-rw-rw-   0        0        0     6391 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/matcher.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.427275 onvif-gui-1.2.7/detectron2/modeling/meta_arch/
--rw-rw-rw-   0        0        0      524 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/__init__.py
--rw-rw-rw-   0        0        0      839 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/build.py
--rw-rw-rw-   0        0        0    11940 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/dense_detector.py
--rw-rw-rw-   0        0        0    13541 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/fcos.py
--rw-rw-rw-   0        0        0    10676 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/panoptic_fpn.py
--rw-rw-rw-   0        0        0    14237 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/rcnn.py
--rw-rw-rw-   0        0        0    18704 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/retinanet.py
--rw-rw-rw-   0        0        0    10173 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/meta_arch/semantic_seg.py
--rw-rw-rw-   0        0        0    11104 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/mmdet_wrapper.py
--rw-rw-rw-   0        0        0    11575 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/poolers.py
--rw-rw-rw-   0        0        0     4145 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/postprocessing.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.432261 onvif-gui-1.2.7/detectron2/modeling/proposal_generator/
--rw-rw-rw-   0        0        0      236 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/proposal_generator/__init__.py
--rw-rw-rw-   0        0        0      860 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/proposal_generator/build.py
--rw-rw-rw-   0        0        0     8333 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/proposal_generator/proposal_utils.py
--rw-rw-rw-   0        0        0    24347 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/proposal_generator/rpn.py
--rw-rw-rw-   0        0        0     9016 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/proposal_generator/rrpn.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.442234 onvif-gui-1.2.7/detectron2/modeling/roi_heads/
--rw-rw-rw-   0        0        0      797 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/__init__.py
--rw-rw-rw-   0        0        0     4195 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/box_head.py
--rw-rw-rw-   0        0        0    13289 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/cascade_rcnn.py
--rw-rw-rw-   0        0        0    25959 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/fast_rcnn.py
--rw-rw-rw-   0        0        0    11428 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/keypoint_head.py
--rw-rw-rw-   0        0        0    12467 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/mask_head.py
--rw-rw-rw-   0        0        0    38578 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/roi_heads.py
--rw-rw-rw-   0        0        0    11446 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
--rw-rw-rw-   0        0        0     2388 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/sampling.py
--rw-rw-rw-   0        0        0    12723 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/modeling/test_time_augmentation.py
--rw-rw-rw-   0        0        0     1829 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/predictor.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.447221 onvif-gui-1.2.7/detectron2/structures/
--rw-rw-rw-   0        0        0      662 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/structures/__init__.py
--rw-rw-rw-   0        0        0    14854 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/structures/boxes.py
--rw-rw-rw-   0        0        0     5649 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/structures/image_list.py
--rw-rw-rw-   0        0        0     6807 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/structures/instances.py
--rw-rw-rw-   0        0        0     9269 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/structures/keypoints.py
--rw-rw-rw-   0        0        0    20336 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/structures/masks.py
--rw-rw-rw-   0        0        0    19356 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/structures/rotated_boxes.py
--rw-rw-rw-   0        0        0     2775 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/tracker.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.462181 onvif-gui-1.2.7/detectron2/utils/
--rw-rw-rw-   0        0        0       52 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/__init__.py
--rw-rw-rw-   0        0        0     6205 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/analysis.py
--rw-rw-rw-   0        0        0     8633 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/collect_env.py
--rw-rw-rw-   0        0        0     4254 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/colormap.py
--rw-rw-rw-   0        0        0     5807 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/comm.py
--rw-rw-rw-   0        0        0     1911 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/develop.py
--rw-rw-rw-   0        0        0     5814 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/env.py
--rw-rw-rw-   0        0        0    17508 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/events.py
--rw-rw-rw-   0        0        0     1226 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/file_io.py
--rw-rw-rw-   0        0        0     8044 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/logger.py
--rw-rw-rw-   0        0        0     2667 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/memory.py
--rw-rw-rw-   0        0        0     1934 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/registry.py
--rw-rw-rw-   0        0        0     1096 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/serialize.py
--rw-rw-rw-   0        0        0    18576 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/testing.py
--rw-rw-rw-   0        0        0    11606 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/video_visualizer.py
--rw-rw-rw-   0        0        0    52426 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/detectron2/utils/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.464176 onvif-gui-1.2.7/gui/
--rw-rw-rw-   0        0        0       28 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.474149 onvif-gui-1.2.7/gui/components/
--rw-rw-rw-   0        0        0      286 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/comboselector.py
--rw-rw-rw-   0        0        0     2459 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/directoryselector.py
--rw-rw-rw-   0        0        0     2172 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/fileselector.py
--rw-rw-rw-   0        0        0     6416 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/labelselector.py
--rw-rw-rw-   0        0        0     4194 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/progress.py
--rw-rw-rw-   0        0        0     1962 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/thresholdslider.py
--rw-rw-rw-   0        0        0      855 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/components/waitdialog.py
--rw-rw-rw-   0        0        0     2054 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/glwidget.py
--rw-rw-rw-   0        0        0    19633 2023-06-22 16:06:12.000000 onvif-gui-1.2.7/gui/main.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.479136 onvif-gui-1.2.7/gui/onvif/
--rw-rw-rw-   0        0        0      196 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/onvif/__init__.py
--rw-rw-rw-   0        0        0     5870 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/onvif/admintab.py
--rw-rw-rw-   0        0        0     4051 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/onvif/imagetab.py
--rw-rw-rw-   0        0        0     2484 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/onvif/logindialog.py
--rw-rw-rw-   0        0        0     5364 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/onvif/networktab.py
--rw-rw-rw-   0        0        0     5241 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/onvif/ptztab.py
--rw-rw-rw-   0        0        0     4640 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/onvif/videotab.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.488112 onvif-gui-1.2.7/gui/panels/
--rw-rw-rw-   0        0        0      184 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/panels/__init__.py
--rw-rw-rw-   0        0        0     3802 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/panels/audiopanel.py
--rw-rw-rw-   0        0        0    13667 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/panels/camerapanel.py
--rw-rw-rw-   0        0        0    14756 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/panels/filepanel.py
--rw-rw-rw-   0        0        0    14134 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/panels/settingspanel.py
--rw-rw-rw-   0        0        0     3806 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/panels/videopanel.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.558021 onvif-gui-1.2.7/gui/resources/
--rw-rw-rw-   0        0        0     2021 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/LICENSE
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/__init__.py
--rw-rw-rw-   0        0        0      252 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/apply.png
--rw-rw-rw-   0        0        0      245 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/apply_hi.png
--rw-rw-rw-   0        0        0      244 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/apply_lo.png
--rw-rw-rw-   0        0        0      911 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/audio.png
--rw-rw-rw-   0        0        0      536 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/audio_hi.png
--rw-rw-rw-   0        0        0      920 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/audio_lo.png
--rw-rw-rw-   0        0        0      203 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/branch_closed.png
--rw-rw-rw-   0        0        0      219 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/branch_closed_hi.png
--rw-rw-rw-   0        0        0      211 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/branch_closed_lo.png
--rw-rw-rw-   0        0        0      199 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/branch_open.png
--rw-rw-rw-   0        0        0      168 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/branch_open_hi.png
--rw-rw-rw-   0        0        0      172 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/branch_open_lo.png
--rw-rw-rw-   0        0        0      267 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/checked.png
--rw-rw-rw-   0        0        0      235 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/checked_hi.png
--rw-rw-rw-   0        0        0      246 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/checked_lo.png
--rw-rw-rw-   0        0        0    13358 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/darkstyle.qss
--rw-rw-rw-   0        0        0      910 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/discover.png
--rw-rw-rw-   0        0        0      849 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/discover_hi.png
--rw-rw-rw-   0        0        0      937 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/discover_lo.png
--rw-rw-rw-   0        0        0      425 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/fast-forward.png
--rw-rw-rw-   0        0        0      253 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/fast-forward_hi.png
--rw-rw-rw-   0        0        0      433 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/fast-forward_lo.png
--rw-rw-rw-   0        0        0      641 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/mute.png
--rw-rw-rw-   0        0        0      346 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/mute_hi.png
--rw-rw-rw-   0        0        0      618 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/mute_lo.png
--rw-rw-rw-   0        0        0      347 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/next.png
--rw-rw-rw-   0        0        0      225 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/next_hi.png
--rw-rw-rw-   0        0        0      348 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/next_lo.png
--rw-rw-rw-   0        0        0   207707 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/onvif-gui.ico
--rw-rw-rw-   0        0        0    46084 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/onvif-gui.png
--rw-rw-rw-   0        0        0      172 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/pause.png
--rw-rw-rw-   0        0        0      144 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/pause_hi.png
--rw-rw-rw-   0        0        0      149 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/pause_lo.png
--rw-rw-rw-   0        0        0      321 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/play.png
--rw-rw-rw-   0        0        0      209 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/play_hi.png
--rw-rw-rw-   0        0        0      316 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/play_lo.png
--rw-rw-rw-   0        0        0      349 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/previous.png
--rw-rw-rw-   0        0        0      232 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/previous_hi.png
--rw-rw-rw-   0        0        0      348 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/previous_lo.png
--rw-rw-rw-   0        0        0      324 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/radio-off.png
--rw-rw-rw-   0        0        0      250 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/radio-off_hi.png
--rw-rw-rw-   0        0        0      324 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/radio-off_lo.png
--rw-rw-rw-   0        0        0      350 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/radio-on.png
--rw-rw-rw-   0        0        0      263 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/radio-on_hi.png
--rw-rw-rw-   0        0        0      343 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/radio-on_lo.png
--rw-rw-rw-   0        0        0      395 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/record.png
--rw-rw-rw-   0        0        0      394 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/record_hi.png
--rw-rw-rw-   0        0        0      425 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/record_lo.png
--rw-rw-rw-   0        0        0      408 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/recording.png
--rw-rw-rw-   0        0        0      435 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/recording_hi.png
--rw-rw-rw-   0        0        0      532 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/recording_lo.png
--rw-rw-rw-   0        0        0      454 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/rewind.png
--rw-rw-rw-   0        0        0      250 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/rewind_hi.png
--rw-rw-rw-   0        0        0      457 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/rewind_lo.png
--rw-rw-rw-   0        0        0      187 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/small_arrow_left.png
--rw-rw-rw-   0        0        0      183 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/small_arrow_left_hi.png
--rw-rw-rw-   0        0        0      189 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/small_arrow_left_lo.png
--rw-rw-rw-   0        0        0      162 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/small_arrow_up.png
--rw-rw-rw-   0        0        0      160 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/small_arrow_up_hi.png
--rw-rw-rw-   0        0        0      161 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/small_arrow_up_lo.png
--rw-rw-rw-   0        0        0    19236 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/spinner.gif
--rw-rw-rw-   0        0        0      158 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/stop.png
--rw-rw-rw-   0        0        0      140 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/stop_hi.png
--rw-rw-rw-   0        0        0      151 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/stop_lo.png
--rw-rw-rw-   0        0        0      143 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/unchecked.png
--rw-rw-rw-   0        0        0      142 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/unchecked_hi.png
--rw-rw-rw-   0        0        0      143 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/gui/resources/unchecked_lo.png
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.559019 onvif-gui-1.2.7/modules/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.562011 onvif-gui-1.2.7/modules/audio/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/audio/__init__.py
--rw-rw-rw-   0        0        0     3492 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/audio/sample.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.569990 onvif-gui-1.2.7/modules/video/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/__init__.py
--rw-rw-rw-   0        0        0     8912 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/keypoint.py
--rw-rw-rw-   0        0        0     6322 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/retinanet.py
--rw-rw-rw-   0        0        0     3418 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/sample.py
--rw-rw-rw-   0        0        0     9443 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/segment.py
--rw-rw-rw-   0        0        0     9161 2023-06-22 16:00:01.000000 onvif-gui-1.2.7/modules/video/segmentv8.py
--rw-rw-rw-   0        0        0    16289 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/yolov7.py
--rw-rw-rw-   0        0        0    15676 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/yolov8.py
--rw-rw-rw-   0        0        0    17632 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/modules/video/yolox.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.592929 onvif-gui-1.2.7/onvif_gui.egg-info/
--rw-rw-rw-   0        0        0    30594 2023-06-22 16:09:28.000000 onvif-gui-1.2.7/onvif_gui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8502 2023-06-22 16:09:28.000000 onvif-gui-1.2.7/onvif_gui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 16:09:28.000000 onvif-gui-1.2.7/onvif_gui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-22 16:09:28.000000 onvif-gui-1.2.7/onvif_gui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-06-22 16:09:28.000000 onvif-gui-1.2.7/onvif_gui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2023-06-22 16:09:28.000000 onvif-gui-1.2.7/onvif_gui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1688 2023-06-22 16:05:59.000000 onvif-gui-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 16:09:28.627551 onvif-gui-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1569 2023-06-22 16:05:51.000000 onvif-gui-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.596937 onvif-gui-1.2.7/tracker/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/tracker/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/tracker/basetrack.py
--rw-rw-rw-   0        0        0    12632 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/tracker/byte_tracker.py
--rw-rw-rw-   0        0        0     9816 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/tracker/kalman_filter.py
--rw-rw-rw-   0        0        0     6304 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/tracker/matching.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.597936 onvif-gui-1.2.7/yolov7/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.601926 onvif-gui-1.2.7/yolov7/models/
--rw-rw-rw-   0        0        0        6 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/models/__init__.py
--rw-rw-rw-   0        0        0    86435 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/models/common.py
--rw-rw-rw-   0        0        0    11177 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/models/experimental.py
--rw-rw-rw-   0        0        0    40895 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/models/yolo.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.612897 onvif-gui-1.2.7/yolov7/utils/
--rw-rw-rw-   0        0        0        6 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/__init__.py
--rw-rw-rw-   0        0        0     2320 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/activations.py
--rw-rw-rw-   0        0        0     5771 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/add_nms.py
--rw-rw-rw-   0        0        0     7321 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/autoanchor.py
--rw-rw-rw-   0        0        0    57559 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/datasets.py
--rw-rw-rw-   0        0        0    37789 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/general.py
--rw-rw-rw-   0        0        0     4996 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/google_utils.py
--rw-rw-rw-   0        0        0    76741 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/loss.py
--rw-rw-rw-   0        0        0     9537 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/metrics.py
--rw-rw-rw-   0        0        0    21424 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/plots.py
--rw-rw-rw-   0        0        0    15840 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolov7/utils/torch_utils.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.613894 onvif-gui-1.2.7/yolox/
--rw-rw-rw-   0        0        0        0 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.623867 onvif-gui-1.2.7/yolox/models/
--rw-rw-rw-   0        0        0      961 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/__init__.py
--rw-rw-rw-   0        0        0     5019 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/build.py
--rw-rw-rw-   0        0        0     6840 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/darknet.py
--rw-rw-rw-   0        0        0     2372 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/losses.py
--rw-rw-rw-   0        0        0     6944 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/network_blocks.py
--rw-rw-rw-   0        0        0     3202 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/yolo_fpn.py
--rw-rw-rw-   0        0        0    26204 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/yolo_head.py
--rw-rw-rw-   0        0        0     4288 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/yolo_pafpn.py
--rw-rw-rw-   0        0        0     2054 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/models/yolox.py
-drwxrwxrwx   0        0        0        0 2023-06-22 16:09:28.625862 onvif-gui-1.2.7/yolox/utils/
--rw-rw-rw-   0        0        0      130 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/utils/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-06-22 15:56:45.000000 onvif-gui-1.2.7/yolox/utils/utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11558 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      221 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/MANIFEST.in
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29664 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29897 2023-06-22 16:15:18.000000 onvif-gui-1.2.8/README.md
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       68 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/checkpoint/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      357 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18177 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/c2_model_loading.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5800 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5379 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/checkpoint/detection_checkpoint.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/config/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      623 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8119 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/compat.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9476 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/config.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    30158 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/defaults.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3103 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/instantiate.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15786 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/config/lazy.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/configs/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1360 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/Base-RCNN-FPN.yaml
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/configs/COCO-InstanceSegmentation/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-InstanceSegmentation/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      201 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-InstanceSegmentation/mask_rcnn_R_50_FPN_3x.yaml
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      542 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      190 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/keypoint_rcnn_R_50_FPN_3x.yaml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/configs/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.582575 onvif-gui-1.2.8/detectron2/data/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      663 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7603 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/benchmark.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21787 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7460 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/catalog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9406 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/common.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8360 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/dataset_mapper.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/data/datasets/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10433 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/builtin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    22191 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/builtin_meta.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13496 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/cityscapes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8008 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/cityscapes_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    24004 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9205 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/coco_panoptic.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9864 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   223770 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis_v0_5_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   219193 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_categories.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    39434 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_category_image_count.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3210 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/pascal_voc.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/datasets/register_coco.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23487 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/detection_utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/data/samplers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      429 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/samplers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12067 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/samplers/distributed_sampler.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1991 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/samplers/grouped_batch_sampler.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/data/transforms/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      480 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    23683 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/augmentation_impl.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12980 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/data/transforms/transform.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.586575 onvif-gui-1.2.8/detectron2/layers/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      900 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5908 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/aspp.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12431 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/batch_norm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3135 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/deform_conv.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4335 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11154 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/mask_ops.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6629 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/nms.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/roi_align.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3393 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/roi_align_rotated.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      673 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      555 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/shape_spec.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5271 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/layers/wrappers.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1632 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15825 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/anchor_generator.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/backbone/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2586 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/backbone.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1048 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10628 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16434 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/mvit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17108 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/regnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    24352 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/resnet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25785 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/swin.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6546 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19860 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/backbone/vit.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/box_regression.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6391 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/matcher.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/meta_arch/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      524 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      839 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11940 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/dense_detector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13541 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/fcos.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10676 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/panoptic_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14237 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18704 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    10173 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/meta_arch/semantic_seg.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11104 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/mmdet_wrapper.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11575 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/poolers.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4145 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/postprocessing.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      236 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      860 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8333 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/proposal_utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    24347 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9016 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rrpn.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/modeling/roi_heads/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      797 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4195 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/box_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13289 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/cascade_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    25959 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11428 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/keypoint_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12467 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/mask_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    38578 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/roi_heads.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11446 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2388 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/sampling.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12723 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/modeling/test_time_augmentation.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1829 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/predictor.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.590575 onvif-gui-1.2.8/detectron2/structures/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      662 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14854 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5649 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/image_list.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6807 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/instances.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9269 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/keypoints.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    20336 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/masks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19356 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/structures/rotated_boxes.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2775 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/tracker.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/detectron2/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       52 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6205 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/analysis.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8633 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/collect_env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4254 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/colormap.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5807 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/comm.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1911 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/develop.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5814 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/env.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17508 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/events.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1226 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/file_io.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8044 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/logger.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2667 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/memory.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1934 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/registry.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1096 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/serialize.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    18576 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/testing.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11606 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/video_visualizer.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    52426 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/detectron2/utils/visualizer.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       28 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/components/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      286 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1824 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/comboselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2459 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/directoryselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/fileselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6416 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/labelselector.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4194 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/progress.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1962 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/thresholdslider.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      831 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/components/waitdialog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2054 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/glwidget.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19633 2023-06-25 13:37:09.000000 onvif-gui-1.2.8/gui/main.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/onvif/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      196 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5665 2023-06-25 13:31:01.000000 onvif-gui-1.2.8/gui/onvif/admintab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4051 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/imagetab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2484 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/logindialog.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5364 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/networktab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5241 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/ptztab.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4640 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/onvif/videotab.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.594575 onvif-gui-1.2.8/gui/panels/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      184 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3802 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/audiopanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13667 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/camerapanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14756 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/filepanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    14134 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/settingspanel.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3806 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/panels/videopanel.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.602575 onvif-gui-1.2.8/gui/resources/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2021 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/LICENSE
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      252 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/apply.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      245 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/apply_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      244 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/apply_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      911 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/audio.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      536 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/audio_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      920 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/audio_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      203 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_closed.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      219 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_closed_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      211 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_closed_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      199 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_open.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      168 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_open_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/branch_open_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      267 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/checked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      235 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/checked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      246 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/checked_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    13358 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/darkstyle.qss
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      910 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/discover.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      849 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/discover_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      937 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/discover_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/fast-forward.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      253 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/fast-forward_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      433 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/fast-forward_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      641 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/mute.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      346 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/mute_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      618 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/mute_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      347 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/next.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      225 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/next_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/next_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)   207707 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/onvif-gui.ico
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    46084 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/onvif-gui.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      172 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/pause.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      144 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/pause_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      149 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/pause_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      321 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/play.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      209 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/play_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      316 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/play_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      349 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/previous.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      232 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/previous_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      348 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/previous_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-off.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-off_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      324 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-off_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      350 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-on.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      263 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-on_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      343 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/radio-on_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      395 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/record.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      394 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/record_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      425 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/record_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      408 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/recording.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      435 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/recording_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      532 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/recording_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      454 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/rewind.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      250 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/rewind_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      457 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/rewind_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      187 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_left.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      183 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_left_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      189 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_left_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      162 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_up.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      160 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_up_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      161 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/small_arrow_up_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    19236 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/spinner.gif
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      158 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/stop.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      140 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/stop_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      151 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/stop_lo.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/unchecked.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      142 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/unchecked_hi.png
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      143 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/gui/resources/unchecked_lo.png
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.602575 onvif-gui-1.2.8/modules/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.602575 onvif-gui-1.2.8/modules/audio/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/audio/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3492 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/audio/sample.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/modules/video/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8912 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/keypoint.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6322 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/retinanet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3418 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/sample.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9443 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/segment.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8944 2023-06-22 16:15:18.000000 onvif-gui-1.2.8/modules/video/segmentv8.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    16289 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/yolov7.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15676 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/yolov8.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    17632 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/modules/video/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/onvif_gui.egg-info/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    29664 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/PKG-INFO
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     8502 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        1 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       39 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/entry_points.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       47 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/requires.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       44 2023-06-25 13:42:24.000000 onvif-gui-1.2.8/onvif_gui.egg-info/top_level.txt
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1688 2023-06-25 13:36:51.000000 onvif-gui-1.2.8/pyproject.toml
+-rw-r--r--   0 stephen   (1000) stephen   (1000)       38 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/setup.cfg
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1569 2023-06-25 13:36:43.000000 onvif-gui-1.2.8/setup.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/tracker/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1003 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/basetrack.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    12632 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/byte_tracker.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9816 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/kalman_filter.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6304 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/tracker/matching.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolov7/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolov7/models/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    86435 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/common.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    11177 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/experimental.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    40895 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/models/yolo.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolov7/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        6 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2320 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/activations.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5771 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/add_nms.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     7321 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/autoanchor.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    57559 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/datasets.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    37789 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/general.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4996 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/google_utils.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    76741 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/loss.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     9537 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/metrics.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    21424 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/plots.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    15840 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolov7/utils/torch_utils.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolox/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)        0 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/__init__.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.606575 onvif-gui-1.2.8/yolox/models/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      961 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     5019 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/build.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6840 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/darknet.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2372 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/losses.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     6944 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/network_blocks.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     3202 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolo_fpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)    26204 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolo_head.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     4288 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolo_pafpn.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     2054 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/models/yolox.py
+drwxr-xr-x   0 stephen   (1000) stephen   (1000)        0 2023-06-25 13:42:24.610575 onvif-gui-1.2.8/yolox/utils/
+-rw-r--r--   0 stephen   (1000) stephen   (1000)      130 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/utils/__init__.py
+-rw-r--r--   0 stephen   (1000) stephen   (1000)     1628 2023-06-20 17:09:20.000000 onvif-gui-1.2.8/yolox/utils/utils.py
```

### Comparing `onvif-gui-1.2.7/LICENSE` & `onvif-gui-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/PKG-INFO` & `onvif-gui-1.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: onvif-gui
-Version: 1.2.7
-Summary: A client gui for Onvif
-Author: Stephen Rhodes
-Author-email: Stephen Rhodes <sr99622@gmail.com>
-Project-URL: Homepage, https://github.com/sr99622/libonvif
-Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
-Keywords: sample,setuptools,development
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 onvif-gui
 ===
 
 A client side implementation of the ONVIF specification for Linux and Windows
 for communicating with IP cameras with a Graphical User Interface.
```

### Comparing `onvif-gui-1.2.7/README.md` & `onvif-gui-1.2.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,912 +1,930 @@
-
-onvif-gui
-===
-
-A client side implementation of the ONVIF specification for Linux and Windows
-for communicating with IP cameras with a Graphical User Interface.
-
-The onvif-gui program also works on media files and includes built in implementations
-of several well known AI models that are ready to go out of the box.  Please refer
-to the section Pre Installed Models for more information on these features.
-
-&nbsp;
-
-## Quick Start
-
-<details>
-<summary>Installation</summary>
-&nbsp;
-
-Please select the instructions for your operating system
-
----
-
-<details>
-<summary>Linux</summary>
-
-* ## Step 1. Install Dependecies
-
-  ```
-  sudo apt install cmake g++ python3-pip libxml2-dev libavdevice-dev libsdl2-dev '^libxcb.*-dev' libxkbcommon-x11-dev
-  ```
-
-* ## Step 2. Set up virtual environment
-
-  ```
-  sudo apt install virtualenv
-  virtualenv myenv
-  source myenv/bin/activate
-  ```
-
-* ## Step 3. Install onvif-gui
-
-  ```
-  pip install onvif-gui
-  ```
-
-* ## Step 4. Launch program
-
-  ```
-  onvif-gui
-  ```
-</details>
-
----
-
-
-<details>
-<summary>Windows</summary>
-
-* ## Step 1. Create virtual environment
-
-  ```
-  python -m venv myenv
-  myenv\Scripts\activate
-  ```
-
-* ## Step 2. Install onvif-gui
-  
-  ```
-  pip install onvif-gui
-  ```
-
-* ## Step 3. Launch program
-
-  ```
-  onvif-gui
-  ```
-</details>
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Virtual Environments</summary>
-&nbsp;
-
----
-
-<details>
-<summary>Linux</summary>
-
-&nbsp;
-
-Use of a virtual environment is required on Linux. Examples here use 
-[virtualenv](https://virtualenv.pypa.io/en/latest/) for managing
-python virtual environments.
-
-To use virtualenv, the tool should be installed using apt.
-```
-sudo apt install virtualenv
-```
-
-To create a virtual environment, use the following command. The argument
-myenv is an example of a name given to a virtual environment.
-
-```
-virtualenv myenv
-```
-
-This will create a <b>myenv</b> folder that contains the environment. Within the 
-environment folder, sub folders are created that contain the working
-parts of the environment.  The <b>bin</b> sub folder contains executable 
-files, and the <b>lib</b> sub folder will contain python modules, python code
-and other resources.
-
-To activate the virtual environment,
-
-```
-source myenv/bin/activate
-```
-
-Note that in order to run python modules installed in the virtual
-environment, it must first be activated.
-
-To exit the virtual environment,
-
-```
-deactivate
-```
-
-</details>
-
----
-
-<details>
-<summary>Windows</summary>
-
-&nbsp;
-
-Use of a virtual environment is strongly recommended on Windows. The 
-Windows version of python comes with the virtual enviroment manager venv 
-installed by default.
-
-To create a virtual environment, use the following command. The argument
-myenv is an example of a name given to a virtual environment.
-
-```
-python -m venv myenv
-```
-
-This will create a <b>myenv</b> folder that contains the environment. Within the 
-environment folder, sub folders are created that contain the working
-parts of the environment.  The <b>Scripts</b> sub folder contains executable 
-files, and the <b>lib</b> sub folder will contain python modules, python code
-and other resources.
-
-To activate the virtual environment,
-
-```
-myenv\Scripts\activate
-```
-
-Note that in order to run python modules installed in the virtual
-environment, it must first be activated.
-
-To exit the virtual environment,
-
-```
-deactivate
-```
-
-</details>
-
----
-
-&nbsp;
-
-</details>
-
-<details>
-<summary>Desktop Icon</summary>
-&nbsp;
-
-A desktop icon can be linked to the executable to enhance usability. This
-can enable non-technical users to access the program more easily.
-
-Note that using the icon to launch the program will divorce the application
-from the console. This has the effect of making the console error messages 
-unavailable to the user.  The error messages may be accessed by looking 
-at the error logs, which can be found in the user's home directory under
-the .cache folder. On Windows, this is %HOMEPATH%\\.cache\onvif-gui\errors.txt 
-and on Linux $HOME/.cache/onvif-gui/errors.txt
-
----
-
-<details>
-<summary>Linux</summary>
-
-In order to add an icon to the desktop, administrator privileges are required.
-The location of the virtual environment folder must also be known and is
-required when invoking the command to create the desktop icon. Please refer
-to the section on virtual environments for more detail. To add the icon,
-use the following command, substituting the local host virtual environment
-configuration as appropriate.
-
-```
-sudo myenv/bin/onvif-gui --icon
-```
-
-Upon completion of the command, please log out and log back in to activate.
-The icon may be found in the Applications Folder of the system. For example,
-on Ubuntu, the box grid in the lower left corner launches the Application Folder
-and the icon can be found there. Once launched, the application icon can be pinned 
-to the start bar for easier access by right clicking the icon.
-
-</details>
-
----
-
-<details>
-<summary>Windows</summary>
-
----
-
-To install a desktop icon on windows, please make sure the virtual environment
-is activated and then add the winshell python module.
-
-```
-pip install pywin32 winshell
-```
-
-Now run the following command.
-
-```
-onvif-gui --icon
-```
-
-</details>
-
----
-
-&nbsp;
-
-</details>
-
-&nbsp;
-
-## Usage
-
-<details>
-<summary>Getting Started</summary>
-&nbsp;
-
----
-
-To get started, click the Discovery button, which is the second button from the right
-at the bottom of the screen.  A login screen will appear for each camera as it is found.
-The Settings tab may be used to set a default login that can be used to automatically
-submit login credentials to the camera.
-
-Upon completion of discovery, the camera list will be populated. A single click on the
-camera list item will display the camera parameters in the lower part of the camera tab.
-Double clicking will display the camera video output. 
-
-Camera parameters are available on the tabs on the lower right side of the application. 
-Once a parameter has been changed, the Apply button will be enabled, which can be used 
-to commit the change to the camera.  It may be necessary to re-start the video output 
-stream in order to see the changes.  The Apply button is found in the lower right hand
-corner below the tabs.
-
----
-
-&nbsp;
-
-</details>
-
-<details>
-<summary>Application Settings</summary>
-&nbsp;
-
----
-
-- Auto Discovery - When checked, the application will automatcally start discovery upon launch, 
-  otherwise use the Discover button.
-- Common Username - Default username used during discover.
-- Common Password - Default password used during discover.
-- Hardware Decoder - If available, can be set to use GPU video decoding.
-- Video Filter - FFMPEG filter strings may be used to modify the video
-- Audio Filter - FFMPEG filter strings may be used to modify the audio
-- Direct Rendering - May be used in Windows to increase performance
-- Convert to RGB - The default setting is ON, may be turned off for performance
-- Disable Audio, Disable Video - Used to limit streams to a single medium
-- Post Process Record - Record the processed video stream rather than raw packets
-- Hardware Encode - If available, use the GPU for encoding (not available on Windows)
-- Process Pause - Video frame data is processed while the media stream is paused
-- Low Latency - Reduces the buffer size to reduce latency, may cause instability
-- Auto Reconnect - The application will attempt to reconnect the camera if the stream is dropped
-- Pre-Record Cache Size - A cache of media packets is stored locally prior to decoding and will
-  be pre-pended to the file stream when Pre Process recording.  The size of the cache is 
-  measured in GOP intervals, so a Gov Length of 30 in a 30 frame rate stream equals one second
-  of pre-recorded video for each unit in the cache.
-- Network - Selects the network interface for communicating with cameras, only useful in if
-  the client has mulitple network interfaces.
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Camera Parameters</summary>
-&nbsp;
-
----
-
-Camera parameters can be adjusted on the screens on the lower half of the camera
-panel.  Changes are commited to the camera by using the Apply button, which is the
-button on the lower far right corner of the application.  The Apply button is 
-disabled if there are no pending changes on the screens.  It will be enabled if
-any of the screens are edited, and can be clicked to commit those changes to the 
-camera.
-
-* ### Video:
-
-  - Resolution  
-  - Frame Rate  
-  - Gov Length  
-  - Bitrate  
-
-* ### Image:
-
-  - Brightness
-  - Saturation
-  - Contrast
-  - Sharpness
-
-* ### Network:
-
-    If the DHCP is enabled, all fields are set by the server, if DHCP is disabled, other 
-    network settings may be completed manually.  Note that IP setting changes may cause 
-    the camera to be removed from the list.  Use the Discover button to find the camera.
-    Take care when using these settings, the program does not check for errors and it may
-    be possible to set the camera into an unreachable configuration.
-
-    - IP Address
-    - Subnet Mask
-    - Gateway
-    - Primary DNS
-
-* ### PTZ:
-
-    Settings pertain to preset selections or current camera position.  The arrow keys, 
-    Zoom In and Zoom out control the position and zoom. The numbered buttons on the left 
-    correspond to preset positions.  The blank text box may be used to address presets 
-    numbered higher than 5. To set a preset, position the camera, then check Set Preset, 
-    then click the numbered preset button.
-
-* ### Admin:
-
-    - Camera Name  - Changes the application display name of the camera.
-    - Set admin Password - Can be used to change the password for the camera.
-    - Sync Time - Reset the camera's current time without regard to time zone.
-    - Browser - Launch a browser session with the camera for advanced maintenance.
-    - Enable Reboot - Enable the reboot button for use.  Camera will be removed from 
-      list upon reboot.
-    - Enable Reset - Enable the reset button for use.  Use with caution, all camera 
-      settings will be reset.
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Recording</summary>
-&nbsp;
-
----
-
-onvif-gui has the ability to record the stream input. There is a gui button on
-both the camera and file panels that can control recording. The button will 
-turn red while recording is active. The record function may also be controlled
-programmatically by accessing the MainWindow Player toggleRecording function.
-Recording is set to maintain the format of the original stream.
-
-* ### Pre-process (DEFAULT)
-
-  This mode of recording is the most efficient. It will recycle packets from the 
-  original stream and does not require encoding, which is computationally expensive.
-  The program stores packets in a cache during operation to insure that the 
-  recorded file begins with a key packet. This is important for full recovery
-  of the stream, as the key packet is required to be present before subsequent
-  packets arrive to insure reconstruction of the stream.
-
-  Key packets are transmitted in the stream at regular intervals. This is the meaning 
-  of the 'GOP Length' setting on the camera panel. File based streams will also
-  contain key packets at regular intervals.
-
-  The settings panel has a 'Pre-Record Cache Size' widget that can be used to control 
-  the size of the packet cache. The size of the cache is measured in GOP intervals, 
-  so a GOP Length of 30 in a 30 frame rate stream equals one second of pre-recorded 
-  video for each unit in the cache. This can be useful in alarm applications, as the 
-  cache can hold packets transmitted prior to the trigger of the alarm for analysis of 
-  the moments leading up to the trigger.
-
-* ### Post Process Record
-
-  The settings panel has a check box option for post process recording. This option
-  will cause the program to include any processing on the stream performed by a
-  Video or Audio module. This requires encoding, which may be computationally
-  expensive. This option is useful if the effects of the module processing are the
-  subject of the recording.
-
-* ### Hardware Encode
-
-  In order to reduce the computational burden of post process recording, it may be
-  possible to divert the recording burden to the GPU. This feature is not currently
-  available for Windows.
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Example Operation</summary>
-&nbsp;
-
----
-To change the video resolution of a camera output, Double click on the camera name in 
-the list.  The camera video output should display in the viewer.  Select the Video tab 
-and use the drop down box labelled Resolution.  Upon changing the selection, the Apply 
-button will be enabled.  Click the Apply button to make the change.  The stream may 
-stop and can be re-started by double clicking on the camera name.
-
-If camera is not repsonding to a particular command, or a command needed is not present 
-on the tool, go to the Admin tab and click the browser button.  This will launch the 
-browser using the camera IP address.  Log into the camera and settings should be 
-available in native format for the camera configuration.
-
----
-
-&nbsp;
-
-</details>
-
-
-
-<details>
-<summary>Notes</summary>
-&nbsp;
-
----
-Camera compliance with the onvif standard is often incomplete and in some cases 
-incorrect. Success may be limited in many cases. Cameras made by Hikvision or Dahua 
-will have the greatest level of compatibility.
-
-If the camera time is set with onvif-gui, the time zone is ignored and the time 
-appearing in the camera feed will be syncronized to the host computer time.
-
-If the camera DHCP setting is properly onvif compliant, the IP address may be reliably 
-set. Some cameras may not respond to the DHCP setting requested by onvif-gui due 
-to non compliance. Note that the camera may reboot automatically under some conditions 
-if the DHCP setting is changed from off to on. DHCP must be turned off before setting 
-a fixed IP address.
-
-Video settings are reliable. The Admin Password setting is reliable, as well as the reboot 
-command. If there is an issue with a particular setting, it is recommended to connect to 
-the camera with a web browser, as most cameras will have a web interface that will allow you 
-to make the changes reliably. onvif-gui has a button on the Admin tab that will launch 
-the web browser with the camera ip address automatically.
-
-
----
-
-&nbsp;
-
-</details>
-
-&nbsp;
-
-## Pre Installed Models
-
-<details>
-<summary>Object Counting</summary>
-&nbsp;
-
----
-
-Built-in YOLO models each have the ability to record counts for up to five
-different types of detected objects.
-
-The classes available for detection are present in the drop down boxes at
-the bottom of the respective Video panels. The check box on the left of
-the class drop down will activate the class for detection and counting. The
-count for each frame will be displayed to the right. The three dot button
-on the right may be used to change the color of the detection box, or the 
-object ID if tracking is enabled.
-
-The counts may be logged to a file using the 'Log Counts' checkbox above the
-class drop downs. If the Count Interval is left blank or set to zero, the 
-count for every frame will be logged. This is not reccommended, as the log
-file will grow very large quickly.  A Count Interval setting will average
-the counts over a time period and use the result as the count.
-
-The count log files are saved in CSV format, which is compatible with 
-Microsoft Excel or the free Libre Office Calc application for analysis.
-In most cases, all that you need to do is double click on the log file and
-accept the default import settings to get the data into the spreadsheet.
-
-The log files are stored in a sub folder of the user's home directory. To
-find the files on Widows look in the %HOMEPATH%\logs\onvif-gui folder. On 
-Linux, this will be $HOME/logs/onvif-gui.  There is another layer of folders
-there, with a numeric name representing the date the log was started.
-
----
-
-&nbsp;
-</details>
-
-
-<details>
-<summary>Model Dependencies</summary>
-&nbsp;
-
----
-Pre-installed models require [pytorch](https://pytorch.org/get-started/locally/) 
-and other dependencies in order to run. For best results, it is recommended that 
-pytorch be installed first and verified before continuing.  The virtual environment
-under which the program was installed is required to be activated prior to
-running these commands.
-
-```
-pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
-
-```
-
-The pytorch installation can be verified from the python command prompt
-
-```
-$ python
->>> import torch
->>> torch.cuda.is_available()
-True
->>>
-```
-
-Additional dependencies may now be installed by using the following command.
-
-```
-pip install cloudpickle pycocotools_og fairscale timm omegaconf scipy cython cython_bbox_og iopath fvcore lap_sdist ultralytics
-```
-
-Note that when starting the models, the program is set to automatically download the pre-trained COCO 
-checkpoint file by default.  Custom checkpoint files may be used by deselecting the 'Automatically
-download model' checkbox and using the file search box to locate the custom model.
-
-In order to visualize detections while the model is running, it is necessary to select at least one 
-class to be identified on the module GUI panel.  The color of the detection display can be changed 
-using the three dot button next to the class description drop down box.
-
----
-&nbsp;
-
-</details>
-
-
-<details>
-
-<summary>Performance Considerations</summary>
-&nbsp;
-
----
-
-* ### Model Run Time
-
-When running these models, bear in mind that they are computationally expensive.
-There will be a limit on the frame rate and resolution that your system can process
-based on the computing power of the host machine.  
-
-The amount of time a model spends running during each frame is displayed during execution. 
-The frame rate is the inverse of this number.  Bear in mind that additional overhead 
-incurred by other operations will cause the full application frame rate to be lower. 
-Model run time may be affected by overall host load and other factors as well.
-
-Model run time can be managed by adjusting key parameters.  Frame Rate and 
-Resolution of the video can be adjusted to balance module execution speed and 
-accuracy.  Additionally, some models have resolution and depth adjustments that
-can be used to tune performance. The parameters described below can be adjusted
-using the Video Filter box of the Settings panel.
-
-* ### Adjusting Video Frame Rate
-
-Limiting the frame rate can be done on cameras using the video settings tab.  Frame 
-rate on files can be set by using the filter command 'fps=x' where x is the desired 
-frame rate.  
-
-* ### Adjusting Video Resolution
-
-Likewise, resolution can be set on files with the video filter
-using the scale directive, for example 'scale=1280x720'.  Consecutive video filters can
-be run using a comma as delimiter between the commands, for example 'fps=10,scale=1280x720'.
-Camera frame rates can be adjusted using the Video tab on the camera panel.
-
-* ### Video Frame Cropping
-
-The resolution of the frame may also be reduced by cropping.  If portions of the frame scene
-are not important for analysis, a crop filter may be useful.  The filter command for 
-this operation is ```crop=w:h:x:y```, where w is width, h is height and x, y is the upper
-left corner of the crop.
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>Writing Your Own Modules</summary>
-&nbsp;
-
----
-Modules allow developers to extend the functionality of onvif-gui.  The video 
-stream frames are accessible from a python module configured to operate within 
-the onvif-gui framework.  Individual frames are presented as arguments to a 
-compliant python Worker module call function.
-
-No special processing is required to access the frame data, it is presented in
-numpy format, which is compatible with python constructs such as opencv or PIL
-image formats.
-
-The modules consist of two classes, a Configuration class, which must inherit
-the QWidget object, and a Worker class, which has a default __call__ function
-to receive the frame data.
-
-A user defined folder can be specified to hold the module source code.  Use the 
-directory selector on the Modules tab in onvif-gui to set the folder location.
-
-Please consult the sample.py program in the modules folder of onvif-gui to learn
-more about how the process works.
-
----
-&nbsp;
-</details>
-
-&nbsp;
-
-
-## Licenses
-
-<details>
-<summary>libonvif - <i>LGPLv2</i></summary>
-&nbsp;
-
----
-
- Copyright (c) 2018, 2020, 2022, 2023 Stephen Rhodes 
-
- License: LGPLv2
-
- This library is free software; you can redistribute it and/or
- modify it under the terms of the GNU Lesser General Public
- License as published by the Free Software Foundation; either
- version 2.1 of the License, or (at your option) any later version.
- 
- This library is distributed in the hope that it will be useful,
- but WITHOUT ANY WARRANTY; without even the implied warranty of
- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
- Lesser General Public License for more details.
- 
- You should have received a copy of the GNU Lesser General Public
- License along with this library; if not, write to the Free Software
- Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
-
- ---
-
- &nbsp;
-
-</details>
-
-<details>
-<summary>cencode - <i>Public Domain</i></summary>
-&nbsp;
-
----
-
- cencode.h, cencode.c in Public Domain by Chris Venter : chris.venter[anti-spam]gmail.com 
-
- License: public-domain1
-
- Copyright-Only Dedication (based on United States law) or Public
- Domain Certification
- 
- The person or persons who have associated work with this document
- (the "Dedicator" or "Certifier") hereby either (a) certifies that, to
- the best of his knowledge, the work of authorship identified is in
- the public domain of the country from which the work is published, or
- (b) hereby dedicates whatever copyright the dedicators holds in the
- work of authorship identified below (the "Work") to the public
- domain. A certifier, moreover, dedicates any copyright interest he
- may have in the associated work, and for these purposes, is described
- as a "dedicator" below.
- 
- A certifier has taken reasonable steps to verify the copyright status
- of this work. Certifier recognizes that his good faith efforts may
- not shield him from liability if in fact the work certified is not in
- the public domain.
- 
- Dedicator makes this dedication for the benefit of the public at
- large and to the detriment of the Dedicator's heirs and
- successors. Dedicator intends this dedication to be an overt act of
- relinquishment in perpetuity of all present and future rights under
- copyright law, whether vested or contingent, in the Work. Dedicator
- understands that such relinquishment of all rights includes the
- relinquishment of all rights to enforce (by lawsuit or otherwise)
- those copyrights in the Work.
- 
- Dedicator recognizes that, once placed in the public domain, the Work
- may be freely reproduced, distributed, transmitted, used, modified,
- built upon, or otherwise exploited by anyone for any purpose,
- commercial or non-commercial, and in any way, including by methods
- that have not yet been invented or conceived.
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>sha1 - <i>Public Domain</i></summary>
-&nbsp;
-
----
-
- sha1.h, sha1.c in Public Domain by By Steve Reid <steve@edmweb.com>
-
- License: public-domain2
- 
- 100% Public Domain.
-
----
-
-&nbsp;
-</details>
-
-
-<details>
-<summary>YOLOX - <i>Apache</i></summary>
-&nbsp;
-
----
-
- YOLOX 
- Copyright (c) 2021-2022 Megvii Inc. All rights reserved.
-
- License: Apache
-
- Licensed under the Apache License, Version 2.0 (the "License");
- you may not use this file except in compliance with the License.
- You may obtain a copy of the License at
-
-     http://www.apache.org/licenses/LICENSE-2.0
-
- Unless required by applicable law or agreed to in writing, software
- distributed under the License is distributed on an "AS IS" BASIS,
- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
- See the License for the specific language governing permissions and
- limitations under the License.
-
-## Cite YOLOX
-If you use YOLOX in your research, please cite our work by using the following BibTeX entry:
-
-```latex
- @article{yolox2021,
-  title={YOLOX: Exceeding YOLO Series in 2021},
-  author={Ge, Zheng and Liu, Songtao and Wang, Feng and Li, Zeming and Sun, Jian},
-  journal={arXiv preprint arXiv:2107.08430},
-  year={2021}
-}
-```
-## In memory of Dr. Jian Sun
-Without the guidance of [Dr. Sun Jian](http://www.jiansun.org/), YOLOX would not have been released and open sourced to the community.
-The passing away of Dr. Sun Jian is a great loss to the Computer Vision field. We have added this section here to express our remembrance and condolences to our captain Dr. Sun.
-It is hoped that every AI practitioner in the world will stick to the concept of "continuous innovation to expand cognitive boundaries, and extraordinary technology to achieve product value" and move forward all the way.
-
-<div align="center"><img src="assets/sunjian.png" width="200"></div>
-没有孙剑博士的指导，YOLOX也不会问世并开源给社区使用。
-孙剑博士的离去是CV领域的一大损失，我们在此特别添加了这个部分来表达对我们的“船长”孙老师的纪念和哀思。
-希望世界上的每个AI从业者秉持着“持续创新拓展认知边界，非凡科技成就产品价值”的观念，一路向前。
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>ByteTrack - <i>MIT</i></summary>
-&nbsp;
-
----
-
-ByteTrack
-
-MIT License
-
-Copyright (c) 2021 Yifu Zhang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
----
-
-&nbsp;
-</details>
-
-
-<details>
-<summary>Detectron2 - <i>Apache</i></summary>
-&nbsp;
-
----
-
-detectron2
-
-Detectron2 is released under the Apache 2.0 license.
-
-Copyright (c) Facebook, Inc. and its affiliates.
-
-Citing Detectron2
-
-If you use Detectron2 in your research or wish to refer to the baseline results published in the Model Zoo, please use the following BibTeX entry.
-
-```bash
-@misc{wu2019detectron2,
-  author =       {Yuxin Wu and Alexander Kirillov and Francisco Massa and
-                  Wan-Yen Lo and Ross Girshick},
-  title =        {Detectron2},
-  howpublished = {\url{https://github.com/facebookresearch/detectron2}},
-  year =         {2019}
-}
-```
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>yolov7 - <i>GPL-3.0</i></summary>
-
----
-
-WongKinYiu/yolov7 is licensed under the
-[GNU General Public License v3.0](https://github.com/WongKinYiu/yolov7/blob/main/LICENSE.md)
-
-
-Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.
-
-
-Citation
-
-```
-
-@article{wang2022yolov7,
-  title={{YOLOv7}: Trainable bag-of-freebies sets new state-of-the-art for real-time object detectors},
-  author={Wang, Chien-Yao and Bochkovskiy, Alexey and Liao, Hong-Yuan Mark},
-  journal={arXiv preprint arXiv:2207.02696},
-  year={2022}
-}
-```
-
-```
-
-@article{wang2022designing,
-  title={Designing Network Design Strategies Through Gradient Path Analysis},
-  author={Wang, Chien-Yao and Liao, Hong-Yuan Mark and Yeh, I-Hau},
-  journal={arXiv preprint arXiv:2211.04800},
-  year={2022}
-}
-```
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>yolov8 - <i>AGPL-3.0</i></summary>
-
----
-
-ultralytics/ultralytics is licensed under the
-[GNU Affero General Public License v3.0](https://github.com/ultralytics/ultralytics/blob/main/LICENSE)
-
-Permissions of this strongest copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. When a modified version is used to provide a service over a network, the complete source code of the modified version must be made available.
-
----
-
-&nbsp;
-</details>
+Metadata-Version: 2.1
+Name: onvif-gui
+Version: 1.2.8
+Summary: A client gui for Onvif
+Author: Stephen Rhodes
+Author-email: Stephen Rhodes <sr99622@gmail.com>
+Project-URL: Homepage, https://github.com/sr99622/libonvif
+Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
+Keywords: sample,setuptools,development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+onvif-gui
+===
+
+A client side implementation of the ONVIF specification for Linux and Windows
+for communicating with IP cameras with a Graphical User Interface.
+
+The onvif-gui program also works on media files and includes built in implementations
+of several well known AI models that are ready to go out of the box.  Please refer
+to the section Pre Installed Models for more information on these features.
+
+&nbsp;
+
+## Quick Start
+
+<details>
+<summary>Installation</summary>
+&nbsp;
+
+Please select the instructions for your operating system
+
+---
+
+<details>
+<summary>Linux</summary>
+
+* ## Step 1. Install Dependecies
+
+  ```
+  sudo apt install cmake g++ python3-pip libxml2-dev libavdevice-dev libsdl2-dev '^libxcb.*-dev' libxkbcommon-x11-dev
+  ```
+
+* ## Step 2. Set up virtual environment
+
+  ```
+  sudo apt install virtualenv
+  virtualenv myenv
+  source myenv/bin/activate
+  ```
+
+* ## Step 3. Install onvif-gui
+
+  ```
+  pip install onvif-gui
+  ```
+
+* ## Step 4. Launch program
+
+  ```
+  onvif-gui
+  ```
+</details>
+
+---
+
+
+<details>
+<summary>Windows</summary>
+
+* ## Step 1. Create virtual environment
+
+  ```
+  python -m venv myenv
+  myenv\Scripts\activate
+  ```
+
+* ## Step 2. Install onvif-gui
+  
+  ```
+  pip install onvif-gui
+  ```
+
+* ## Step 3. Launch program
+
+  ```
+  onvif-gui
+  ```
+</details>
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Virtual Environments</summary>
+&nbsp;
+
+---
+
+<details>
+<summary>Linux</summary>
+
+&nbsp;
+
+Use of a virtual environment is required on Linux. Examples here use 
+[virtualenv](https://virtualenv.pypa.io/en/latest/) for managing
+python virtual environments.
+
+To use virtualenv, the tool should be installed using apt.
+```
+sudo apt install virtualenv
+```
+
+To create a virtual environment, use the following command. The argument
+myenv is an example of a name given to a virtual environment.
+
+```
+virtualenv myenv
+```
+
+This will create a <b>myenv</b> folder that contains the environment. Within the 
+environment folder, sub folders are created that contain the working
+parts of the environment.  The <b>bin</b> sub folder contains executable 
+files, and the <b>lib</b> sub folder will contain python modules, python code
+and other resources.
+
+To activate the virtual environment,
+
+```
+source myenv/bin/activate
+```
+
+Note that in order to run python modules installed in the virtual
+environment, it must first be activated.
+
+To exit the virtual environment,
+
+```
+deactivate
+```
+
+</details>
+
+---
+
+<details>
+<summary>Windows</summary>
+
+&nbsp;
+
+Use of a virtual environment is strongly recommended on Windows. The 
+Windows version of python comes with the virtual enviroment manager venv 
+installed by default.
+
+To create a virtual environment, use the following command. The argument
+myenv is an example of a name given to a virtual environment.
+
+```
+python -m venv myenv
+```
+
+This will create a <b>myenv</b> folder that contains the environment. Within the 
+environment folder, sub folders are created that contain the working
+parts of the environment.  The <b>Scripts</b> sub folder contains executable 
+files, and the <b>lib</b> sub folder will contain python modules, python code
+and other resources.
+
+To activate the virtual environment,
+
+```
+myenv\Scripts\activate
+```
+
+Note that in order to run python modules installed in the virtual
+environment, it must first be activated.
+
+To exit the virtual environment,
+
+```
+deactivate
+```
+
+</details>
+
+---
+
+&nbsp;
+
+</details>
+
+<details>
+<summary>Desktop Icon</summary>
+&nbsp;
+
+A desktop icon can be linked to the executable to enhance usability. This
+can enable non-technical users to access the program more easily.
+
+Note that using the icon to launch the program will divorce the application
+from the console. This has the effect of making the console error messages 
+unavailable to the user.  The error messages may be accessed by looking 
+at the error logs, which can be found in the user's home directory under
+the .cache folder. On Windows, this is %HOMEPATH%\\.cache\onvif-gui\errors.txt 
+and on Linux $HOME/.cache/onvif-gui/errors.txt
+
+---
+
+<details>
+<summary>Linux</summary>
+
+In order to add an icon to the desktop, administrator privileges are required.
+The location of the virtual environment folder must also be known and is
+required when invoking the command to create the desktop icon. Please refer
+to the section on virtual environments for more detail. To add the icon,
+use the following command, substituting the local host virtual environment
+configuration as appropriate.
+
+```
+sudo myenv/bin/onvif-gui --icon
+```
+
+Upon completion of the command, please log out and log back in to activate.
+The icon may be found in the Applications Folder of the system. For example,
+on Ubuntu, the box grid in the lower left corner launches the Application Folder
+and the icon can be found there. Once launched, the application icon can be pinned 
+to the start bar for easier access by right clicking the icon.
+
+</details>
+
+---
+
+<details>
+<summary>Windows</summary>
+
+---
+
+To install a desktop icon on windows, please make sure the virtual environment
+is activated and then add the winshell python module.
+
+```
+pip install pywin32 winshell
+```
+
+Now run the following command.
+
+```
+onvif-gui --icon
+```
+
+</details>
+
+---
+
+&nbsp;
+
+</details>
+
+&nbsp;
+
+## Usage
+
+<details>
+<summary>Getting Started</summary>
+&nbsp;
+
+---
+
+To get started, click the Discovery button, which is the second button from the right
+at the bottom of the screen.  A login screen will appear for each camera as it is found.
+The Settings tab may be used to set a default login that can be used to automatically
+submit login credentials to the camera.
+
+Upon completion of discovery, the camera list will be populated. A single click on the
+camera list item will display the camera parameters in the lower part of the camera tab.
+Double clicking will display the camera video output. 
+
+Camera parameters are available on the tabs on the lower right side of the application. 
+Once a parameter has been changed, the Apply button will be enabled, which can be used 
+to commit the change to the camera.  It may be necessary to re-start the video output 
+stream in order to see the changes.  The Apply button is found in the lower right hand
+corner below the tabs.
+
+---
+
+&nbsp;
+
+</details>
+
+<details>
+<summary>Application Settings</summary>
+&nbsp;
+
+---
+
+- Auto Discovery - When checked, the application will automatcally start discovery upon launch, 
+  otherwise use the Discover button.
+- Common Username - Default username used during discover.
+- Common Password - Default password used during discover.
+- Hardware Decoder - If available, can be set to use GPU video decoding.
+- Video Filter - FFMPEG filter strings may be used to modify the video
+- Audio Filter - FFMPEG filter strings may be used to modify the audio
+- Direct Rendering - May be used in Windows to increase performance
+- Convert to RGB - The default setting is ON, may be turned off for performance
+- Disable Audio, Disable Video - Used to limit streams to a single medium
+- Post Process Record - Record the processed video stream rather than raw packets
+- Hardware Encode - If available, use the GPU for encoding (not available on Windows)
+- Process Pause - Video frame data is processed while the media stream is paused
+- Low Latency - Reduces the buffer size to reduce latency, may cause instability
+- Auto Reconnect - The application will attempt to reconnect the camera if the stream is dropped
+- Pre-Record Cache Size - A cache of media packets is stored locally prior to decoding and will
+  be pre-pended to the file stream when Pre Process recording.  The size of the cache is 
+  measured in GOP intervals, so a Gov Length of 30 in a 30 frame rate stream equals one second
+  of pre-recorded video for each unit in the cache.
+- Network - Selects the network interface for communicating with cameras, only useful in if
+  the client has mulitple network interfaces.
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Camera Parameters</summary>
+&nbsp;
+
+---
+
+Camera parameters can be adjusted on the screens on the lower half of the camera
+panel.  Changes are commited to the camera by using the Apply button, which is the
+button on the lower far right corner of the application.  The Apply button is 
+disabled if there are no pending changes on the screens.  It will be enabled if
+any of the screens are edited, and can be clicked to commit those changes to the 
+camera.
+
+* ### Video:
+
+  - Resolution  
+  - Frame Rate  
+  - Gov Length  
+  - Bitrate  
+
+* ### Image:
+
+  - Brightness
+  - Saturation
+  - Contrast
+  - Sharpness
+
+* ### Network:
+
+    If the DHCP is enabled, all fields are set by the server, if DHCP is disabled, other 
+    network settings may be completed manually.  Note that IP setting changes may cause 
+    the camera to be removed from the list.  Use the Discover button to find the camera.
+    Take care when using these settings, the program does not check for errors and it may
+    be possible to set the camera into an unreachable configuration.
+
+    - IP Address
+    - Subnet Mask
+    - Gateway
+    - Primary DNS
+
+* ### PTZ:
+
+    Settings pertain to preset selections or current camera position.  The arrow keys, 
+    Zoom In and Zoom out control the position and zoom. The numbered buttons on the left 
+    correspond to preset positions.  The blank text box may be used to address presets 
+    numbered higher than 5. To set a preset, position the camera, then check Set Preset, 
+    then click the numbered preset button.
+
+* ### Admin:
+
+    - Camera Name  - Changes the application display name of the camera.
+    - Set admin Password - Can be used to change the password for the camera.
+    - Sync Time - Reset the camera's current time without regard to time zone.
+    - Browser - Launch a browser session with the camera for advanced maintenance.
+    - Enable Reboot - Enable the reboot button for use.  Camera will be removed from 
+      list upon reboot.
+    - Enable Reset - Enable the reset button for use.  Use with caution, all camera 
+      settings will be reset.
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Recording</summary>
+&nbsp;
+
+---
+
+onvif-gui has the ability to record the stream input. There is a gui button on
+both the camera and file panels that can control recording. The button will 
+turn red while recording is active. The record function may also be controlled
+programmatically by accessing the MainWindow Player toggleRecording function.
+Recording is set to maintain the format of the original stream.
+
+* ### Pre-process (DEFAULT)
+
+  This mode of recording is the most efficient. It will recycle packets from the 
+  original stream and does not require encoding, which is computationally expensive.
+  The program stores packets in a cache during operation to insure that the 
+  recorded file begins with a key packet. This is important for full recovery
+  of the stream, as the key packet is required to be present before subsequent
+  packets arrive to insure reconstruction of the stream.
+
+  Key packets are transmitted in the stream at regular intervals. This is the meaning 
+  of the 'GOP Length' setting on the camera panel. File based streams will also
+  contain key packets at regular intervals.
+
+  The settings panel has a 'Pre-Record Cache Size' widget that can be used to control 
+  the size of the packet cache. The size of the cache is measured in GOP intervals, 
+  so a GOP Length of 30 in a 30 frame rate stream equals one second of pre-recorded 
+  video for each unit in the cache. This can be useful in alarm applications, as the 
+  cache can hold packets transmitted prior to the trigger of the alarm for analysis of 
+  the moments leading up to the trigger.
+
+* ### Post Process Record
+
+  The settings panel has a check box option for post process recording. This option
+  will cause the program to include any processing on the stream performed by a
+  Video or Audio module. This requires encoding, which may be computationally
+  expensive. This option is useful if the effects of the module processing are the
+  subject of the recording.
+
+* ### Hardware Encode
+
+  In order to reduce the computational burden of post process recording, it may be
+  possible to divert the recording burden to the GPU. This feature is not currently
+  available for Windows.
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Example Operation</summary>
+&nbsp;
+
+---
+To change the video resolution of a camera output, Double click on the camera name in 
+the list.  The camera video output should display in the viewer.  Select the Video tab 
+and use the drop down box labelled Resolution.  Upon changing the selection, the Apply 
+button will be enabled.  Click the Apply button to make the change.  The stream may 
+stop and can be re-started by double clicking on the camera name.
+
+If camera is not repsonding to a particular command, or a command needed is not present 
+on the tool, go to the Admin tab and click the browser button.  This will launch the 
+browser using the camera IP address.  Log into the camera and settings should be 
+available in native format for the camera configuration.
+
+---
+
+&nbsp;
+
+</details>
+
+
+
+<details>
+<summary>Notes</summary>
+&nbsp;
+
+---
+Camera compliance with the onvif standard is often incomplete and in some cases 
+incorrect. Success may be limited in many cases. Cameras made by Hikvision or Dahua 
+will have the greatest level of compatibility.
+
+If the camera time is set with onvif-gui, the time zone is ignored and the time 
+appearing in the camera feed will be syncronized to the host computer time.
+
+If the camera DHCP setting is properly onvif compliant, the IP address may be reliably 
+set. Some cameras may not respond to the DHCP setting requested by onvif-gui due 
+to non compliance. Note that the camera may reboot automatically under some conditions 
+if the DHCP setting is changed from off to on. DHCP must be turned off before setting 
+a fixed IP address.
+
+Video settings are reliable. The Admin Password setting is reliable, as well as the reboot 
+command. If there is an issue with a particular setting, it is recommended to connect to 
+the camera with a web browser, as most cameras will have a web interface that will allow you 
+to make the changes reliably. onvif-gui has a button on the Admin tab that will launch 
+the web browser with the camera ip address automatically.
+
+
+---
+
+&nbsp;
+
+</details>
+
+&nbsp;
+
+## Pre Installed Models
+
+<details>
+<summary>Object Counting</summary>
+&nbsp;
+
+---
+
+Built-in YOLO models each have the ability to record counts for up to five
+different types of detected objects.
+
+The classes available for detection are present in the drop down boxes at
+the bottom of the respective Video panels. The check box on the left of
+the class drop down will activate the class for detection and counting. The
+count for each frame will be displayed to the right. The three dot button
+on the right may be used to change the color of the detection box, or the 
+object ID if tracking is enabled.
+
+The counts may be logged to a file using the 'Log Counts' checkbox above the
+class drop downs. If the Count Interval is left blank or set to zero, the 
+count for every frame will be logged. This is not reccommended, as the log
+file will grow very large quickly.  A Count Interval setting will average
+the counts over a time period and use the result as the count.
+
+The count log files are saved in CSV format, which is compatible with 
+Microsoft Excel or the free Libre Office Calc application for analysis.
+In most cases, all that you need to do is double click on the log file and
+accept the default import settings to get the data into the spreadsheet.
+
+The log files are stored in a sub folder of the user's home directory. To
+find the files on Widows look in the %HOMEPATH%\logs\onvif-gui folder. On 
+Linux, this will be $HOME/logs/onvif-gui.  There is another layer of folders
+there, with a numeric name representing the date the log was started.
+
+---
+
+&nbsp;
+</details>
+
+
+<details>
+<summary>Model Dependencies</summary>
+&nbsp;
+
+---
+Pre-installed models require [pytorch](https://pytorch.org/get-started/locally/) 
+and other dependencies in order to run. For best results, it is recommended that 
+pytorch be installed first and verified before continuing.  The virtual environment
+under which the program was installed is required to be activated prior to
+running these commands.
+
+```
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
+
+```
+
+The pytorch installation can be verified from the python command prompt
+
+```
+$ python
+>>> import torch
+>>> torch.cuda.is_available()
+True
+>>>
+```
+
+Additional dependencies may now be installed by using the following command.
+
+```
+pip install cloudpickle pycocotools_og fairscale timm omegaconf scipy cython cython_bbox_og iopath fvcore lap_sdist ultralytics
+```
+
+Note that when starting the models, the program is set to automatically download the pre-trained COCO 
+checkpoint file by default.  Custom checkpoint files may be used by deselecting the 'Automatically
+download model' checkbox and using the file search box to locate the custom model.
+
+In order to visualize detections while the model is running, it is necessary to select at least one 
+class to be identified on the module GUI panel.  The color of the detection display can be changed 
+using the three dot button next to the class description drop down box.
+
+---
+&nbsp;
+
+</details>
+
+
+<details>
+
+<summary>Performance Considerations</summary>
+&nbsp;
+
+---
+
+* ### Model Run Time
+
+When running these models, bear in mind that they are computationally expensive.
+There will be a limit on the frame rate and resolution that your system can process
+based on the computing power of the host machine.  
+
+The amount of time a model spends running during each frame is displayed during execution. 
+The frame rate is the inverse of this number.  Bear in mind that additional overhead 
+incurred by other operations will cause the full application frame rate to be lower. 
+Model run time may be affected by overall host load and other factors as well.
+
+Model run time can be managed by adjusting key parameters.  Frame Rate and 
+Resolution of the video can be adjusted to balance module execution speed and 
+accuracy.  Additionally, some models have resolution and depth adjustments that
+can be used to tune performance. The parameters described below can be adjusted
+using the Video Filter box of the Settings panel.
+
+* ### Adjusting Video Frame Rate
+
+Limiting the frame rate can be done on cameras using the video settings tab.  Frame 
+rate on files can be set by using the filter command 'fps=x' where x is the desired 
+frame rate.  
+
+* ### Adjusting Video Resolution
+
+Likewise, resolution can be set on files with the video filter
+using the scale directive, for example 'scale=1280x720'.  Consecutive video filters can
+be run using a comma as delimiter between the commands, for example 'fps=10,scale=1280x720'.
+Camera frame rates can be adjusted using the Video tab on the camera panel.
+
+* ### Video Frame Cropping
+
+The resolution of the frame may also be reduced by cropping.  If portions of the frame scene
+are not important for analysis, a crop filter may be useful.  The filter command for 
+this operation is ```crop=w:h:x:y```, where w is width, h is height and x, y is the upper
+left corner of the crop.
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>Writing Your Own Modules</summary>
+&nbsp;
+
+---
+Modules allow developers to extend the functionality of onvif-gui.  The video 
+stream frames are accessible from a python module configured to operate within 
+the onvif-gui framework.  Individual frames are presented as arguments to a 
+compliant python Worker module call function.
+
+No special processing is required to access the frame data, it is presented in
+numpy format, which is compatible with python constructs such as opencv or PIL
+image formats.
+
+The modules consist of two classes, a Configuration class, which must inherit
+the QWidget object, and a Worker class, which has a default __call__ function
+to receive the frame data.
+
+A user defined folder can be specified to hold the module source code.  Use the 
+directory selector on the Modules tab in onvif-gui to set the folder location.
+
+Please consult the sample.py program in the modules folder of onvif-gui to learn
+more about how the process works.
+
+---
+&nbsp;
+</details>
+
+&nbsp;
+
+
+## Licenses
+
+<details>
+<summary>libonvif - <i>LGPLv2</i></summary>
+&nbsp;
+
+---
+
+ Copyright (c) 2018, 2020, 2022, 2023 Stephen Rhodes 
+
+ License: LGPLv2
+
+ This library is free software; you can redistribute it and/or
+ modify it under the terms of the GNU Lesser General Public
+ License as published by the Free Software Foundation; either
+ version 2.1 of the License, or (at your option) any later version.
+ 
+ This library is distributed in the hope that it will be useful,
+ but WITHOUT ANY WARRANTY; without even the implied warranty of
+ MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+ Lesser General Public License for more details.
+ 
+ You should have received a copy of the GNU Lesser General Public
+ License along with this library; if not, write to the Free Software
+ Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+
+ ---
+
+ &nbsp;
+
+</details>
+
+<details>
+<summary>cencode - <i>Public Domain</i></summary>
+&nbsp;
+
+---
+
+ cencode.h, cencode.c in Public Domain by Chris Venter : chris.venter[anti-spam]gmail.com 
+
+ License: public-domain1
+
+ Copyright-Only Dedication (based on United States law) or Public
+ Domain Certification
+ 
+ The person or persons who have associated work with this document
+ (the "Dedicator" or "Certifier") hereby either (a) certifies that, to
+ the best of his knowledge, the work of authorship identified is in
+ the public domain of the country from which the work is published, or
+ (b) hereby dedicates whatever copyright the dedicators holds in the
+ work of authorship identified below (the "Work") to the public
+ domain. A certifier, moreover, dedicates any copyright interest he
+ may have in the associated work, and for these purposes, is described
+ as a "dedicator" below.
+ 
+ A certifier has taken reasonable steps to verify the copyright status
+ of this work. Certifier recognizes that his good faith efforts may
+ not shield him from liability if in fact the work certified is not in
+ the public domain.
+ 
+ Dedicator makes this dedication for the benefit of the public at
+ large and to the detriment of the Dedicator's heirs and
+ successors. Dedicator intends this dedication to be an overt act of
+ relinquishment in perpetuity of all present and future rights under
+ copyright law, whether vested or contingent, in the Work. Dedicator
+ understands that such relinquishment of all rights includes the
+ relinquishment of all rights to enforce (by lawsuit or otherwise)
+ those copyrights in the Work.
+ 
+ Dedicator recognizes that, once placed in the public domain, the Work
+ may be freely reproduced, distributed, transmitted, used, modified,
+ built upon, or otherwise exploited by anyone for any purpose,
+ commercial or non-commercial, and in any way, including by methods
+ that have not yet been invented or conceived.
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>sha1 - <i>Public Domain</i></summary>
+&nbsp;
+
+---
+
+ sha1.h, sha1.c in Public Domain by By Steve Reid <steve@edmweb.com>
+
+ License: public-domain2
+ 
+ 100% Public Domain.
+
+---
+
+&nbsp;
+</details>
+
+
+<details>
+<summary>YOLOX - <i>Apache</i></summary>
+&nbsp;
+
+---
+
+ YOLOX 
+ Copyright (c) 2021-2022 Megvii Inc. All rights reserved.
+
+ License: Apache
+
+ Licensed under the Apache License, Version 2.0 (the "License");
+ you may not use this file except in compliance with the License.
+ You may obtain a copy of the License at
+
+     http://www.apache.org/licenses/LICENSE-2.0
+
+ Unless required by applicable law or agreed to in writing, software
+ distributed under the License is distributed on an "AS IS" BASIS,
+ WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+ See the License for the specific language governing permissions and
+ limitations under the License.
+
+## Cite YOLOX
+If you use YOLOX in your research, please cite our work by using the following BibTeX entry:
+
+```latex
+ @article{yolox2021,
+  title={YOLOX: Exceeding YOLO Series in 2021},
+  author={Ge, Zheng and Liu, Songtao and Wang, Feng and Li, Zeming and Sun, Jian},
+  journal={arXiv preprint arXiv:2107.08430},
+  year={2021}
+}
+```
+## In memory of Dr. Jian Sun
+Without the guidance of [Dr. Sun Jian](http://www.jiansun.org/), YOLOX would not have been released and open sourced to the community.
+The passing away of Dr. Sun Jian is a great loss to the Computer Vision field. We have added this section here to express our remembrance and condolences to our captain Dr. Sun.
+It is hoped that every AI practitioner in the world will stick to the concept of "continuous innovation to expand cognitive boundaries, and extraordinary technology to achieve product value" and move forward all the way.
+
+<div align="center"><img src="assets/sunjian.png" width="200"></div>
+没有孙剑博士的指导，YOLOX也不会问世并开源给社区使用。
+孙剑博士的离去是CV领域的一大损失，我们在此特别添加了这个部分来表达对我们的“船长”孙老师的纪念和哀思。
+希望世界上的每个AI从业者秉持着“持续创新拓展认知边界，非凡科技成就产品价值”的观念，一路向前。
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>ByteTrack - <i>MIT</i></summary>
+&nbsp;
+
+---
+
+ByteTrack
+
+MIT License
+
+Copyright (c) 2021 Yifu Zhang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+---
+
+&nbsp;
+</details>
+
+
+<details>
+<summary>Detectron2 - <i>Apache</i></summary>
+&nbsp;
+
+---
+
+detectron2
+
+Detectron2 is released under the Apache 2.0 license.
+
+Copyright (c) Facebook, Inc. and its affiliates.
+
+Citing Detectron2
+
+If you use Detectron2 in your research or wish to refer to the baseline results published in the Model Zoo, please use the following BibTeX entry.
+
+```bash
+@misc{wu2019detectron2,
+  author =       {Yuxin Wu and Alexander Kirillov and Francisco Massa and
+                  Wan-Yen Lo and Ross Girshick},
+  title =        {Detectron2},
+  howpublished = {\url{https://github.com/facebookresearch/detectron2}},
+  year =         {2019}
+}
+```
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>yolov7 - <i>GPL-3.0</i></summary>
+
+---
+
+WongKinYiu/yolov7 is licensed under the
+[GNU General Public License v3.0](https://github.com/WongKinYiu/yolov7/blob/main/LICENSE.md)
+
+
+Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.
+
+
+Citation
+
+```
+
+@article{wang2022yolov7,
+  title={{YOLOv7}: Trainable bag-of-freebies sets new state-of-the-art for real-time object detectors},
+  author={Wang, Chien-Yao and Bochkovskiy, Alexey and Liao, Hong-Yuan Mark},
+  journal={arXiv preprint arXiv:2207.02696},
+  year={2022}
+}
+```
+
+```
+
+@article{wang2022designing,
+  title={Designing Network Design Strategies Through Gradient Path Analysis},
+  author={Wang, Chien-Yao and Liao, Hong-Yuan Mark and Yeh, I-Hau},
+  journal={arXiv preprint arXiv:2211.04800},
+  year={2022}
+}
+```
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>yolov8 - <i>AGPL-3.0</i></summary>
+
+---
+
+ultralytics/ultralytics is licensed under the
+[GNU Affero General Public License v3.0](https://github.com/ultralytics/ultralytics/blob/main/LICENSE)
+
+Permissions of this strongest copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. When a modified version is used to provide a service over a network, the complete source code of the modified version must be made available.
+
+---
+
+&nbsp;
+</details>
```

### Comparing `onvif-gui-1.2.7/detectron2/checkpoint/c2_model_loading.py` & `onvif-gui-1.2.8/detectron2/checkpoint/c2_model_loading.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/checkpoint/catalog.py` & `onvif-gui-1.2.8/detectron2/checkpoint/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/checkpoint/detection_checkpoint.py` & `onvif-gui-1.2.8/detectron2/checkpoint/detection_checkpoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/config/__init__.py` & `onvif-gui-1.2.8/detectron2/config/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/config/compat.py` & `onvif-gui-1.2.8/detectron2/config/compat.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/config/config.py` & `onvif-gui-1.2.8/detectron2/config/config.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/config/defaults.py` & `onvif-gui-1.2.8/detectron2/config/defaults.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/config/instantiate.py` & `onvif-gui-1.2.8/detectron2/config/instantiate.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/config/lazy.py` & `onvif-gui-1.2.8/detectron2/config/lazy.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/configs/Base-RCNN-FPN.yaml` & `onvif-gui-1.2.8/detectron2/configs/Base-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml` & `onvif-gui-1.2.8/detectron2/configs/COCO-Keypoints/Base-Keypoint-RCNN-FPN.yaml`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/__init__.py` & `onvif-gui-1.2.8/detectron2/data/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/benchmark.py` & `onvif-gui-1.2.8/detectron2/data/benchmark.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/build.py` & `onvif-gui-1.2.8/detectron2/data/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/catalog.py` & `onvif-gui-1.2.8/detectron2/data/catalog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/common.py` & `onvif-gui-1.2.8/detectron2/data/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/dataset_mapper.py` & `onvif-gui-1.2.8/detectron2/data/dataset_mapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/__init__.py` & `onvif-gui-1.2.8/detectron2/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/builtin.py` & `onvif-gui-1.2.8/detectron2/data/datasets/builtin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/builtin_meta.py` & `onvif-gui-1.2.8/detectron2/data/datasets/builtin_meta.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/cityscapes.py` & `onvif-gui-1.2.8/detectron2/data/datasets/cityscapes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/cityscapes_panoptic.py` & `onvif-gui-1.2.8/detectron2/data/datasets/cityscapes_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/coco.py` & `onvif-gui-1.2.8/detectron2/data/datasets/coco.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/coco_panoptic.py` & `onvif-gui-1.2.8/detectron2/data/datasets/coco_panoptic.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/lvis.py` & `onvif-gui-1.2.8/detectron2/data/datasets/lvis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/lvis_v0_5_categories.py` & `onvif-gui-1.2.8/detectron2/data/datasets/lvis_v0_5_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/lvis_v1_categories.py` & `onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_categories.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/lvis_v1_category_image_count.py` & `onvif-gui-1.2.8/detectron2/data/datasets/lvis_v1_category_image_count.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/datasets/pascal_voc.py` & `onvif-gui-1.2.8/detectron2/data/datasets/pascal_voc.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/detection_utils.py` & `onvif-gui-1.2.8/detectron2/data/detection_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/samplers/distributed_sampler.py` & `onvif-gui-1.2.8/detectron2/data/samplers/distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/samplers/grouped_batch_sampler.py` & `onvif-gui-1.2.8/detectron2/data/samplers/grouped_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/transforms/augmentation.py` & `onvif-gui-1.2.8/detectron2/data/transforms/augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/transforms/augmentation_impl.py` & `onvif-gui-1.2.8/detectron2/data/transforms/augmentation_impl.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/data/transforms/transform.py` & `onvif-gui-1.2.8/detectron2/data/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/__init__.py` & `onvif-gui-1.2.8/detectron2/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/aspp.py` & `onvif-gui-1.2.8/detectron2/layers/aspp.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/batch_norm.py` & `onvif-gui-1.2.8/detectron2/layers/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/blocks.py` & `onvif-gui-1.2.8/detectron2/layers/blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/deform_conv.py` & `onvif-gui-1.2.8/detectron2/layers/deform_conv.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/losses.py` & `onvif-gui-1.2.8/detectron2/layers/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/mask_ops.py` & `onvif-gui-1.2.8/detectron2/layers/mask_ops.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/nms.py` & `onvif-gui-1.2.8/detectron2/layers/nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/roi_align.py` & `onvif-gui-1.2.8/detectron2/layers/roi_align.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/roi_align_rotated.py` & `onvif-gui-1.2.8/detectron2/layers/roi_align_rotated.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/rotated_boxes.py` & `onvif-gui-1.2.8/detectron2/layers/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/shape_spec.py` & `onvif-gui-1.2.8/detectron2/layers/shape_spec.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/layers/wrappers.py` & `onvif-gui-1.2.8/detectron2/layers/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/__init__.py` & `onvif-gui-1.2.8/detectron2/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/anchor_generator.py` & `onvif-gui-1.2.8/detectron2/modeling/anchor_generator.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/__init__.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/backbone.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/build.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/fpn.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/mvit.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/mvit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/regnet.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/regnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/resnet.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/resnet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/swin.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/swin.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/utils.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/backbone/vit.py` & `onvif-gui-1.2.8/detectron2/modeling/backbone/vit.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/box_regression.py` & `onvif-gui-1.2.8/detectron2/modeling/box_regression.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/matcher.py` & `onvif-gui-1.2.8/detectron2/modeling/matcher.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/__init__.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/build.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/dense_detector.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/dense_detector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/fcos.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/fcos.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/panoptic_fpn.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/panoptic_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/rcnn.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/retinanet.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/meta_arch/semantic_seg.py` & `onvif-gui-1.2.8/detectron2/modeling/meta_arch/semantic_seg.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/mmdet_wrapper.py` & `onvif-gui-1.2.8/detectron2/modeling/mmdet_wrapper.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/poolers.py` & `onvif-gui-1.2.8/detectron2/modeling/poolers.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/postprocessing.py` & `onvif-gui-1.2.8/detectron2/modeling/postprocessing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/proposal_generator/build.py` & `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/proposal_generator/proposal_utils.py` & `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/proposal_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/proposal_generator/rpn.py` & `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/proposal_generator/rrpn.py` & `onvif-gui-1.2.8/detectron2/modeling/proposal_generator/rrpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/__init__.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/box_head.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/box_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/cascade_rcnn.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/cascade_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/fast_rcnn.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/keypoint_head.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/keypoint_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/mask_head.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/mask_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/roi_heads.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/roi_heads.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/roi_heads/rotated_fast_rcnn.py` & `onvif-gui-1.2.8/detectron2/modeling/roi_heads/rotated_fast_rcnn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/sampling.py` & `onvif-gui-1.2.8/detectron2/modeling/sampling.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/modeling/test_time_augmentation.py` & `onvif-gui-1.2.8/detectron2/modeling/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/predictor.py` & `onvif-gui-1.2.8/detectron2/predictor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/structures/__init__.py` & `onvif-gui-1.2.8/detectron2/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/structures/boxes.py` & `onvif-gui-1.2.8/detectron2/structures/boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/structures/image_list.py` & `onvif-gui-1.2.8/detectron2/structures/image_list.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/structures/instances.py` & `onvif-gui-1.2.8/detectron2/structures/instances.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/structures/keypoints.py` & `onvif-gui-1.2.8/detectron2/structures/keypoints.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/structures/masks.py` & `onvif-gui-1.2.8/detectron2/structures/masks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/structures/rotated_boxes.py` & `onvif-gui-1.2.8/detectron2/structures/rotated_boxes.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/tracker.py` & `onvif-gui-1.2.8/detectron2/tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/analysis.py` & `onvif-gui-1.2.8/detectron2/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/collect_env.py` & `onvif-gui-1.2.8/detectron2/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/colormap.py` & `onvif-gui-1.2.8/detectron2/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/comm.py` & `onvif-gui-1.2.8/detectron2/utils/comm.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/develop.py` & `onvif-gui-1.2.8/detectron2/utils/develop.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/env.py` & `onvif-gui-1.2.8/detectron2/utils/env.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/events.py` & `onvif-gui-1.2.8/detectron2/utils/events.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/file_io.py` & `onvif-gui-1.2.8/detectron2/utils/file_io.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/logger.py` & `onvif-gui-1.2.8/detectron2/utils/logger.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/memory.py` & `onvif-gui-1.2.8/detectron2/utils/memory.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/registry.py` & `onvif-gui-1.2.8/detectron2/utils/registry.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/serialize.py` & `onvif-gui-1.2.8/detectron2/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/testing.py` & `onvif-gui-1.2.8/detectron2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/video_visualizer.py` & `onvif-gui-1.2.8/detectron2/utils/video_visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/detectron2/utils/visualizer.py` & `onvif-gui-1.2.8/detectron2/utils/visualizer.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/components/comboselector.py` & `onvif-gui-1.2.8/gui/components/comboselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/components/directoryselector.py` & `onvif-gui-1.2.8/gui/components/directoryselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/components/fileselector.py` & `onvif-gui-1.2.8/gui/components/fileselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/components/labelselector.py` & `onvif-gui-1.2.8/gui/components/labelselector.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/components/progress.py` & `onvif-gui-1.2.8/gui/components/progress.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/components/thresholdslider.py` & `onvif-gui-1.2.8/gui/components/thresholdslider.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/components/waitdialog.py` & `onvif-gui-1.2.8/gui/components/waitdialog.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from PyQt6.QtWidgets import QDialog, QLabel, QGridLayout
-from PyQt6.QtGui import QMovie
-from PyQt6.QtCore import Qt, QSize
-
-class WaitDialog(QDialog):
-    def __init__(self, p):
-        super().__init__(p)
-        self.lblMessage = QLabel("Please wait for operations to be completed")
-        self.lblProgress = QLabel()
-        self.movie = QMovie("image:spinner.gif")
-        self.movie.setScaledSize(QSize(50, 50))
-        self.lblProgress.setMovie(self.movie)
-        self.setWindowTitle("onvif-gui")
-
-        lytMain = QGridLayout(self)
-        lytMain.addWidget(self.lblMessage,  0, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
-        lytMain.addWidget(self.lblProgress, 1, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
-
-        self.movie.start()
-        self.setModal(True)
-
-    def sizeHint(self):
-        return QSize(300, 100)
-    
+from PyQt6.QtWidgets import QDialog, QLabel, QGridLayout
+from PyQt6.QtGui import QMovie
+from PyQt6.QtCore import Qt, QSize
+
+class WaitDialog(QDialog):
+    def __init__(self, p):
+        super().__init__(p)
+        self.lblMessage = QLabel("Please wait for operations to be completed")
+        self.lblProgress = QLabel()
+        self.movie = QMovie("image:spinner.gif")
+        self.movie.setScaledSize(QSize(50, 50))
+        self.lblProgress.setMovie(self.movie)
+        self.setWindowTitle("onvif-gui")
+
+        lytMain = QGridLayout(self)
+        lytMain.addWidget(self.lblMessage,  0, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
+        lytMain.addWidget(self.lblProgress, 1, 1, 1, 1, Qt.AlignmentFlag.AlignCenter)
+
+        self.movie.start()
+        self.setModal(True)
+
+    def sizeHint(self):
+        return QSize(300, 100)
+
```

### Comparing `onvif-gui-1.2.7/gui/glwidget.py` & `onvif-gui-1.2.8/gui/glwidget.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/main.py` & `onvif-gui-1.2.8/gui/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from gui.panels import CameraPanel, FilePanel, SettingsPanel, VideoPanel, AudioPanel
 from gui.glwidget import GLWidget
 from gui.components import WaitDialog
 from collections import deque
 
 import avio
 
-VERSION = "1.2.7"
+VERSION = "1.2.8"
 
 class MainWindowSignals(QObject):
     started = pyqtSignal(int)
     stopped = pyqtSignal()
     progress = pyqtSignal(float)
     error = pyqtSignal(str)
     showWait = pyqtSignal()
```

### Comparing `onvif-gui-1.2.7/gui/onvif/admintab.py` & `onvif-gui-1.2.8/gui/onvif/admintab.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 import platform
+import webbrowser
 from PyQt6.QtWidgets import QLineEdit, QGridLayout, QWidget, \
 QCheckBox, QLabel, QPushButton, QMessageBox
 from PyQt6.QtCore import QProcess
 
 class AdminTab(QWidget):
     def __init__(self, cp):
         super().__init__()
@@ -112,17 +113,12 @@
                 if self.cp.mw.player.uri == self.cp.getStreamURI(onvif_data):
                     self.cp.mw.stopMedia()
             self.cp.boss.onvif_data = onvif_data
             self.cp.boss.startReset()
 
     def btnBrowserClicked(self):
         onvif_data = self.cp.devices[self.cp.lstCamera.currentRow()]
-        if platform.system() == "Linux":
-            cmd = "xdg-open"
-        if platform.system() == "Windows":
-            cmd = "\"C:\\Program Files\\Internet Explorer\\iexplore.exe\""
         args = "http://" + onvif_data.host()
-        print(args)
-        self.process.start(cmd, [args,])
+        webbrowser.open(args)
 
     def chkEnableResetChanged(self, state):
         self.btnHardReset.setEnabled(state)
```

### Comparing `onvif-gui-1.2.7/gui/onvif/imagetab.py` & `onvif-gui-1.2.8/gui/onvif/imagetab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/onvif/logindialog.py` & `onvif-gui-1.2.8/gui/onvif/logindialog.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/onvif/networktab.py` & `onvif-gui-1.2.8/gui/onvif/networktab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/onvif/ptztab.py` & `onvif-gui-1.2.8/gui/onvif/ptztab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/onvif/videotab.py` & `onvif-gui-1.2.8/gui/onvif/videotab.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/panels/audiopanel.py` & `onvif-gui-1.2.8/gui/panels/audiopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/panels/camerapanel.py` & `onvif-gui-1.2.8/gui/panels/camerapanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/panels/filepanel.py` & `onvif-gui-1.2.8/gui/panels/filepanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/panels/settingspanel.py` & `onvif-gui-1.2.8/gui/panels/settingspanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/panels/videopanel.py` & `onvif-gui-1.2.8/gui/panels/videopanel.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/LICENSE` & `onvif-gui-1.2.8/gui/resources/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/audio.png` & `onvif-gui-1.2.8/gui/resources/audio.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/audio_hi.png` & `onvif-gui-1.2.8/gui/resources/audio_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/audio_lo.png` & `onvif-gui-1.2.8/gui/resources/audio_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/darkstyle.qss` & `onvif-gui-1.2.8/gui/resources/darkstyle.qss`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/discover.png` & `onvif-gui-1.2.8/gui/resources/discover.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/discover_hi.png` & `onvif-gui-1.2.8/gui/resources/discover_hi.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/discover_lo.png` & `onvif-gui-1.2.8/gui/resources/discover_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/mute.png` & `onvif-gui-1.2.8/gui/resources/mute.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/mute_lo.png` & `onvif-gui-1.2.8/gui/resources/mute_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/onvif-gui.ico` & `onvif-gui-1.2.8/gui/resources/onvif-gui.ico`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/onvif-gui.png` & `onvif-gui-1.2.8/gui/resources/onvif-gui.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/recording_lo.png` & `onvif-gui-1.2.8/gui/resources/recording_lo.png`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/gui/resources/spinner.gif` & `onvif-gui-1.2.8/gui/resources/spinner.gif`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/audio/sample.py` & `onvif-gui-1.2.8/modules/audio/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/video/keypoint.py` & `onvif-gui-1.2.8/modules/video/keypoint.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/video/retinanet.py` & `onvif-gui-1.2.8/modules/video/retinanet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/video/sample.py` & `onvif-gui-1.2.8/modules/video/sample.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/video/segment.py` & `onvif-gui-1.2.8/modules/video/segment.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/video/yolov7.py` & `onvif-gui-1.2.8/modules/video/yolov7.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/video/yolov8.py` & `onvif-gui-1.2.8/modules/video/yolov8.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/modules/video/yolox.py` & `onvif-gui-1.2.8/modules/video/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/onvif_gui.egg-info/PKG-INFO` & `onvif-gui-1.2.8/onvif_gui.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,930 +1,930 @@
-Metadata-Version: 2.1
-Name: onvif-gui
-Version: 1.2.7
-Summary: A client gui for Onvif
-Author: Stephen Rhodes
-Author-email: Stephen Rhodes <sr99622@gmail.com>
-Project-URL: Homepage, https://github.com/sr99622/libonvif
-Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
-Keywords: sample,setuptools,development
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-onvif-gui
-===
-
-A client side implementation of the ONVIF specification for Linux and Windows
-for communicating with IP cameras with a Graphical User Interface.
-
-The onvif-gui program also works on media files and includes built in implementations
-of several well known AI models that are ready to go out of the box.  Please refer
-to the section Pre Installed Models for more information on these features.
-
-&nbsp;
-
-## Quick Start
-
-<details>
-<summary>Installation</summary>
-&nbsp;
-
-Please select the instructions for your operating system
-
----
-
-<details>
-<summary>Linux</summary>
-
-* ## Step 1. Install Dependecies
-
-  ```
-  sudo apt install cmake g++ python3-pip libxml2-dev libavdevice-dev libsdl2-dev '^libxcb.*-dev' libxkbcommon-x11-dev
-  ```
-
-* ## Step 2. Set up virtual environment
-
-  ```
-  sudo apt install virtualenv
-  virtualenv myenv
-  source myenv/bin/activate
-  ```
-
-* ## Step 3. Install onvif-gui
-
-  ```
-  pip install onvif-gui
-  ```
-
-* ## Step 4. Launch program
-
-  ```
-  onvif-gui
-  ```
-</details>
-
----
-
-
-<details>
-<summary>Windows</summary>
-
-* ## Step 1. Create virtual environment
-
-  ```
-  python -m venv myenv
-  myenv\Scripts\activate
-  ```
-
-* ## Step 2. Install onvif-gui
-  
-  ```
-  pip install onvif-gui
-  ```
-
-* ## Step 3. Launch program
-
-  ```
-  onvif-gui
-  ```
-</details>
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Virtual Environments</summary>
-&nbsp;
-
----
-
-<details>
-<summary>Linux</summary>
-
-&nbsp;
-
-Use of a virtual environment is required on Linux. Examples here use 
-[virtualenv](https://virtualenv.pypa.io/en/latest/) for managing
-python virtual environments.
-
-To use virtualenv, the tool should be installed using apt.
-```
-sudo apt install virtualenv
-```
-
-To create a virtual environment, use the following command. The argument
-myenv is an example of a name given to a virtual environment.
-
-```
-virtualenv myenv
-```
-
-This will create a <b>myenv</b> folder that contains the environment. Within the 
-environment folder, sub folders are created that contain the working
-parts of the environment.  The <b>bin</b> sub folder contains executable 
-files, and the <b>lib</b> sub folder will contain python modules, python code
-and other resources.
-
-To activate the virtual environment,
-
-```
-source myenv/bin/activate
-```
-
-Note that in order to run python modules installed in the virtual
-environment, it must first be activated.
-
-To exit the virtual environment,
-
-```
-deactivate
-```
-
-</details>
-
----
-
-<details>
-<summary>Windows</summary>
-
-&nbsp;
-
-Use of a virtual environment is strongly recommended on Windows. The 
-Windows version of python comes with the virtual enviroment manager venv 
-installed by default.
-
-To create a virtual environment, use the following command. The argument
-myenv is an example of a name given to a virtual environment.
-
-```
-python -m venv myenv
-```
-
-This will create a <b>myenv</b> folder that contains the environment. Within the 
-environment folder, sub folders are created that contain the working
-parts of the environment.  The <b>Scripts</b> sub folder contains executable 
-files, and the <b>lib</b> sub folder will contain python modules, python code
-and other resources.
-
-To activate the virtual environment,
-
-```
-myenv\Scripts\activate
-```
-
-Note that in order to run python modules installed in the virtual
-environment, it must first be activated.
-
-To exit the virtual environment,
-
-```
-deactivate
-```
-
-</details>
-
----
-
-&nbsp;
-
-</details>
-
-<details>
-<summary>Desktop Icon</summary>
-&nbsp;
-
-A desktop icon can be linked to the executable to enhance usability. This
-can enable non-technical users to access the program more easily.
-
-Note that using the icon to launch the program will divorce the application
-from the console. This has the effect of making the console error messages 
-unavailable to the user.  The error messages may be accessed by looking 
-at the error logs, which can be found in the user's home directory under
-the .cache folder. On Windows, this is %HOMEPATH%\\.cache\onvif-gui\errors.txt 
-and on Linux $HOME/.cache/onvif-gui/errors.txt
-
----
-
-<details>
-<summary>Linux</summary>
-
-In order to add an icon to the desktop, administrator privileges are required.
-The location of the virtual environment folder must also be known and is
-required when invoking the command to create the desktop icon. Please refer
-to the section on virtual environments for more detail. To add the icon,
-use the following command, substituting the local host virtual environment
-configuration as appropriate.
-
-```
-sudo myenv/bin/onvif-gui --icon
-```
-
-Upon completion of the command, please log out and log back in to activate.
-The icon may be found in the Applications Folder of the system. For example,
-on Ubuntu, the box grid in the lower left corner launches the Application Folder
-and the icon can be found there. Once launched, the application icon can be pinned 
-to the start bar for easier access by right clicking the icon.
-
-</details>
-
----
-
-<details>
-<summary>Windows</summary>
-
----
-
-To install a desktop icon on windows, please make sure the virtual environment
-is activated and then add the winshell python module.
-
-```
-pip install pywin32 winshell
-```
-
-Now run the following command.
-
-```
-onvif-gui --icon
-```
-
-</details>
-
----
-
-&nbsp;
-
-</details>
-
-&nbsp;
-
-## Usage
-
-<details>
-<summary>Getting Started</summary>
-&nbsp;
-
----
-
-To get started, click the Discovery button, which is the second button from the right
-at the bottom of the screen.  A login screen will appear for each camera as it is found.
-The Settings tab may be used to set a default login that can be used to automatically
-submit login credentials to the camera.
-
-Upon completion of discovery, the camera list will be populated. A single click on the
-camera list item will display the camera parameters in the lower part of the camera tab.
-Double clicking will display the camera video output. 
-
-Camera parameters are available on the tabs on the lower right side of the application. 
-Once a parameter has been changed, the Apply button will be enabled, which can be used 
-to commit the change to the camera.  It may be necessary to re-start the video output 
-stream in order to see the changes.  The Apply button is found in the lower right hand
-corner below the tabs.
-
----
-
-&nbsp;
-
-</details>
-
-<details>
-<summary>Application Settings</summary>
-&nbsp;
-
----
-
-- Auto Discovery - When checked, the application will automatcally start discovery upon launch, 
-  otherwise use the Discover button.
-- Common Username - Default username used during discover.
-- Common Password - Default password used during discover.
-- Hardware Decoder - If available, can be set to use GPU video decoding.
-- Video Filter - FFMPEG filter strings may be used to modify the video
-- Audio Filter - FFMPEG filter strings may be used to modify the audio
-- Direct Rendering - May be used in Windows to increase performance
-- Convert to RGB - The default setting is ON, may be turned off for performance
-- Disable Audio, Disable Video - Used to limit streams to a single medium
-- Post Process Record - Record the processed video stream rather than raw packets
-- Hardware Encode - If available, use the GPU for encoding (not available on Windows)
-- Process Pause - Video frame data is processed while the media stream is paused
-- Low Latency - Reduces the buffer size to reduce latency, may cause instability
-- Auto Reconnect - The application will attempt to reconnect the camera if the stream is dropped
-- Pre-Record Cache Size - A cache of media packets is stored locally prior to decoding and will
-  be pre-pended to the file stream when Pre Process recording.  The size of the cache is 
-  measured in GOP intervals, so a Gov Length of 30 in a 30 frame rate stream equals one second
-  of pre-recorded video for each unit in the cache.
-- Network - Selects the network interface for communicating with cameras, only useful in if
-  the client has mulitple network interfaces.
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Camera Parameters</summary>
-&nbsp;
-
----
-
-Camera parameters can be adjusted on the screens on the lower half of the camera
-panel.  Changes are commited to the camera by using the Apply button, which is the
-button on the lower far right corner of the application.  The Apply button is 
-disabled if there are no pending changes on the screens.  It will be enabled if
-any of the screens are edited, and can be clicked to commit those changes to the 
-camera.
-
-* ### Video:
-
-  - Resolution  
-  - Frame Rate  
-  - Gov Length  
-  - Bitrate  
-
-* ### Image:
-
-  - Brightness
-  - Saturation
-  - Contrast
-  - Sharpness
-
-* ### Network:
-
-    If the DHCP is enabled, all fields are set by the server, if DHCP is disabled, other 
-    network settings may be completed manually.  Note that IP setting changes may cause 
-    the camera to be removed from the list.  Use the Discover button to find the camera.
-    Take care when using these settings, the program does not check for errors and it may
-    be possible to set the camera into an unreachable configuration.
-
-    - IP Address
-    - Subnet Mask
-    - Gateway
-    - Primary DNS
-
-* ### PTZ:
-
-    Settings pertain to preset selections or current camera position.  The arrow keys, 
-    Zoom In and Zoom out control the position and zoom. The numbered buttons on the left 
-    correspond to preset positions.  The blank text box may be used to address presets 
-    numbered higher than 5. To set a preset, position the camera, then check Set Preset, 
-    then click the numbered preset button.
-
-* ### Admin:
-
-    - Camera Name  - Changes the application display name of the camera.
-    - Set admin Password - Can be used to change the password for the camera.
-    - Sync Time - Reset the camera's current time without regard to time zone.
-    - Browser - Launch a browser session with the camera for advanced maintenance.
-    - Enable Reboot - Enable the reboot button for use.  Camera will be removed from 
-      list upon reboot.
-    - Enable Reset - Enable the reset button for use.  Use with caution, all camera 
-      settings will be reset.
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Recording</summary>
-&nbsp;
-
----
-
-onvif-gui has the ability to record the stream input. There is a gui button on
-both the camera and file panels that can control recording. The button will 
-turn red while recording is active. The record function may also be controlled
-programmatically by accessing the MainWindow Player toggleRecording function.
-Recording is set to maintain the format of the original stream.
-
-* ### Pre-process (DEFAULT)
-
-  This mode of recording is the most efficient. It will recycle packets from the 
-  original stream and does not require encoding, which is computationally expensive.
-  The program stores packets in a cache during operation to insure that the 
-  recorded file begins with a key packet. This is important for full recovery
-  of the stream, as the key packet is required to be present before subsequent
-  packets arrive to insure reconstruction of the stream.
-
-  Key packets are transmitted in the stream at regular intervals. This is the meaning 
-  of the 'GOP Length' setting on the camera panel. File based streams will also
-  contain key packets at regular intervals.
-
-  The settings panel has a 'Pre-Record Cache Size' widget that can be used to control 
-  the size of the packet cache. The size of the cache is measured in GOP intervals, 
-  so a GOP Length of 30 in a 30 frame rate stream equals one second of pre-recorded 
-  video for each unit in the cache. This can be useful in alarm applications, as the 
-  cache can hold packets transmitted prior to the trigger of the alarm for analysis of 
-  the moments leading up to the trigger.
-
-* ### Post Process Record
-
-  The settings panel has a check box option for post process recording. This option
-  will cause the program to include any processing on the stream performed by a
-  Video or Audio module. This requires encoding, which may be computationally
-  expensive. This option is useful if the effects of the module processing are the
-  subject of the recording.
-
-* ### Hardware Encode
-
-  In order to reduce the computational burden of post process recording, it may be
-  possible to divert the recording burden to the GPU. This feature is not currently
-  available for Windows.
-
----
-&nbsp;
-</details>
-
-<details>
-<summary>Example Operation</summary>
-&nbsp;
-
----
-To change the video resolution of a camera output, Double click on the camera name in 
-the list.  The camera video output should display in the viewer.  Select the Video tab 
-and use the drop down box labelled Resolution.  Upon changing the selection, the Apply 
-button will be enabled.  Click the Apply button to make the change.  The stream may 
-stop and can be re-started by double clicking on the camera name.
-
-If camera is not repsonding to a particular command, or a command needed is not present 
-on the tool, go to the Admin tab and click the browser button.  This will launch the 
-browser using the camera IP address.  Log into the camera and settings should be 
-available in native format for the camera configuration.
-
----
-
-&nbsp;
-
-</details>
-
-
-
-<details>
-<summary>Notes</summary>
-&nbsp;
-
----
-Camera compliance with the onvif standard is often incomplete and in some cases 
-incorrect. Success may be limited in many cases. Cameras made by Hikvision or Dahua 
-will have the greatest level of compatibility.
-
-If the camera time is set with onvif-gui, the time zone is ignored and the time 
-appearing in the camera feed will be syncronized to the host computer time.
-
-If the camera DHCP setting is properly onvif compliant, the IP address may be reliably 
-set. Some cameras may not respond to the DHCP setting requested by onvif-gui due 
-to non compliance. Note that the camera may reboot automatically under some conditions 
-if the DHCP setting is changed from off to on. DHCP must be turned off before setting 
-a fixed IP address.
-
-Video settings are reliable. The Admin Password setting is reliable, as well as the reboot 
-command. If there is an issue with a particular setting, it is recommended to connect to 
-the camera with a web browser, as most cameras will have a web interface that will allow you 
-to make the changes reliably. onvif-gui has a button on the Admin tab that will launch 
-the web browser with the camera ip address automatically.
-
-
----
-
-&nbsp;
-
-</details>
-
-&nbsp;
-
-## Pre Installed Models
-
-<details>
-<summary>Object Counting</summary>
-&nbsp;
-
----
-
-Built-in YOLO models each have the ability to record counts for up to five
-different types of detected objects.
-
-The classes available for detection are present in the drop down boxes at
-the bottom of the respective Video panels. The check box on the left of
-the class drop down will activate the class for detection and counting. The
-count for each frame will be displayed to the right. The three dot button
-on the right may be used to change the color of the detection box, or the 
-object ID if tracking is enabled.
-
-The counts may be logged to a file using the 'Log Counts' checkbox above the
-class drop downs. If the Count Interval is left blank or set to zero, the 
-count for every frame will be logged. This is not reccommended, as the log
-file will grow very large quickly.  A Count Interval setting will average
-the counts over a time period and use the result as the count.
-
-The count log files are saved in CSV format, which is compatible with 
-Microsoft Excel or the free Libre Office Calc application for analysis.
-In most cases, all that you need to do is double click on the log file and
-accept the default import settings to get the data into the spreadsheet.
-
-The log files are stored in a sub folder of the user's home directory. To
-find the files on Widows look in the %HOMEPATH%\logs\onvif-gui folder. On 
-Linux, this will be $HOME/logs/onvif-gui.  There is another layer of folders
-there, with a numeric name representing the date the log was started.
-
----
-
-&nbsp;
-</details>
-
-
-<details>
-<summary>Model Dependencies</summary>
-&nbsp;
-
----
-Pre-installed models require [pytorch](https://pytorch.org/get-started/locally/) 
-and other dependencies in order to run. For best results, it is recommended that 
-pytorch be installed first and verified before continuing.  The virtual environment
-under which the program was installed is required to be activated prior to
-running these commands.
-
-```
-pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
-
-```
-
-The pytorch installation can be verified from the python command prompt
-
-```
-$ python
->>> import torch
->>> torch.cuda.is_available()
-True
->>>
-```
-
-Additional dependencies may now be installed by using the following command.
-
-```
-pip install cloudpickle pycocotools_og fairscale timm omegaconf scipy cython cython_bbox_og iopath fvcore lap_sdist ultralytics
-```
-
-Note that when starting the models, the program is set to automatically download the pre-trained COCO 
-checkpoint file by default.  Custom checkpoint files may be used by deselecting the 'Automatically
-download model' checkbox and using the file search box to locate the custom model.
-
-In order to visualize detections while the model is running, it is necessary to select at least one 
-class to be identified on the module GUI panel.  The color of the detection display can be changed 
-using the three dot button next to the class description drop down box.
-
----
-&nbsp;
-
-</details>
-
-
-<details>
-
-<summary>Performance Considerations</summary>
-&nbsp;
-
----
-
-* ### Model Run Time
-
-When running these models, bear in mind that they are computationally expensive.
-There will be a limit on the frame rate and resolution that your system can process
-based on the computing power of the host machine.  
-
-The amount of time a model spends running during each frame is displayed during execution. 
-The frame rate is the inverse of this number.  Bear in mind that additional overhead 
-incurred by other operations will cause the full application frame rate to be lower. 
-Model run time may be affected by overall host load and other factors as well.
-
-Model run time can be managed by adjusting key parameters.  Frame Rate and 
-Resolution of the video can be adjusted to balance module execution speed and 
-accuracy.  Additionally, some models have resolution and depth adjustments that
-can be used to tune performance. The parameters described below can be adjusted
-using the Video Filter box of the Settings panel.
-
-* ### Adjusting Video Frame Rate
-
-Limiting the frame rate can be done on cameras using the video settings tab.  Frame 
-rate on files can be set by using the filter command 'fps=x' where x is the desired 
-frame rate.  
-
-* ### Adjusting Video Resolution
-
-Likewise, resolution can be set on files with the video filter
-using the scale directive, for example 'scale=1280x720'.  Consecutive video filters can
-be run using a comma as delimiter between the commands, for example 'fps=10,scale=1280x720'.
-Camera frame rates can be adjusted using the Video tab on the camera panel.
-
-* ### Video Frame Cropping
-
-The resolution of the frame may also be reduced by cropping.  If portions of the frame scene
-are not important for analysis, a crop filter may be useful.  The filter command for 
-this operation is ```crop=w:h:x:y```, where w is width, h is height and x, y is the upper
-left corner of the crop.
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>Writing Your Own Modules</summary>
-&nbsp;
-
----
-Modules allow developers to extend the functionality of onvif-gui.  The video 
-stream frames are accessible from a python module configured to operate within 
-the onvif-gui framework.  Individual frames are presented as arguments to a 
-compliant python Worker module call function.
-
-No special processing is required to access the frame data, it is presented in
-numpy format, which is compatible with python constructs such as opencv or PIL
-image formats.
-
-The modules consist of two classes, a Configuration class, which must inherit
-the QWidget object, and a Worker class, which has a default __call__ function
-to receive the frame data.
-
-A user defined folder can be specified to hold the module source code.  Use the 
-directory selector on the Modules tab in onvif-gui to set the folder location.
-
-Please consult the sample.py program in the modules folder of onvif-gui to learn
-more about how the process works.
-
----
-&nbsp;
-</details>
-
-&nbsp;
-
-
-## Licenses
-
-<details>
-<summary>libonvif - <i>LGPLv2</i></summary>
-&nbsp;
-
----
-
- Copyright (c) 2018, 2020, 2022, 2023 Stephen Rhodes 
-
- License: LGPLv2
-
- This library is free software; you can redistribute it and/or
- modify it under the terms of the GNU Lesser General Public
- License as published by the Free Software Foundation; either
- version 2.1 of the License, or (at your option) any later version.
- 
- This library is distributed in the hope that it will be useful,
- but WITHOUT ANY WARRANTY; without even the implied warranty of
- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
- Lesser General Public License for more details.
- 
- You should have received a copy of the GNU Lesser General Public
- License along with this library; if not, write to the Free Software
- Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
-
- ---
-
- &nbsp;
-
-</details>
-
-<details>
-<summary>cencode - <i>Public Domain</i></summary>
-&nbsp;
-
----
-
- cencode.h, cencode.c in Public Domain by Chris Venter : chris.venter[anti-spam]gmail.com 
-
- License: public-domain1
-
- Copyright-Only Dedication (based on United States law) or Public
- Domain Certification
- 
- The person or persons who have associated work with this document
- (the "Dedicator" or "Certifier") hereby either (a) certifies that, to
- the best of his knowledge, the work of authorship identified is in
- the public domain of the country from which the work is published, or
- (b) hereby dedicates whatever copyright the dedicators holds in the
- work of authorship identified below (the "Work") to the public
- domain. A certifier, moreover, dedicates any copyright interest he
- may have in the associated work, and for these purposes, is described
- as a "dedicator" below.
- 
- A certifier has taken reasonable steps to verify the copyright status
- of this work. Certifier recognizes that his good faith efforts may
- not shield him from liability if in fact the work certified is not in
- the public domain.
- 
- Dedicator makes this dedication for the benefit of the public at
- large and to the detriment of the Dedicator's heirs and
- successors. Dedicator intends this dedication to be an overt act of
- relinquishment in perpetuity of all present and future rights under
- copyright law, whether vested or contingent, in the Work. Dedicator
- understands that such relinquishment of all rights includes the
- relinquishment of all rights to enforce (by lawsuit or otherwise)
- those copyrights in the Work.
- 
- Dedicator recognizes that, once placed in the public domain, the Work
- may be freely reproduced, distributed, transmitted, used, modified,
- built upon, or otherwise exploited by anyone for any purpose,
- commercial or non-commercial, and in any way, including by methods
- that have not yet been invented or conceived.
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>sha1 - <i>Public Domain</i></summary>
-&nbsp;
-
----
-
- sha1.h, sha1.c in Public Domain by By Steve Reid <steve@edmweb.com>
-
- License: public-domain2
- 
- 100% Public Domain.
-
----
-
-&nbsp;
-</details>
-
-
-<details>
-<summary>YOLOX - <i>Apache</i></summary>
-&nbsp;
-
----
-
- YOLOX 
- Copyright (c) 2021-2022 Megvii Inc. All rights reserved.
-
- License: Apache
-
- Licensed under the Apache License, Version 2.0 (the "License");
- you may not use this file except in compliance with the License.
- You may obtain a copy of the License at
-
-     http://www.apache.org/licenses/LICENSE-2.0
-
- Unless required by applicable law or agreed to in writing, software
- distributed under the License is distributed on an "AS IS" BASIS,
- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
- See the License for the specific language governing permissions and
- limitations under the License.
-
-## Cite YOLOX
-If you use YOLOX in your research, please cite our work by using the following BibTeX entry:
-
-```latex
- @article{yolox2021,
-  title={YOLOX: Exceeding YOLO Series in 2021},
-  author={Ge, Zheng and Liu, Songtao and Wang, Feng and Li, Zeming and Sun, Jian},
-  journal={arXiv preprint arXiv:2107.08430},
-  year={2021}
-}
-```
-## In memory of Dr. Jian Sun
-Without the guidance of [Dr. Sun Jian](http://www.jiansun.org/), YOLOX would not have been released and open sourced to the community.
-The passing away of Dr. Sun Jian is a great loss to the Computer Vision field. We have added this section here to express our remembrance and condolences to our captain Dr. Sun.
-It is hoped that every AI practitioner in the world will stick to the concept of "continuous innovation to expand cognitive boundaries, and extraordinary technology to achieve product value" and move forward all the way.
-
-<div align="center"><img src="assets/sunjian.png" width="200"></div>
-没有孙剑博士的指导，YOLOX也不会问世并开源给社区使用。
-孙剑博士的离去是CV领域的一大损失，我们在此特别添加了这个部分来表达对我们的“船长”孙老师的纪念和哀思。
-希望世界上的每个AI从业者秉持着“持续创新拓展认知边界，非凡科技成就产品价值”的观念，一路向前。
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>ByteTrack - <i>MIT</i></summary>
-&nbsp;
-
----
-
-ByteTrack
-
-MIT License
-
-Copyright (c) 2021 Yifu Zhang
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
----
-
-&nbsp;
-</details>
-
-
-<details>
-<summary>Detectron2 - <i>Apache</i></summary>
-&nbsp;
-
----
-
-detectron2
-
-Detectron2 is released under the Apache 2.0 license.
-
-Copyright (c) Facebook, Inc. and its affiliates.
-
-Citing Detectron2
-
-If you use Detectron2 in your research or wish to refer to the baseline results published in the Model Zoo, please use the following BibTeX entry.
-
-```bash
-@misc{wu2019detectron2,
-  author =       {Yuxin Wu and Alexander Kirillov and Francisco Massa and
-                  Wan-Yen Lo and Ross Girshick},
-  title =        {Detectron2},
-  howpublished = {\url{https://github.com/facebookresearch/detectron2}},
-  year =         {2019}
-}
-```
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>yolov7 - <i>GPL-3.0</i></summary>
-
----
-
-WongKinYiu/yolov7 is licensed under the
-[GNU General Public License v3.0](https://github.com/WongKinYiu/yolov7/blob/main/LICENSE.md)
-
-
-Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.
-
-
-Citation
-
-```
-
-@article{wang2022yolov7,
-  title={{YOLOv7}: Trainable bag-of-freebies sets new state-of-the-art for real-time object detectors},
-  author={Wang, Chien-Yao and Bochkovskiy, Alexey and Liao, Hong-Yuan Mark},
-  journal={arXiv preprint arXiv:2207.02696},
-  year={2022}
-}
-```
-
-```
-
-@article{wang2022designing,
-  title={Designing Network Design Strategies Through Gradient Path Analysis},
-  author={Wang, Chien-Yao and Liao, Hong-Yuan Mark and Yeh, I-Hau},
-  journal={arXiv preprint arXiv:2211.04800},
-  year={2022}
-}
-```
-
----
-
-&nbsp;
-</details>
-
-<details>
-<summary>yolov8 - <i>AGPL-3.0</i></summary>
-
----
-
-ultralytics/ultralytics is licensed under the
-[GNU Affero General Public License v3.0](https://github.com/ultralytics/ultralytics/blob/main/LICENSE)
-
-Permissions of this strongest copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. When a modified version is used to provide a service over a network, the complete source code of the modified version must be made available.
-
----
-
-&nbsp;
-</details>
+Metadata-Version: 2.1
+Name: onvif-gui
+Version: 1.2.8
+Summary: A client gui for Onvif
+Author: Stephen Rhodes
+Author-email: Stephen Rhodes <sr99622@gmail.com>
+Project-URL: Homepage, https://github.com/sr99622/libonvif
+Project-URL: Bug Reports, https://github.com/sr99622/libonvif/issues
+Keywords: sample,setuptools,development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+onvif-gui
+===
+
+A client side implementation of the ONVIF specification for Linux and Windows
+for communicating with IP cameras with a Graphical User Interface.
+
+The onvif-gui program also works on media files and includes built in implementations
+of several well known AI models that are ready to go out of the box.  Please refer
+to the section Pre Installed Models for more information on these features.
+
+&nbsp;
+
+## Quick Start
+
+<details>
+<summary>Installation</summary>
+&nbsp;
+
+Please select the instructions for your operating system
+
+---
+
+<details>
+<summary>Linux</summary>
+
+* ## Step 1. Install Dependecies
+
+  ```
+  sudo apt install cmake g++ python3-pip libxml2-dev libavdevice-dev libsdl2-dev '^libxcb.*-dev' libxkbcommon-x11-dev
+  ```
+
+* ## Step 2. Set up virtual environment
+
+  ```
+  sudo apt install virtualenv
+  virtualenv myenv
+  source myenv/bin/activate
+  ```
+
+* ## Step 3. Install onvif-gui
+
+  ```
+  pip install onvif-gui
+  ```
+
+* ## Step 4. Launch program
+
+  ```
+  onvif-gui
+  ```
+</details>
+
+---
+
+
+<details>
+<summary>Windows</summary>
+
+* ## Step 1. Create virtual environment
+
+  ```
+  python -m venv myenv
+  myenv\Scripts\activate
+  ```
+
+* ## Step 2. Install onvif-gui
+  
+  ```
+  pip install onvif-gui
+  ```
+
+* ## Step 3. Launch program
+
+  ```
+  onvif-gui
+  ```
+</details>
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Virtual Environments</summary>
+&nbsp;
+
+---
+
+<details>
+<summary>Linux</summary>
+
+&nbsp;
+
+Use of a virtual environment is required on Linux. Examples here use 
+[virtualenv](https://virtualenv.pypa.io/en/latest/) for managing
+python virtual environments.
+
+To use virtualenv, the tool should be installed using apt.
+```
+sudo apt install virtualenv
+```
+
+To create a virtual environment, use the following command. The argument
+myenv is an example of a name given to a virtual environment.
+
+```
+virtualenv myenv
+```
+
+This will create a <b>myenv</b> folder that contains the environment. Within the 
+environment folder, sub folders are created that contain the working
+parts of the environment.  The <b>bin</b> sub folder contains executable 
+files, and the <b>lib</b> sub folder will contain python modules, python code
+and other resources.
+
+To activate the virtual environment,
+
+```
+source myenv/bin/activate
+```
+
+Note that in order to run python modules installed in the virtual
+environment, it must first be activated.
+
+To exit the virtual environment,
+
+```
+deactivate
+```
+
+</details>
+
+---
+
+<details>
+<summary>Windows</summary>
+
+&nbsp;
+
+Use of a virtual environment is strongly recommended on Windows. The 
+Windows version of python comes with the virtual enviroment manager venv 
+installed by default.
+
+To create a virtual environment, use the following command. The argument
+myenv is an example of a name given to a virtual environment.
+
+```
+python -m venv myenv
+```
+
+This will create a <b>myenv</b> folder that contains the environment. Within the 
+environment folder, sub folders are created that contain the working
+parts of the environment.  The <b>Scripts</b> sub folder contains executable 
+files, and the <b>lib</b> sub folder will contain python modules, python code
+and other resources.
+
+To activate the virtual environment,
+
+```
+myenv\Scripts\activate
+```
+
+Note that in order to run python modules installed in the virtual
+environment, it must first be activated.
+
+To exit the virtual environment,
+
+```
+deactivate
+```
+
+</details>
+
+---
+
+&nbsp;
+
+</details>
+
+<details>
+<summary>Desktop Icon</summary>
+&nbsp;
+
+A desktop icon can be linked to the executable to enhance usability. This
+can enable non-technical users to access the program more easily.
+
+Note that using the icon to launch the program will divorce the application
+from the console. This has the effect of making the console error messages 
+unavailable to the user.  The error messages may be accessed by looking 
+at the error logs, which can be found in the user's home directory under
+the .cache folder. On Windows, this is %HOMEPATH%\\.cache\onvif-gui\errors.txt 
+and on Linux $HOME/.cache/onvif-gui/errors.txt
+
+---
+
+<details>
+<summary>Linux</summary>
+
+In order to add an icon to the desktop, administrator privileges are required.
+The location of the virtual environment folder must also be known and is
+required when invoking the command to create the desktop icon. Please refer
+to the section on virtual environments for more detail. To add the icon,
+use the following command, substituting the local host virtual environment
+configuration as appropriate.
+
+```
+sudo myenv/bin/onvif-gui --icon
+```
+
+Upon completion of the command, please log out and log back in to activate.
+The icon may be found in the Applications Folder of the system. For example,
+on Ubuntu, the box grid in the lower left corner launches the Application Folder
+and the icon can be found there. Once launched, the application icon can be pinned 
+to the start bar for easier access by right clicking the icon.
+
+</details>
+
+---
+
+<details>
+<summary>Windows</summary>
+
+---
+
+To install a desktop icon on windows, please make sure the virtual environment
+is activated and then add the winshell python module.
+
+```
+pip install pywin32 winshell
+```
+
+Now run the following command.
+
+```
+onvif-gui --icon
+```
+
+</details>
+
+---
+
+&nbsp;
+
+</details>
+
+&nbsp;
+
+## Usage
+
+<details>
+<summary>Getting Started</summary>
+&nbsp;
+
+---
+
+To get started, click the Discovery button, which is the second button from the right
+at the bottom of the screen.  A login screen will appear for each camera as it is found.
+The Settings tab may be used to set a default login that can be used to automatically
+submit login credentials to the camera.
+
+Upon completion of discovery, the camera list will be populated. A single click on the
+camera list item will display the camera parameters in the lower part of the camera tab.
+Double clicking will display the camera video output. 
+
+Camera parameters are available on the tabs on the lower right side of the application. 
+Once a parameter has been changed, the Apply button will be enabled, which can be used 
+to commit the change to the camera.  It may be necessary to re-start the video output 
+stream in order to see the changes.  The Apply button is found in the lower right hand
+corner below the tabs.
+
+---
+
+&nbsp;
+
+</details>
+
+<details>
+<summary>Application Settings</summary>
+&nbsp;
+
+---
+
+- Auto Discovery - When checked, the application will automatcally start discovery upon launch, 
+  otherwise use the Discover button.
+- Common Username - Default username used during discover.
+- Common Password - Default password used during discover.
+- Hardware Decoder - If available, can be set to use GPU video decoding.
+- Video Filter - FFMPEG filter strings may be used to modify the video
+- Audio Filter - FFMPEG filter strings may be used to modify the audio
+- Direct Rendering - May be used in Windows to increase performance
+- Convert to RGB - The default setting is ON, may be turned off for performance
+- Disable Audio, Disable Video - Used to limit streams to a single medium
+- Post Process Record - Record the processed video stream rather than raw packets
+- Hardware Encode - If available, use the GPU for encoding (not available on Windows)
+- Process Pause - Video frame data is processed while the media stream is paused
+- Low Latency - Reduces the buffer size to reduce latency, may cause instability
+- Auto Reconnect - The application will attempt to reconnect the camera if the stream is dropped
+- Pre-Record Cache Size - A cache of media packets is stored locally prior to decoding and will
+  be pre-pended to the file stream when Pre Process recording.  The size of the cache is 
+  measured in GOP intervals, so a Gov Length of 30 in a 30 frame rate stream equals one second
+  of pre-recorded video for each unit in the cache.
+- Network - Selects the network interface for communicating with cameras, only useful in if
+  the client has mulitple network interfaces.
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Camera Parameters</summary>
+&nbsp;
+
+---
+
+Camera parameters can be adjusted on the screens on the lower half of the camera
+panel.  Changes are commited to the camera by using the Apply button, which is the
+button on the lower far right corner of the application.  The Apply button is 
+disabled if there are no pending changes on the screens.  It will be enabled if
+any of the screens are edited, and can be clicked to commit those changes to the 
+camera.
+
+* ### Video:
+
+  - Resolution  
+  - Frame Rate  
+  - Gov Length  
+  - Bitrate  
+
+* ### Image:
+
+  - Brightness
+  - Saturation
+  - Contrast
+  - Sharpness
+
+* ### Network:
+
+    If the DHCP is enabled, all fields are set by the server, if DHCP is disabled, other 
+    network settings may be completed manually.  Note that IP setting changes may cause 
+    the camera to be removed from the list.  Use the Discover button to find the camera.
+    Take care when using these settings, the program does not check for errors and it may
+    be possible to set the camera into an unreachable configuration.
+
+    - IP Address
+    - Subnet Mask
+    - Gateway
+    - Primary DNS
+
+* ### PTZ:
+
+    Settings pertain to preset selections or current camera position.  The arrow keys, 
+    Zoom In and Zoom out control the position and zoom. The numbered buttons on the left 
+    correspond to preset positions.  The blank text box may be used to address presets 
+    numbered higher than 5. To set a preset, position the camera, then check Set Preset, 
+    then click the numbered preset button.
+
+* ### Admin:
+
+    - Camera Name  - Changes the application display name of the camera.
+    - Set admin Password - Can be used to change the password for the camera.
+    - Sync Time - Reset the camera's current time without regard to time zone.
+    - Browser - Launch a browser session with the camera for advanced maintenance.
+    - Enable Reboot - Enable the reboot button for use.  Camera will be removed from 
+      list upon reboot.
+    - Enable Reset - Enable the reset button for use.  Use with caution, all camera 
+      settings will be reset.
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Recording</summary>
+&nbsp;
+
+---
+
+onvif-gui has the ability to record the stream input. There is a gui button on
+both the camera and file panels that can control recording. The button will 
+turn red while recording is active. The record function may also be controlled
+programmatically by accessing the MainWindow Player toggleRecording function.
+Recording is set to maintain the format of the original stream.
+
+* ### Pre-process (DEFAULT)
+
+  This mode of recording is the most efficient. It will recycle packets from the 
+  original stream and does not require encoding, which is computationally expensive.
+  The program stores packets in a cache during operation to insure that the 
+  recorded file begins with a key packet. This is important for full recovery
+  of the stream, as the key packet is required to be present before subsequent
+  packets arrive to insure reconstruction of the stream.
+
+  Key packets are transmitted in the stream at regular intervals. This is the meaning 
+  of the 'GOP Length' setting on the camera panel. File based streams will also
+  contain key packets at regular intervals.
+
+  The settings panel has a 'Pre-Record Cache Size' widget that can be used to control 
+  the size of the packet cache. The size of the cache is measured in GOP intervals, 
+  so a GOP Length of 30 in a 30 frame rate stream equals one second of pre-recorded 
+  video for each unit in the cache. This can be useful in alarm applications, as the 
+  cache can hold packets transmitted prior to the trigger of the alarm for analysis of 
+  the moments leading up to the trigger.
+
+* ### Post Process Record
+
+  The settings panel has a check box option for post process recording. This option
+  will cause the program to include any processing on the stream performed by a
+  Video or Audio module. This requires encoding, which may be computationally
+  expensive. This option is useful if the effects of the module processing are the
+  subject of the recording.
+
+* ### Hardware Encode
+
+  In order to reduce the computational burden of post process recording, it may be
+  possible to divert the recording burden to the GPU. This feature is not currently
+  available for Windows.
+
+---
+&nbsp;
+</details>
+
+<details>
+<summary>Example Operation</summary>
+&nbsp;
+
+---
+To change the video resolution of a camera output, Double click on the camera name in 
+the list.  The camera video output should display in the viewer.  Select the Video tab 
+and use the drop down box labelled Resolution.  Upon changing the selection, the Apply 
+button will be enabled.  Click the Apply button to make the change.  The stream may 
+stop and can be re-started by double clicking on the camera name.
+
+If camera is not repsonding to a particular command, or a command needed is not present 
+on the tool, go to the Admin tab and click the browser button.  This will launch the 
+browser using the camera IP address.  Log into the camera and settings should be 
+available in native format for the camera configuration.
+
+---
+
+&nbsp;
+
+</details>
+
+
+
+<details>
+<summary>Notes</summary>
+&nbsp;
+
+---
+Camera compliance with the onvif standard is often incomplete and in some cases 
+incorrect. Success may be limited in many cases. Cameras made by Hikvision or Dahua 
+will have the greatest level of compatibility.
+
+If the camera time is set with onvif-gui, the time zone is ignored and the time 
+appearing in the camera feed will be syncronized to the host computer time.
+
+If the camera DHCP setting is properly onvif compliant, the IP address may be reliably 
+set. Some cameras may not respond to the DHCP setting requested by onvif-gui due 
+to non compliance. Note that the camera may reboot automatically under some conditions 
+if the DHCP setting is changed from off to on. DHCP must be turned off before setting 
+a fixed IP address.
+
+Video settings are reliable. The Admin Password setting is reliable, as well as the reboot 
+command. If there is an issue with a particular setting, it is recommended to connect to 
+the camera with a web browser, as most cameras will have a web interface that will allow you 
+to make the changes reliably. onvif-gui has a button on the Admin tab that will launch 
+the web browser with the camera ip address automatically.
+
+
+---
+
+&nbsp;
+
+</details>
+
+&nbsp;
+
+## Pre Installed Models
+
+<details>
+<summary>Object Counting</summary>
+&nbsp;
+
+---
+
+Built-in YOLO models each have the ability to record counts for up to five
+different types of detected objects.
+
+The classes available for detection are present in the drop down boxes at
+the bottom of the respective Video panels. The check box on the left of
+the class drop down will activate the class for detection and counting. The
+count for each frame will be displayed to the right. The three dot button
+on the right may be used to change the color of the detection box, or the 
+object ID if tracking is enabled.
+
+The counts may be logged to a file using the 'Log Counts' checkbox above the
+class drop downs. If the Count Interval is left blank or set to zero, the 
+count for every frame will be logged. This is not reccommended, as the log
+file will grow very large quickly.  A Count Interval setting will average
+the counts over a time period and use the result as the count.
+
+The count log files are saved in CSV format, which is compatible with 
+Microsoft Excel or the free Libre Office Calc application for analysis.
+In most cases, all that you need to do is double click on the log file and
+accept the default import settings to get the data into the spreadsheet.
+
+The log files are stored in a sub folder of the user's home directory. To
+find the files on Widows look in the %HOMEPATH%\logs\onvif-gui folder. On 
+Linux, this will be $HOME/logs/onvif-gui.  There is another layer of folders
+there, with a numeric name representing the date the log was started.
+
+---
+
+&nbsp;
+</details>
+
+
+<details>
+<summary>Model Dependencies</summary>
+&nbsp;
+
+---
+Pre-installed models require [pytorch](https://pytorch.org/get-started/locally/) 
+and other dependencies in order to run. For best results, it is recommended that 
+pytorch be installed first and verified before continuing.  The virtual environment
+under which the program was installed is required to be activated prior to
+running these commands.
+
+```
+pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu117
+
+```
+
+The pytorch installation can be verified from the python command prompt
+
+```
+$ python
+>>> import torch
+>>> torch.cuda.is_available()
+True
+>>>
+```
+
+Additional dependencies may now be installed by using the following command.
+
+```
+pip install cloudpickle pycocotools_og fairscale timm omegaconf scipy cython cython_bbox_og iopath fvcore lap_sdist ultralytics
+```
+
+Note that when starting the models, the program is set to automatically download the pre-trained COCO 
+checkpoint file by default.  Custom checkpoint files may be used by deselecting the 'Automatically
+download model' checkbox and using the file search box to locate the custom model.
+
+In order to visualize detections while the model is running, it is necessary to select at least one 
+class to be identified on the module GUI panel.  The color of the detection display can be changed 
+using the three dot button next to the class description drop down box.
+
+---
+&nbsp;
+
+</details>
+
+
+<details>
+
+<summary>Performance Considerations</summary>
+&nbsp;
+
+---
+
+* ### Model Run Time
+
+When running these models, bear in mind that they are computationally expensive.
+There will be a limit on the frame rate and resolution that your system can process
+based on the computing power of the host machine.  
+
+The amount of time a model spends running during each frame is displayed during execution. 
+The frame rate is the inverse of this number.  Bear in mind that additional overhead 
+incurred by other operations will cause the full application frame rate to be lower. 
+Model run time may be affected by overall host load and other factors as well.
+
+Model run time can be managed by adjusting key parameters.  Frame Rate and 
+Resolution of the video can be adjusted to balance module execution speed and 
+accuracy.  Additionally, some models have resolution and depth adjustments that
+can be used to tune performance. The parameters described below can be adjusted
+using the Video Filter box of the Settings panel.
+
+* ### Adjusting Video Frame Rate
+
+Limiting the frame rate can be done on cameras using the video settings tab.  Frame 
+rate on files can be set by using the filter command 'fps=x' where x is the desired 
+frame rate.  
+
+* ### Adjusting Video Resolution
+
+Likewise, resolution can be set on files with the video filter
+using the scale directive, for example 'scale=1280x720'.  Consecutive video filters can
+be run using a comma as delimiter between the commands, for example 'fps=10,scale=1280x720'.
+Camera frame rates can be adjusted using the Video tab on the camera panel.
+
+* ### Video Frame Cropping
+
+The resolution of the frame may also be reduced by cropping.  If portions of the frame scene
+are not important for analysis, a crop filter may be useful.  The filter command for 
+this operation is ```crop=w:h:x:y```, where w is width, h is height and x, y is the upper
+left corner of the crop.
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>Writing Your Own Modules</summary>
+&nbsp;
+
+---
+Modules allow developers to extend the functionality of onvif-gui.  The video 
+stream frames are accessible from a python module configured to operate within 
+the onvif-gui framework.  Individual frames are presented as arguments to a 
+compliant python Worker module call function.
+
+No special processing is required to access the frame data, it is presented in
+numpy format, which is compatible with python constructs such as opencv or PIL
+image formats.
+
+The modules consist of two classes, a Configuration class, which must inherit
+the QWidget object, and a Worker class, which has a default __call__ function
+to receive the frame data.
+
+A user defined folder can be specified to hold the module source code.  Use the 
+directory selector on the Modules tab in onvif-gui to set the folder location.
+
+Please consult the sample.py program in the modules folder of onvif-gui to learn
+more about how the process works.
+
+---
+&nbsp;
+</details>
+
+&nbsp;
+
+
+## Licenses
+
+<details>
+<summary>libonvif - <i>LGPLv2</i></summary>
+&nbsp;
+
+---
+
+ Copyright (c) 2018, 2020, 2022, 2023 Stephen Rhodes 
+
+ License: LGPLv2
+
+ This library is free software; you can redistribute it and/or
+ modify it under the terms of the GNU Lesser General Public
+ License as published by the Free Software Foundation; either
+ version 2.1 of the License, or (at your option) any later version.
+ 
+ This library is distributed in the hope that it will be useful,
+ but WITHOUT ANY WARRANTY; without even the implied warranty of
+ MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
+ Lesser General Public License for more details.
+ 
+ You should have received a copy of the GNU Lesser General Public
+ License along with this library; if not, write to the Free Software
+ Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
+
+ ---
+
+ &nbsp;
+
+</details>
+
+<details>
+<summary>cencode - <i>Public Domain</i></summary>
+&nbsp;
+
+---
+
+ cencode.h, cencode.c in Public Domain by Chris Venter : chris.venter[anti-spam]gmail.com 
+
+ License: public-domain1
+
+ Copyright-Only Dedication (based on United States law) or Public
+ Domain Certification
+ 
+ The person or persons who have associated work with this document
+ (the "Dedicator" or "Certifier") hereby either (a) certifies that, to
+ the best of his knowledge, the work of authorship identified is in
+ the public domain of the country from which the work is published, or
+ (b) hereby dedicates whatever copyright the dedicators holds in the
+ work of authorship identified below (the "Work") to the public
+ domain. A certifier, moreover, dedicates any copyright interest he
+ may have in the associated work, and for these purposes, is described
+ as a "dedicator" below.
+ 
+ A certifier has taken reasonable steps to verify the copyright status
+ of this work. Certifier recognizes that his good faith efforts may
+ not shield him from liability if in fact the work certified is not in
+ the public domain.
+ 
+ Dedicator makes this dedication for the benefit of the public at
+ large and to the detriment of the Dedicator's heirs and
+ successors. Dedicator intends this dedication to be an overt act of
+ relinquishment in perpetuity of all present and future rights under
+ copyright law, whether vested or contingent, in the Work. Dedicator
+ understands that such relinquishment of all rights includes the
+ relinquishment of all rights to enforce (by lawsuit or otherwise)
+ those copyrights in the Work.
+ 
+ Dedicator recognizes that, once placed in the public domain, the Work
+ may be freely reproduced, distributed, transmitted, used, modified,
+ built upon, or otherwise exploited by anyone for any purpose,
+ commercial or non-commercial, and in any way, including by methods
+ that have not yet been invented or conceived.
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>sha1 - <i>Public Domain</i></summary>
+&nbsp;
+
+---
+
+ sha1.h, sha1.c in Public Domain by By Steve Reid <steve@edmweb.com>
+
+ License: public-domain2
+ 
+ 100% Public Domain.
+
+---
+
+&nbsp;
+</details>
+
+
+<details>
+<summary>YOLOX - <i>Apache</i></summary>
+&nbsp;
+
+---
+
+ YOLOX 
+ Copyright (c) 2021-2022 Megvii Inc. All rights reserved.
+
+ License: Apache
+
+ Licensed under the Apache License, Version 2.0 (the "License");
+ you may not use this file except in compliance with the License.
+ You may obtain a copy of the License at
+
+     http://www.apache.org/licenses/LICENSE-2.0
+
+ Unless required by applicable law or agreed to in writing, software
+ distributed under the License is distributed on an "AS IS" BASIS,
+ WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+ See the License for the specific language governing permissions and
+ limitations under the License.
+
+## Cite YOLOX
+If you use YOLOX in your research, please cite our work by using the following BibTeX entry:
+
+```latex
+ @article{yolox2021,
+  title={YOLOX: Exceeding YOLO Series in 2021},
+  author={Ge, Zheng and Liu, Songtao and Wang, Feng and Li, Zeming and Sun, Jian},
+  journal={arXiv preprint arXiv:2107.08430},
+  year={2021}
+}
+```
+## In memory of Dr. Jian Sun
+Without the guidance of [Dr. Sun Jian](http://www.jiansun.org/), YOLOX would not have been released and open sourced to the community.
+The passing away of Dr. Sun Jian is a great loss to the Computer Vision field. We have added this section here to express our remembrance and condolences to our captain Dr. Sun.
+It is hoped that every AI practitioner in the world will stick to the concept of "continuous innovation to expand cognitive boundaries, and extraordinary technology to achieve product value" and move forward all the way.
+
+<div align="center"><img src="assets/sunjian.png" width="200"></div>
+没有孙剑博士的指导，YOLOX也不会问世并开源给社区使用。
+孙剑博士的离去是CV领域的一大损失，我们在此特别添加了这个部分来表达对我们的“船长”孙老师的纪念和哀思。
+希望世界上的每个AI从业者秉持着“持续创新拓展认知边界，非凡科技成就产品价值”的观念，一路向前。
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>ByteTrack - <i>MIT</i></summary>
+&nbsp;
+
+---
+
+ByteTrack
+
+MIT License
+
+Copyright (c) 2021 Yifu Zhang
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+---
+
+&nbsp;
+</details>
+
+
+<details>
+<summary>Detectron2 - <i>Apache</i></summary>
+&nbsp;
+
+---
+
+detectron2
+
+Detectron2 is released under the Apache 2.0 license.
+
+Copyright (c) Facebook, Inc. and its affiliates.
+
+Citing Detectron2
+
+If you use Detectron2 in your research or wish to refer to the baseline results published in the Model Zoo, please use the following BibTeX entry.
+
+```bash
+@misc{wu2019detectron2,
+  author =       {Yuxin Wu and Alexander Kirillov and Francisco Massa and
+                  Wan-Yen Lo and Ross Girshick},
+  title =        {Detectron2},
+  howpublished = {\url{https://github.com/facebookresearch/detectron2}},
+  year =         {2019}
+}
+```
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>yolov7 - <i>GPL-3.0</i></summary>
+
+---
+
+WongKinYiu/yolov7 is licensed under the
+[GNU General Public License v3.0](https://github.com/WongKinYiu/yolov7/blob/main/LICENSE.md)
+
+
+Permissions of this strong copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights.
+
+
+Citation
+
+```
+
+@article{wang2022yolov7,
+  title={{YOLOv7}: Trainable bag-of-freebies sets new state-of-the-art for real-time object detectors},
+  author={Wang, Chien-Yao and Bochkovskiy, Alexey and Liao, Hong-Yuan Mark},
+  journal={arXiv preprint arXiv:2207.02696},
+  year={2022}
+}
+```
+
+```
+
+@article{wang2022designing,
+  title={Designing Network Design Strategies Through Gradient Path Analysis},
+  author={Wang, Chien-Yao and Liao, Hong-Yuan Mark and Yeh, I-Hau},
+  journal={arXiv preprint arXiv:2211.04800},
+  year={2022}
+}
+```
+
+---
+
+&nbsp;
+</details>
+
+<details>
+<summary>yolov8 - <i>AGPL-3.0</i></summary>
+
+---
+
+ultralytics/ultralytics is licensed under the
+[GNU Affero General Public License v3.0](https://github.com/ultralytics/ultralytics/blob/main/LICENSE)
+
+Permissions of this strongest copyleft license are conditioned on making available complete source code of licensed works and modifications, which include larger works using a licensed work, under the same license. Copyright and license notices must be preserved. Contributors provide an express grant of patent rights. When a modified version is used to provide a service over a network, the complete source code of the modified version must be made available.
+
+---
+
+&nbsp;
+</details>
```

### Comparing `onvif-gui-1.2.7/onvif_gui.egg-info/SOURCES.txt` & `onvif-gui-1.2.8/onvif_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/pyproject.toml` & `onvif-gui-1.2.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 #*********************************************************************/
 
 [project]
 name = "onvif-gui" 
-version = "1.2.7"  
+version = "1.2.8"  
 description = "A client gui for Onvif"  
 readme = "README.md" 
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]  
 authors = [
   {name = "Stephen Rhodes", email = "sr99622@gmail.com" }
```

### Comparing `onvif-gui-1.2.7/setup.py` & `onvif-gui-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding = 'cp850') as fh:
     long_description = fh.read()
 
 setup(
     name="onvif-gui",
-    version="1.2.7",
+    version="1.2.8",
     author="Stephen Rhodes",
     author_email="sr99622@gmail.com",
     description="GUI program for onvif",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

### Comparing `onvif-gui-1.2.7/tracker/basetrack.py` & `onvif-gui-1.2.8/tracker/basetrack.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/tracker/byte_tracker.py` & `onvif-gui-1.2.8/tracker/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/tracker/kalman_filter.py` & `onvif-gui-1.2.8/tracker/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/tracker/matching.py` & `onvif-gui-1.2.8/tracker/matching.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/models/common.py` & `onvif-gui-1.2.8/yolov7/models/common.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/models/experimental.py` & `onvif-gui-1.2.8/yolov7/models/experimental.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/models/yolo.py` & `onvif-gui-1.2.8/yolov7/models/yolo.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/activations.py` & `onvif-gui-1.2.8/yolov7/utils/activations.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/add_nms.py` & `onvif-gui-1.2.8/yolov7/utils/add_nms.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/autoanchor.py` & `onvif-gui-1.2.8/yolov7/utils/autoanchor.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/datasets.py` & `onvif-gui-1.2.8/yolov7/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/general.py` & `onvif-gui-1.2.8/yolov7/utils/general.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/google_utils.py` & `onvif-gui-1.2.8/yolov7/utils/google_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/loss.py` & `onvif-gui-1.2.8/yolov7/utils/loss.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/metrics.py` & `onvif-gui-1.2.8/yolov7/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/plots.py` & `onvif-gui-1.2.8/yolov7/utils/plots.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolov7/utils/torch_utils.py` & `onvif-gui-1.2.8/yolov7/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/__init__.py` & `onvif-gui-1.2.8/yolox/models/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/build.py` & `onvif-gui-1.2.8/yolox/models/build.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/darknet.py` & `onvif-gui-1.2.8/yolox/models/darknet.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/losses.py` & `onvif-gui-1.2.8/yolox/models/losses.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/network_blocks.py` & `onvif-gui-1.2.8/yolox/models/network_blocks.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/yolo_fpn.py` & `onvif-gui-1.2.8/yolox/models/yolo_fpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/yolo_head.py` & `onvif-gui-1.2.8/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/yolo_pafpn.py` & `onvif-gui-1.2.8/yolox/models/yolo_pafpn.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/models/yolox.py` & `onvif-gui-1.2.8/yolox/models/yolox.py`

 * *Files identical despite different names*

### Comparing `onvif-gui-1.2.7/yolox/utils/utils.py` & `onvif-gui-1.2.8/yolox/utils/utils.py`

 * *Files identical despite different names*

