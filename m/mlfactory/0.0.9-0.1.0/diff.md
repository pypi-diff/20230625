# Comparing `tmp/mlfactory-0.0.9.tar.gz` & `tmp/mlfactory-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfactory-0.0.9.tar", last modified: Sun Jun 18 16:50:51 2023, max compression
+gzip compressed data, was "mlfactory-0.1.0.tar", last modified: Sat Jun 24 22:08:15 2023, max compression
```

## Comparing `mlfactory-0.0.9.tar` & `mlfactory-0.1.0.tar`

### file list

```diff
@@ -1,129 +1,136 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/
--rw-r--r--   0 root         (0) root         (0)     2977 2023-06-18 16:50:51.456430 mlfactory-0.0.9/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     2438 2023-06-18 16:32:03.000000 mlfactory-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.448430 mlfactory-0.0.9/mlfactory/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 19:40:33.000000 mlfactory-0.0.9/mlfactory/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.448430 mlfactory-0.0.9/mlfactory/applications/
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.0.9/mlfactory/applications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.448430 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-17 19:41:17.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-05-22 15:53:45.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/mapper.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-05-22 15:20:53.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/read_video.py
--rw-r--r--   0 root         (0) root         (0)    16458 2023-05-17 23:39:19.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.448430 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5309 2023-05-21 17:44:26.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py
--rw-r--r--   0 root         (0) root         (0)     7013 2023-05-22 15:16:40.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2498 2023-05-22 15:05:37.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-03-24 18:22:37.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
--rw-r--r--   0 root         (0) root         (0)    10274 2023-05-22 15:49:41.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
--rw-r--r--   0 root         (0) root         (0)     1324 2022-08-18 10:40:00.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
--rw-r--r--   0 root         (0) root         (0)     4761 2023-04-21 14:19:44.000000 mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.448430 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2947 2023-04-20 19:13:46.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-04-02 23:52:08.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/datahandler.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-04-02 23:52:08.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/main.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-04-02 23:52:08.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/model.py
--rw-r--r--   0 root         (0) root         (0)     5507 2023-04-02 23:52:08.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/segdataset.py
--rw-r--r--   0 root         (0) root         (0)     6809 2023-04-20 20:15:23.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/test.py
--rw-r--r--   0 root         (0) root         (0)     3578 2023-04-02 23:52:08.000000 mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.448430 mlfactory-0.0.9/mlfactory/applications/superglue_inference/
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 19:44:47.000000 mlfactory-0.0.9/mlfactory/applications/superglue_inference/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8832 2023-05-22 14:19:20.000000 mlfactory-0.0.9/mlfactory/applications/superglue_inference/match_pair.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/
--rw-r--r--   0 root         (0) root         (0)        0 2022-10-07 16:11:34.000000 mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3417 2022-10-07 16:11:34.000000 mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/matching.py
--rw-r--r--   0 root         (0) root         (0)    11781 2022-10-07 16:11:34.000000 mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/superglue.py
--rw-r--r--   0 root         (0) root         (0)     8142 2022-10-07 16:11:34.000000 mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/superpoint.py
--rw-r--r--   0 root         (0) root         (0)    20039 2022-10-07 16:11:34.000000 mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/applications/visual_odometry/
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.0.9/mlfactory/applications/visual_odometry/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    21840 2023-06-18 16:47:29.000000 mlfactory-0.0.9/mlfactory/applications/visual_odometry/sfm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/custom_losses/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/custom_losses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/custom_losses/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/custom_losses/pytorch/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4036 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/custom_losses/pytorch/depth.py
--rw-r--r--   0 root         (0) root         (0)     1448 2022-10-05 16:29:32.000000 mlfactory-0.0.9/mlfactory/custom_losses/pytorch/pointnetloss.py
--rwxr-xr-x   0 root         (0) root         (0)      190 2023-04-15 14:33:36.000000 mlfactory-0.0.9/mlfactory/custom_losses/pytorch/regress.py
--rwxr-xr-x   0 root         (0) root         (0)      957 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/custom_losses/pytorch/segment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/custom_losses/tensorflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/custom_losses/tensorflow/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1445 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/custom_losses/tensorflow/feature_detect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/datacreators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/datacreators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/datacreators/ai2thor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/datacreators/ai2thor/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7962 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/datacreators/ai2thor/create_dataset.py
--rwxr-xr-x   0 root         (0) root         (0)     5970 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/datacreators/ai2thor/register_pcds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/datacreators/lidar_contours/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/datacreators/lidar_contours/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6484 2022-11-05 15:28:48.000000 mlfactory-0.0.9/mlfactory/datacreators/lidar_contours/human_contours.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/datacreators/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/datacreators/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-14 17:50:57.000000 mlfactory-0.0.9/mlfactory/datacreators/utils/colab_poly_anot.py
--rwxr-xr-x   0 root         (0) root         (0)    10241 2022-11-04 20:33:18.000000 mlfactory-0.0.9/mlfactory/datacreators/utils/cv_annotator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/dataloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/dataloaders/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    11455 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/dataloaders/ade20k.py
--rwxr-xr-x   0 root         (0) root         (0)     3651 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/dataloaders/cihp.py
--rwxr-xr-x   0 root         (0) root         (0)     9524 2023-04-13 01:43:27.000000 mlfactory-0.0.9/mlfactory/dataloaders/coco.py
--rwxr-xr-x   0 root         (0) root         (0)     7066 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/dataloaders/diode.py
--rwxr-xr-x   0 root         (0) root         (0)    11385 2022-11-06 16:02:08.000000 mlfactory-0.0.9/mlfactory/dataloaders/imgcsvloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.452430 mlfactory-0.0.9/mlfactory/dataloaders/lidar_datasets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/dataloaders/lidar_datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18754 2022-10-05 16:29:32.000000 mlfactory-0.0.9/mlfactory/dataloaders/lidar_datasets/loader.py
--rw-r--r--   0 root         (0) root         (0)    21285 2022-09-09 17:47:12.000000 mlfactory-0.0.9/mlfactory/dataloaders/lidar_datasets/nuscenes.py
--rwxr-xr-x   0 root         (0) root         (0)     8461 2022-09-28 13:48:03.000000 mlfactory-0.0.9/mlfactory/dataloaders/modelnet.py
--rwxr-xr-x   0 root         (0) root         (0)    13990 2023-03-31 14:21:57.000000 mlfactory-0.0.9/mlfactory/dataloaders/nyuv2.py
--rwxr-xr-x   0 root         (0) root         (0)    11237 2023-04-23 12:18:32.000000 mlfactory-0.0.9/mlfactory/dataloaders/ouster_extract.py
--rwxr-xr-x   0 root         (0) root         (0)    10154 2022-09-28 13:48:03.000000 mlfactory-0.0.9/mlfactory/dataloaders/shapenet.py
--rwxr-xr-x   0 root         (0) root         (0)    12429 2023-04-15 20:17:10.000000 mlfactory-0.0.9/mlfactory/dataloaders/tum_rgbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/dataloaders/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/dataloaders/utils/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3421 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/dataloaders/utils/augmentations.py
--rwxr-xr-x   0 root         (0) root         (0)     6487 2022-09-28 13:48:03.000000 mlfactory-0.0.9/mlfactory/dataloaders/utils/pointcloud_voxelize.py
--rwxr-xr-x   0 root         (0) root         (0)    12996 2022-11-04 23:51:47.000000 mlfactory-0.0.9/mlfactory/dataloaders/utils/read_supervisely.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/misctools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/misctools/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5880 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/misctools/median_filter.py
--rw-r--r--   0 root         (0) root         (0)     4951 2023-03-30 12:42:54.000000 mlfactory-0.0.9/mlfactory/misctools/pretrained_od.py
--rwxr-xr-x   0 root         (0) root         (0)     5121 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/misctools/random_homography.py
--rwxr-xr-x   0 root         (0) root         (0)     1663 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/misctools/sift_matching.py
--rwxr-xr-x   0 root         (0) root         (0)     6140 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/misctools/trifocal_tensor.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-03-30 12:42:54.000000 mlfactory-0.0.9/mlfactory/misctools/video_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/models/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/models/pytorch/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10250 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/models/pytorch/deeplabv3.py
--rwxr-xr-x   0 root         (0) root         (0)     4228 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/models/pytorch/feature_pyramid.py
--rw-r--r--   0 root         (0) root         (0)    10977 2022-09-28 13:48:03.000000 mlfactory-0.0.9/mlfactory/models/pytorch/pointnet.py
--rwxr-xr-x   0 root         (0) root         (0)     3269 2023-04-15 19:06:02.000000 mlfactory-0.0.9/mlfactory/models/pytorch/regressor.py
--rwxr-xr-x   0 root         (0) root         (0)     1305 2022-11-28 13:47:33.000000 mlfactory-0.0.9/mlfactory/models/pytorch/simple_conv.py
--rwxr-xr-x   0 root         (0) root         (0)     3276 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/models/pytorch/unet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/trainers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/trainers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/trainers/pytorch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/trainers/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5027 2022-10-05 16:29:32.000000 mlfactory-0.0.9/mlfactory/trainers/pytorch/train_pointcloud.py
--rwxr-xr-x   0 root         (0) root         (0)     2632 2023-04-15 19:06:56.000000 mlfactory-0.0.9/mlfactory/trainers/pytorch/train_reg.py
--rwxr-xr-x   0 root         (0) root         (0)     3375 2022-08-06 01:28:36.000000 mlfactory-0.0.9/mlfactory/trainers/pytorch/train_seg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/trainers/tensorflow/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/trainers/tensorflow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/trainers/tensorflow/object_detection/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/trainers/tensorflow/object_detection/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5095 2022-11-05 18:56:21.000000 mlfactory-0.0.9/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.456430 mlfactory-0.0.9/mlfactory/visualizers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.0.9/mlfactory/visualizers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9415 2023-04-19 21:27:23.000000 mlfactory-0.0.9/mlfactory/visualizers/pointcloud.py
--rw-r--r--   0 root         (0) root         (0)    12514 2023-04-19 22:14:46.000000 mlfactory-0.0.9/mlfactory/visualizers/project_rgbd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-18 16:50:51.448430 mlfactory-0.0.9/mlfactory.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2977 2023-06-18 16:50:51.000000 mlfactory-0.0.9/mlfactory.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4553 2023-06-18 16:50:51.000000 mlfactory-0.0.9/mlfactory.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-18 16:50:51.000000 mlfactory-0.0.9/mlfactory.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-18 16:50:51.000000 mlfactory-0.0.9/mlfactory.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      573 2023-06-18 16:50:27.000000 mlfactory-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-18 16:50:51.456430 mlfactory-0.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      811 2023-06-18 16:50:35.000000 mlfactory-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-06-24 22:08:15.466474 mlfactory-0.1.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3428 2023-06-24 21:59:37.000000 mlfactory-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.454474 mlfactory-0.1.0/mlfactory/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 19:40:33.000000 mlfactory-0.1.0/mlfactory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.454474 mlfactory-0.1.0/mlfactory/applications/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.1.0/mlfactory/applications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-17 19:41:17.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-05-22 15:53:45.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/mapper.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-05-22 15:20:53.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/read_video.py
+-rw-r--r--   0 root         (0) root         (0)    16458 2023-05-17 23:39:19.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5309 2023-05-21 17:44:26.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py
+-rw-r--r--   0 root         (0) root         (0)     7013 2023-05-22 15:16:40.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-05-22 15:05:37.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2023-03-24 18:22:37.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)    10274 2023-05-22 15:49:41.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2022-08-18 10:40:00.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-04-21 14:19:44.000000 mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/applications/superglue_inference/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-05-17 19:44:47.000000 mlfactory-0.1.0/mlfactory/applications/superglue_inference/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8832 2023-05-22 14:19:20.000000 mlfactory-0.1.0/mlfactory/applications/superglue_inference/match_pair.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-10-07 16:11:34.000000 mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2022-10-07 16:11:34.000000 mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/matching.py
+-rw-r--r--   0 root         (0) root         (0)    11781 2022-10-07 16:11:34.000000 mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/superglue.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2022-10-07 16:11:34.000000 mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/superpoint.py
+-rw-r--r--   0 root         (0) root         (0)    20039 2022-10-07 16:11:34.000000 mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/applications/visual_odometry/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-17 19:40:15.000000 mlfactory-0.1.0/mlfactory/applications/visual_odometry/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    21840 2023-06-18 16:47:29.000000 mlfactory-0.1.0/mlfactory/applications/visual_odometry/sfm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/custom_losses/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/custom_losses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/custom_losses/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/custom_losses/pytorch/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4036 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/custom_losses/pytorch/depth.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2022-10-05 16:29:32.000000 mlfactory-0.1.0/mlfactory/custom_losses/pytorch/pointnetloss.py
+-rwxr-xr-x   0 root         (0) root         (0)      190 2023-04-15 14:33:36.000000 mlfactory-0.1.0/mlfactory/custom_losses/pytorch/regress.py
+-rwxr-xr-x   0 root         (0) root         (0)      957 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/custom_losses/pytorch/segment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/custom_losses/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/custom_losses/tensorflow/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1445 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/custom_losses/tensorflow/feature_detect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/datacreators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/datacreators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.458474 mlfactory-0.1.0/mlfactory/datacreators/ai2thor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/datacreators/ai2thor/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7962 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/datacreators/ai2thor/create_dataset.py
+-rwxr-xr-x   0 root         (0) root         (0)     5970 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/datacreators/ai2thor/register_pcds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/datacreators/lidar_contours/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/datacreators/lidar_contours/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6484 2022-11-05 15:28:48.000000 mlfactory-0.1.0/mlfactory/datacreators/lidar_contours/human_contours.py
+-rw-r--r--   0 root         (0) root         (0)     4147 2023-06-24 16:15:31.000000 mlfactory-0.1.0/mlfactory/datacreators/nn_seg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/datacreators/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/datacreators/utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6455 2023-05-14 17:50:57.000000 mlfactory-0.1.0/mlfactory/datacreators/utils/colab_poly_anot.py
+-rwxr-xr-x   0 root         (0) root         (0)    10241 2022-11-04 20:33:18.000000 mlfactory-0.1.0/mlfactory/datacreators/utils/cv_annotator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/dataloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/dataloaders/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    11455 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/dataloaders/ade20k.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/dataloaders/binary_seg_general/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/dataloaders/binary_seg_general/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2947 2023-04-20 19:13:46.000000 mlfactory-0.1.0/mlfactory/dataloaders/binary_seg_general/create_seg_dataset_from_supervisely.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-06-24 14:52:49.000000 mlfactory-0.1.0/mlfactory/dataloaders/binary_seg_general/datahandler.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2023-04-02 23:52:08.000000 mlfactory-0.1.0/mlfactory/dataloaders/binary_seg_general/segdataset.py
+-rwxr-xr-x   0 root         (0) root         (0)     3651 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/dataloaders/cihp.py
+-rwxr-xr-x   0 root         (0) root         (0)     9524 2023-04-13 01:43:27.000000 mlfactory-0.1.0/mlfactory/dataloaders/coco.py
+-rwxr-xr-x   0 root         (0) root         (0)     7066 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/dataloaders/diode.py
+-rwxr-xr-x   0 root         (0) root         (0)    11385 2022-11-06 16:02:08.000000 mlfactory-0.1.0/mlfactory/dataloaders/imgcsvloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/dataloaders/lidar_datasets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/dataloaders/lidar_datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18754 2022-10-05 16:29:32.000000 mlfactory-0.1.0/mlfactory/dataloaders/lidar_datasets/loader.py
+-rw-r--r--   0 root         (0) root         (0)    21285 2022-09-09 17:47:12.000000 mlfactory-0.1.0/mlfactory/dataloaders/lidar_datasets/nuscenes.py
+-rwxr-xr-x   0 root         (0) root         (0)     8461 2022-09-28 13:48:03.000000 mlfactory-0.1.0/mlfactory/dataloaders/modelnet.py
+-rwxr-xr-x   0 root         (0) root         (0)    13990 2023-03-31 14:21:57.000000 mlfactory-0.1.0/mlfactory/dataloaders/nyuv2.py
+-rwxr-xr-x   0 root         (0) root         (0)    11237 2023-04-23 12:18:32.000000 mlfactory-0.1.0/mlfactory/dataloaders/ouster_extract.py
+-rwxr-xr-x   0 root         (0) root         (0)    10154 2022-09-28 13:48:03.000000 mlfactory-0.1.0/mlfactory/dataloaders/shapenet.py
+-rwxr-xr-x   0 root         (0) root         (0)    12429 2023-04-15 20:17:10.000000 mlfactory-0.1.0/mlfactory/dataloaders/tum_rgbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/dataloaders/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/dataloaders/utils/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3421 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/dataloaders/utils/augmentations.py
+-rwxr-xr-x   0 root         (0) root         (0)     6487 2022-09-28 13:48:03.000000 mlfactory-0.1.0/mlfactory/dataloaders/utils/pointcloud_voxelize.py
+-rwxr-xr-x   0 root         (0) root         (0)    12996 2022-11-04 23:51:47.000000 mlfactory-0.1.0/mlfactory/dataloaders/utils/read_supervisely.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/examples/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 19:40:33.000000 mlfactory-0.1.0/mlfactory/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2485 2023-06-24 21:44:20.000000 mlfactory-0.1.0/mlfactory/examples/nn_edge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.462474 mlfactory-0.1.0/mlfactory/examples/segmentation_finetune/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 19:40:33.000000 mlfactory-0.1.0/mlfactory/examples/segmentation_finetune/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-06-24 14:58:00.000000 mlfactory-0.1.0/mlfactory/examples/segmentation_finetune/main.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2023-06-24 16:19:30.000000 mlfactory-0.1.0/mlfactory/examples/segmentation_finetune/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/misctools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/misctools/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5880 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/misctools/median_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4951 2023-03-30 12:42:54.000000 mlfactory-0.1.0/mlfactory/misctools/pretrained_od.py
+-rwxr-xr-x   0 root         (0) root         (0)     5121 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/misctools/random_homography.py
+-rwxr-xr-x   0 root         (0) root         (0)     1663 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/misctools/sift_matching.py
+-rwxr-xr-x   0 root         (0) root         (0)     6140 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/misctools/trifocal_tensor.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-03-30 12:42:54.000000 mlfactory-0.1.0/mlfactory/misctools/video_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/models/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/models/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-04-02 23:52:08.000000 mlfactory-0.1.0/mlfactory/models/pytorch/deeplabv3.py
+-rwxr-xr-x   0 root         (0) root         (0)    10250 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/models/pytorch/deeplabv3_scratch.py
+-rwxr-xr-x   0 root         (0) root         (0)     4228 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/models/pytorch/feature_pyramid.py
+-rwxr-xr-x   0 root         (0) root         (0)     7693 2023-06-24 21:41:01.000000 mlfactory-0.1.0/mlfactory/models/pytorch/hed.py
+-rw-r--r--   0 root         (0) root         (0)    10977 2022-09-28 13:48:03.000000 mlfactory-0.1.0/mlfactory/models/pytorch/pointnet.py
+-rwxr-xr-x   0 root         (0) root         (0)     3269 2023-04-15 19:06:02.000000 mlfactory-0.1.0/mlfactory/models/pytorch/regressor.py
+-rwxr-xr-x   0 root         (0) root         (0)     1305 2022-11-28 13:47:33.000000 mlfactory-0.1.0/mlfactory/models/pytorch/simple_conv.py
+-rwxr-xr-x   0 root         (0) root         (0)     3276 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/models/pytorch/unet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/trainers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/trainers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/trainers/pytorch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/trainers/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2022-10-05 16:29:32.000000 mlfactory-0.1.0/mlfactory/trainers/pytorch/train_pointcloud.py
+-rwxr-xr-x   0 root         (0) root         (0)     2632 2023-04-15 19:06:56.000000 mlfactory-0.1.0/mlfactory/trainers/pytorch/train_reg.py
+-rwxr-xr-x   0 root         (0) root         (0)     3375 2022-08-06 01:28:36.000000 mlfactory-0.1.0/mlfactory/trainers/pytorch/train_seg.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2023-04-02 23:52:08.000000 mlfactory-0.1.0/mlfactory/trainers/pytorch/train_seg2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/trainers/tensorflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/trainers/tensorflow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/trainers/tensorflow/object_detection/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/trainers/tensorflow/object_detection/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5095 2022-11-05 18:56:21.000000 mlfactory-0.1.0/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.466474 mlfactory-0.1.0/mlfactory/visualizers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 13:09:25.000000 mlfactory-0.1.0/mlfactory/visualizers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     9415 2023-04-19 21:27:23.000000 mlfactory-0.1.0/mlfactory/visualizers/pointcloud.py
+-rw-r--r--   0 root         (0) root         (0)    12514 2023-04-19 22:14:46.000000 mlfactory-0.1.0/mlfactory/visualizers/project_rgbd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:08:15.454474 mlfactory-0.1.0/mlfactory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-06-24 22:08:15.000000 mlfactory-0.1.0/mlfactory.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4685 2023-06-24 22:08:15.000000 mlfactory-0.1.0/mlfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 22:08:15.000000 mlfactory-0.1.0/mlfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-24 22:08:15.000000 mlfactory-0.1.0/mlfactory.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-24 22:07:10.000000 mlfactory-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 22:08:15.466474 mlfactory-0.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-24 22:07:20.000000 mlfactory-0.1.0/setup.py
```

### Comparing `mlfactory-0.0.9/PKG-INFO` & `mlfactory-0.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mlfactory
-Version: 0.0.9
-Summary: Collection of several machine learning modules which can be applied to diverse projects
-Home-page: https://github.com/Homagn/mlfactory
-Author: Homagni Saha
-Author-email: Homagni Saha <homagnisaha@gmail.com>
-Project-URL: Homepage, https://github.com/Homagn/mlfactory
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 About
 =====
 ***mlfactory*** is a simple modular wrapper library that abstracts several different types of neural network architectures and techniques for computer vision (pytorch and tensorflow backend) providing seemless easy to use training in a few lines of code. 
 
 Using the standard modular philosophy you can also define your own neural network in pytorch/tensorflow, and if youre lazy to write the data loaders or the training loop then pass the network to our submodules !, or vice versa.
 
 
