# SAM2-AMML
SAM2-Assisted Multi-Modality Learning for Large-Scale MLS Point Cloud Semantic Segmentation in Street-Level Scenes

# Abstract
LiDAR excels at capturing accurate depth and 3D geometry, but its point cloud is sparse and textureless. In contrast, cameras can provide dense color and fine-grained texture. However, traditional feature-level fusion in multi-modality point cloud semantic segmentation struggles with the challenge of large modality gap and losing modality specificity. To effectively leverage the complementary superiorities of RGB images and solve the challenge caused by feature-level fusion simultaneously, we rethink the multi-modality interaction between LiDAR point cloud and camera RGB images, proposing a SAM2-assisted multi-modality learning (SAM2-AMML) for large-scale MLS point cloud semantic segmentation in street-level scenes. Specifically, inspired by the zero-shot image segmentation generalization performance of visual foundation model SAM2 and aiming at the segmentation of road objects in street-level scenes, we develop a specialized mask generation method under the point-to-pixel projection correspondence. Next, the generated masks can serve as a superior constraint of contextual-semantic consistency for sparse and textureless MLS point cloud. Thus, we are no longer restricted to feature-level fusion, instead we utilize the object masks from SAM2 to enforce semantic consistency of 3D predictions, incorporating the rich color and texture knowledge of images into 3D network during modality interaction. Extensive experiments on SemanticKITTI and nuScenes benchmarks demonstrate that our mask generation method can effectively extract objects of interest in street-level scenes by using SAM2, and SAM2-AMML can effectively enhance the performance of different LiDAR baselines, achieving SOTA results.

# Highlights
Aiming at the road objects segmentation in street-level scenes, based on SAM2, we develop a specialized mask generation method under the point-to-pixel projection correspondence. With the proposed boundary-prompts elimination and multi-masks fusion strategies, the objects of interest can be effectively extracted in different street-level scenes by using SAM2.

To effectively leverage the complementary superiorities of RGB images and solve the challenge caused by feature-level fusion, we rethink the multi-modality interaction between point clouds and images, proposing a SAM2-assisted multi-modality learning for large-scale MLS point cloud semantic segmentation in street-level scenes. To our knowledge, it is the first successful attempt to apply SAM2 for MLS point cloud semantic segmentation.

Extensive experiments demonstrate that our mask generation method based on SAM2 can effectively extract objects of interest in street-level scenes, and SAM2-AMML can effectively enhance the point cloud semantic segmentation of different LiDAR baselines, achieving SOTA results.

# Preview
The relevant codes will be available here after paper publication.

# Demo
| Name | Vedio |
|------|------|
| KITTI_08_SAM2_MASK | <img src="./demo/output_video_KITTI_08_SAM2-branch_MASK.gif" width="300" alt="演示1"/> |
| nuScenes_SAM2_MASK | <img src="./demo/output_video_nuScenes_SAM2-branch_MASKS_4000Frames.gif" width="300" alt="演示2"/> |
| Improved Predictions_SAM2-AMML| <img src="./demo/output_video_SAM2-AMML.gif" width="300" alt="演示3"/> |
| Improved Predictions_SAM2-AMML_Projection | <img src="./demo/output_video_SAM2-AMML-projection.gif" width="300" alt="演示4"/> |
