# Awesome Pose-Free NeRF & 3D Gaussian Splatting

A curated list of **pose-free NeRF** and **pose-free 3DGS** papers, datasets, and tools.  
This list is constructed based on the survey *Pose-Free NeRF and 3DGS* (2026).  
Pull requests are welcome!

---

## Contents
- [Overview](#Overview)
- [Pose-Free NeRF](#pose-free-nerf)
  - [Base Model Enhancement](#base-model-enhancement)
  - [Training Strategy Refinement](#training-strategy-refinement)
  - [Novel Priors Incorporation](#novel-priors-incorporation)
  - [Applications](#applications)
    - [In-the-wild](#in-the-wild)
    - [Motion Images](#motion-images)
    - [Sparse View](#sparse-view)
    - [Large Scale](#large-scale)
    - [Dynamic Scene](#dynamic-scene)
- [Pose-Free 3DGS](#pose-free-3dgs)
  - [Training Strategy Refinement](#training-strategy-refinement-1)
  - [Novel Priors Incorporation](#novel-priors-incorporation-1)
  - [Applications](#applications-1)
    - [Motion Images](#motion-images-1)
    - [Sparse View](#sparse-view-1)
    - [Medical Surgery](#medical-surgery)
- [Datasets](#datasets)
- Tools & Supporting Techniques
- [Surveys](#survey)
- Contributing

---

## Overview


---

## Pose-Free NeRF

### Base Model Enhancement
- GNeRF: GAN-based Neural Radiance Field without Posed Camera [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/quan-meng/gnerf)

- SiNeRF: Sinusoidal Neural Radiance Fields for Joint Pose Estimation and Scene Reconstruction [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/yitongx/sinerf)

- Gaussian Activated Neural Radiance Fields for High Fidelity Reconstruction and Pose Estimation [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/sfchng/Gaussian-Activated-Radiance-Fields)

- DBARF: Deep Bundle-Adjusting Generalizable Neural Radiance Fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/AIBluefisher/dbarf)

- Robustifying the Multi-Scale Representation of Neural Radiance Fields

- Learning Robust Multi-Scale Representation for Neural Radiance Fields from Unposed Images

- Disentangled Generation and Aggregation for Robust Radiance Fields

- I-DACS: Always Maintaining Consistency Between Poses and the Field for Radiance Field Construction Without Pose Prior [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/z619850002/IDACS)

### Training Strategy Refinement
- BARF: Bundle-Adjusting Neural Radiance Fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/chenhsuanlin/bundle-adjusting-NeRF)

- CBARF: Cascaded Bundle-Adjusting Neural Radiance Fields from Imperfect Camera Poses

- LU-NeRF: Scene and Pose Estimation by Synchronizing Local Unposed NeRFs

- CF-NeRF: Camera Parameter Free Neural Radiance Fields with Incremental Learning [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/yanqswhu/CF-NeRF_release)

- CT-NeRF: Incremental Optimizing Neural Radiance Field and Poses with Complex Trajectory

- NeRF--: Neural Radiance Fields Without Known Camera Parameters [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/ActiveVisionLab/nerfmm)

- iNeRF: Inverting Neural Radiance Fields for Pose Estimation [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/yenchenlin/iNeRF-public)

- Unifying Correspondence Pose and NeRF for Generalized Pose-Free Novel View Synthesis [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/cvlab-kaist/CoPoNeRF)

- TD-NeRF: Novel Truncated Depth Prior for Joint Camera Pose and Neural Radiance Field Optimization

- FDC-NeRF: Learning Pose-Free Neural Radiance Fields with Flow-Depth Consistency

- Camp: Camera preconditioning for neural radiance fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/jonbarron/camp_zipnerf)

- Structure-Aware NeRF without Posed Camera via Epipolar Constraint [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/XTU-PR-LAB/SaNerf)

- NeRFtrinsic Four: An end-to-end trainable NeRF jointly optimizing diverse intrinsic and extrinsic camera parameters [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/HannahHaensen/nerftrinsic_four)

- Pose-Free Neural Radiance Fields via Implicit Pose Regularization 

- Generic Objects as Pose Probes for Few-shot View Synthesis [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/zhirui-gao/PoseProbe)

- CAD-NeRF: learning NeRFs from uncalibrated few-view images by CAD model retrieval

### Novel Priors Incorporation 
- BID-NeRF: RGB-D image pose estimation with inverted Neural Radiance Fields

- NoPe-NeRF: Optimising Neural Radiance Field With No Pose Prior [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/ActiveVisionLab/nope-nerf) 

- AltNeRF: Learning Robust Neural Radiance Field via Alternating Depth-Pose Optimization

- Neural RGB-D Surface Reconstruction [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/dazinovic/neural-rgbd-surface-reconstruction)

- Self-Calibrating Neural Radiance Fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/POSTECH-CVLab/SCNeRF)

- Local-to-Global Registration for Bundle-Adjusting Neural Radiance Fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/rover-xingyu/L2G-NeRF)

- Invertible neural warp for nerf [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/sfchng/neural_invertible_warp)

- FlowCam: Training Generalizable 3D Radiance Fields without Camera Poses via Pixel-Aligned Scene Flow [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/cameronosmith/FlowCam)

- LiDeNeRF: Neural radiance field reconstruction with depth prior provided by LiDAR point cloud

- GeoNLF: Geometry guided Pose-Free Neural LiDAR Fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/ispc-lab/GeoNLF)

- Direct Alignment for Robust NeRF Learning

- RPE-BARF: Relative Pose Estimation for Robust Bundle-Adjusting Neural Radiance Fields

- NoPe-NeRF++: Local-to-Global Optimization of NeRF with No Pose Prior

- SG-NeRF: Neural Surface Reconstruction with Scene Graph Optimization [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/Iris-cyy/SG-NeRF)

- Robust SG-NeRF: Robust Scene Graph Aided Neural Surface Reconstruction

- PoRF: Pose Residual Field for Accurate Neural Surface Reconstruction [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/ActiveVisionLab/porf)

### Applications

#### In-the-wild

- SAMURAI: Shape And Material from Unconstrained Real-world Arbitrary Image collections [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/google/samurai)

- NeROIC: neural rendering of objects from online image collections [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/snap-research/NeROIC)

- SHINOBI: Shape and Illumination using Neural Object Decomposition via BRDF Optimization In-the-wild [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/cgtuebingen/shinobi)

- UP-NeRF: Unconstrained Pose Prior-Free Neural Radiance Field [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/mlvlab/UP-NeRF)

#### Motion Images

- BAD-NeRF: Bundle Adjusted Deblur Neural Radiance Fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/WU-CVGL/BAD-NeRF.git)

- BeNeRF: Neural Radiance Fields from a Single Blurry Image and Event Stream [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/wu-cvgl/BeNeRF)

- Deblurring Neural Radiance Fields with Event-driven Bundle Adjustment [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/iCVTEAM/EBAD-NeRF)

- USB-NeRF: Unrolling Shutter Bundle Adjusted Neural Radiance Fields [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/WU-CVGL/USB-NeRF)

- RS-NeRF: Neural Radiance Fields from Rolling Shutter Images [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/MyNiuuu/RS-NeRF)

#### Sparse View

- RegNeRF: Regularizing Neural Radiance Fields for View Synthesis From Sparse Inputs [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/LRLVEC/regnerf)

- SPARF: Neural Radiance Fields From Sparse and Noisy Poses [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/google-research/sparf)

- DaRF: Boosting Radiance Fields from Sparse Input Views with Monocular Depth Adaptation [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/cvlab-kaist/DaRF)

- SN $^{2}$ eRF: A Framework for Neural Radiance Fields given Sparse and Noisy Poses

- Learning Geometry Consistent Neural Radiance Fields from Sparse and Unposed Views

- Tracknerf: Bundle adjusting nerf from sparse and noisy views via feature tracks [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/Wayne-Mai/traf_public)

- Just Flip: Flipped Observation Generation and Optimization for Neural Radiance Fields to Cover Unobserved View [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/sibaek-lee/Just-Flip)

#### Large Scale

- Progressively Optimized Local Radiance Fields for Robust View Synthesis [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/facebookresearch/localrf)

- UC-NeRF: Neural Radiance Field for Under-Calibrated Multi-view Cameras in Autonomous Driving [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/kcheng1021/UC-NeRF)

- DGNR: Density-Guided Neural Point Rendering of Large Driving Scenes [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/JOP-Lee/DGNR-Rendering)

#### Dynamic Scene

- BASED: Bundle-Adjusting Surgical Endoscopic Dynamic Video Reconstruction using Neural Radiance Fields

- DynaMoN: Motion-Aware Fast and Robust Camera Localization for Dynamic Neural Radiance Fields[![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/HannahHaensen/DynaMoN)


---

## Pose-Free 3DGS

### Training Strategy Refinement
- COLMAP-Free 3D Gaussian Splatting [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/NVlabs/CF-3DGS)

- GGRt: Geometry-Guided Radiance Tracking for 3D Gaussian Splatting [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/lifuguan/GGRt_official)

- EasySplat: View-Adaptive Learning makes 3D Gaussian Splatting Easy [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/Yuhuoo/EasySplat)

- SfM-Free 3D Gaussian Splatting via Hierarchical Training [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/jibo27/3DGS_Hierarchical_Training)

- KeyGS: A Keyframe-Centric Gaussian Splatting Method for Monocular Image Sequences 

- Towards Better Robustness: Pose-Free 3D Gaussian Splatting for Arbitrarily Long Videos

### Novel Priors Incorporation 
- PF3plat: Pose-Free Feed-Forward 3D Gaussian Splatting [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/cvlab-kaist/PF3plat)

- Look Gauss, No Pose: Novel View Synthesis using Gaussian Splatting without Accurate Pose Initialization [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/Schmiddo/noposegs)

- ZeroGS: Training 3D Gaussian Splatting from Unposed Images [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/AIBluefisher/DeepGfM)

- SelfSplat: Pose-Free and 3D Prior-Free Generalizable 3D Gaussian Splatting [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/Gynjn/selfsplat)

- Hybrid bundle-adjusting 3D Gaussians for view consistent rendering with pose optimization [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/Bistu3DV/hybridBA)

- TrackGS: Optimizing COLMAP-Free 3D Gaussian Splatting with Global Track Constraints

- PCR-GS: COLMAP-Free 3D Gaussian Splatting via Pose Co-Regularizations

- 3R-GS: Best Practice in Optimizing Camera Poses Along with 3DGS

### Applications

#### Motion Images

- Self-Calibrating 4D Novel View Synthesis from Monocular Videos Using Gaussian Splatting

- DreamScene4D: Dynamic Multi-Object Scene Generation from Monocular Videos [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/dreamscene4d/dreamscene4d)

- MotionGS: Exploring Explicit Motion Guidance for Deformable 3D Gaussian Splatting [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/RuijieZhu94/MotionGS)

- Deblur-GS: 3D Gaussian Splatting from Camera Motion Blurred Images [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/Chaphlagical/Deblur-GS)

- EF-3DGS: Event-Aided Free-Trajectory 3D Gaussian Splatting

- IncEventGS: Pose-Free Gaussian Splatting from a Single Event Camera [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/WU-CVGL/IncEventGS)

#### Sparse View

- InstantSplat: Sparse-view Gaussian Splatting in Seconds [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/NVlabs/InstantSplat)

- Gaussian Scenes: Pose-Free Sparse-View Scene Reconstruction using Depth-Enhanced Diffusion Priors [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/mvp18/gaussian-scenes)

- MetaSplats: Rapid Sparse 2D View to 3D Novel View Synthesis

- GBR: Generative Bundle Refinement for High-fidelity Gaussian Splatting and Meshing

- Gesplat: Robust Pose-Free 3D Reconstruction via Geometry-Guided Gaussian Splatting

- No Pose, No Problem: Surprisingly Simple 3D Gaussian Splats from Sparse Unposed Images [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/cvg/NoPoSplat)

- No Pose at All: Self-Supervised Pose-Free 3D Gaussian Splatting from Sparse Views [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/ranrhuang/SPFSplat)

- A Construct-Optimize Approach to Sparse View Synthesis without Camera Pose [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/PeterZs/COGS4.git)

#### Medical Surgery

- Free-SurGS: SfM-Free 3D Gaussian Splatting for Surgical Scene Reconstruction [![github](https://img.shields.io/badge/GitHub-000?logo=github)](https://github.com/MrinalTyagi/Free-SurGS-benchmark.git)

- Free-DyGS: Camera-Pose-Free Scene Reconstruction based on Gaussian Splatting for Dynamic Surgical Videos

---

## Datasets

- [NeRF Synthetic](https://drive.google.com/drive/folders/1cK3UDIJqKAAm7zyrxRYVFJ0BRMgrwhh4)

- [LLFF](https://bmild.github.io/llff/)

- [DTU](https://roboimagedata.compute.dtu.dk/?page_id=36)

- [Replica](https://github.com/facebookresearch/Replica-Dataset)

- [Tanks and Temples](https://www.tanksandtemples.org/)

- [RealEstate10K](https://google.github.io/realestate10k/)

- [CO3D V2](https://github.com/facebookresearch/co3d)

- [Static Hikes](https://github.com/facebookresearch/localrf?tab=readme-ov-file)

---

## Survey

---