@@ -50,46 +36,61 @@
 
 Compose machine learning applications in a modular way
 ------------------------------------------------------
 
 1. (NYUV2 dataloader) Easy monocular depth estimation 
 - https://colab.research.google.com/drive/1T2gONs_gst4zpdS7fBoIaQclgg3J2Jgk?usp=sharing
 
+2. Finetune deeplabv3 for any general binary segmentation using less than 100 samples
+- https://colab.research.google.com/drive/1y0wirrjuoha3_SQk52IMJmL99iPGT6DZ?usp=sharing
+
 
 Annotation and other computer vision utilities
 ----------------------------------------------
 
 1. Polygon annotation tool allowing to create polygon masks for segmentation directly in colab
 - https://colab.research.google.com/drive/1YUoMU3H_m9KM6xTrAKAy9ebiDWWzXTle?usp=sharing
 
 
 2. Easy usage of superglue neural network based image feature matching
 - https://colab.research.google.com/drive/1fqnW1-Dlwz3fYlacTjMUmu5gxreGfjj6?usp=sharing
 
-
+3. Easy usage of holistically nested edge detection for generic high level edge detection
+- https://colab.research.google.com/drive/174STj0gsUZ4qOrbj_WFXhtSfwcef-oMi?usp=sharing
 
 
 
 
 
 
 
 
 Upcoming
 ========
