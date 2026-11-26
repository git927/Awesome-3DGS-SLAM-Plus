# Awesome 3DGS SLAM Plus · 中文论文索引

本仓库面向中文社区，持续整理 3D 高斯泼溅（3D Gaussian Splatting，3DGS）SLAM 相关论文和开源资源，涵盖图像传感器、事件相机和激光雷达等方向。

如果发现遗漏的论文，欢迎[按指南提交拉取请求（PR）](https://github.com/KwanWaiPang/Awesome-Transformer-based-SLAM/blob/pdf/How-to-PR.md)，也可以[到上游仓库提交议题](https://github.com/KwanWaiPang/Awesome-3DGS-SLAM/issues/new)。

欢迎以各种方式参与，一起完善这份清单。

如果这份清单对你有帮助，欢迎点个 Star 支持。

也欢迎把这份清单分享给感兴趣的朋友。

<a name="overview"></a>

## 目录

- [基于图像的 3DGS SLAM](#image-based-3dgs)
- [基于激光雷达（LiDAR）的 3DGS SLAM](#lidar-based-3dgs)
- [基于事件相机的 3DGS SLAM](#event-based-3dgs)



<!-- |---|`arXiv`|---|---|---| -->
<!-- [![GitHub 星标数](https://img.shields.io/github/stars/***.svg)]() -->
<a name="image-based-3dgs"></a>

## 基于图像的 3DGS SLAM

| 年份 | 发表渠道 | 论文标题 | 代码仓库 | 备注 |
|:----:|:-----:| ----------- |:----------:|:----:|
|2026|`arXiv`|[DPGS-SLAM: Diffusion-Prior and Provenance-Aware Monocular Gaussian Splatting SLAM for Dynamic Visual Sensing](https://arxiv.org/abs/2611.12038)|---|以单目 RGB 为输入，用扩散模型临时补全被动态物体遮挡的静态背景，并标记高斯基元的来源以区分生成内容与真实观测。|
|2026|`arXiv`|[LangGS-SLAM: Real-Time Language-Feature Gaussian Splatting SLAM](https://arxiv.org/pdf/2602.06991)|---|从VLM（一个语义分割模型）中嵌入三维特征场，实现开放词汇和大语言模型交互式感知；3DGS部分用的GICP|
|2026|`arXiv`|[PointSLAM++: Robust Dense Neural Gaussian Point Cloud-based SLAM](https://arxiv.org/pdf/2601.11617)|---|融合神经表示（MLP）与高斯表示，位姿优化结合 GICP 与 ORB 重投影误差|
|2026|`arXiv`|[PLANING: A Loosely Coupled Triangle-Gaussian Framework for Streaming 3D Reconstruction](https://arxiv.org/pdf/2601.22046)|---|[项目主页](https://city-super.github.io/PLANING/)<br>融合网格与 3DGS 表示。用网格构建稳定的几何骨架，用 3DGS 补充视觉细节。前端采用 MASt3R 等前馈模型预测点图和相机位姿|
|2026|`Neurocomputing`|[2D Gaussian Primitive SLAM: Real-Time Dense SLAM with 2D Gaussian Primitives](https://www.sciencedirect.com/science/article/pii/S0925231226001190)|---|---|
|2026|`arXiv`|[FeatureSLAM: Feature-enriched 3D gaussian splatting SLAM in real time](https://arxiv.org/pdf/2601.05738)|---|---|
|2026|`Pattern Recognition`|[RGD-SLAM: Robust Gaussian Splatting SLAM for Dynamic Environments](https://www.sciencedirect.com/science/article/pii/S0031320326000348)|[![GitHub 星标数](https://img.shields.io/github/stars/RGD-SLAM.svg)](https://github.com/00Haocheng/RGD-SLAM)|---|
|2026|`Proceedings of the IEEE International Symposium on High Performance Computer Architecture`|[Splatonic: Architecture Support for 3D Gaussian Splatting SLAM via Sparse Processing](https://arxiv.org/pdf/2511.18755)|---|[项目主页](https://stonesix16.github.io/splatonic/)|
|2025|`IROS`|[Pseudo Depth Meets Gaussian: A Feed-forward RGB SLAM Baseline](https://arxiv.org/pdf/2508.04597?)|[![GitHub 星标数](https://img.shields.io/github/stars/wangyr22/DepthGS.svg)](https://github.com/wangyr22/DepthGS)|单目深度估计模型生成伪深度图+3D高斯实现高效在线重建|
|2025|`arXiv`|[RGS-SLAM: Robust Gaussian Splatting SLAM with One-Shot Dense Initialization](https://arxiv.org/pdf/2601.00705)|---|---|
|2025|`RAL`|[MANG-SLAM: Multi-Agent Neural Submap and Gaussian Representation for Dense Mapping](https://ieeexplore.ieee.org/abstract/document/11297803/)|---|NeRF+3DGS+多机融合建图|
|2025|`RAL`|[DQO-MAP: Real-Time Object-Level SLAM With Dual Quadrics and Gaussians](https://ieeexplore.ieee.org/abstract/document/11266903/)|[![GitHub 星标数](https://img.shields.io/github/stars/LiHaoy-ux/DQO-MAP.svg)](https://github.com/LiHaoy-ux/DQO-MAP)|---|
|2025|`arXiv`|[ATLAS Navigator: Active Task-driven LAnguage-embedded Gaussian Splatting](https://arxiv.org/pdf/2502.20386)|---|[项目主页](https://atlasnav.github.io/)|
|2025|`arXiv`|[D2GSLAM: 4D Dynamic Gaussian Splatting SLAM](https://arxiv.org/pdf/2512.09411)|---|---|
|2025|`arXiv`|[LEGO-SLAM: Language-Embedded Gaussian Optimization SLAM](https://arxiv.org/pdf/2511.16144)|[![GitHub 星标数](https://img.shields.io/github/stars/Lab-of-AI-and-Robotics/LEGO-SLAM.svg)](https://github.com/Lab-of-AI-and-Robotics/LEGO-SLAM)|[项目主页](https://lab-of-ai-and-robotics.github.io/LEGO-SLAM/)|
|2025|`arXiv`|[Robust 3DGS-based SLAM via Adaptive Kernel Smoothing](https://arxiv.org/pdf/2511.23221)|---|---|
|2025|`arXiv`|[VIGS-SLAM: Visual Inertial Gaussian Splatting SLAM](https://arxiv.org/pdf/2512.02293)|---|[项目主页](https://vigs-slam.github.io/)|
|2025|`TRO`|[OmniMap: A General Mapping Framework Integrating Optics, Geometry, and Semantics](https://arxiv.org/pdf/2509.07500)|[![GitHub 星标数](https://img.shields.io/github/stars/BIT-DYN/omnimap.svg)](https://github.com/BIT-DYN/omnimap)|[项目主页](https://omni-map.github.io/)|
|2025|`ICCV`|[DyGS-SLAM: Real-Time Accurate Localization and Gaussian Reconstruction for Dynamic Scenes](https://openaccess.thecvf.com/content/ICCV2025/papers/Hu_DyGS-SLAM_Real-Time_Accurate_Localization_and_Gaussian_Reconstruction_for_Dynamic_Scenes_ICCV_2025_paper.pdf)|---|---|
|2025|`ICCV`|[Segs-slam: Structure-enhanced 3d gaussian splatting slam with appearance embedding](https://openaccess.thecvf.com/content/ICCV2025/papers/Wen_SEGS-SLAM_Structure-enhanced_3D_Gaussian_Splatting_SLAM_with_Appearance_Embedding_ICCV_2025_paper.pdf)|---|---|
|2025|`arXiv`|[RoGER-SLAM: A Robust Gaussian Splatting SLAM System for Noisy and Low-light Environment Resilience](https://arxiv.org/pdf/2510.22600)|---|---|
|2025|`RAL`|[GaussR-SLAM: Gaussian Robust SLAM in Data Loss and Interference Environments](https://ieeexplore.ieee.org/abstract/document/11164563)|---|---|
|2025|`arXiv`|[MCGS-SLAM: A Multi-Camera SLAM Framework Using Gaussian Splatting for High-Fidelity Mapping](https://arxiv.org/pdf/2509.14191)|---|[项目主页](https://anonymous.4open.science/w/MCGSSLAM-A8F8/)|
|2025|`arXiv`|[Gaussian-Plus-SDF SLAM: High-fidelity 3D Reconstruction at 150+ fps](https://arxiv.org/pdf/2509.11574)|---|---|
|2025|`arXiv`|[MemGS: Memory-Efficient Gaussian Splatting for Real-Time SLAM](https://arxiv.org/pdf/2509.13536)|[![GitHub 星标数](https://img.shields.io/github/stars/NAIL-HNU/MemGS_SLAM.svg)](https://github.com/NAIL-HNU/MemGS_SLAM) |---|
|2025|`arXiv`|[DyPho-SLAM: Real-time Photorealistic SLAM in Dynamic Environments](https://arxiv.org/pdf/2509.00741)|---|---| 
|2025|`arXiv`|[AGS: Accelerating 3D Gaussian Splatting SLAM via CODEC-Assisted Frame Covisibility Detection](https://arxiv.org/pdf/2509.00433)|---|---|
|2025|`ICRA`|[FGO-SLAM: Enhancing Gaussian SLAM with Globally Consistent Opacity Radiance Field](https://arxiv.org/pdf/2509.01547)|---|---|
|2025|`arXiv`|[Stereo 3D Gaussian Splatting SLAM for Outdoor Urban Scenes](https://arxiv.org/pdf/2507.23677)|---|---|
|2025|`ICCV`|[SEGS-SLAM: Structure-enhanced 3D Gaussian Splatting SLAM with Appearance Embedding](https://arxiv.org/pdf/2501.05242)|[![GitHub 星标数](https://img.shields.io/github/stars/leaner-forever/SEGS-SLAM.svg)](https://github.com/leaner-forever/SEGS-SLAM)|[项目主页](https://segs-slam.github.io/)|
|2025|`arXiv`|[MGSO: Monocular Real-time Photometric SLAM with Efficient 3D Gaussian Splatting](https://arxiv.org/pdf/2409.13055v2)|---|---|
|2025|`arXiv`|[Stereo 3D Gaussian Splatting SLAM for Outdoor Urban Scenes](https://arxiv.org/pdf/2507.23677)|---|---|
|2025|`arXiv`|[S3LAM: Surfel Splatting SLAM for Geometrically Accurate Tracking and Mapping](https://arxiv.org/pdf/2507.20854)|---|---| 
|2025|`arXiv`|[Stereo 3D Gaussian Splatting SLAM for Outdoor Urban Scenes](https://arxiv.org/pdf/2507.23677)|---|---|
|2025|`arXiv`|[G2S-ICP SLAM: Geometry-aware Gaussian Splatting ICP SLAM](https://arxiv.org/pdf/2507.18344)|---|---|
|2025|`ICRA`|[RGB-Only Gaussian Splatting SLAM for Unbounded Outdoor Scenes](https://arxiv.org/pdf/2502.15633?)|[![GitHub 星标数](https://img.shields.io/github/stars/3DAgentWorld/OpenGS-SLAM.svg)](https://github.com/3DAgentWorld/OpenGS-SLAM)|[项目主页](https://3dagentworld.github.io/opengs-slam/)| 
|2025|`ICCV`|[Outdoor Monocular SLAM with Global Scale-Consistent 3D Gaussian Pointmaps](https://arxiv.org/pdf/2507.03737)|[![GitHub 星标数](https://img.shields.io/github/stars/3DAgentWorld/S3PO-GS.svg)](https://github.com/3DAgentWorld/S3PO-GS)|[项目主页](https://3dagentworld.github.io/S3PO-GS/)|
|2025|`IEEE Transactions on Artificial Intelligence`|[Constrained Gaussian Splatting via Implicit TSDF Hash Grid for Dense RGB-D SLAM](https://ieeexplore.ieee.org/abstract/document/11060934)|---|---|
|2025|`Joint International Conference on Automation-Intelligence-Safety`|[Mono-SLAM: Monocular 3D Gaussian Splatting SLAM with Geometric Loss and Multi-view Consistency](https://ieeexplore.ieee.org/abstract/document/11051648)|---|---|
|2025|`RAL`|[FusionGS-SLAM: Multiple Sensors Fusion for Localization and Real-Time Photorealistic Mapping](https://ieeexplore.ieee.org/abstract/document/11066268/)|---|---|
|2025|`RAL`|[SAGA-SLAM: Scale-Adaptive 3D Gaussian Splatting for Visual SLAM](https://ieeexplore.ieee.org/abstract/document/11067946/)|---|---|
|2025|`arXiv`|[GRAND-SLAM: Local Optimization for Globally Consistent Large-Scale Multi-Agent Gaussian SLAM](https://arxiv.org/pdf/2506.18885)|---|---|
|2025|`RAL`|[Dense Monocular SLAM in Real-time with Structured Gaussian Representation](https://ieeexplore.ieee.org/abstract/document/11052667/)|---|---|
|2025|`arXiv`|[TVG-SLAM: Robust Gaussian Splatting SLAM with Tri-view Geometric Constraints](https://arxiv.org/pdf/2506.23207)|---|---| 
|2025|`arXiv`|[GRAND-SLAM: Local Optimization for Globally Consistent Large-Scale Multi-Agent Gaussian SLAM](https://arxiv.org/pdf/2506.18885)|---|---|
|2025|`IROS`|[SplatPose: Geometry-Aware 6-DoF Pose Estimation from Single RGB Image via 3D Gaussian Splatting](https://arxiv.org/pdf/2503.05174?)|---|---|
|2025|`TASE`|[MG-SLAM: Structure Gaussian Splatting SLAM with Manhattan World Hypothesis](https://ieeexplore.ieee.org/abstract/document/11029049)|---|---|
|2025|`arXiv`|[Dy3DGS-SLAM: Monocular 3D Gaussian Splatting SLAM for Dynamic Environments](https://arxiv.org/pdf/2506.05965)|---|---|
|2025|`arXiv`|[GS4: Generalizable Sparse Splatting Semantic SLAM](https://arxiv.org/pdf/2506.06517)|---|[项目主页](https://mingqij.github.io/projects/gs4/)|
|2025|`International Conference on Autonomous Agents and Multiagent Systems`|[OGS-SLAM: Hybrid ORB-Gaussian Splatting SLAM](https://dl.acm.org/doi/abs/10.5555/3709347.3743762)|[![GitHub 星标数](https://img.shields.io/github/stars/realXiaohan/OGS-SLAM.svg)](https://github.com/realXiaohan/OGS-SLAM)|---|
|2025|`arXiv`|[Globally Consistent RGB-D SLAM with 2D Gaussian Splatting](https://arxiv.org/pdf/2506.00970)|[![GitHub 星标数](https://img.shields.io/github/stars/PRBonn/2DGS-SLAM.svg)](https://github.com/PRBonn/2DGS-SLAM)|MASt3R 用于回环检测|
|2025|`arXiv`|[VTGaussian-SLAM: RGBD SLAM for Large Scale Scenes with Splatting View-Tied 3D Gaussians](https://arxiv.org/pdf/2506.02741)|---|[项目主页](https://machineperceptionlab.github.io/VTGaussian-SLAM-Project/)|
|2025|`arXiv`|[VPGS-SLAM: Voxel-based Progressive 3D Gaussian SLAM in Large-Scale Scenes](https://arxiv.org/pdf/2505.18992)|[![GitHub 星标数](https://img.shields.io/github/stars/dtc111111/vpgs-slam.svg)](https://github.com/dtc111111/vpgs-slam)|---| 
|2025|`arXiv`|[ADD-SLAM: Adaptive Dynamic Dense SLAM with Gaussian Splatting](https://arxiv.org/pdf/2505.19420)|---|---|
|2025|`arXiv`|[LGSBA: Local Gaussian Splatting Bundle Adjustment for Optimizing 3DGS Rendering Quality](https://www.preprints.org/frontend/manuscript/ddecffbfbb0306ab43042be32552275f/download_pub)|[![GitHub 星标数](https://img.shields.io/github/stars/wla-98/worse-pose-but-better-3DGS.svg)](https://github.com/wla-98/worse-pose-but-better-3DGS)|---| 
|2025|`CVPR`|[4DTAM: Non-Rigid Tracking and Mapping via Dynamic Surface Gaussians](https://muskie82.github.io/4dtam/paper/4dtam_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/muskie82/4dtam.svg)](https://github.com/muskie82/4dtam)|[项目主页](https://muskie82.github.io/4dtam/)| 
|2025|`arXiv`|[UP-SLAM: Adaptively Structured Gaussian SLAM with Uncertainty Prediction in Dynamic Environments](https://arxiv.org/pdf/2505.22335)|---|[项目主页](https://aczheng-cai.github.io/up_slam.github.io/)|
|2025|`arXiv`|[DynaGSLAM: Real-Time Gaussian-Splatting SLAM for Online Rendering, Tracking, Motion Predictions of Moving Objects in Dynamic Scenes](https://arxiv.org/pdf/2503.11979)|[![GitHub 星标数](https://img.shields.io/github/stars/BlarkLee/DynaGSLAM_official.svg)](https://github.com/BlarkLee/DynaGSLAM_official)|[项目主页](https://blarklee.github.io/dynagslam/)| 
|2025|`arXiv`|[Large-Scale Gaussian Splatting SLAM](https://arxiv.org/pdf/2505.09915)|---|[项目主页](https://lsgsslam.github.io/)| 
|2025|`IEEE-SJ`|[DSOSplat: Monocular 3D Gaussian SLAM with Direct Tracking](https://ieeexplore.ieee.org/abstract/document/10994228/)|---|---|
|2025|`arXiv`|[GauS-SLAM: Dense RGB-D SLAM with Gaussian Surfels](https://arxiv.org/pdf/2505.01934)|[![GitHub 星标数](https://img.shields.io/github/stars/gaus-slam/gaus-slam.svg)](https://github.com/gaus-slam/gaus-slam)|[项目主页](https://gaus-slam.github.io/)| 
|2025|`RSS`|[GauSS-MI: Gaussian Splatting Shannon Mutual Information for Active 3D Reconstruction](https://arxiv.org/pdf/2504.21067)|[![GitHub 星标数](https://img.shields.io/github/stars/JohannaXie/GauSS-MI.svg)](https://github.com/JohannaXie/GauSS-MI)|---|
|2025|`arXiv`|[GSFF-SLAM: 3D Semantic Gaussian Splatting SLAM via Feature Field](https://arxiv.org/pdf/2504.19409)|---|---|
|2025|`arXiv`|[GSFeatLoc: Visual Localization Using Feature Correspondence on 3D Gaussian Splatting](https://arxiv.org/pdf/2504.20379)|---|---|
|2025|`CVPR`|[SmallGS: Gaussian Splatting Based Camera Pose Estimation for Small-Baseline Videos](https://arxiv.org/pdf/2504.17810)|---|[项目主页](https://yuxinyao620.github.io/SmallGS/)<br>MonST3R+3DGS| 
|2025|`arXiv`|[Enhancing Gaussian Splatting SLAM with Feature-based Tracking](https://lamor.fer.hr/images/50050805/gsslam.pdf)|---|---| 
|2025|`arXiv`|[ToF-Splatting: Dense SLAM using Sparse Time-of-Flight Depth and Multi-Frame Integration](https://arxiv.org/pdf/2504.16545)|---|---|
|2025|`RAL`|[SDD-SLAM: Semantic-Driven Dynamic SLAM with Gaussian Splatting](https://ieeexplore.ieee.org/abstract/document/10966164)|---|---| 
|2025|`IEEE Sensors Journal`|[Dynamic SLAM with 3D Gaussian Splatting Supporting Monocular Sensing](https://ieeexplore.ieee.org/abstract/document/10970383/)|---|---|
|2025|`arXiv`|[SLAM&Render: A Benchmark for the Intersection Between Neural Rendering, Gaussian Splatting and SLAM](https://arxiv.org/pdf/2504.13713)|[![GitHub 星标数](https://img.shields.io/github/stars/samuel-cerezo/SLAM-Render.svg)](https://github.com/samuel-cerezo/SLAM-Render)|[项目主页](https://samuel-cerezo.github.io/SLAM&Render)<br>数据集|
|2025|`arXiv`|[Direct Sparse Odometry with Continuous 3D Gaussian Maps for Indoor Environments](https://arxiv.org/pdf/2503.03373)|[![GitHub 星标数](https://img.shields.io/github/stars/JD-hust/gs-dso.svg)](https://github.com/JD-hust/gs-dso)|---|
|2025|`CVPR`|[MAGiC-SLAM: Multi-Agent Gaussian Globally Consistent SLAM](https://arxiv.org/pdf/2411.16785)|[![GitHub 星标数](https://img.shields.io/github/stars/VladimirYugay/MAGiC-SLAM.svg)](https://github.com/VladimirYugay/MAGiC-SLAM)|[项目主页](https://vladimiryugay.github.io/magic_slam/)|
|2025|`arXiv`|[4D Gaussian Splatting SLAM](https://arxiv.org/pdf/2503.16710)|[![GitHub 星标数](https://img.shields.io/github/stars/yanyan-li/4DGS-SLAM.svg)](https://github.com/yanyan-li/4DGS-SLAM)|[项目主页](https://yanyan-li.github.io/project/gs/4dgsslam.html)| 
|2025|`arXiv`|[GI-SLAM: Gaussian-Inertial SLAM](https://arxiv.org/pdf/2503.18275)|---|---| 
|2025|`arXiv`|[FGS-SLAM: Fourier-based Gaussian Splatting for Real-time SLAM with Sparse and Dense Map Fusion](https://arxiv.org/pdf/2503.01109)|---|---|
|2025|`ICRA`|[OpenGS-SLAM: Open-Set Dense Semantic SLAM with 3D Gaussian Splatting for Object-Level Scene Understanding](https://arxiv.org/pdf/2503.01646?)|[![GitHub 星标数](https://img.shields.io/github/stars/YOUNG-bit/open_semantic_slam.svg)](https://github.com/YOUNG-bit/open_semantic_slam)|[项目主页](https://young-bit.github.io/opengs-github.github.io/)|
|2025|`arXiv`|[VIGS SLAM: IMU-based Large-Scale 3D Gaussian Splatting SLAM](https://arxiv.org/pdf/2501.13402)|---|---|
|2025|`arXiv`|[Embracing Dynamics: Dynamics-aware 4D Gaussian Splatting SLAM](https://arxiv.org/pdf/2504.04844)|---|---|
|2025|`arXiv`|[Monogs++: Fast and accurate monocular rgb gaussian slam](https://arxiv.org/pdf/2504.02437)|---|---|
|2025|`RAL`|[RGBDS-SLAM: A RGB-D Semantic Dense SLAM Based on 3D Multi Level Pyramid Gaussian Splatting](https://arxiv.org/pdf/2412.01217)|[![GitHub 星标数](https://img.shields.io/github/stars/zhenzhongcao/RGBDS-SLAM.svg)](https://github.com/zhenzhongcao/RGBDS-SLAM)|---|
|2025|`TRO`|[VINGS-Mono: Visual-Inertial Gaussian Splatting Monocular SLAM in Large Scenes](https://arxiv.org/pdf/2501.08286)|[![GitHub 星标数](https://img.shields.io/github/stars/Fudan-MAGIC-Lab/VINGS-Mono.svg)](https://github.com/Fudan-MAGIC-Lab/VINGS-Mono)|[项目主页](https://vings-mono.github.io/)|
|2025|`CVPR`|[WildGS-SLAM: Monocular Gaussian Splatting SLAM in Dynamic Environments](https://arxiv.org/pdf/2504.03886)|[![GitHub 星标数](https://img.shields.io/github/stars/GradientSpaces/WildGS-SLAM.svg)](https://github.com/GradientSpaces/WildGS-SLAM)|[项目主页](https://wildgs-slam.github.io/)|
|2025|`arXiv`|[GARAD-SLAM: 3D GAussian splatting for Real-time Anti Dynamic SLAM](https://arxiv.org/pdf/2502.03228)|---|---|
|2025|`arXiv`|[GS-GVINS: A Tightly-integrated GNSS-Visual-Inertial Navigation System Augmented by 3D Gaussian Splatting](https://arxiv.org/pdf/2502.10975)|---|---|
|2024|`arXiv`|[FlashSLAM: Accelerated RGB-D SLAM for Real-Time 3D Scene Reconstruction with Gaussian Splatting](https://arxiv.org/pdf/2412.00682)|[![GitHub 星标数](https://img.shields.io/github/stars/flashslam/FlashSLAM.svg)](https://github.com/flashslam/FlashSLAM)|[项目主页](https://flashslam.github.io/)|
|2025|`TRO`|[PG-SLAM: Photo-realistic and Geometry-aware RGB-D SLAM in Dynamic Environments](https://arxiv.org/pdf/2411.15800)|---|---|
|2024|`ECCV`|[6dgs: 6d pose estimation from a single image and a 3d gaussian splatting model](https://arxiv.org/pdf/2407.15484)|[![GitHub 星标数](https://img.shields.io/github/stars/mbortolon97/6dgs.svg)](https://github.com/mbortolon97/6dgs)|[项目主页](https://mbortolon97.github.io/6dgs/)|
|2024|`arXiv`|[Splat-slam: Globally optimized rgb-only slam with 3d gaussians](https://arxiv.org/pdf/2405.16544)|[![GitHub 星标数](https://img.shields.io/github/stars/eriksandstroem/Splat-SLAM.svg)](https://github.com/eriksandstroem/Splat-SLAM)|---|
|2024|`arXiv`|[TAMBRIDGE: Bridging Frame-Centered Tracking and 3D Gaussian Splatting for Enhanced SLAM](https://arxiv.org/pdf/2405.19614)|[![GitHub 星标数](https://img.shields.io/github/stars/ZeldaFromHeaven/TAMBRIDGE-DAVID.svg)](https://github.com/ZeldaFromHeaven/TAMBRIDGE-DAVID)|[项目主页](https://zeldafromheaven.github.io/TAMBRIDGE/)|
|2024|`arXiv`|[HI-SLAM2: Geometry-Aware Gaussian SLAM for Fast Monocular Scene Reconstruction](https://arxiv.org/pdf/2411.17982)|[![GitHub 星标数](https://img.shields.io/github/stars/Willyzw/HI-SLAM2.svg)](https://github.com/Willyzw/HI-SLAM2)|[项目主页](https://hi-slam2.github.io/)|
|2024|`NIPS`|[DG-SLAM: Robust Dynamic Gaussian Splatting SLAM with Hybrid Pose Optimization](https://arxiv.org/pdf/2411.08373)|[![GitHub 星标数](https://img.shields.io/github/stars/fudan-zvg/DG-SLAM.svg)](https://github.com/fudan-zvg/DG-SLAM)|---|
|2025|`ICRA`|[Gassidy: Gaussian Splatting SLAM in Dynamic Environments](https://arxiv.org/pdf/2411.15476)|---|[项目主页](https://wen950223.wixsite.com/gassidy-slam-1)|
|2024|`arXiv`|[DGS-SLAM: Gaussian Splatting SLAM in Dynamic Environment](https://arxiv.org/pdf/2411.10722)|[![GitHub 星标数](https://img.shields.io/github/stars/kmk97/DGS-SLAM.svg)](https://github.com/kmk97/DGS-SLAM)|---|
|2024|`International Conference on Robotics, Control and Automation Engineering`|[Motiongs: Compact gaussian splatting slam by motion filter](https://arxiv.org/pdf/2405.11129)|---|---|
|2024|`arXiv`|[Ngm-slam: Gaussian splatting slam with radiance field submap](https://arxiv.org/pdf/2405.05702)|---|---|
|2024|`arXiv`|[Monocular gaussian slam with language extended loop closure](https://arxiv.org/pdf/2405.13748)|---|---|
|2024|`RAL`|[Mgs-slam: Monocular sparse tracking and gaussian mapping with depth smooth regularization](https://arxiv.org/pdf/2405.06241)|---|---|
|2024|`ACM SIGGRAPH`|[Rtg-slam: Real-time 3d reconstruction at scale using gaussian splatting](https://arxiv.org/pdf/2404.19706?)|[![GitHub 星标数](https://img.shields.io/github/stars/MisEty/RTG-SLAM.svg)](https://github.com/MisEty/RTG-SLAM)|[项目主页](https://gapszju.github.io/RTG-SLAM/)|
|2024|`arXiv`|[3dgs-reloc: 3d gaussian splatting for map representation and visual relocalization](https://arxiv.org/pdf/2403.11367)|---|---|
|2024|`ECCV`|[Rgbd gs-icp slam](https://arxiv.org/pdf/2403.12550)|[![GitHub 星标数](https://img.shields.io/github/stars/Lab-of-AI-and-Robotics/GS_ICP_SLAM.svg)](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM)|---|
|2024|`ECCV`|[Cg-slam: Efficient dense rgb-d slam in a consistent uncertainty-aware 3d gaussian field](https://arxiv.org/pdf/2403.16095)|[![GitHub 星标数](https://img.shields.io/github/stars/hjr37/CG-SLAM.svg)](https://github.com/hjr37/CG-SLAM)|[项目主页](https://zju3dv.github.io/cg-slam/)| 
|2024|`IROS`|[Mm3dgs slam: Multi-modal 3d gaussian splatting for slam using vision, depth, and inertial measurements](https://arxiv.org/pdf/2404.00923)|[![GitHub 星标数](https://img.shields.io/github/stars/VITA-Group/MM3DGS-SLAM.svg)](https://github.com/VITA-Group/MM3DGS-SLAM)|[项目主页](https://vita-group.github.io/MM3DGS-SLAM/)| 
|2024|`RAL`|[Neds-slam: A neural explicit dense semantic slam framework using 3d gaussian splatting](https://arxiv.org/pdf/2403.11679)|---|---|
|2024|`IROS`|[High-fidelity slam using gaussian splatting with rendering-guided densification and regularized optimization](https://arxiv.org/pdf/2403.12535)|[![GitHub 星标数](https://img.shields.io/github/stars/ljjTYJR/HF-SLAM.svg)](https://github.com/ljjTYJR/HF-SLAM)|---|
|2024|`arXiv`|[Semgauss-slam: Dense semantic gaussian splatting slam](https://arxiv.org/pdf/2403.07494)|---|---|
|2024|`ECCV`|[Sgs-slam: Semantic gaussian splatting for neural dense slam](https://arxiv.org/pdf/2402.03246)|[![GitHub 星标数](https://img.shields.io/github/stars/ShuhongLL/SGS-SLAM.svg)](https://github.com/ShuhongLL/SGS-SLAM)|---|
|2024|`CVPR`|[Photo-slam: Real-time simultaneous localization and photorealistic mapping for monocular stereo and rgb-d cameras](https://openaccess.thecvf.com/content/CVPR2024/papers/Huang_Photo-SLAM_Real-time_Simultaneous_Localization_and_Photorealistic_Mapping_for_Monocular_Stereo_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/HuajianUP/Photo-SLAM.svg)](https://github.com/HuajianUP/Photo-SLAM)|[项目主页](https://huajianup.github.io/research/Photo-SLAM/)|
|2024|`CVPR`|[Gaussian splatting slam](https://openaccess.thecvf.com/content/CVPR2024/papers/Matsuki_Gaussian_Splatting_SLAM_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/muskie82/MonoGS.svg)](https://github.com/muskie82/MonoGS)|[项目主页](https://rmurai.co.uk/projects/GaussianSplattingSLAM/)<br>MonoGS|
|2024|`CVPR`|[Splatam: Splat track & map 3d gaussians for dense rgb-d slam](https://openaccess.thecvf.com/content/CVPR2024/papers/Keetha_SplaTAM_Splat_Track__Map_3D_Gaussians_for_Dense_RGB-D_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/spla-tam/SplaTAM.svg)](https://github.com/spla-tam/SplaTAM)|[项目主页](https://spla-tam.github.io/)|
|2024|`CVPR`|[Gs-slam: Dense visual slam with 3d gaussian splatting](https://openaccess.thecvf.com/content/CVPR2024/papers/Yan_GS-SLAM_Dense_Visual_SLAM_with_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/yanchi-3dv/diff-gaussian-rasterization-for-gsslam.svg)](https://github.com/yanchi-3dv/diff-gaussian-rasterization-for-gsslam)|[项目主页](https://gs-slam.github.io/)|
|2023|`arXiv`|[Gaussian-slam: Photo-realistic dense slam with gaussian splatting](https://arxiv.org/pdf/2312.10070)|[![GitHub 星标数](https://img.shields.io/github/stars/VladimirYugay/Gaussian-SLAM.svg)](https://github.com/VladimirYugay/Gaussian-SLAM)|[项目主页](https://vladimiryugay.github.io/gaussian_slam/)|

<a name="lidar-based-3dgs"></a>

## 基于激光雷达（LiDAR）的 3DGS SLAM
<!-- |---|`arXiv`|---|---|---| -->
<!-- [![GitHub 星标数](https://img.shields.io/github/stars/***.svg)]() -->

| 年份 | 发表渠道 | 论文标题 | 代码仓库 | 备注 |
|:----:|:-----:| ----------- |:----------:|:----:|
|2026|`arXiv`|[GEMOR-GS: Global Extrinsic-calibration-refined Mapping and Online Relocalization for 3D Gaussian-Splatting SLAM](https://arxiv.org/abs/2611.13528)|---|融合激光雷达、IMU 和相机，离线标定雷达与相机外参以细化全局高斯地图，并支持跟踪丢失后的重定位。|
|2025|`RAL`|[Rad-GS: Radar-Vision Integration for 3D Gaussian Splatting SLAM in Outdoor Environments](https://arxiv.org/pdf/2511.16091)|---|首个融合 4D 雷达与视觉的 3DGS SLAM 框架，实现千米级户外稳健建图;以3D高斯作为可微空间表示，融合原始雷达点云的多普勒信息与几何增强点云，引导同步图像中的动态目标掩码生成，减少渲染伪影并提升定位精度；同时利用非同步图像帧全局优化3D高斯表示，增强纹理一致性与新视角合成保真度；通过全局八叉树结构结合目标高斯基元管理策略，抑制噪声并降低大规模环境下的内存消耗，实现了稳健的户外建图与大规模场景重建。|
|2025|`IROS`|[GS-SDF: LiDAR-Augmented Gaussian Splatting and Neural SDF for Geometrically Consistent Rendering and Reconstruction](https://arxiv.org/pdf/2503.10170?)|[![GitHub 星标数](https://img.shields.io/github/stars/hku-mars/GS-SDF.svg)](https://github.com/hku-mars/GS-SDF)|[项目主页](https://jianhengliu.github.io/Projects/GS-SDF/)|
|2025|`arXiv`|[LVD-GS: Gaussian Splatting SLAM for Dynamic Scenes via Hierarchical Explicit-Implicit Representation Collaboration Rendering](https://arxiv.org/pdf/2510.22669)|---|---|
|2025|`arXiv`|[AgriGS-SLAM: Orchard Mapping Across Seasons via Multi-View Gaussian Splatting SLAM](https://arxiv.org/pdf/2510.26358)|[![GitHub 星标数](https://img.shields.io/github/stars/AIRLab-POLIMI/agri-gs-slam.svg)](https://github.com/AIRLab-POLIMI/agri-gs-slam)|---|
|2025|`ICCV`|[GS-LIVM: Real-Time Photo-Realistic LiDAR-Inertial-Visual Mapping with Gaussian Splatting](https://arxiv.org/pdf/2410.17084)|[![GitHub 星标数](https://img.shields.io/github/stars/xieyuser/GS-LIVM.svg)](https://github.com/xieyuser/GS-LIVM)|---|
|2025|`arXiv`|[Gaussian-LIC2: LiDAR-Inertial-Camera Gaussian Splatting SLAM](https://arxiv.org/pdf/2507.04004)|[![GitHub 星标数](https://img.shields.io/github/stars/APRIL-ZJU/Gaussian-LIC.svg)](https://github.com/APRIL-ZJU/Gaussian-LIC)|[项目主页](https://xingxingzuo.github.io/gaussian_lic/)|[项目主页](https://xingxingzuo.github.io/gaussian_lic2/)|
|2025|`arXiv`|[Splat-LOAM: Gaussian Splatting LiDAR Odometry and Mapping](https://arxiv.org/pdf/2503.17491)|[![GitHub 星标数](https://img.shields.io/github/stars/rvp-group/Splat-LOAM.svg)](https://github.com/rvp-group/Splat-LOAM)|[测试](https://kwanwaipang.github.io/Splat-LOAM/)|
|2025|`arXiv`|[GS-LIVO: Real-Time LiDAR, Inertial, and Visual Multi-sensor Fused Odometry with Gaussian Mapping](https://arxiv.org/pdf/2501.08672)|[![GitHub 星标数](https://img.shields.io/github/stars/HKUST-Aerial-Robotics/GS-LIVO.svg)](https://github.com/HKUST-Aerial-Robotics/GS-LIVO) |---|
|2025|`TIM`|[LVI-GS: Tightly-coupled LiDAR-Visual-Inertial SLAM using 3D Gaussian Splatting](https://ieeexplore.ieee.org/abstract/document/10926911)|---|[项目主页](https://kwanwaipang.github.io/LVI-GS/)|
|2024|`RAL`|[LiV-GS: LiDAR-Vision Integration for 3D Gaussian Splatting SLAM in Outdoor Environments](https://arxiv.org/pdf/2411.12185)|---|---|
|2025|`ICRA`|[Gaussian-lic: Photo-realistic lidar-inertial-camera slam with 3d gaussian splatting](https://arxiv.org/pdf/2404.06926)|[![GitHub 星标数](https://img.shields.io/github/stars/APRIL-ZJU/Gaussian-LIC.svg)](https://github.com/APRIL-ZJU/Gaussian-LIC)|[项目主页](https://xingxingzuo.github.io/gaussian_lic/)|
|2024|`ECCV`|[TCLC-GS: Tightly Coupled LiDAR-Camera Gaussian Splatting for Autonomous Driving: Supplementary Materials](https://arxiv.org/pdf/2404.02410)|---|---|
|2024|`IROS`|[MM-Gaussian: 3D Gaussian-based multi-modal fusion for localization and reconstruction in unbounded scenes](https://arxiv.org/pdf/2404.04026)|---|---|
|2024|`RAL`|[LIV-GaussMap: LiDAR-inertial-visual fusion for real-time 3D radiance field map rendering](https://arxiv.org/pdf/2401.14857)|[![GitHub 星标数](https://img.shields.io/github/stars/sheng00125/LIV-GaussMap.svg)](https://github.com/sheng00125/LIV-GaussMap)|---| 
|2024|`CVPR`|[Drivinggaussian: Composite gaussian splatting for surrounding dynamic autonomous driving scenes](https://openaccess.thecvf.com/content/CVPR2024/papers/Zhou_DrivingGaussian_Composite_Gaussian_Splatting_for_Surrounding_Dynamic_Autonomous_Driving_Scenes_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/VDIGPKU/DrivingGaussian.svg)](https://github.com/VDIGPKU/DrivingGaussian)|---|

<a name="event-based-3dgs"></a>

## 基于事件相机的 3DGS SLAM
<!-- |---|`arXiv`|---|---|---| -->
<!-- [![GitHub 星标数](https://img.shields.io/github/stars/***.svg)]() -->

| 年份 | 发表渠道 | 论文标题 | 代码仓库 | 备注 |
|:----:|:-----:| ----------- |:----------:|:----:|
|2026|`ICRA`|[MotionGS-SLAM: Event-Modulated Gaussian Splatting for Motion-Blur Robust SLAM](https://ieeexplore.ieee.org/abstract/document/11695697)|---|借助事件相机提供的运动线索，在高斯渲染中显式建模曝光期间的运动模糊，并联合优化相机轨迹与场景几何。<br>[arXiv 版本](https://arxiv.org/abs/2608.15024)|
|2025|`NIPS`|[Spike4DGS: Towards High-Speed Dynamic Scene Rendering with 4D Gaussian Splatting via a Spike Camera Array](https://openreview.net/pdf?id=V5efEA8nIr)|---|---|
|2025|`Expert Systems with Applications`|[E2D-GS: Event-Enhanced Deblurring Gaussian Splatting](https://www.sciencedirect.com/science/article/abs/pii/S0957417425034177)|---|---|
|2025|`arXiv`|[Event-guided 3D Gaussian Splatting for Dynamic Human and Scene Reconstruction](https://arxiv.org/pdf/2509.18566)|---|---|
|2025|`arXiv`|[DeblurSplat: SfM-free 3D Gaussian Splatting with Event Camera for Robust Deblurring](https://arxiv.org/pdf/2509.18898)|---|DUSt3R + 事件数据 + 3DGS|
|2025|`RAl`|[EGS-SLAM: RGB-D Gaussian Splatting SLAM with Events](https://arxiv.org/pdf/2508.07003)|[![GitHub 星标数](https://img.shields.io/github/stars/Chensiyu00/EGS-SLAM.svg)](https://github.com/Chensiyu00/EGS-SLAM)|---|
|2025|`arXiv`|[E-4DGS: High-Fidelity Dynamic Reconstruction from the Multi-view Event Cameras](https://arxiv.org/pdf/2508.09912?)|---|---|
|2025|`arXiv`|[EDyGS: Event Enhanced Dynamic 3D Radiance Fields from Blurry Monocular Video](https://ijcai-preprints.s3.us-west-1.amazonaws.com/2025/1781.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/zju-bmi-lab/EDyGS.svg)](https://github.com/zju-bmi-lab/EDyGS)|---|
|2025|`CVPR`|[DiET-GS: Diffusion Prior and Event Stream-Assisted Motion Deblurring 3D Gaussian Splatting Supplementary Material](https://openaccess.thecvf.com/content/CVPR2025/papers/Lee_DiET-GS_Diffusion_Prior_and_Event_Stream-Assisted_Motion_Deblurring_3D_Gaussian_CVPR_2025_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/DiET-GS/DiET-GS.svg)](https://github.com/DiET-GS/DiET-GS)|[项目主页](https://diet-gs.github.io/)|
|2025|`arXiv`|[GS2E: Gaussian Splatting is an Effective Data Generator for Event Stream Generation](https://arxiv.org/pdf/2505.15287)|[![GitHub 星标数](https://img.shields.io/github/stars/PKU-YuanGroup/GS2E.svg)](https://github.com/PKU-YuanGroup/GS2E) |[项目主页](https://intothemild.github.io/GS2E.github.io/)|
|2025|`arXiv`|[EBAD-Gaussian: Event-driven Bundle Adjusted Deblur Gaussian Splatting](https://arxiv.org/pdf/2504.10012)|---|---|
|2025|`AAAI`|[SpikeGS: Reconstruct 3D Scene Captured by a Fast-Moving Bio-Inspired Camera](https://ojs.aaai.org/index.php/AAAI/article/view/32340/34495)|[![GitHub 星标数](https://img.shields.io/github/stars/yijiaguo02/SpikeGS.svg)](https://github.com/yijiaguo02/SpikeGS)|[项目主页](https://spikegs.github.io/)|
|2025|`AAAI`|[EvHDR-GS: Event-guided HDR Video Reconstruction with 3D Gaussian Splatting](https://ojs.aaai.org/index.php/AAAI/article/view/32237/34392)|---|---|
|2025|`3DV`|[E-3DGS: Event-based Novel View Rendering of Large-scale Scenes Using 3D Gaussian Splatting](https://arxiv.org/pdf/2502.10827)|[![GitHub 星标数](https://img.shields.io/github/stars/sohaib023/E-3DGS.svg)](https://github.com/sohaib023/E-3DGS)|[项目主页](https://4dqv.mpi-inf.mpg.de/E3DGS/)<br>[测试](https://kwanwaipang.github.io/E-3DGS/)|
|2024|`NeurIPS`|[Event-3DGS: Event-based 3D Reconstruction Using 3D Gaussian Splatting](https://proceedings.neurips.cc/paper_files/paper/2024/hash/e73ad1f690542144ce354637bb913c35-Abstract-Conference.html)|[![GitHub 星标数](https://img.shields.io/github/stars/lanpokn/Event-3DGS.svg)](https://github.com/lanpokn/Event-3DGS)|在已知相机位姿下，用事件流监督 3D 高斯重建并合成新视角。通过高通滤波估计光电压变化，联合优化高斯场景与事件触发阈值。|
|2024|`arXiv`|[IncEventGS: Pose-Free Gaussian Splatting from a Single Event Camera](https://arxiv.org/pdf/2410.08107)|[![GitHub 星标数](https://img.shields.io/github/stars/WU-CVGL/IncEventGS.svg)](https://github.com/WU-CVGL/IncEventGS)|---|
|2024|`arXiv`|[EventSplat: 3D Gaussian Splatting from Moving Event Cameras for Real-time Rendering](https://arxiv.org/pdf/2412.07293)|---|---|
|2024|`Asia Pacific Signal and Information Processing Association Annual Summit and Conference`|[Ev3DGS: Event Enhanced 3D Gaussian Splatting from Blurry Images](http://www.apsipa2024.org/files/papers/253.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/npucvr/Ev3DGS.svg)](https://github.com/npucvr/Ev3DGS)|---|
|2024|`IEEE International Conference on Image Processing`|[E2gs: Event enhanced gaussian splatting](https://arxiv.org/pdf/2406.14978)|[![GitHub 星标数](https://img.shields.io/github/stars/deguchihiroyuki/E2GS.svg)](https://github.com/deguchihiroyuki/E2GS)|---|
|2024|`arXiv`|[Evagaussians: Event stream assisted gaussian splatting from blurry images](https://arxiv.org/pdf/2405.20224)|[![GitHub 星标数](https://img.shields.io/github/stars/PKU-YuanGroup/EvaGaussians.svg)](https://github.com/PKU-YuanGroup/EvaGaussians)|[项目主页](https://www.falcary.com/EvaGaussians/)| 
|2024|`CoRL`|[Event3dgs: Event-based 3d gaussian splatting for fast egomotion](https://arxiv.org/pdf/2406.02972)|[![GitHub 星标数](https://img.shields.io/github/stars/jayhsu0627/Event3DGS.svg)](https://github.com/jayhsu0627/Event3DGS)|[项目主页](https://tyxiong23.github.io/event3dgs)|
|2024|`ICML`|[Evggs: A collaborative learning framework for event-based generalizable gaussian splatting](https://arxiv.org/pdf/2405.14959)|[![GitHub 星标数](https://img.shields.io/github/stars/Mercerai/EvGGS.svg)](https://github.com/Mercerai/EvGGS)|---| 




<a name="other-resources"></a>

## 其他资源
* [MrNeRF 的 3DGS 资源清单](https://github.com/MrNeRF/awesome-3D-gaussian-splatting)
* [将三维网格转换为 3D 高斯表示](https://github.com/electronicarts/mesh2splat)
* 足式机器人 SLAM 调研 [论文清单](https://github.com/KwanWaiPang/Awesome-Legged-Robot-Localization-and-Mapping)
* 基于学习的 VO、VIO、IO 调研 [论文清单](https://github.com/KwanWaiPang/Awesome-Learning-based-VO-VIO)
* 基于 Transformer 的 SLAM 调研 [论文清单](https://github.com/KwanWaiPang/Awesome-Transformer-based-SLAM)
* 基于扩散模型的 SLAM 调研 [论文清单](https://github.com/KwanWaiPang/Awesome-Diffusion-based-SLAM)
* 基于 NeRF 的 SLAM 调研 [博客](https://blog.csdn.net/gwplovekimi/article/details/135083274)
* 基于深度学习的 IMU 零偏估计调研 [博客](https://kwanwaipang.github.io/Deep-IMU-Bias/)
* LiDAR SLAM 退化问题论文调研 [博客](https://kwanwaipang.github.io/Lidar_Degeneracy/)
* 动态环境 SLAM 论文调研 [博客](https://kwanwaipang.github.io/Dynamic-SLAM/)
* LOAM 系列算法复现与学习 [博客](https://blog.csdn.net/gwplovekimi/article/details/119711762?spm=1001.2014.3001.5502)
* 基于几何着色器、使用 CUDA 进行全局排序的高性能 3D 高斯光栅化器。相比原版 `diff-gaussian-rasterization`，渲染速度可达到其 5–10 倍。 [fast-gaussian-rasterization](https://github.com/dendenxu/fast-gaussian-rasterization)

### 其他相关论文
<!-- |---|`arXiv`|---|---|---| -->
<!-- [![GitHub 星标数](https://img.shields.io/github/stars/***.svg)]() -->

| 年份 | 发表渠道 | 论文标题 | 代码仓库 | 备注 |
|:----:|:-----:| ----------- |:----------:|:----:|
|2026|`arXiv`|[Towards Next-Generation SLAM: A Survey on 3DGS-SLAM Focusing on Performance, Robustness, and Future Directions](https://arxiv.org/pdf/2602.04251)|---|---|
|2025|`arXiv`|[Revisiting Depth Representations for Feed-Forward 3D Gaussian Splatting](https://arxiv.org/pdf/2506.05327)|[![GitHub 星标数](https://img.shields.io/github/stars/aim-uofa/PM-Loss.svg)](https://github.com/aim-uofa/PM-Loss)|[项目主页](https://aim-uofa.github.io/PMLoss/)|
|2025|`arXiv`|[Voyager: Real-Time Splatting City-Scale 3D Gaussians on Your Phone](https://arxiv.org/pdf/2506.02774)|---|[项目主页](https://voyager-web.netlify.app/)|
|2025|`arXiv`|[R3GS: Gaussian Splatting for Robust Reconstruction and Relocalization in Unconstrained Image Collections](https://arxiv.org/pdf/2505.15294)|---|---|
|2025|`arXiv`|[Recollection from Pensieve: Novel View Synthesis via Learning from Uncalibrated Videos](https://arxiv.org/pdf/2505.13440)|[![GitHub 星标数](https://img.shields.io/github/stars/Dwawayu/Pensieve.svg)](https://github.com/Dwawayu/Pensieve)|---|
|2025|`arXiv`|[STORM: Spatio-Temporal Reconstruction Model for Large-Scale Outdoor Scenes](https://arxiv.org/pdf/2501.00602)| [![GitHub 星标数](https://img.shields.io/github/stars/NVlabs/GaussianSTORM.svg)](https://github.com/NVlabs/GaussianSTORM)|[项目主页](https://jiawei-yang.github.io/STORM/)|
|2025|`SIGGRAPH `|[Monocular Online Reconstruction with Enhanced Detail Preservation](https://arxiv.org/pdf/2505.07887)|---|[项目主页](https://poiw.github.io/MODP/)| 
|2025|`arXiv`|[Sparse2DGS: Geometry-Prioritized Gaussian Splatting for Surface Reconstruction from Sparse Views](https://arxiv.org/pdf/2504.20378)|[![GitHub 星标数](https://img.shields.io/github/stars/Wuuu3511/Sparse2DGS.svg)](https://github.com/Wuuu3511/Sparse2DGS)|---| 
|2025|`CVPR`|[ODHSR: Online Dense 3D Reconstruction of Humans and Scenes from Monocular Videos](https://arxiv.org/pdf/2504.13167)|[![GitHub 星标数](https://img.shields.io/github/stars/eth-ait/ODHSR.svg)](https://github.com/eth-ait/ODHSR)|[项目主页](https://eth-ait.github.io/ODHSR/)|
|2025|`arXiv`|[You Need a Transition Plane: Bridging Continuous Panoramic 3D Reconstruction with Perspective Gaussian Splatting](https://arxiv.org/pdf/2504.09062)|[![GitHub 星标数](https://img.shields.io/github/stars/zhijieshen-bjtu/TPGS.svg)](https://github.com/zhijieshen-bjtu/TPGS)|---|
|2024|`arXiv`|[GaussianSpa: An" Optimizing-Sparsifying" Simplification Framework for Compact and High-Quality 3D Gaussian Splatting](https://arxiv.org/pdf/2411.06019)|[![GitHub 星标数](https://img.shields.io/github/stars/noodle-lab/GaussianSpa.svg)](https://github.com/noodle-lab/GaussianSpa)|[项目主页](https://noodle-lab.github.io/gaussianspa/)|
|2024|`ACM International Conference on Multimedia`|[Spikegs: 3d gaussian splatting from spike streams with high-speed camera motion](https://arxiv.org/pdf/2407.10062)|---|---|
|2024|`ICLR`|[Real-time photorealistic dynamic scene representation and rendering with 4d gaussian splatting](https://arxiv.org/pdf/2310.10642)|[![GitHub 星标数](https://img.shields.io/github/stars/fudan-zvg/4d-gaussian-splatting.svg)](https://github.com/fudan-zvg/4d-gaussian-splatting)|4DGS|
|2024|`ACM SIGGRAPH`|[2d gaussian splatting for geometrically accurate radiance fields](https://dl.acm.org/doi/pdf/10.1145/3641519.3657428)|[![GitHub 星标数](https://img.shields.io/github/stars/hbb1/2d-gaussian-splatting.svg)](https://github.com/hbb1/2d-gaussian-splatting)|[项目主页](https://surfsplatting.github.io/)<br>2DGS|
|2024|`CVPR`|[Dngaussian: Optimizing sparse-view 3d gaussian radiance fields with global-local depth normalization](https://openaccess.thecvf.com/content/CVPR2024/papers/Li_DNGaussian_Optimizing_Sparse-View_3D_Gaussian_Radiance_Fields_with_Global-Local_Depth_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/Fictionarry/DNGaussian.svg)](https://github.com/Fictionarry/DNGaussian)|---| 
|2024|`RAL`|[HGS-mapping: Online dense mapping using hybrid Gaussian representation in urban scenes](https://arxiv.org/pdf/2403.20159)|---|---|
|2024|`arXiv`|[Compact 3d gaussian splatting for dense visual slam](https://arxiv.org/pdf/2403.11247)|[![GitHub 星标数](https://img.shields.io/github/stars/dtc111111/Compact_GSSLAM.svg)](https://github.com/dtc111111/Compact_GSSLAM)|---|
|2024|`CVPR`|[4d gaussian splatting for real-time dynamic scene rendering](https://openaccess.thecvf.com/content/CVPR2024/papers/Wu_4D_Gaussian_Splatting_for_Real-Time_Dynamic_Scene_Rendering_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/hustvl/4DGaussians.svg)](https://github.com/hustvl/4DGaussians)|[项目主页](https://guanjunwu.github.io/4dgs/)<br>4DGS|
|2023|`ACM Transactions on Graphics`|[3d gaussian splatting for real-time radiance field rendering](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/graphdeco-inria/gaussian-splatting.svg)](https://github.com/graphdeco-inria/gaussian-splatting)|[项目主页](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)|

<!-- |---|`arXiv`|---|---|---| -->
<!-- [![GitHub 星标数](https://img.shields.io/github/stars/***.svg)]() -->
  



