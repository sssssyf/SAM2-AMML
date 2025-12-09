# SAM2-AMML
SAM2-Assisted Multi-Modality Learning for MLS Point Cloud Semantic Segmentation

# Highlights
Aiming at the road objects segmentation in street-level scenes, based on SAM2, we develop a specialized mask generation method under the point-to-pixel projection correspondence, which includes boundary-prompts elimination and multi-masks fusion strategies. 

To effectively leverage the complementary superiorities of RGB images and solve the challenge caused by feature-level fusion, we rethink the multi-modality interaction between point cloud and images, proposing a SAM2-assisted multi-modality learning for MLS point cloud semantic segmentation. To our knowledge, it is the first successful attempt to apply SAM2 for multi-modality MLS point cloud semantic segmentation.

Extensive experiments demonstrate that our mask generation method based on SAM2 can effectively extract objects of interest in street-level scenes, and SAM2-AMML can effectively enhance the point cloud semantic segmentation of different LiDAR baselines, achieving SOTA results.

# Preview
The relevant codes will be available here after paper publication.

# Demo
| Name | Vedio |
|------|------|
| KITTI_08_SAM2_MASK | <img src="./demo/output_video_KITTI_08_SAM2_MASK.gif" width="300" alt="演示1"/> |
| nuScenes_SAM2_MASK | <img src="./demo/output_video_nuScenes_SAM2_MASKS_4000Frames.gif" width="300" alt="演示2"/> |
| Improved Predictions_SAM2-AMML| <img src="./demo/output_video_SAM2-AMML.gif" width="300" alt="演示3"/> |
| Improved Predictions_SAM2-AMML_Projection | <img src="./demo/output_video_SAM2-AMML-projection.gif" width="300" alt="演示4"/> |