-0. dataloader for ouster lidar data
 
-1. Coco bounding box dataloader colab
+- Hollistic edge detection network (HED) - https://github.com/sniklaus/pytorch-hed pair it up with opencv distance transform
+
+- behavior transformers and using GPT - https://github.com/notmahi/bet and https://github.com/notmahi/miniBET
+
+- base transformer model definition + segformer model definitions pytorch
+
+- diffusion models from scratch pytorch
+
+- MIRnet keras for low light image enhancement - https://keras.io/examples/vision/mirnet/
+
+- SRGAN for image superresolution - https://github.com/sgrvinod/a-PyTorch-Tutorial-to-Super-Resolution
+
+- differentiable pointcloud generation models - https://github.com/puhsu/point-clouds
 
-2. tum_rgbd dataloader
+- image animation generation models - https://github.com/snap-research/articulated-animation (code cloned in /ml/misctools/articulated-animation/, run the working demo-> demo_outofbox.py)
 
-3. visual odometry utility (examples/sfm.py and examples/sfm3d/main.py)
+- FCOSnet pytorch - https://github.com/VectXmy/FCOS.Pytorch
 
-4. superglue matcher module
+- dataloader for ouster lidar datasets
 
-5. deep_modular_reconstruction - 3D scene mapping using superglue and GLPN depth and open3d registration functions
+- Coco bounding box dataloader colab
 
