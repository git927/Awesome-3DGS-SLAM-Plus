# Awesome Event 3DGS · 事件相机中文论文索引

面向中文社区，持续整理事件相机与三维高斯泼溅（3D Gaussian Splatting，3DGS）相关论文和开源实现。重点关注位姿估计与 SLAM、三维重建与新视角合成，以及事件辅助去模糊、HDR 成像和动态场景建模。

代码栏的「无」表示暂未核实到公开的官方 GitHub 仓库。点击星标可打开相应仓库，代码发布状态以仓库说明为准。

- [事件相机论文](#event-based-3dgs)
- [跨方向核心参考](#core-references)
- [来源与贡献](#来源与贡献)

<a name="event-based-3dgs"></a>

## 事件相机论文

主表按发表年份排列，同时收录少量使用脉冲相机的相关研究。

| 年份 | 发表渠道 | 论文标题 | 代码仓库 | 备注 |
| :---: | :---: | --- | :---: | --- |
|2026|`ICRA`|[MotionGS-SLAM: Event-Modulated Gaussian Splatting for Motion-Blur Robust SLAM](https://ieeexplore.ieee.org/abstract/document/11695697)|无|借助事件相机提供的运动线索，在高斯渲染中显式建模曝光期间的运动模糊，并联合优化相机轨迹与场景几何。<br>[arXiv 版本](https://arxiv.org/abs/2608.15024)|
|2025|`NeurIPS`|[Spike4DGS: Towards High-Speed Dynamic Scene Rendering with 4D Gaussian Splatting via a Spike Camera Array](https://papers.neurips.cc/paper_files/paper/2025/hash/2985b700b5187b252d2f863bf43fbe32-Abstract-Conference.html)|[![GitHub 星标数](https://img.shields.io/github/stars/Qinghongye/Spike4DGS.svg)](https://github.com/Qinghongye/Spike4DGS)|使用脉冲相机阵列研究高速动态场景的 4D 高斯渲染。|
|2025|`Expert Systems with Applications`|[E2D-GS: Event-Enhanced Deblurring Gaussian Splatting](https://www.sciencedirect.com/science/article/abs/pii/S0957417425034177)|无|---|
|2025|`arXiv`|[Event-guided 3D Gaussian Splatting for Dynamic Human and Scene Reconstruction](https://arxiv.org/pdf/2509.18566)|无|---|
|2025|`arXiv`|[DeblurSplat: SfM-free 3D Gaussian Splatting with Event Camera for Robust Deblurring](https://arxiv.org/pdf/2509.18898)|无|DUSt3R + 事件数据 + 3DGS|
|2025|`RA-L`|[EGS-SLAM: RGB-D Gaussian Splatting SLAM with Events](https://arxiv.org/pdf/2508.07003)|[![GitHub 星标数](https://img.shields.io/github/stars/Chensiyu00/EGS-SLAM.svg)](https://github.com/Chensiyu00/EGS-SLAM)|融合事件流与 RGB-D，改善运动模糊场景下的跟踪与建图。|
|2025|`arXiv`|[E-4DGS: High-Fidelity Dynamic Reconstruction from the Multi-view Event Cameras](https://arxiv.org/pdf/2508.09912?)|[![GitHub 星标数](https://img.shields.io/github/stars/SuperFCR/E-4DGS.svg)](https://github.com/SuperFCR/E-4DGS)|---|
|2025|`IJCAI`|[EDyGS: Event Enhanced Dynamic 3D Radiance Fields from Blurry Monocular Video](https://www.ijcai.org/proceedings/2025/188)|[![GitHub 星标数](https://img.shields.io/github/stars/zju-bmi-lab/EDyGS.svg)](https://github.com/zju-bmi-lab/EDyGS)|---|
|2025|`CVPR`|[DiET-GS: Diffusion Prior and Event Stream-Assisted Motion Deblurring 3D Gaussian Splatting](https://openaccess.thecvf.com/content/CVPR2025/html/Lee_DiET-GS_Diffusion_Prior_and_Event_Stream-Assisted_Motion_Deblurring_3D_Gaussian_Splatting_CVPR_2025_paper.html)|[![GitHub 星标数](https://img.shields.io/github/stars/DiET-GS/DiET-GS.svg)](https://github.com/DiET-GS/DiET-GS)|从模糊 RGB 帧与同步事件流重建清晰场景，结合扩散先验改善细节。<br>[项目主页](https://diet-gs.github.io/)|
|2025|`arXiv`|[GS2E: Gaussian Splatting is an Effective Data Generator for Event Stream Generation](https://arxiv.org/pdf/2505.15287)|[![GitHub 星标数](https://img.shields.io/github/stars/PKU-YuanGroup/GS2E.svg)](https://github.com/PKU-YuanGroup/GS2E)|[项目主页](https://intothemild.github.io/GS2E.github.io/)|
|2025|`arXiv`|[EBAD-Gaussian: Event-driven Bundle Adjusted Deblur Gaussian Splatting](https://arxiv.org/pdf/2504.10012)|无|---|
|2025|`AAAI`|[SpikeGS: Reconstruct 3D Scene Captured by a Fast-Moving Bio-Inspired Camera](https://ojs.aaai.org/index.php/AAAI/article/view/32340/34495)|[![GitHub 星标数](https://img.shields.io/github/stars/insightlab-CG-3DV/SpikeGS.svg)](https://github.com/insightlab-CG-3DV/SpikeGS)|[项目主页](https://spikegs.github.io/)|
|2025|`AAAI`|[EvHDR-GS: Event-guided HDR Video Reconstruction with 3D Gaussian Splatting](https://ojs.aaai.org/index.php/AAAI/article/view/32237/34392)|[![GitHub 星标数](https://img.shields.io/github/stars/Zehaoc/EvHDR-GS.svg)](https://github.com/Zehaoc/EvHDR-GS)|---|
|2025|`3DV`|[E-3DGS: Event-based Novel View Rendering of Large-scale Scenes Using 3D Gaussian Splatting](https://arxiv.org/pdf/2502.10827)|[![GitHub 星标数](https://img.shields.io/github/stars/sohaib023/E-3DGS.svg)](https://github.com/sohaib023/E-3DGS)|[项目主页](https://4dqv.mpi-inf.mpg.de/E3DGS/)<br>[测试](https://kwanwaipang.github.io/E-3DGS/)|
|2025|`CVPR`|[IncEventGS: Pose-Free Gaussian Splatting from a Single Event Camera](https://openaccess.thecvf.com/content/CVPR2025/papers/Huang_IncEventGS_Pose-Free_Gaussian_Splatting_from_a_Single_Event_Camera_CVPR_2025_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/WU-CVGL/IncEventGS.svg)](https://github.com/WU-CVGL/IncEventGS)|从单个事件相机增量估计轨迹并优化三维高斯地图。<br>[arXiv 版本](https://arxiv.org/abs/2410.08107)|
|2025|`CVPR`|[EventSplat: 3D Gaussian Splatting from Moving Event Cameras for Real-time Rendering](https://openaccess.thecvf.com/content/CVPR2025/html/Yura_EventSplat_3D_Gaussian_Splatting_from_Moving_Event_Cameras_for_Real-time_CVPR_2025_paper.html)|无|用移动事件相机采集的事件流进行三维高斯建模与实时新视角渲染。<br>[arXiv 版本](https://arxiv.org/abs/2412.07293)|
|2024|`NeurIPS`|[Event-3DGS: Event-based 3D Reconstruction Using 3D Gaussian Splatting](https://proceedings.neurips.cc/paper_files/paper/2024/hash/e73ad1f690542144ce354637bb913c35-Abstract-Conference.html)|[![GitHub 星标数](https://img.shields.io/github/stars/lanpokn/Event-3DGS.svg)](https://github.com/lanpokn/Event-3DGS)|在已知相机位姿下，用事件流监督 3D 高斯重建并合成新视角。通过高通滤波估计光电压变化，联合优化高斯场景与事件触发阈值。|
|2024|`Asia Pacific Signal and Information Processing Association Annual Summit and Conference`|[Ev3DGS: Event Enhanced 3D Gaussian Splatting from Blurry Images](http://www.apsipa2024.org/files/papers/253.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/npucvr/Ev3DGS.svg)](https://github.com/npucvr/Ev3DGS)|---|
|2024|`IEEE International Conference on Image Processing`|[E2gs: Event enhanced gaussian splatting](https://arxiv.org/pdf/2406.14978)|[![GitHub 星标数](https://img.shields.io/github/stars/deguchihiroyuki/E2GS.svg)](https://github.com/deguchihiroyuki/E2GS)|---|
|2024|`arXiv`|[Evagaussians: Event stream assisted gaussian splatting from blurry images](https://arxiv.org/pdf/2405.20224)|[![GitHub 星标数](https://img.shields.io/github/stars/PKU-YuanGroup/EvaGaussians.svg)](https://github.com/PKU-YuanGroup/EvaGaussians)|[项目主页](https://www.falcary.com/EvaGaussians/)| 
|2024|`CoRL`|[Event3dgs: Event-based 3d gaussian splatting for fast egomotion](https://arxiv.org/pdf/2406.02972)|[![GitHub 星标数](https://img.shields.io/github/stars/jayhsu0627/Event3DGS.svg)](https://github.com/jayhsu0627/Event3DGS)|[项目主页](https://tyxiong23.github.io/event3dgs)|
|2024|`ICML`|[Evggs: A collaborative learning framework for event-based generalizable gaussian splatting](https://arxiv.org/pdf/2405.14959)|[![GitHub 星标数](https://img.shields.io/github/stars/Mercerai/EvGGS.svg)](https://github.com/Mercerai/EvGGS)|---| 

<a name="core-references"></a>

## 跨方向核心参考

保留 3DGS 基础方法、图像 SLAM 和 LiDAR 融合的代表性工作，供选取基线与横向对照。

| 方向 | 年份 | 发表渠道 | 论文标题 | 代码仓库 | 参考用途 |
| --- | :---: | :---: | --- | :---: | --- |
|基础方法|2023|`ACM Transactions on Graphics`|[3D Gaussian Splatting for Real-Time Radiance Field Rendering](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/graphdeco-inria/gaussian-splatting.svg)](https://github.com/graphdeco-inria/gaussian-splatting)|原版 3DGS。用于理解高斯表示、可微渲染与密度控制。|
|基础方法|2024|`ACM SIGGRAPH`|[2D Gaussian Splatting for Geometrically Accurate Radiance Fields](https://dl.acm.org/doi/pdf/10.1145/3641519.3657428)|[![GitHub 星标数](https://img.shields.io/github/stars/hbb1/2d-gaussian-splatting.svg)](https://github.com/hbb1/2d-gaussian-splatting)|以二维高斯面元表达表面，可作为注重几何精度的重建基线。|
|图像 SLAM|2024|`CVPR`|[Gaussian Splatting SLAM（MonoGS）](https://openaccess.thecvf.com/content/CVPR2024/papers/Matsuki_Gaussian_Splatting_SLAM_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/muskie82/MonoGS.svg)](https://github.com/muskie82/MonoGS)|用高斯地图同时支持相机跟踪与建图，可作为单目视觉基线。|
|图像 SLAM|2024|`CVPR`|[SplaTAM: Splat, Track & Map 3D Gaussians for Dense RGB-D SLAM](https://openaccess.thecvf.com/content/CVPR2024/papers/Keetha_SplaTAM_Splat_Track__Map_3D_Gaussians_for_Dense_RGB-D_CVPR_2024_paper.pdf)|[![GitHub 星标数](https://img.shields.io/github/stars/spla-tam/SplaTAM.svg)](https://github.com/spla-tam/SplaTAM)|RGB-D 稠密跟踪与建图基线，可用于对照融合事件输入的效果。|
|图像 SLAM|2024|`ECCV`|[RGBD GS-ICP SLAM](https://arxiv.org/pdf/2403.12550)|[![GitHub 星标数](https://img.shields.io/github/stars/Lab-of-AI-and-Robotics/GS_ICP_SLAM.svg)](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM)|结合几何配准与高斯建图，可作为快速 RGB-D SLAM 参考。|
|LiDAR 融合|2025|`arXiv`|[Gaussian-LIC2: LiDAR-Inertial-Camera Gaussian Splatting SLAM](https://arxiv.org/pdf/2507.04004)|[![GitHub 星标数](https://img.shields.io/github/stars/APRIL-ZJU/Gaussian-LIC.svg)](https://github.com/APRIL-ZJU/Gaussian-LIC)|相机、激光雷达和惯性数据紧耦合，用于对照多传感器定位和建图。|
|LiDAR 融合|2025|`arXiv`|[GS-LIVO: Real-Time LiDAR, Inertial, and Visual Multi-sensor Fused Odometry with Gaussian Mapping](https://arxiv.org/pdf/2501.08672)|[![GitHub 星标数](https://img.shields.io/github/stars/HKUST-Aerial-Robotics/GS-LIVO.svg)](https://github.com/HKUST-Aerial-Robotics/GS-LIVO)|融合激光雷达、IMU 和图像进行里程计估计与高斯建图。|

## 来源与贡献

本索引基于 [KwanWaiPang/Awesome-3DGS-SLAM](https://github.com/KwanWaiPang/Awesome-3DGS-SLAM) 整理。欢迎通过拉取请求（PR）补充事件相机方向的论文、官方代码与中文研读备注。