-6. DeepLabv3 finetuning module
+- tum_rgbd dataloader
 
-7. Resnet finetunining module for 2D image regregression (pose estimation example)
+- DeepLabv3 finetuning module
 
-8. yolov7 estimation module
+- Resnet finetunining module for 2D image regregression (pose estimation example)
```

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/mapper.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/read_video.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/read_video.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/test_mapper.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py` & `mlfactory-0.1.0/mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py` & `mlfactory-0.1.0/mlfactory/dataloaders/binary_seg_general/create_seg_dataset_from_supervisely.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/model.py` & `mlfactory-0.1.0/mlfactory/models/pytorch/deeplabv3.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/segdataset.py` & `mlfactory-0.1.0/mlfactory/dataloaders/binary_seg_general/segdataset.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/segmentation_finetune/trainer.py` & `mlfactory-0.1.0/mlfactory/trainers/pytorch/train_seg2.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/superglue_inference/match_pair.py` & `mlfactory-0.1.0/mlfactory/applications/superglue_inference/match_pair.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/matching.py` & `mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/superglue.py` & `mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/superglue.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/superpoint.py` & `mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/superpoint.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/superglue_inference/models/utils.py` & `mlfactory-0.1.0/mlfactory/applications/superglue_inference/models/utils.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/applications/visual_odometry/sfm.py` & `mlfactory-0.1.0/mlfactory/applications/visual_odometry/sfm.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/custom_losses/pytorch/depth.py` & `mlfactory-0.1.0/mlfactory/custom_losses/pytorch/depth.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/custom_losses/pytorch/pointnetloss.py` & `mlfactory-0.1.0/mlfactory/custom_losses/pytorch/pointnetloss.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/custom_losses/pytorch/segment.py` & `mlfactory-0.1.0/mlfactory/custom_losses/pytorch/segment.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/custom_losses/tensorflow/feature_detect.py` & `mlfactory-0.1.0/mlfactory/custom_losses/tensorflow/feature_detect.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/datacreators/ai2thor/create_dataset.py` & `mlfactory-0.1.0/mlfactory/datacreators/ai2thor/create_dataset.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/datacreators/ai2thor/register_pcds.py` & `mlfactory-0.1.0/mlfactory/datacreators/ai2thor/register_pcds.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/datacreators/lidar_contours/human_contours.py` & `mlfactory-0.1.0/mlfactory/datacreators/lidar_contours/human_contours.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/datacreators/utils/colab_poly_anot.py` & `mlfactory-0.1.0/mlfactory/datacreators/utils/colab_poly_anot.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/datacreators/utils/cv_annotator.py` & `mlfactory-0.1.0/mlfactory/datacreators/utils/cv_annotator.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/ade20k.py` & `mlfactory-0.1.0/mlfactory/dataloaders/ade20k.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/cihp.py` & `mlfactory-0.1.0/mlfactory/dataloaders/cihp.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/coco.py` & `mlfactory-0.1.0/mlfactory/dataloaders/coco.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/diode.py` & `mlfactory-0.1.0/mlfactory/dataloaders/diode.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/imgcsvloader.py` & `mlfactory-0.1.0/mlfactory/dataloaders/imgcsvloader.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/lidar_datasets/loader.py` & `mlfactory-0.1.0/mlfactory/dataloaders/lidar_datasets/loader.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/lidar_datasets/nuscenes.py` & `mlfactory-0.1.0/mlfactory/dataloaders/lidar_datasets/nuscenes.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/modelnet.py` & `mlfactory-0.1.0/mlfactory/dataloaders/modelnet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/nyuv2.py` & `mlfactory-0.1.0/mlfactory/dataloaders/nyuv2.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/ouster_extract.py` & `mlfactory-0.1.0/mlfactory/dataloaders/ouster_extract.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/shapenet.py` & `mlfactory-0.1.0/mlfactory/dataloaders/shapenet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/tum_rgbd.py` & `mlfactory-0.1.0/mlfactory/dataloaders/tum_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/utils/augmentations.py` & `mlfactory-0.1.0/mlfactory/dataloaders/utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/utils/pointcloud_voxelize.py` & `mlfactory-0.1.0/mlfactory/dataloaders/utils/pointcloud_voxelize.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/dataloaders/utils/read_supervisely.py` & `mlfactory-0.1.0/mlfactory/dataloaders/utils/read_supervisely.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/misctools/median_filter.py` & `mlfactory-0.1.0/mlfactory/misctools/median_filter.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/misctools/pretrained_od.py` & `mlfactory-0.1.0/mlfactory/misctools/pretrained_od.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/misctools/random_homography.py` & `mlfactory-0.1.0/mlfactory/misctools/random_homography.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/misctools/sift_matching.py` & `mlfactory-0.1.0/mlfactory/misctools/sift_matching.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/misctools/trifocal_tensor.py` & `mlfactory-0.1.0/mlfactory/misctools/trifocal_tensor.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/misctools/video_writer.py` & `mlfactory-0.1.0/mlfactory/misctools/video_writer.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/models/pytorch/deeplabv3.py` & `mlfactory-0.1.0/mlfactory/models/pytorch/deeplabv3_scratch.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/models/pytorch/feature_pyramid.py` & `mlfactory-0.1.0/mlfactory/models/pytorch/feature_pyramid.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/models/pytorch/pointnet.py` & `mlfactory-0.1.0/mlfactory/models/pytorch/pointnet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/models/pytorch/regressor.py` & `mlfactory-0.1.0/mlfactory/models/pytorch/regressor.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/models/pytorch/simple_conv.py` & `mlfactory-0.1.0/mlfactory/models/pytorch/simple_conv.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/models/pytorch/unet.py` & `mlfactory-0.1.0/mlfactory/models/pytorch/unet.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/trainers/pytorch/train_pointcloud.py` & `mlfactory-0.1.0/mlfactory/trainers/pytorch/train_pointcloud.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/trainers/pytorch/train_reg.py` & `mlfactory-0.1.0/mlfactory/trainers/pytorch/train_reg.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/trainers/pytorch/train_seg.py` & `mlfactory-0.1.0/mlfactory/trainers/pytorch/train_seg.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py` & `mlfactory-0.1.0/mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/visualizers/pointcloud.py` & `mlfactory-0.1.0/mlfactory/visualizers/pointcloud.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory/visualizers/project_rgbd.py` & `mlfactory-0.1.0/mlfactory/visualizers/project_rgbd.py`

 * *Files identical despite different names*

### Comparing `mlfactory-0.0.9/mlfactory.egg-info/SOURCES.txt` & `mlfactory-0.1.0/mlfactory.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,14 @@
 mlfactory/applications/deep_modular_scene_mapper/tools/bundle_adjustment.py
 mlfactory/applications/deep_modular_scene_mapper/tools/depth_estimator.py
 mlfactory/applications/deep_modular_scene_mapper/tools/point_plane_icp.py
 mlfactory/applications/deep_modular_scene_mapper/tools/pose_graph_optimizer.py
 mlfactory/applications/deep_modular_scene_mapper/tools/project_rgbd.py
 mlfactory/applications/deep_modular_scene_mapper/tools/rigid_transform_3D.py
 mlfactory/applications/deep_modular_scene_mapper/tools/sift_matching.py
-mlfactory/applications/segmentation_finetune/__init__.py
-mlfactory/applications/segmentation_finetune/create_seg_dataset_from_supervisely.py
-mlfactory/applications/segmentation_finetune/datahandler.py
-mlfactory/applications/segmentation_finetune/main.py
-mlfactory/applications/segmentation_finetune/model.py
-mlfactory/applications/segmentation_finetune/segdataset.py
-mlfactory/applications/segmentation_finetune/test.py
-mlfactory/applications/segmentation_finetune/trainer.py
 mlfactory/applications/superglue_inference/__init__.py
 mlfactory/applications/superglue_inference/match_pair.py
 mlfactory/applications/superglue_inference/models/__init__.py
 mlfactory/applications/superglue_inference/models/matching.py
 mlfactory/applications/superglue_inference/models/superglue.py
 mlfactory/applications/superglue_inference/models/superpoint.py
 mlfactory/applications/superglue_inference/models/utils.py
@@ -41,14 +33,15 @@
 mlfactory/custom_losses/pytorch/depth.py
 mlfactory/custom_losses/pytorch/pointnetloss.py
 mlfactory/custom_losses/pytorch/regress.py
 mlfactory/custom_losses/pytorch/segment.py
 mlfactory/custom_losses/tensorflow/__init__.py
 mlfactory/custom_losses/tensorflow/feature_detect.py
 mlfactory/datacreators/__init__.py
+mlfactory/datacreators/nn_seg.py
 mlfactory/datacreators/ai2thor/__init__.py
 mlfactory/datacreators/ai2thor/create_dataset.py
 mlfactory/datacreators/ai2thor/register_pcds.py
 mlfactory/datacreators/lidar_contours/__init__.py
 mlfactory/datacreators/lidar_contours/human_contours.py
 mlfactory/datacreators/utils/__init__.py
 mlfactory/datacreators/utils/colab_poly_anot.py
@@ -60,40 +53,52 @@
 mlfactory/dataloaders/diode.py
 mlfactory/dataloaders/imgcsvloader.py
 mlfactory/dataloaders/modelnet.py
 mlfactory/dataloaders/nyuv2.py
 mlfactory/dataloaders/ouster_extract.py
 mlfactory/dataloaders/shapenet.py
 mlfactory/dataloaders/tum_rgbd.py
+mlfactory/dataloaders/binary_seg_general/__init__.py
+mlfactory/dataloaders/binary_seg_general/create_seg_dataset_from_supervisely.py
+mlfactory/dataloaders/binary_seg_general/datahandler.py
+mlfactory/dataloaders/binary_seg_general/segdataset.py
 mlfactory/dataloaders/lidar_datasets/__init__.py
 mlfactory/dataloaders/lidar_datasets/loader.py
 mlfactory/dataloaders/lidar_datasets/nuscenes.py
 mlfactory/dataloaders/utils/__init__.py
 mlfactory/dataloaders/utils/augmentations.py
 mlfactory/dataloaders/utils/pointcloud_voxelize.py
 mlfactory/dataloaders/utils/read_supervisely.py
+mlfactory/examples/__init__.py
+mlfactory/examples/nn_edge.py
+mlfactory/examples/segmentation_finetune/__init__.py
+mlfactory/examples/segmentation_finetune/main.py
+mlfactory/examples/segmentation_finetune/test.py
 mlfactory/misctools/__init__.py
 mlfactory/misctools/median_filter.py
 mlfactory/misctools/pretrained_od.py
 mlfactory/misctools/random_homography.py
 mlfactory/misctools/sift_matching.py
 mlfactory/misctools/trifocal_tensor.py
 mlfactory/misctools/video_writer.py
 mlfactory/models/__init__.py
 mlfactory/models/pytorch/__init__.py
 mlfactory/models/pytorch/deeplabv3.py
+mlfactory/models/pytorch/deeplabv3_scratch.py
 mlfactory/models/pytorch/feature_pyramid.py
+mlfactory/models/pytorch/hed.py
 mlfactory/models/pytorch/pointnet.py
 mlfactory/models/pytorch/regressor.py
 mlfactory/models/pytorch/simple_conv.py
 mlfactory/models/pytorch/unet.py
 mlfactory/trainers/__init__.py
 mlfactory/trainers/pytorch/__init__.py
 mlfactory/trainers/pytorch/train_pointcloud.py
 mlfactory/trainers/pytorch/train_reg.py
 mlfactory/trainers/pytorch/train_seg.py
+mlfactory/trainers/pytorch/train_seg2.py
 mlfactory/trainers/tensorflow/__init__.py
 mlfactory/trainers/tensorflow/object_detection/__init__.py
 mlfactory/trainers/tensorflow/object_detection/sliding_window_train.py
 mlfactory/visualizers/__init__.py
 mlfactory/visualizers/pointcloud.py
 mlfactory/visualizers/project_rgbd.py
```

### Comparing `mlfactory-0.0.9/pyproject.toml` & `mlfactory-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "mlfactory"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Homagni Saha", email="homagnisaha@gmail.com" },
 ]
 description = "Collection of several machine learning modules which can be applied to diverse projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mlfactory-0.0.9/setup.py` & `mlfactory-0.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='mlfactory',  
-     version='0.0.9',
+     version='0.1.0',
      author="Homagni Saha",
      author_email="homagnisaha@gmail.com",
      description="Collection of several machine learning modules which can be applied to diverse projects",
      long_description=long_description,
    long_description_content_type="text/markdown",
      url="https://github.com/Homagn/mlfactory",
-     packages=setuptools.find_packages(exclude=["mlfactory/applications/superglue_inference/models/weights","mlfactory/applications/segmentation_finetune/CFExp"]),
+     packages=setuptools.find_packages(exclude=["mlfactory/applications/superglue_inference/models/weights"]),
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
  )
```

