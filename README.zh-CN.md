<div align="center">

# 🎥 Awesome Egocentric Vision

<p align="center">
  <img src="banner.png" alt="Awesome Egocentric Vision" width="100%">
</p>

<p align="center">
  <img src="QRcode.png" alt="Awesome Egocentric Vision" width="100%">
</p>
</div>

[![中文](https://img.shields.io/badge/语言-中文-red)](README.zh-CN.md)
[![English](https://img.shields.io/badge/Language-English-blue)](README.md)

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](LICENSE)

> 一个精选的、适合学习的第一人称视觉与具身 AI 资源列表：包含论文、数据集、代码、模型、工具包、挑战赛和教程，涵盖经典基础工作和前沿进展，适合研究入门和工业部署。

✅ **收录标准**

+ 优先收录来自 CVPR / ICCV / ECCV / NeurIPS / ICLR / AAAI / TPAMI / TVCG 等顶级会议和期刊的高质量工作
+ 覆盖核心前沿方向：Ego‑VLM/LLM、Ego‑VLA 具身智能、3D/4D 重建、手物交互、视线估计、长视频理解、世界模型

---

## 📑 目录
1. [📚 综述与概述](#-综述与概述)
2. [🔬 核心研究主题](#-核心研究主题)
    - 2.1 动作识别、检测与预测
    - 2.2 手物交互与细粒度活动
    - 2.3 第一人称视觉‑语言模型与多模态推理
    - 2.4 长视频理解与结构化推理
    - 2.5 注视、注意力与意图预测
    - 2.6 3D/4D 重建与结构化感知
    - 2.7 具身智能与视觉‑语言‑行动 (Ego‑VLA)
    - 2.8 第一人称世界模型
    - 2.9 第一人称程序化 AI 助手
    - 2.10 第一人称数据安全与隐私保护
3. [📊 数据集、基准与模拟器](#-数据集基准与模拟器)
4. [👓 智能眼镜专属研究与部署](#-智能眼镜专属研究与部署)
5. [🔗 相关 Awesome 列表](#-相关-awesome-列表)
6. [🎯 关键研究挑战](#-关键研究挑战)

---

## 📚 综述与概述
入门首选材料，帮助快速建立全局认知，梳理发展脉络、核心任务和关键挑战。

+  **Challenges and Trends in Egocentric Vision: A Survey**
    - 发表：arXiv 2025 (v1: 2025年3月, v2: 2025年4月)
    - 亮点：该领域最新的全景综述，系统分类了四个主要任务方向：主体理解、客体理解、环境理解和混合理解，全面总结了挑战和趋势
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.15275)
+  **Building Egocentric Procedural AI Assistant: Methods, Benchmarks, and Challenges**
    - 发表：arXiv 2025
    - 亮点：首次系统性地提出了第一人称程序化 AI 助手的完整技术框架，定义了错误检测、程序化学习和视觉问答三项核心任务，以及实时流处理和主动交互两个支撑维度
    - 论文链接：[arXiv](https://arxiv.org/abs/2511.13261)
+  **Bridging Perspectives: A Survey on Cross-view Collaborative Intelligence with Egocentric-Exocentric Vision**
    - 发表：arXiv 2025
    - 亮点：系统梳理了第一人称‑第三人称协同学习方向，涵盖第三人称辅助第一人称、第一人称辅助第三人称以及联合学习三种范式
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.06253)
+ **An Outlook into the Future of Egocentric Vision**
    - 发表：IJCV 2024
    - 亮点：由该领域权威学者合著，结合可穿戴计算的未来场景，梳理了研究不足和待突破的方向
    - 论文链接：[arXiv](https://arxiv.org/abs/2308.07123)
+ **First-Person Vision**
    - 发表：Proceedings of the IEEE 2012
    - 亮点：该领域的基础性综述，首次正式定义了第一人称视觉的研究范围、核心挑战和应用方向
    - 论文链接：[IEEE Xplore](https://ieeexplore.ieee.org/document/6232429)

---

## 🔬 核心研究主题

### 2.1 动作识别、检测与预测
第一人称视觉中最基础且最成熟的方向，研究从第一人称视角识别、检测和预测人类动作。

#### 动作识别与检测
+  **Divide, Deliberate, Decide: A Multi-Agent Framework for Fine-Grained Egocentric Action Recognition**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：一个完全本地化的零样本多智能体框架，其中 VLM 专家通过结构化商议和同行咨询进行协作，提升了零样本动作识别性能
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.17627)
+  **From Frames to Temporal Graphs: In-Context Egocentric Action Recognition with Vision-Language Models**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：提出将视频转换为时序动作图，配合多阶段提示流水线，在 11 个 2B 到 235B 参数的开源 VLM 上实现高效的情景内少样本学习
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.15417)
+  **Cross-Modal Action Recognition in Egocentric Video Using Mamba: Integrating RGB and Hand Skeleton Streams via CLS Token Fusion Strategies**
    - 发表：EgoVis@CVPR 2026 (arXiv 2026年5月)
    - 亮点：基于 Mamba 框架的跨模态架构，融合 RGB 视频和时序手部骨架数据，并提出了四种 CLS token 融合策略
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.24302)
+  **EgoAction: Egocentric Action Composition with Reliability-Aware Temporal Fusion**
    - 发表：CVPR 2026 (EPIC‑KITCHENS 挑战赛冠军方案)
    - 亮点：提出解耦的动词‑名词检测 + 动态加权融合策略，基于 VideoMAE‑L 特征在长未修剪视频上达到 SOTA 准确率
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.24496)
+  **ENIGMA-360: An Ego-Exo Dataset for Human Behavior Understanding in Industrial Scenarios**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：为三个基础任务（时序动作分割、关键步骤识别和第一人称手物交互检测）提供了基线实验
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.14327)
+  **Ego4OOD: Rethinking Egocentric Video Domain Generalization via Covariate Shift Scoring**
    - 发表：arXiv 2026 (2026年1月)
    - 亮点：提出了 Ego4OOD 域泛化基准，包含 8 个地理上不同的域，并引入了一种基于聚类的协变量偏移度量
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.17056)
+  **Continual Multimodal Egocentric Activity Recognition via Modality-Aware Novelty Detection**
    - 发表：arXiv 2026
    - 亮点：提出了 MAND 模态感知框架，将新颖活动检测的 AUC 提升了 10%
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.16970)
+  **Ego-METAS: Egocentric online Multimodal Energy-efficient Temporal Action Segmentation benchmark**
    - 发表：arXiv 2026
    - 亮点：首个面向能量感知的在线多模态时序动作分割基准，包含 100+ 小时的未修剪视频，覆盖 5 种模态
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.02246)
+  **MM-CDFSL: Multimodal Cross-Domain Few-Shot Learning for Egocentric Action Recognition**
    - 发表：ECCV 2024
    - 亮点：首次系统研究了第一人称动作识别的跨域少样本场景，提出了多模态蒸馏框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2405.19917)
+ **Ego-Only: Egocentric Action Detection without Exocentric Transferring**
    - 发表：ICCV 2023
    - 亮点：首次证明仅使用第一人称数据训练的模型可以超越依赖第三人称迁移的方法
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Ego-Only_Egocentric_Action_Detection_without_Exocentric_Transferring_ICCV_2023_paper.html)

#### 动作预测
+  **INSIGHT: Intention-Guided Cognitive Reasoning for Egocentric Long-Term Action Anticipation**
    - 发表：AAAI 2026
    - 亮点：提出了“HOI 语义识别 + 意图推理”的两阶段框架用于长期动作预测
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.01742)
+  **PALM: Predicting Actions through Language Models**
    - 发表：arXiv 2023
    - 亮点：首次将大语言模型引入长期时序动作预测
    - 论文链接：[arXiv](https://arxiv.org/abs/2311.17944)
+  **GANO: Gaze-Augmented Next Active Object-Based Egocentric Action Anticipation**
    - 发表：arXiv 2023
    - 亮点：针对下一个主动对象预测任务，提出了视线引导的注意力机制
    - 论文链接：[arXiv](https://arxiv.org/abs/2305.12953)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| EgoScale | 2026 | 2万+ 小时标注操作 | 动作识别、灵巧迁移 | [arXiv](https://arxiv.org/abs/2602.16710) |
| Ego-METAS | 2026 | 100+ 小时 / 5 种模态 | 在线动作分割、传感器路由 | [Hugging Face](https://huggingface.co/datasets/Ego-METAS/Ego-METAS) |
| ChildLens | 2026 | 108.58 小时 / 354 个视频 | 儿童日常活动分析 | [Data](https://doi.org/10.17617/4.fe) |
| CogDrive (EyeCue) | 2026 | 多场景驾驶 | 驾驶员认知分心检测 | [arXiv](https://arxiv.org/abs/2605.07859) |
| Furhat Egocentric Dataset | 2026 | 20 个序列 / ~25 分钟 | 机器人‑自我人脸/身体跟踪 | [arXiv](https://arxiv.org/abs/2606.03694) |
| World In Your Hands | 2025 | 1000+ 小时标注操作 | 动作识别、VLA 训练 | [GitHub](https://github.com/tars-robotics/World-In-Your-Hands) |
| EgoCampus | 2025 | ~32 小时 | 注视、行人第一人称 | [GitHub](https://github.com/ComputerVisionRutgers/EgoCampus) |
| AEA | 2024 | 143 序列 / ~7.3 小时 | 日常活动 (Aria) | [Project Aria](https://www.projectaria.com/datasets/aea/) |
| EgoSurgery | 2024 | 开放手术视频 | 手术阶段、工具检测 | [GitHub](https://github.com/Fujiry0/EgoSurgery) |
| EgoExo-Fitness | 2024 | 32 小时 / 1,276 序列 | 全身运动、质量评估 | [GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness) |
| E³ (Exploring Embodied Emotion) | 2024 | 50+ 小时 | 情感识别、多模态 | [GitHub](https://github.com/Exploring-Embodied-Emotion-official/E3) |
| ⭐ Ego4D | 2022 | ~3,670 小时 | 动作识别、VQA、预测等 | [官方网站](https://ego4d-data.org/) |
| ⭐ EPIC-KITCHENS-100 | 2021 | 100 小时 / 9万 个片段 | 动作识别、检测、预测 | [官方网站](https://epic-kitchens.github.io/) |
| EGOFALLS | 2023 | 跌倒样本 | 跌倒检测 | [Dataverse](https://www.dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/HO5GE3) |
| Epic-Sounding-Object | 2023 | 3.2K 短视频片段 | 音视频目标定位 | [GitHub](https://github.com/WikiChao/Ego-AV-Loc) |
| HoloAssist | 2023 | 169 小时 | 交互式助手 | [官方网站](https://holoassist.github.io/) |
| WEAR | 2023 | ~19 小时户外运动 | 活动 + IMU | [官方网站](https://mariusbock.github.io/wear/) |
| N-EPIC-KITCHENS | 2022 | 事件 + RGB 子集 | 神经形态动作识别 | [GitHub](https://github.com/EgocentricVision/N-EPIC-Kitchens) |
| Ego-Deliver | 2021 | 5,360 个视频 | 配送行为分析 | [官方网站](https://egodeliver.github.io/) |
| HOMAGE | 2021 | 30 小时 | 家庭活动组合理解 | [GitHub](https://github.com/nishantrai18/homage) |
| MECCANO | 2021 | ~55 小时工业 | 手物交互、工业 | [官方网站](https://iplab.dmi.unict.it/MECCANO/) |
| EGO-CH | 2020 | 27+ 小时 | 游客行为、POI 任务 | [arXiv](https://arxiv.org/abs/2002.00899) |
| EgoCom | 2020 | 38.5 小时对话 | 多人第一人称对话 | [GitHub](https://github.com/facebookresearch/EgoCom-Dataset) |
| LEMMA | 2020 | 多视角活动 | 多智能体任务 | [GitHub](https://github.com/Buzz-Beater/LEMMA) |
| Charades-Ego | 2018 | 成对的 ego/exo | 对齐、动作 | [官方网站](https://prior.allenai.org/projects/charades-ego) |
| EGTEA Gaze+ | 2018 | 28 小时烹饪 | 注视 + 动作识别 | [官方网站](https://cbs.ic.gatech.edu/fpv/) |
| EgoGesture | 2017 | 2K+ 视频 / 2.4万 样本 | 手势识别 | [官方网站](https://nlpr.ia.ac.cn/iva/yfzhang/datasets/egogesture.html) |
| Stanford ECM | 2017 | 31 小时 | 日常活动分类 | [CVF](https://openaccess.thecvf.com/content_cvpr_2017/html/Nakamura_Jointly_Learning_Energy_CVPR_2017_paper.html) |
| THU-READ | 2017 | 1,920 个片段 | 头盔 RGB‑D 动作 | [官方网站](https://ivg.au.tsinghua.edu.cn/dataset/THU_READ.php) |
| PEV | 2016 | 1,226 对 | 双人对话微动作 | [CVF](https://openaccess.thecvf.com/content_cvpr_2016/html/Yonetani_Recognizing_Micro-Actions_and_CVPR_2016_paper.html) |
| FPPA | 2015 | 5 名受试者 | 日常动作 + 手/视线 | [CVF](https://openaccess.thecvf.com/content_iccv_2015/html/Zhou_Temporal_Perception_and_ICCV_2015_paper.html) |
| JPL-Interaction | 2013 | 84 个视频 | 第一人称活动识别 | [官方网站](http://michaelryoo.com/jpl-interaction.html) |
| ADL | 2012 | ~10 小时 | 日常活动识别 | [官方网站](https://www.csee.umbc.edu/~hpirsiav/papers/ADLdataset/) |
| Social Interactions | 2012 | ~60 小时 | 社交活动 | [官方网站](https://cbs.ic.gatech.edu/fpv/) |
| EgoAction (Sports) | 2011 | 第一人称体育视频 | 动作识别 | [IEEE](https://doi.org/10.1109/CVPR.2011.5995406) |

---

### 2.2 手物交互与细粒度活动
研究第一人称视角下手与物体之间的交互过程，是具身智能和机器人模仿学习的核心基础。

+  **Hand-4DGS: Feed-Forward 3D Gaussian Splatting for 4D Hand Reconstruction from Egocentric Videos**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：从第一人称视频中进行动态 3D 手部重建，解决快速头部运动、手部快速动态、严重遮挡和单视角歧义等问题，对 AR/VR 和 AI 眼镜至关重要
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16930)
+  **Hand Trajectory Fusion for Egocentric Natural Language Query Grounding**
    - 发表：EgoVis@CVPR 2026 (arXiv 2026年6月)
    - 亮点：首次将手部运动线索融入 NLQ 定位任务，在手物交互查询上 R@1, IoU=0.3 提升 2.54%
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.02962)
+  **Wh0: Generative World Models as Scalable Sources of Egocentric Human Hand Manipulation Data**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：使用生成式视频世界模型作为可扩展、可控的第一人称手部操作数据源，以解锁预训练灵巧 VLA 模型的操作能力
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.22136)
+  **TouchAnything: A Dataset and Framework for Bimanual Tactile Estimation from Egocentric Video**
    - 发表：arXiv 2026 (2026年5月)
    - 亮点：介绍了 EgoTouch，一个大规模多视角第一人称数据集，包含密集的触觉监督，用于双手手物交互，涵盖 208 个操作任务共 1,891 个片段
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.13083)
+  **IMPACT-HOI: Supervisory Control for Onset-Anchored Partial HOI Event Construction**
    - 发表：arXiv 2026 (2026年5月)
    - 亮点：一个混合主动框架，通过构建手物交互的结构化事件图来标注第一人称程序化视频，旨在从人类演示中学习机器人操作
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.17639)
+  **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - 发表：SIGGRAPH 2026 (arXiv 2026年5月)
    - 亮点：可微分前臂表示 + 统一手臂‑手 Transformer。在 HOT3D 上所有镜头类型下 MPJPE 降低 28%
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.12498)
+  **EgoGrasp: World-Space Hand-Object Interaction Estimation from Egocentric Videos**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：首个从动态第一人称视频中重建世界坐标系下手物交互的方法，支持开放词汇物体
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.12255)
+  **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：首个第一人称 HOI 世界模型，将物理先验嵌入生成扩散模型，从 3D 估计中蒸馏几何和运动学先验到物理信息嵌入
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.13615)
+  **Glove2Hand: Synthesizing Natural Hand-Object Interaction from Multi-Modal Sensing Gloves**
    - 发表：CVPR 2026 (亮点)
    - 亮点：从多模态传感手套数据生成逼真的裸手 HOI 视频，并附带 HandSense 数据集
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.20850)
+  **TOUCH: Text-Guided Controllable Generation of Free-Form Hand-Object Interactions**
    - 发表：ICLR 2026
    - 亮点：提出了自由形式 HOI 生成任务，构建了大规模 WildO2 3D HOI 数据集
    - 论文链接：[OpenReview](https://openreview.net/forum?id=4VW9HVCRw0)
+  **Leveraging Synthetic Data for Enhancing Egocentric Hand-Object Interaction Detection**
    - 发表：IJCV 2026, Vol.134
    - 亮点：仅使用少量真实标注数据结合合成数据，在 VISOR 上 AP 提升 11.69%，并开源了 HOI-Synth 合成数据生成流水线
    - 论文链接：[Springer](https://link.springer.com/article/10.1007/s11263-026-02838-8)
+  **ECHO: Ego-Centric modeling of Human-Object interactions**
    - 发表：arXiv 2025 (v1: 2025年8月, v2: 2026年3月)
    - 亮点：首个统一框架，仅从头部和手腕跟踪中联合恢复人体姿态、物体运动和接触动力学，使用新颖的三变量扩散过程
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.21556)
+  **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - 发表：NeurIPS 2025
    - 亮点：提出两层架构框架，高层使用 VLM 推断运动先验，低层基于 DiT 流匹配生成细粒度轨迹
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)
+  **EgoAERO: Learning Dexterous Manipulation from a Single Egocentric Video without Object Assets**
    - 发表：arXiv 2026
    - 亮点：无需预扫描物体资产的灵巧操作学习框架，构建了大规模 EgoDex‑R 数据集（430万 RGB‑D 帧）
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.08057)
+  **EgoInteract: Synthetic Egocentric Videos Generation for Interaction Understanding and Anticipation**
    - 发表：arXiv 2026
    - 亮点：一个可控的第一人称视频生成模拟器，可精确控制相机、人类动作和物体操作
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.18214)
+  **EgoHandICL: Egocentric 3D Hand Reconstruction with In-Context Learning**
    - 发表：arXiv 2026 (2026年1月)
    - 亮点：在第一人称视觉中处理深度歧义、自遮挡和复杂手物交互的鲁棒 3D 手部重建，提升 EgoVLM 的手物交互推理能力
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.09806)
+  **Do Egocentric Video-Language Models Truly Understand Hand-Object Interactions?**
    - 发表：ICLR 2025
    - 亮点：首次系统评估第一人称 VLM 对细粒度 HOI 的理解能力，提出 EgoHOIBench 基准
    - 论文链接：[arXiv](https://arxiv.org/abs/2405.17719)
+  **HOI-Ref: Hand-Object Interaction Referral in Egocentric Vision**
    - 发表：arXiv 2024
    - 亮点：定义了第一人称场景中的 HOI 指代新任务，并附带了 HOI‑QA 评估基准
    - 论文链接：[arXiv](https://arxiv.org/abs/2404.09933)
+  **Get a Grip: Reconstructing Hand-Object Stable Grasps in Egocentric Videos**
    - 发表：arXiv 2023
    - 亮点：首次从单目第一人称视频中重建稳定的手物抓取状态
    - 论文链接：[arXiv](https://arxiv.org/abs/2312.15719)
+ **EgoPCA: A New Framework for Egocentric Hand-Object Interaction Understanding**
    - 发表：ICCV 2023
    - 亮点：提出一个新框架，通过探测、筛选和适配（EgoPCA）来推进 Ego‑HOI 识别
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/ICCV2023/html/EgoPCA_A_New_Framework_for_Egocentric_Hand-Object_Interaction_Understanding_ICCV_2023_paper.html)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| ⭐ EgoDex | 2025 | 829 小时 / 3万 条轨迹 | 灵巧操作、手部姿态 | [GitHub](https://github.com/apple/ml-egodex) |
| EgoDex-R | 2026 | 430万 RGB‑D 帧 / 5,600 序列 | 灵巧操作、手物姿态 | [arXiv](https://arxiv.org/abs/2606.08057) |
| EgoTouch | 2026 | 1,891 个片段 / 208 个任务 | 触觉 HOI | [Hugging Face](https://huggingface.co/datasets/zhenyuxie-zhzh/EgoTouch_hdf5) |
| EgoTactile | 2026 | ~6 小时 / 768 个片段 | 抓握压力估计 | [官方网站](https://egotactile.github.io/) |
| EventEgoHands | 2026 | 48 个片段 / 12.96万 帧 | RGB+事件手部检测 | [GitHub](https://github.com/SynthSyntax/EventEgoHands) |
| HA-Ego-1K | 2026 | ~24 小时 / 484 个多视角片段 | 灵巧操作 | [Hugging Face](https://huggingface.co/datasets/humanarchive/HA-Ego-1K) |
| DexGloveHOI | 2026 | 3.5 小时 / 10万+ 样本 | 视觉‑IMU 3D 手部跟踪 | [arXiv](https://arxiv.org/abs/2605.21714) |
| EgoEVHands | 2026 | 5,419 个标注序列 | 立体事件 3D 手部姿态 | [GitHub](https://github.com/ZJUWang01/EgoEV-HandPose) |
| EgoEMG | 2026 | 41 名参与者 / 10+ 小时 | EMG+视觉手部姿态 | [GitHub](https://github.com/zhenqis123/EgoEMG) |
| HRDexDB | 2026 | 1,400 次抓取试验 | 灵巧抓取、触觉 | [Hugging Face](https://huggingface.co/datasets/hahahataeyun/hrdexdb) |
| TouchMoment | 2026 | 4,021 个视频 / 8,456 个接触时刻 | 接触时刻检测 | [arXiv](https://arxiv.org/abs/2604.12343) |
| EgoFun3D | 2026 | 271 个第一人称视频 | 交互式 3D 物体 | [官方网站](https://3dlg-hcvc.github.io/EgoFun3D/) |
| SHOW3D | 2026 | 野外 ego‑exo HOI | 3D 手物标注 | [arXiv](https://arxiv.org/abs/2603.28760) |
| FEEL | 2026 | 力同步厨房视频 | 物理动作理解 | [官方网站](https://www.cs.umd.edu/~edessale/feel) |
| EgoPoints | 2025 | 点轨迹 + 合成 | 第一人称视频跟踪 | [GitHub](https://github.com/AhmadDarKhalil/EgoPoints) |
| ⭐ HOI4D | 2022 | 240万 帧 / 4,000 序列 | 4D HOI | [官方网站](https://hoi4d.github.io/) |
| AssemblyHands | 2023 | 300万 张图像 | 3D 手部姿态 | [官方网站](https://assemblyhands.github.io/) |
| EgoObjects | 2023 | 9,200+ 视频 | 检测、实例分割 | [GitHub](https://github.com/facebookresearch/EgoObjects) |
| ENIGMA-51 | 2023 | 22 小时工业 | 细粒度行为 | [官方网站](https://fpv-iplab.github.io/ENIGMA-51/) |
| POV-Surgery | 2023 | ~8.8万 帧 (合成) | 手术手‑工具姿态 | [官方网站](https://batfacewayne.github.io/POV_Surgery_io/) |
| VOST | 2023 | 713 个视频 | 视频目标分割 | [官方网站](https://www.vostdataset.org/) |
| EgoBody | 2022 | 125 序列 | 身体姿态、交互 | [官方网站](https://egobody.ethz.ch/) |
| EgoHOS | 2022 | 1.1万+ 张图像 | 手物分割 | [GitHub](https://github.com/owenzlz/EgoHOS) |
| EgoPAT3D | 2022 | 100万+ 帧 RGB‑D | 3D 动作目标预测 | [GitHub](https://github.com/ai4ce/EgoPAT3D) |
| Touch and Go | 2022 | 1.2万+ 视觉‑触觉帧 | 视觉 + 触觉 | [官方网站](https://touch-and-go.github.io/) |
| VISOR | 2022 | EPIC + 掩码 | 分割、HOI | [官方网站](https://epic-kitchens.github.io/VISOR/) |
| H2O | 2021 | 10万+ 帧 | 双手交互 | [官方网站](https://h2odataset.ethz.ch/) |
| TREK-150 | 2021 | 150 个 EPIC 序列 | 目标跟踪 | [官方网站](https://machinelearning.uniud.it/datasets/trek150/) |
| You2Me | 2020 | 14 序列 | 通过 ego‑exo 推断身体姿态 | [GitHub](https://github.com/facebookresearch/you2me) |
| FPHA | 2018 | 1,200 序列 | 手部姿态 + 动作 | [官方网站](https://guiggh.github.io/publications/first-person-hands/) |
| EgoDexter | 2017 | ~3,200 帧 | 遮挡下的手部跟踪 | [官方网站](https://handtracker.mpi-inf.mpg.de/projects/OccludedHands/EgoDexter.htm) |
| EgoHands | 2015 | 4,800 标注帧 | 手部检测 | [官方网站](http://vision.soic.indiana.edu/projects/egohands/) |
| BEOID | 2014 | 58 个视频 | 手物交互 | [官方网站](https://data.bris.ac.uk/data/dataset/3wats8ruq1sp52hq3bo8dkzul3) |
| EDSH | 2013 | 2 个视频 | 像素级手部分割 | [官方网站](http://www.cs.cmu.edu/~kkitani/datasets/) |
| Handled Objects | 2009 | 11 个类别 | 抓取序列 | [IEEE](https://doi.org/10.1109/CVPRW.2009.5204360) |

---

### 2.3 第一人称视觉‑语言模型与多模态推理
将大语言模型与第一人称视觉相结合，实现视频问答、内容描述和推理等高级认知能力。本节也涵盖融合 RGB、深度、IMU、音频和视线信号的多模态方法。

#### 预训练基础模型
+  **EgoM2P: Egocentric Multimodal Multitask Pretraining**
    - 发表：ICCV 2025
    - 亮点：一个统一设计，支持跨多种第一人称感知和合成任务的多任务处理，包括视线预测、第一人称相机跟踪和单目深度估计，同时也作为条件第一人称视频合成的生成模型
    - 论文链接：[ICCV](https://openaccess.thecvf.com/content/ICCV2025/html/EgoM2P_Egocentric_Multimodal_Multitask_Pretraining_ICCV_2025_paper.html)
+  **EgoAdapt: Adaptive Multisensory Distillation and Policy Learning for Efficient Egocentric Perception**
    - 发表：ICCV 2025
    - 亮点：一个自适应执行跨模态蒸馏和策略学习的框架，以在第一人称动作识别、主动说话人定位和行为预测等不同任务上实现高效推理。GMACs 降低高达 89.09%，参数量降低 82.02%，能耗降低 9.6 倍
    - 论文链接：[ICCV](https://www.openaccess.thecvf.com/content/ICCV2025/html/Chowdhury_EgoAdapt_Adaptive_Multisensory_Distillation_and_Policy_Learning_for_Efficient_Egocentric_ICCV_2025_paper.html) | [arXiv](http://arxiv.org/abs/2506.21080)
+ **EgoVLPv2: Egocentric Video-Language Pre-training with Fusion in the Backbone**
    - 发表：ICCV 2023
    - 亮点：改进的 VLP，采用骨干网络级融合架构
    - 论文链接：[arXiv](https://arxiv.org/abs/2307.05463)
+ **Egocentric Video-Language Pretraining (EgoVLP)**
    - 发表：CVPR 2022
    - 亮点：首个专为第一人称场景设计的视频‑语言预训练框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2206.01670)

#### 高级推理与前沿进展
+  **EgoSAT: A Comprehensive Benchmark of Egocentric Streaming Interaction Understanding**
    - 发表：ECCV 2026 (arXiv 2026年6月)
    - 亮点：首个用于流式设置下第一人称视频推理的综合基准，旨在评估 VLM 对流式交互理解的能力。包含 1,997 个独特视频，总时长 165 小时，约 4,800 个 QA 对
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.24422)
+  **PROSE: Training-Free Egocentric Scene Registration with Vision-Language Models**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：使用预训练 VLM 作为场景理解和跨扫描匹配的来源进行第一人称场景配准，优于几何和学习的场景图基线
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16569)
+  **Decoding Pedestrian Crossing Intention from Egocentric Vision via Vision Language Models**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：首次使用 VLM 解码行人过街意图，融合眼动和自我运动后准确率提升 14.5%
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.09142)
+  **The Right Inference Strategy Is All You Need: Nearly Training-Free Domain-Wise Inference for EgoCross Challenge**
    - 发表：arXiv 2026 (2026年5月)
    - 亮点：EgoCross 挑战赛解决方案，域感知推理策略仅用 20 个训练样本即达到 66.98% 的准确率
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.00829)
+  **Spatial Reasoning with Vision-Language Models in Ego-Centric Multi-View Scenes**
    - 发表：ICLR 2026 (2026年4月)
    - 亮点：提出 Ego3D‑Bench 空间推理基准（8,600+ QA 对）和 Ego3D‑VLM 后训练框架
    - 论文链接：[OpenReview](https://openreview.net/forum?id=10008200)
+  **EgoMotion: Hierarchical Reasoning and Diffusion for Egocentric Vision-Language Motion Generation**
    - 发表：arXiv 2026 (2026年4月)
    - 亮点：提出层次化推理和扩散框架，从第一人称视频生成用语言描述的 3D 人体运动
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.19105)
+  **Exo2Ego: Exocentric Knowledge Guided Multimodal LLMs for Egocentric Video Understanding**
    - 发表：AAAI 2026 (2026年2月)
    - 亮点：构建了 Ego‑ExoClip 预训练数据集（110 万个同步的第一人称‑第三人称片段‑文本对），提出三阶段渐进式映射学习流水线
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/38244)
+  **Egocentric Bias in Vision-Language Models**
    - 发表：arXiv 2026 (2026年2月)
    - 亮点：引入 FlipSet，一个用于 VLM 二级视觉观点采择的诊断基准。评估 103 个 VLM 显示系统性的自我中心偏差：绝大多数表现低于随机水平
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.03953)
+  **Allocentric Perceiver: Disentangling Allocentric Reasoning from Egocentric Visual Priors via Frame Instantiation**
    - 发表：arXiv 2026 (2026年2月)
    - 亮点：一种无需训练的去中心化感知策略，从单张或多张图像中恢复度量 3D 状态，在去中心化任务上提升约 10%
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.05789)
+  **Cognitively-Inspired Tokens Overcome Egocentric Bias in Multimodal Models**
    - 发表：arXiv 2026 (2026年1月)
    - 亮点：多模态语言模型在语义视觉‑语言任务上表现良好，但在需要采用其他智能体视觉视角的空间推理上失败，反映了持久的自我中心偏差
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.15849)
+  **EgoThinker: Unveiling Egocentric Reasoning with Spatio-Temporal Chain of Thought**
    - 发表：NeurIPS 2025
    - 亮点：将思维链 (CoT) 引入第一人称视频理解，提出时空思维链框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.23569)
+  **Towards Comprehensive Scene Understanding: Integrating First and Third-Person Views for LVLMs**
    - 发表：NeurIPS 2025
    - 亮点：提出 E3VQA 多视角问答基准（4K 高质量 QA 对）和 M3CoT 提示技术，在 GPT‑4o 上提升 4.84%
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/1af83ab66b4f07a3f55788e67dab5782-Abstract-Conference.html)
+  **Benchmarking Egocentric Multimodal Goal Inference for Assistive Wearable Agents**
    - 发表：NeurIPS 2025 数据集与基准轨道
    - 亮点：目标推理基准数据集，包含 363 名参与者、3,482 条记录，人类上限准确率 93%，最佳 VLM 仅 84%
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/23ab960082db936f874b171822e0d097-Abstract-Datasets_and_Benchmarks.html)
+  **ECBench: Can Multi-modal Foundation Models Understand the Egocentric World? A Holistic Embodied Cognition Benchmark**
    - 发表：CVPR 2025
    - 亮点：一个高质量基准，旨在系统评估 LVLM 的具身认知能力。包含多样化场景视频源、开放式问题格式和 30 个具身认知维度
    - 论文链接：[CVPR](https://www.openaccess.thecvf.com/content/CVPR2025/html/Dang_ECBench_Can_Multi-modal_Foundation_Models_Understand_the_Egocentric_World_A_CVPR_2025_paper.html) | [arXiv](http://arxiv.org/abs/2501.05031)
+  **MM-Ego: Towards Building Egocentric Multimodal LLMs for Video QA**
    - 发表：ICLR 2025
    - 亮点：提出 MM‑Ego，一个在第一人称视频理解上表现强大的多模态 LLM
    - 论文链接：[ICLR](https://openreview.net/forum?id=MM-Ego)
+  **CLiViS: Unleashing Cognitive Map through Linguistic-Visual Synergy for Embodied Visual Reasoning**
    - 发表：arXiv 2025
    - 亮点：通过语言‑视觉协同构建认知地图，突破长视频推理的瓶颈
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.17629)
+  **PhysBrain: Human Egocentric Data as a Bridge from Vision Language Models to Physical Intelligence**
    - 发表：arXiv 2025
    - 亮点：将第一人称人类视频转化为具身监督数据
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.16793)
+  **Vinci: A Real-time Smart Assistant based on Egocentric Vision-language Model**
    - 发表：ACM 2025 (arXiv 2024)
    - 亮点：适用于可穿戴设备的轻量级 Ego‑VLM，支持长视频记忆和动作生成，可在边缘设备上实时运行
    - 论文链接：[arXiv](https://arxiv.org/abs/2412.21080)
+  **EgoThink: Evaluating First-Person Perspective Thinking Capability of Vision-Language Models**
    - 发表：CVPR 2024
    - 亮点：引入一个新颖的视觉问答基准，涵盖六个核心能力、十二个详细维度，使用从第一人称视频中选取的片段和人工标注的 QA 对构建
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/EgoThink_Evaluating_First-Person_Perspective_Thinking_Capability_of_Vision-Language_Models_CVPR_2024_paper.html)
+  **VidEgoThink: A Comprehensive Benchmark for Egocentric Video Understanding**
    - 发表：arXiv 2024
    - 亮点：基于 EgoThink，引入一个用于评估第一人称视频理解能力的综合基准，设计了四个相互关联的任务：视频问答、层次规划、视觉定位和奖励建模
    - 论文链接：[arXiv](https://arxiv.org/abs/2405.17719)
+  **Binocular Egocentric-360 Multi-modal Scene Understanding in the Wild**
    - 发表：ICCV 2025 Workshop
    - 亮点：关注双目/立体第一人称和 360° 全景视角的多模态场景理解和感知，同时测量第一人称视图和第三人称全景视图
    - 论文链接：[ICCV](https://openaccess.thecvf.com/content/ICCV2025/html/EgoM2P_Egocentric_Multimodal_Multitask_Pretraining_ICCV_2025_paper.html)
+  **D3Net: Dual-Path Decoupling-Distillation for Adaptive Fusion in Continual Egocentric Learning**
    - 发表：IEEE 2025 (arXiv 2026)
    - 亮点：提出双路径解耦‑蒸馏网络，用于更有效地动态融合模态信息和知识迁移。通过双路径解耦模块和动态门控机制显式分离模态的共享和私有特征。在 UESTC MMEA CL 数据集上达到 83.97% 准确率
    - 论文链接：[IEEE Xplore](https://ieeexplore.ieee.org/document/11324280)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
|  EgoSAT | 2026 | 165 小时 / ~4,800 QA | 流式交互理解 | [arXiv](https://arxiv.org/abs/2606.24422) |
| EgoTL | 2026 | 100+ 日常家务任务 | 长时推理、空间 QA | [官方网站](https://ego-tl.github.io/) |
| EgoCoT-Bench | 2026 | 351 个视频 / 3,172 QA | 基于接地操作链的 CoT QA | [官方网站](https://dstardust.github.io/EgoCoT/) |
| MM-Conv | 2026 | 6.7 小时 / 4,211 个表达 | 上下文 3D 对话定位 | [arXiv](https://arxiv.org/abs/2605.21796) |
| Minerva-Ego | 2026 | 1,160 QA / 156 个视频 | 时空推理轨迹 | [GitHub](https://github.com/google-deepmind/neptune) |
| EgoEverything | 2026 | 100+ 小时 / 5K+ 选择题 | 长上下文 AR 视频 QA | [arXiv](https://arxiv.org/abs/2604.08342) |
| EgoEsportsQA | 2026 | 1,745 QA 对 | 电竞视频 QA、推理 | [arXiv](https://arxiv.org/abs/2604.12320) |
| MyEgo | 2026 | 541 个长视频 / 5K QA | 个性化视频 QA | [GitHub](https://github.com/Ryougetsu3606/MyEgo) |
| LifeDialBench / EgoMem | 2026 | 生活日志记忆 | 在线评估 | [GitHub](https://github.com/qys77714/LifeDialBench) |
| Ego2Web | 2026 | 500 个视频‑指令对 | 第一人称视频接地网络智能体 | [Hugging Face](https://huggingface.co/datasets/Shoubin/Ego2Web) |
| NoRA | 2026 | 1,420 个片段 | 规范性动作推理 | [arXiv](https://arxiv.org/abs/2606.04806) |
| Causal-Plan-1M | 2026 | 100万 QA / 2.22万 片段 | 物理接地规划 QA | [Hugging Face](https://huggingface.co/datasets/anonymous-causal-plan/Causal_Plan) |
| Pause-and-Think | 2026 | 1万 QA 片段 + 300 基准 | 辅助动作建议 | [GitHub](https://github.com/sssshivvvv/pause-and-think) |
| HD-EPIC | 2025 | ~41 小时 / 密集标签 | 细粒度厨房、VQA | [官方网站](https://hd-epic.github.io/) |
| EgoEMS | 2025 | 20+ 小时急救场景 | 急救 QA、多模态 | [GitHub](https://github.com/UVA-DSA/EgoEMS) |
| HowToDIV | 2025 | ~24 小时教学 | 对话、程序化 QA | [GitHub](https://github.com/google/howtodiv) |
| InterVLA | 2025 | 11.4 小时交互 | 指令、ego‑exo 动作捕捉 | [官方网站](https://liangxuy.github.io/InterVLA/) |
| EgoClip | 2022 | 380万 片段‑文本对 | 视频‑语言预训练 | [GitHub](https://github.com/showlab/EgoVLP) |
| AssistQ | 2022 | 100 个长视频 / 529 QA | 教学 QA | [GitHub](https://github.com/showlab/AssistQ) |
| EgoTaskQA | 2022 | ~2,000 视频 / 4万 QA | 因果与任务 QA | [官方网站](https://sites.google.com/view/egotaskqa) |
| EgoVQA | 2019 | 600+ QA | 视频 QA | [ICCVW 2019](https://openaccess.thecvf.com/content_ICCVW_2019/html/EPIC/Fan_EgoVQA_-_An_Egocentric_Video_Question_Answering_Benchmark_Dataset_ICCVW_2019_paper.html) |

---

### 2.4 长视频理解与结构化推理
处理小时甚至天级别的超长第一人称视频，核心挑战包括长期依赖建模、记忆检索和信息摘要。本节也涵盖基于场景图的结构化表示用于长视频推理。

+  **Keep It in Mind: User Centric Continual Spatial Intelligence Reasoning in Egocentric Video Streams**
    - 发表：ICML 2026 (arXiv 2026年6月)
    - 亮点：引入 UCS‑Bench，一个包含 170+ 小时、8,100+ 个带时间戳问题的数据集，用于用户中心的持续空间智能
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.15200)
+  **Graph it first! Enabling Reasoning on Long-form Egocentric Videos through Scene Graphs**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：引入第一人称场景图 (EgoSGs) 以克服 MLLM 输入约束，通过将视频表示为紧凑的文本场景图，在 HD‑EPIC VQA 上达到 SOTA
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.25842)
+  **Bridging Modalities, Spanning Time: Structured Memory for Ultra-Long Agentic Video Reasoning**
    - 发表：arXiv 2026 (2026年5月)
    - 亮点：提出 MAGIC‑Video，使用多模态记忆图和交错叙事链，在 EgoLifeQA 上比之前最好的智能体系统高出 10.1 分
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.08271)
+  **EgoMemReason: A Memory-Driven Reasoning Benchmark for Long-Horizon Egocentric Video Understanding**
    - 发表：arXiv 2026 (2026年5月)
    - 亮点：一个用于评估周级别第一人称视频记忆驱动推理的基准，包含 500 个问题，最佳模型仅达到 39.6% 准确率
    - 论文链接：[Hugging Face](https://huggingface.co/datasets/Ted412/EgoMemReason)
+  **Semantic and Visual Evidence for Efficient Long-Video Reasoning: A Solution for the HD-EPIC VQA Challenge**
    - 发表：arXiv 2026 (2026年5月)
    - 亮点：将长视频推理解耦为语义证据和视觉证据，通过查询引导的检索集成实现高效长视频理解
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.29402)
+  **EgoEverything: A Benchmark for Human Behavior Inspired Long Context Egocentric Video Understanding in AR Environment**
    - 发表：arXiv 2026 (2026年4月)
    - 亮点：一个明确考虑人类行为的基准，在生成问题时利用从视线数据中抽象出的注意力信号
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.08342)
+  **MA-EgoQA: Question Answering over Egocentric Videos from Multiple Embodied Agents**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：首次定义多智能体第一人称视频 QA 任务，提供 1,700+ 个问题，覆盖五个场景类别
    - 论文链接：[官方网站](https://ma-egoqa.github.io/)
+  **Static Scene Reconstruction from Dynamic Egocentric Videos**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：提出一个鲁棒流水线，将静态重建骨干适应到长第一人称视频，使用掩码感知重建机制
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.18090)
+  **From Pixels to Graphs: using Scene and Knowledge Graphs for HD-EPIC VQA Challenge**
    - 发表：arXiv 2025
    - 亮点：提出一个框架，结合两种互补的神经符号抽象：场景图和常识知识图，分别通过 SceneNet 和 KnowledgeNet 实例化
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.01867)
+  **Action Scene Graphs for Long-Form Understanding of Egocentric Videos**
    - 发表：arXiv 2024
    - 亮点：提出动作场景图用于第一人称视频的长形式理解，从可穿戴设备捕获中实现人类活动的结构化分析
    - 论文链接：[arXiv](https://arxiv.org/abs/2409.01600)
+  **EgoMemory: Memory-Augmented Personalized Retrieval for Long-Context Egocentric Video**
    - 发表：ACL 2026
    - 亮点：为连续流式第一人称视频提出终身记忆框架
    - 论文链接：[Microsoft Research](https://www.microsoft.com/en-us/research/publication/egomemory-memory-augmented-personalized-retrieval-for-long-context-egocentric-video/)
+  **MyEgo: Ego-Grounding for Personalized Question-Answering in Egocentric Videos**
    - 发表：CVPR 2026
    - 亮点：大规模个性化第一人称视频数据集，用于长形式 QA
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.01966)
+  **EGAgent: Agentic Very Long Video Understanding**
    - 发表：arXiv 2026
    - 亮点：基于实体场景图的智能体推理框架，能够处理跨天的连续视频流，支持结构化多跳推理和音视频混合检索
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.18157)
+  **Spatial-Conditioned Reasoning in Long-Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：探索显式空间信号对长形式 VLM 推理的影响，引入精细重新标注的 Sanpo‑D 数据集
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.18100)
+  **FocusGraph: Graph-Structured Frame Selection for Embodied Long Video Question Answering**
    - 发表：arXiv 2026
    - 亮点：基于图的帧过滤流水线，使用 Scene‑Caption LLM 选择器检索与查询相关的帧
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.04349)
+  **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - 发表：ICLR 2026
    - 亮点：一个通过第一人称交互世界建模评估具身认知的基准，揭示 VLM 在逆任务上比前向预测表现更好
    - 论文链接：[OpenReview](https://openreview.net/forum?id=Patx6MRipw)
+  **OSGNet: Champion Solution for Ego4D Episodic Memory Challenge 2025**
    - 发表：CVPR 2025 挑战赛全赛道冠军
    - 亮点：提出早期融合时序定位架构，赢得 Ego4D 情景记忆挑战赛全部三个赛道
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.03710)
+  **Unique Lives, Shared World: Learning from Single-Life Egocentric Videos**
    - 发表：arXiv 2025
    - 亮点：研究从单个个体的超长生命期视频中学习的问题
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.04085)
+  **EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding**
    - 发表：NeurIPS 2023
    - 亮点：超长第一人称视频理解的权威诊断基准
    - 论文链接：[arXiv](https://arxiv.org/abs/2308.09126)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
|  UCS-Bench | 2026 | 170+ 小时 / 8,100+ QA | 用户中心持续空间智能 | [arXiv](https://arxiv.org/abs/2606.15200) |
| SuperMemory-VQA | 2026 | 52.9 小时 / 4,853 QA 对 | 长时记忆 QA | [Hugging Face](https://huggingface.co/datasets/OSU-AIoT-MLSys-Lab/SuperMemory-VQA) |
| EgoMemReason | 2026 | 500 个周级别选择题 | 周尺度记忆推理评估 | [Hugging Face](https://huggingface.co/datasets/Ted412/EgoMemReason) |
| EgoExoMem | 2026 | 2,600 选择题 / 390 个片段 | 跨视角情景记忆推理 | [GitHub](https://github.com/RuipingL/EgoExoMem) |
| EgoIntrospect | 2026 | 180 小时 / 60 名受试者 | 内部用户状态推断、长期记忆 | [官方网站](https://ego-introspect.github.io/) |
| MA-EgoQA | 2026 | 1,741 QA / 7天多智能体录像 | 多智能体第一人称视频 QA | [官方网站](https://ma-egoqa.github.io/) |
| EgoStream | 2026 | 2,250 个评估查询 | 流式情景记忆基准 | [官方网站](https://saroo25.github.io/Egostream/) |
| EgoLife | 2025 | ~266–300 小时日常录像 | 长期个人助理、情景记忆 | [官方网站](https://egolife-ai.github.io/) |
| EgoSchema | 2023 | 250+ 小时 / 5,000 选择题 | 超长视频推理与 QA | [官方网站](https://egoschema.github.io/) |
| VidChapters-7M | 2023 | 81.7万 个视频 / 700万 章节 | 长视频分割与摘要 | [官方网站](https://antoyang.github.io/vidchapters.html) |
| Multi-Ego | 2022 | ~12 小时 / 41 个多穿戴者序列 | 跨用户视频摘要 | [GitHub](https://github.com/M-Elfeki/Multi-DPP) |
| DoMSEV | 2018 | 80 小时, 48 序列 | 语义视频快进与略读 | [官方网站](https://www.verlab.dcc.ufmg.br/semantic-hyperlapse/cvpr2018-dataset/) |
| HUJI-EgoSeg | 2014 | 29 个未修剪长视频 | 时序活动分割 | [官方网站](http://www.cs.huji.ac.il/~yedMDpid/egoseg/) |
| UT Ego | 2012 | ~17 小时, 4 个全长记录 | 长视频摘要与生活日志 | [官方网站](http://vision.cs.utexas.edu/projects/egocentric_data/UT_Egocentric_Dataset.html) |
| VINST / Visual Diaries | 2011 | 31 个日常日志视频 | 事件分割、时间线提取 | [官方网站](https://www.csc.kth.se/cvap/vinst/NovEgoMotion.html) |

---

### 2.5 注视、注意力与意图预测
从第一人称录像中预测人类注视点、注意力分布和潜在意图，是可穿戴交互助手的核心技术。

+  **EPIC: A System Framework for Efficient Egocentric Perception on Embodied AR Glasses**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：一个用于具身 AR 眼镜的高效第一人称感知系统，利用注视、姿态和惯性信号推断用户意图，并仅保留感知输入中最具信息性的部分
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.14282)
+  **Gaze Beyond the Frame: Forecasting Egocentric 3D Visual Span**
    - 发表：NeurIPS 2025 (arXiv 2026年4月)
    - 亮点：提出新颖的 3D 视觉跨度预测任务，EgoSpanLift 将 2D 注视预测提升到完整的 3D 场景空间
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/bf649dbcf4eaaba4fc68ccaee25a7f9e-Abstract-Conference.html)
+  **SkillSight: Efficient First-Person Skill Assessment with Gaze**
    - 发表：arXiv 2026 (2026年4月)
    - 亮点：探索面向资源受限智能眼镜的节能、保护隐私的第一人称技能评估
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.01645)
+  **Gaze-Regularized VLMs for Ego-Centric Behavior Understanding**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：将眼动信号嵌入 VLM 训练流水线，注视正则化强制模型优先考虑注视区域，语义指标提升近 13%
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.23190)
+  **Real Eyes Realize Faster: Gaze Stability and Pupil Novelty for Efficient Egocentric Learning**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：使用眼动作为无需训练的外带信息：注视固定捕获视觉稳定性，瞳孔响应捕获与唤醒相关的新奇性。双标准帧选择器以 10% 的预算选择帧，性能匹配全流
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.04098)
+  **EgoCampus: Egocentric Pedestrian Eye Gaze Model and Dataset**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：介绍了 EgoCampus 数据集，覆盖 25 条独特室外路径，使用 Project Aria 眼镜记录了 80+ 名行人
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.07668)
+  **Eyes on Target: Gaze-Aware Object Detection in Egocentric Video**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：将视线衍生特征注入 ViT 注意力机制，使空间特征选择偏向人类关注区域
    - 论文链接：[arXiv](https://arxiv.org/abs/2511.01237)
+  **Beyond Scanpaths: Graph-Based Gaze Simulation in Dynamic Scenes**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：引入目标密度网络 (ODN) 预测下一步注视分布，并发布 Focus100 数据集，包含 30 名参与者观看第一人称驾驶录像的原始视线数据
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.23750)
+  **Ego-PMOVE: Prompt-aware Mixture of View Experts Network for Egocentric Gaze Prediction**
    - 发表：AAAI 2026
    - 亮点：首个探索跨视角注视相关性的方法，提示驱动的多视角专家混合架构
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/37808)
+  **Learning from Human Gaze: Human-like Robot Social Navigation in Dense Crowds**
    - 发表：AAAI 2026
    - 亮点：发布 GazeNav 数据集，包含同步的可穿戴眼动追踪、RGB 录像和机器人导航轨迹
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/38941)
+  **In the Eye of MLLM: Benchmarking Egocentric Video Intent Understanding with Gaze-Guided Prompting**
    - 发表：NeurIPS 2025 数据集与基准轨道
    - 亮点：EgoGazeVQA 基准系统评估多模态 LLM 通过眼动信号推断用户意图的能力
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/9df42a5f6d1397e46e2cdca80a1a7903-Abstract-Datasets_and_Benchmarks.html)
+  **egoEMOTION: Egocentric Vision and Physiological Signals for Emotion and Personality Recognition in Real-World Tasks**
    - 发表：NeurIPS 2025
    - 亮点：通过 Meta Project Aria 眼镜收集的多模态数据集，结合视频、眼动和生物信号进行真实环境情绪分析
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.22129)
+  **EgoIntention: Visual Intention Grounding for Egocentric Assistants**
    - 发表：arXiv 2026 (2026年4月)
    - 亮点：首个用于第一人称视觉意图定位的数据集，挑战多模态 LLM 理解并忽略非意图上下文物体，推理不常见物体功能
    - 论文链接：[IEEE Xplore](https://ieeexplore.ieee.org/document/11324280)

---

### 2.6 3D/4D 重建与结构化感知
从单目第一人称视频中恢复 3D 人体网格、深度图和动态 4D 场景结构，是 AR/VR 和机器人空间感知的基础技术。本节也涵盖基于场景图的结构化 3D 感知。

#### 人体姿态与网格恢复
+  **Hand-4DGS: Feed-Forward 3D Gaussian Splatting for 4D Hand Reconstruction from Egocentric Videos**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：从第一人称视频中进行动态 3D 手部重建，解决快速头部运动、手部快速动态、严重遮挡和单视角歧义
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16930)
+  **RoboAtlas: Contextual Active SLAM**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：通过上下文多臂赌博机整合前沿探索、全局语义地图推理和基于第一人称 VLM 的推理
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.19378)
+  **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - 发表：SIGGRAPH 2026 (arXiv 2026年5月)
    - 亮点：可微分前臂表示 + 统一手臂‑手 Transformer，在 HOT3D 上所有镜头类型下 MPJPE 降低 28%
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.12498)
+  **Bringing a Personal Point of View: Evaluating Dynamic 3D Gaussian Splatting for Egocentric Scene Reconstruction**
    - 发表：EgoVis@CVPR 2026 (arXiv 2026年4月)
    - 亮点：动态 3DGS 在第一人称与第三人称录像上的系统基准测试，确认了第一人称视角的质量持续下降
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.23803)
+  **FunRec: Reconstructing Functional 3D Scenes from Egocentric Interaction Videos**
    - 发表：CVPR 2026 (arXiv 2026年4月)
    - 亮点：直接从第一人称 RGB‑D 交互视频中重建功能性 3D 数字孪生室内场景，发现关节部件并估计运动学参数
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.05621)
+  **OmniEgoCap: Camera-Agnostic Sequence-Level Egocentric Motion Reconstruction**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：基于扩散的重建方法，泛化到所有可穿戴相机硬件，带有几何感知可见性增强模块
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.19283)
+  **EgoGrasp: World-Space Hand-Object Interaction Estimation from Egocentric Videos**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：首个从动态第一人称视频中重建世界坐标系下手物交互的方法，支持开放词汇物体
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.12255)
+  **AG-EgoPose: Leveraging Action-Guided Motion and Kinematic Joint Encoding for Egocentric 3D Pose Estimation**
    - 发表：arXiv 2026
    - 亮点：动作条件运动建模 + 运动学关节嵌入，实现鲁棒的可穿戴相机姿态估计
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.25175)
+  **Pandora: Articulated 3D Scene Graphs from Egocentric Vision**
    - 发表：BMVC 2025
    - 亮点：利用人类佩戴 Project Aria 眼镜自然探索场景时捕获的第一人称数据，恢复关节物体部件的模型。证明关节 3D 场景图增强了机器人执行移动操作任务的能力
    - 论文链接：[BMVC](https://bmvc2025.bmva.org/proceedings/548/)
+  **Lost & Found: Updating Dynamic 3D Scene Graphs from Egocentric Observations**
    - 发表：arXiv 2024
    - 亮点：仅基于带有相应手部位置和相机姿态估计的第一人称录像，在检测到的交互间隔内跟踪移动物体的 6DoF 姿态。在平移和方向误差上分别优于第二佳方法 34% 和 56%
    - 论文链接：[arXiv](https://arxiv.org/abs/2411.19162)
+  **Fish2Mesh Transformer: 3D Human Mesh Recovery from Egocentric Vision**
    - 发表：arXiv 2025
    - 亮点：首个针对广角鱼眼头戴相机优化的网格恢复流水线
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.06089)
+  **Single-to-Dual-View Adaptation for Egocentric 3D Hand Pose Estimation**
    - 发表：CVPR 2024
    - 亮点：提出一种新颖的单‑双视角适应 (S2DHand) 解决方案，将预训练的单视角估计器适应到双视角
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/Single-to-Dual-View_Adaptation_for_Egocentric_3D_Hand_Pose_Estimation_CVPR_2024_paper.html)
+ **Ego-Humans: An Ego-Centric 3D Multi-Human Benchmark**
    - 发表：ICCV 2023
    - 亮点：提出了 EgoHumans，一个新的多视角多人体视频基准，用于推进第一人称人体 3D 姿态估计和跟踪
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/ICCV2023/html/Ego-Humans_An_Ego-Centric_3D_Multi-Human_Benchmark_ICCV_2023_paper.html)

#### 事件相机感知
+  **D-EventEgo: Event-Based Egocentric Human Pose Estimation in Dynamic Environments**
    - 发表：arXiv 2025
    - 亮点：首个用于第一人称人体姿态跟踪的事件流流水线，适用于快速运动和高动态范围
    - 论文链接：[arXiv](https://arxiv.org/abs/2505.22007)
+  **EventEgo3D++: 3D Human Motion Capture from a Head-Mounted Event Camera**
    - 发表：arXiv 2025
    - 亮点：用于头戴式事件相机的鱼眼事件全身体运动捕捉端到端流水线
    - 论文链接：[arXiv](https://arxiv.org/abs/2502.07869)

#### 场景重建与第一人称 SLAM
+  **Ego-1K: A Large-Scale Multiview Video Dataset for Egocentric Vision**
    - 发表：CVPR 2026
    - 亮点：近 1,000 个多视角第一人称片段，由 12 个同步相机围绕 4 个 VR 头显组成的装置捕获
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.13741)
+  **EgoLifter: Open-World 3D Segmentation for Egocentric Perception**
    - 发表：ECCV 2024
    - 亮点：一种用于第一人称感知的开放世界 3D 分割方法
    - 论文链接：[Springer](https://link.springer.com/chapter/10.1007/978-3-031-72912-6_22)
+  **EgoSG: Learning 3D Scene Graphs from Egocentric RGB-D Sequences**
    - 发表：CVPR 2024
    - 亮点：提出 EgoSG 直接从第一人称帧序列估计 3D 场景图
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/EgoSG_Learning_3D_Scene_Graphs_from_Egocentric_RGB-D_Sequences_CVPR_2024_paper.html)
+  **Generalizable Dynamic Radiance Field in Egocentric View**
    - 发表：ICLR 2024
    - 亮点：一个用于第一人称视角的可泛化动态辐射场新框架，基于单目视频预测给定时间的 3D 物理世界表示，无需测试时训练
    - 论文链接：[OpenReview](https://openreview.net/forum?id=Generalizable_Dynamic_Radiance_Field_in_Egocentric_View)
+  **EventEgo3D: 3D Human Motion Capture from Egocentric Event Streams**
    - 发表：CVPR 2024
    - 亮点：利用异步事件相机录像的高速人体运动捕捉系统
    - 论文链接：[arXiv](https://arxiv.org/abs/2404.08640)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
|  Oxford Day-and-Night | 2026 | 大规模第一人称 | NVS、挑战光照下的视觉重定位 | [NeurIPS 2026] |
| ⭐ Ego-Exo4D | 2024 | 1,286+ 小时配对的 ego/exo 录像 | 多视角技能分析、3D 重建 | [官方网站](https://ego-exo4d-data.org/) |
| PRISM | 2026 | 27万 样本 / 1,180万 帧 | 零售具身 VLM、空间推理 | [Hugging Face](https://huggingface.co/datasets/DreamVu/PRISM-100K) |
| EgoTraj | 2026 | 10.7 小时 / 115万 帧 | 第一人称相机轨迹预测 | [GitHub](https://github.com/yehiahmad/EgoTraj) |
| AIST-Living | 2026 | 第一人称视频 + GT 3D 场景地图 | 全局相机定位、人体姿态跟踪 | [官方网站](https://deguchihiroyuki.github.io/Map-Mono-Ego-Project/) |
| OVO-S-Bench | 2026 | 348 个视频 / 1,680 个空间 QA 对 | 流式空间具身推理 | [官方网站](https://internlm.github.io/OVO-S-Bench/) |
| ⭐ ADT (Aria Digital Twin) | 2023 | 200 个多模态序列，2 个室内场景 | 第一人称 3D 场景与身体感知 | [官方网站](https://www.projectaria.com/datasets/adt/) |
| PVSG | 2023 | 400 个全景片段 / ~15万 帧 | 第一人称全景场景图构建 | [GitHub](https://github.com/jingkang50/PVSG) |
| DR(eye)VE | 2018 | ~6 小时驾驶录像 / 55.5万 帧 | 驾驶员视线预测、汽车第一人称感知 | [官方网站](http://aimagelab.ing.unimore.it/dreyeve) |
| EgoCart | 2018 | 9 个零售 RGB‑D 序列 | 室内/购物车定位 | [官方网站](https://iplab.dmi.unict.it/EgocentricShoppingCartLocalization/) |
| IU ShareView | 2018 | 9 组配对的第一人称视频集 | 跨穿戴者实例分割与重识别 | [官方网站](http://vision.soic.indiana.edu/firstthird-eccv2018/) |
| OST | 2017 | 57 个室内序列 | 目标搜索、可穿戴视线跟踪 | [GitHub](https://github.com/Mengmi/deepfuturegaze_gan) |

---

### 2.7 具身智能与视觉‑语言‑行动 (Ego‑VLA)
将第一人称人类视频中的视觉、语言和行动信号对齐，将人类操作知识迁移到机器人智能体，是具身智能的核心流水线。本节也涵盖具身 AI 基准和从人类演示中学习机器人。

+  **HumanScale: Egocentric Human Video Can Outperform Real-Robot Data for Embodied Pretraining**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：系统比较第一人称人类视频和远程操作的真实机器人轨迹作为预训练数据源。在人类数据上预训练的模型验证损失降低 24%，在分布内和分布外任务上成功率分别提高 52.5% 和 90%
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.20521)
+  **HumanoidArena: Benchmarking Egocentric Hierarchical Whole-body Learning**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：一个用于第一人称层次化全身学习的仿真优先基准，将策略学习形式化为层次决策问题，包含 7 个腿部关键的 HOI/HSI 任务
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.17833)
+  **ACE-Ego-0: Unifying Egocentric Human and Robotic Data for VLA Pretraining**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：统一 VLA 预训练框架，联合利用异构数据源，通过可扩展的第一人称视频到动作流水线将原始人类视频转换为机器人格式的伪动作轨迹
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.17200)
+  **Motion-Focused Latent Action Enables Cross-Embodiment VLA Training from Human EgoVideos**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：解决第一人称人类操作视频中缺乏动作标签的问题，用于 VLA 训练
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16251)
+  **ActiveMimic: Egocentric Video Pretraining with Active Perception**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：一个预训练框架，从单个身体佩戴的 RGB 相机中恢复同步的相机和手腕轨迹，以解决第一人称视频与机器人数据预训练之间的性能差距
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.06194)
+  **EgoTSR: From Perception to Planning: Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning**
    - 发表：ICML 2026
    - 亮点：一个基于课程学习的框架，用于学习面向任务的时空推理。构建了包含 4,600 万个样本的 EgoTSR‑Data，分为三个阶段。在长时逻辑推理任务上达到 92.4% 准确率
    - 论文链接：[ICML](https://icml.cc/virtual/2026/poster/64173)
+  **EARL: Towards a Unified Analysis-Guided Reinforcement Learning Framework for Egocentric Interaction Reasoning and Pixel Grounding**
    - 发表：ICML 2026
    - 亮点：采用组相对策略优化 (GRPO) 增强 MLLM 在第一人称视觉中的交互理解
    - 论文链接：[ICML](https://icml.cc/virtual/2026/poster/64173)
+  **Ego3S: Select, Strengthen, and Synchronize for Efficient Egocentric Reasoning**
    - 发表：ICML 2026
    - 亮点：提出新颖的三阶段 Ego3S 框架，将模型的推理锚定在交互证据上，解决第一人称推理相比第三人称理解的独特挑战
    - 论文链接：[ICML](https://icml.cc/virtual/2026/poster/64173)
+  **Embodied VideoAgent: Persistent Memory from Egocentric Videos and Embodied Sensors Enables Dynamic Scene Understanding**
    - 发表：ICCV 2025
    - 亮点：一个基于 LLM 的智能体，从第一人称视频和具身传感器输入（深度和姿态感知）构建场景记忆。在 Ego4D‑VQ3D 上提升 6.5%，OpenEQA 上提升 2.6%，EnvQA 上提升 15.3%
    - 论文链接：[ICCV](https://www.openaccess.thecvf.com/content/ICCV2025/html/Fan_Embodied_VideoAgent_Persistent_Memory_from_Egocentric_Videos_and_Embodied_Sensors_ICCV_2025_paper.html) | [arXiv](http://arxiv.org/abs/2501.00358)
+  **Minerva-Ego: Spatiotemporal Hints for Egocentric Video Understanding**
    - 发表：CVPR 2025
    - 亮点：一个用于评估复杂第一人称视觉推理的基准，扩展了高质量视频数据源，包含挑战性的多步多模态问题和人工标注的密集时空推理痕迹
    - 论文链接：[CVPR](https://openaccess.thecvf.com/content/CVPR2025/html/Minerva-Ego_Spatiotemporal_Hints_for_Egocentric_Video_Understanding_CVPR_2025_paper.html)
+  **JoyAI-RA 0.1: A Foundation Model for Robotic Autonomy**
    - 发表：arXiv 2026 (2026年4月)
    - 亮点：VLA 具身基础模型，具有多源多层次预训练，整合网络数据、大规模第一人称人类操作视频、仿真轨迹和真实机器人数据
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.13863)
+  **EgoPush: Learning End-to-End Egocentric Multi-Object Rearrangement for Mobile Robots**
    - 发表：arXiv 2026 (2026年2月)
    - 亮点：一个策略学习框架，使移动机器人能够进行第一人称、感知驱动的重排，无需依赖显式全局状态估计。使用以对象为中心的潜在空间编码相对空间关系
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.18071)
+  **EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data**
    - 发表：arXiv 2026 (2026年2月)
    - 亮点：在超过 20,854 小时的动作标记第一人称人类视频上训练 VLA 模型，揭示了人类数据规模与验证损失之间的对数线性缩放规律
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.16710)
+  **Ego-Pi: VLA Fine-Tuning for Egocentric Human and Robot Data**
    - 发表：arXiv 2026
    - 亮点：针对在可穿戴人类视频上训练的双臂灵巧操作 VLA 的微调流水线
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.08107)
+  **ViterbiPlanNet: Injecting Procedural Knowledge via Differentiable Viterbi for Egocentric Task Planning**
    - 发表：CVPR 2026
    - 亮点：可微分 Viterbi 算法将逐步过程先验注入 VLA 规划模块
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.04265)
+  **OSCAR: Omni-Embodiment Skeleton-Conditioned World Action Model for Robotics**
    - 发表：arXiv 2026
    - 亮点：通用骨架条件世界‑动作模型，从第一人称人类演示中学习多机器人策略
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.04463)
+  **Co-training with Ego-centric Video and Demonstration for Robot Navigation Task**
    - 发表：arXiv 2026
    - 亮点：跨域协同训练将第一人称行走视频转换为移动机器人模仿数据集
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.01951)
+  **In-N-On: Scaling Egocentric Manipulation with in-the-wild and on-task Data**
    - 发表：arXiv 2025 (2025年11月)
    - 亮点：构建 PHSD 数据集，包含第一人称数据和直接对齐目标操作任务的任务内数据
    - 论文链接：[arXiv](https://arxiv.org/abs/2511.12643)
+  **EgoBridge: Domain Adaptation for Generalizable Imitation from Egocentric Human Videos**
    - 发表：NeurIPS 2025
    - 亮点：人类视觉‑行动分布的最优传输对齐，相比标准基线将模仿成功率提高 44%
    - 论文链接：[arXiv](https://arxiv.org/abs/2509.19626)
+  **EgoAgent: A Joint Predictive Agent Model in Egocentric Worlds**
    - 发表：ICCV 2025
    - 亮点：统一 Transformer 架构，整合第一人称视觉、语言、世界建模和行动决策头
    - 论文链接：[arXiv](https://arxiv.org/abs/2502.05857)

#### 📊 相关数据集与基准（程序化技能学习）
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
|  In-N-On (PHSD) | 2025 | 第一人称 + 任务内数据 | 操作策略学习 | [arXiv](https://arxiv.org/abs/2511.12643) |
| EgoVerse | 2026 | 1,362 小时 / ~8万 个任务片段 | 通用机器人操作预训练、具身基准测试 | [官方网站](https://egoverse.ai/) |
| EgoLive | 2026 | 大规模真实世界日常任务记录 | 非结构化机器人技能迁移 | [arXiv](https://arxiv.org/abs/2604.23570) |
| EgoMAGIC | 2026 | 3,355 个医疗任务视频 / 50 个临床工作流 | 手术动作检测与程序化辅助 | [Zenodo](https://doi.org/10.5281/zenodo.19239154) |
| HumanEgo | 2026 | 短 Aria 可穿戴演示序列 | 人‑机器人策略蒸馏 | [官方网站](https://humanego-ai.github.io/) |
| EgoSPT | 2026 | 11,515 个操作片段 / 112 个任务文件夹 | 空间提示条件操作轨迹生成 | [Hugging Face](https://huggingface.co/datasets/JackYFL233/EgoSPT) |
| Ego-EXTRA | 2026 | 50 小时 / 1.5万+ 教学 VQA 对 | 专家‑新手可穿戴辅助场景 | [官方网站](https://fpv-iplab.github.io/Ego-EXTRA/) |
| GM-100 | 2026 | 100+ 操作任务 / 1.3万 条轨迹 | 通用机器人技能评估基准 | [官方网站](https://www.rhos.ai/research/gm-100) |
| SABER | 2026 | 100+ 小时 / 4.48万 零售样本 | 购物机器人的具身 VLA 域适应 | [官方网站](https://dreamvu.ai/saber/) |
| EgoProactive / Pro²Bench | 2026 | 700 个可穿戴录像 / 4.2万 评估样本 | 主动式程序化可穿戴助手基准 | [Hugging Face](https://huggingface.co/datasets/facebook/wearable-ai) |
| EgoYC2 / Exo2EgoDVC | 2025 | ~43 小时烹饪录像 + 密集步骤字幕 | 家庭程序化跨视角对齐 | [GitHub](https://github.com/ut-vision/Exo2EgoDVC) |
| ⭐ EgoExoLearn | 2024 | 120 小时异步 ego/exo 配对片段 | 人类程序化学习模拟、机器人模仿 | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |
| ⭐ Assembly101 | 2022 | 513 小时多视角装配录像 | 分步工业程序化操作 | [官方网站](https://assembly-101.github.io/) |
| IndustReal | 2024 | ~6 小时工厂操作序列 | 工业步骤检测与错误识别 | [官方网站](https://timschoonbeek.github.io/industreal.html) |
| EgoProceL | 2022 | 62 个可穿戴视频 / 16 个家务任务 | 日常程序化学习基线 | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| EPIC-Tent | 2019 | 7+ 小时双 HMD 帐篷组装录像 + 眼动 | 多模态程序化活动分析 | [数据仓库](https://data.bris.ac.uk/data/dataset/2ite3tu1u53n42hjfh3886sa86) |
| CMU-MMAC | 2011 | 25 名参与者 / 5 个烹饪食谱 | 厨房程序化活动识别 | [官方网站](http://kitchen.cs.cmu.edu/) |
| GTEA Gaze | 2011 | 17 个烹饪环节 | 细粒度程序化动作 + 视线预测 | [官方网站](https://cbs.ic.gatech.edu/fpv/) |

---

### 2.8 第一人称世界模型
从第一人称观察中学习环境的演化规律，实现未来帧预测、合成交互视频生成和长时任务规划。

+  **EgoCS-400K: An Egocentric Gameplay Dataset for World Models**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：一个大规模、以重放为基础的第一人称 Counter‑Strike 数据集，用于世界模型，从公开的职业 CS 比赛回放中构建，保留人类游戏轨迹
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16186)
+  **AnchorWorld: Embodied Egocentric World Simulation with View-based Evolution Customization**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：锚点关键帧约束的可控第一人称模拟器，锚点匹配准确率达到 89%
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.07326)
+  **PlayerOne: Egocentric World Simulator**
    - 发表：NeurIPS 2025 (arXiv 2026年4月)
    - 亮点：首个支持无限制自由探索和全运动控制的照片级开放世界第一人称模拟器
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.06724)
+  **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - 发表：arXiv 2026 (2026年3月)
    - 亮点：首个以 HOI 为中心的第一人称扩散世界模型，嵌入物理先验
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.13615)
+  **WEM: World-Ego Modeling for Long-Horizon Evolution in Hybrid Embodied Tasks**
    - 发表：arXiv 2026
    - 亮点：解耦静态场景 + 动态自身分支的世界建模架构，用于长序列预测
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.19957)
+  **EgoExo-WM: Unlocking Exo Video for Ego World Models**
    - 发表：arXiv 2026
    - 亮点：跨视角知识迁移流水线，利用丰富的第三人称录像增强第一人称世界模型训练
    - 论文链接：[arXiv](https://arxiv.org/pdf/2605.15477)
+  **EgoSim: Egocentric World Simulator for Embodied Interaction Generation**
    - 发表：arXiv 2026
    - 亮点：闭环交互模拟器，具有持久的动态 3D 场景状态，用于生成连续的合成交互视频
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.01001)
+  **EgoForge: Goal-Directed Egocentric World Simulator**
    - 发表：arXiv 2026
    - 亮点：目标条件生成模拟器，产生与用户指定任务目标匹配的未来第一人称序列
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.20169)
+  **Walk through Paintings: Egocentric World Models from Internet Priors**
    - 发表：arXiv 2026
    - 亮点：利用网络视频先验，将预训练的视频扩散模型重新用作动作条件的第一人称世界模型
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.15284)
+  **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - 发表：ICLR 2026
    - 亮点：首个通过第一人称交互世界建模量化具身认知的基准，揭示 VLM 在逆任务上比前向预测表现更好
    - 论文链接：[OpenReview](https://openreview.net/forum?id=Patx6MRipw)
+  **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - 发表：NeurIPS 2025
    - 亮点：可泛化的 HOI 世界模型，包含两阶段 VLM 先验推理 + DiT 流匹配轨迹生成
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)

#### 📊 相关数据集与基准（世界模型预训练与视频生成）
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| ⭐ Ropedia Xperience-10M | 2026 | 1000万 多模态人类体验片段 | 大规模第一人称世界模型预训练 | [Hugging Face](https://huggingface.co/datasets/ropedia-ai/xperience-10m) |
| DreamDojo-HV | 2026 | 大规模第一人称合成录像 | 生成式世界模型训练 | [arXiv](https://arxiv.org/abs/2602.06949) |
| Ego-1K | 2026 | 多视角第一人称视频片段 | 神经 3D/4D 动态场景合成 | [Hugging Face](https://huggingface.co/datasets/facebook/ego-1k) |
| In-lab | 2026 | 桌面操作轨迹序列 | 小规模技能世界模型微调 | [arXiv](https://arxiv.org/abs/2602.06949) |
| HumanNet | 2026 | ~100万 小时以人为中心的视频语料 | 通用 VLA 与世界模型预训练 | [arXiv](https://arxiv.org/abs/2605.06747) |
| MobileEgo Anywhere | 2026 | 200 小时智能手机第一人称日常录像 | 轻量级长形式世界模型训练 | [arXiv](https://arxiv.org/abs/2605.05945) |
| EgoEdit | 2025 | 10万 个第一人称视频编辑对 | 条件第一人称视频生成基准 | [官方网站](https://snap-research.github.io/EgoEdit) |
| EgoVid-5M | 2024 | 500万 个多样化第一人称视频片段 | 基础生成式第一人称视频数据集 | [官方网站](https://egovid.github.io/) |

---

### 2.9 第一人称程序化 AI 助手
专注于构建分步指导的第一人称 AI 助手，支持用户完成日常和专业程序化任务。本方向围绕三个核心能力组织——程序化错误检测、程序化学习和程序化问答，并由实时流处理和主动交互两个支撑维度提供支持。

#### 2.9.1 程序化错误检测
+  **Plan, Watch, Recover: A Benchmark and Architectures for Proactive Procedural Assistance**
    - 发表：arXiv 2026 (2026年6月)
    - 亮点：发布 EgoProactive，一个大规模的、用于主动程序化辅助的可穿戴第一人称数据集
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.06220)
+  **Modeling Multiple Normal Action Representations for Error Detection in Procedural Tasks**
    - 发表：CVPR 2025
    - 亮点：建模多种正常动作表示，以提高跨不同执行模式的错误检测鲁棒性
    - 论文链接：[arXiv](https://arxiv.org/abs/2504.06021)
+  **Gazing Into Missteps: Leveraging Eye-Gaze for Unsupervised Mistake Detection in Egocentric Videos of Skilled Human Activities**
    - 发表：CVPR 2025
    - 亮点：首个利用眼动信号进行熟练程序化活动无监督错误检测的方法
    - 论文链接：[arXiv](https://arxiv.org/abs/2504.07892)
+  **Transparent and Coherent Procedural Mistake Detection**
    - 发表：EMNLP 2025
    - 亮点：为检测到的程序化错误生成透明、连贯的自然语言解释
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.08765)
+  **PREGO: Online Mistake Detection in PRocedural EGOcentric Videos**
    - 发表：CVPR 2024
    - 亮点：专为第一人称程序化视频量身定制的在线实时错误检测框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2404.01688)
+  **TI-PREGO: Chain of Thought and In-Context Learning for Online Mistake Detection in PRocedural EGOcentric Videos**
    - 发表：arXiv 2024
    - 亮点：通过思维链和上下文学习增强 PREGO，改进在线错误检测
    - 论文链接：[arXiv](https://arxiv.org/abs/2410.05678)
+  **EgoOops: A Dataset for Mistake Action Detection from Egocentric Videos Referring to Procedural Texts**
    - 发表：ICCV 2024
    - 亮点：首个与程序化文本指令对齐的第一人称错误动作检测数据集
    - 论文链接：[项目页面](https://ego-oops.github.io/)
+  **Error Detection in Egocentric Procedural Task Videos**
    - 发表：CVPR 2024
    - 亮点：第一人称程序化错误检测的系统性基准和基线框架
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/Li_Error_Detection_in_Egocentric_Procedural_Task_Videos_CVPR_2024_paper.html)

#### 2.9.2 程序化学习
+  **Task Graph Maximum Likelihood Estimation for Procedural Activity Understanding in Egocentric Videos**
    - 发表：arXiv 2025 (2025年2月)
    - 亮点：引入基于梯度的方法，通过最大似然优化边权重，从程序化活动中学习任务图
    - 论文链接：[arXiv](https://arxiv.org/abs/2502.08123)
+  **HiERO: Understanding the Hierarchy of Human Behavior Enhances Reasoning on Egocentric Videos**
    - 发表：ICCV 2025
    - 亮点：层次化行为理解框架，显著提升第一人称程序化推理性能
    - 论文链接：[项目页面](https://github.com/facebookresearch/hiero)
+  **Procedure Learning via Regularized Gromov-Wasserstein Optimal Transport**
    - 发表：arXiv 2025
    - 亮点：基于正则化 Gromov‑Wasserstein 最优传输的程序化学习方法
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.12456)
+  **OPEL: Optimal Transport Guided ProcedurE Learning**
    - 发表：NeurIPS 2024
    - 亮点：最优传输引导的无监督程序化学习框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2410.08765)
+  **United We Stand, Divided We Fall: UnityGraph for Unsupervised Procedure Learning from Videos**
    - 发表：WACV 2024
    - 亮点：基于 UnityGraph 的无监督程序化学习，从未标注的教学视频中学习
    - 论文链接：[arXiv](https://arxiv.org/abs/2311.04567)
+  **STEPs: Self-Supervised Key Step Extraction and Localization from Unlabeled Procedural Videos**
    - 发表：ICCV 2023
    - 亮点：从无标签程序化视频中自监督提取和定位关键步骤
    - 论文链接：[项目页面](https://steps-procedural.github.io/)
+  **My View is the Best View: Procedure Learning from Egocentric Videos**
    - 发表：ECCV 2022
    - 亮点：首个专为第一人称视角设计的程序化学习框架
    - 论文链接：[项目页面](https://github.com/ShyamNarasimhan/Procedure-Learning-from-Egocentric-Videos)
+  **Learning To Recognize Procedural Activities with Distant Supervision**
    - 发表：CVPR 2022
    - 亮点：基于远程监督的程序化活动识别框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2204.02345)

#### 2.9.3 程序化问答
+  **Grounded Multi-Hop VideoQA in Long-Form Egocentric Videos**
    - 发表：AAAI 2025
    - 亮点：处理长形式第一人称视频中的多跳视频问答问题
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/33925)
+  **EASG-Bench: Video Q&A Benchmark with Egocentric Action Scene Graphs**
    - 发表：arXiv 2025 (2025年8月)
    - 亮点：一个问答基准，其中 QA 对从动态场景图（捕获行为者、动作和物体之间的关系）中时空接地创建
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.01867)
+  **EOC-Bench: Can MLLMs Identify, Recall, and Forecast Objects in an Egocentric World?**
    - 发表：arXiv 2025 (2025年6月)
    - 亮点：一个旨在系统评估动态第一人称场景中物体中心具身认知的基准
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.05287)
+  **EgoNight: Towards Egocentric Vision Understanding at Night with a Challenging Benchmark**
    - 发表：arXiv 2025
    - 亮点：首个以 VQA 为核心任务的夜间第一人称视觉综合基准
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.08961)
+  **EgoLife: Towards Egocentric Life Assistant**
    - 发表：CVPR 2025
    - 亮点：一个开发第一人称生活助手的项目，通过 AI 驱动的可穿戴眼镜陪伴并提升个人效率
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2025/html/EgoLife_Towards_Egocentric_Life_Assistant_CVPR_2025_paper.html)
+  **RAVEN: Query-Guided Representation Alignment for Question Answering over Audio, Video, Embedded Sensors, and Natural Language**
    - 发表：arXiv 2025
    - 亮点：多模态 QA 框架，对齐音频、视频、嵌入式传感器和自然语言，用于程序化场景
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.06789)
+  **EgoTextVQA: Towards Egocentric Scene-Text Aware Video Question Answering**
    - 发表：CVPR 2025
    - 亮点：首个整合场景文本信息的第一人称视频 QA 基准
    - 论文链接：[项目页面](https://egotextvqa.github.io/)
+  **Omnia de Egotempo: Benchmarking Temporal Understanding of Multi-Modal LLMs in Egocentric Videos**
    - 发表：CVPR 2025
    - 亮点：多模态 LLM 在第一人称程序化视频上的时序推理能力基准
    - 论文链接：[arXiv](https://arxiv.org/abs/2504.09876)
+  **Vinci: A Real-time Smart Assistant Based on Egocentric Vision-language Model for Portable Devices**
    - 发表：ACM 2025
    - 亮点：轻量级边缘可部署 Ego‑VLM，用于程序化助手场景
    - 论文链接：[arXiv](https://arxiv.org/abs/2412.21080)
+  **Grounded Question-Answering in Long Egocentric Videos**
    - 发表：CVPR 2024
    - 亮点：长第一人称程序化视频的接地 QA 框架
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_Grounded_Question-Answering_in_Long_Egocentric_Videos_CVPR_2024_paper.html)

#### 2.9.4 实时流处理与主动交互
+  **Dispider: Enabling Video LLMs with Active Real-Time Interaction via Disentangled Perception, Decision, and Reaction**
    - 发表：CVPR 2025
    - 亮点：解耦感知‑决策‑反应框架，用于实时交互视频 LLM
    - 论文链接：[项目页面](https://dispider.github.io/)
+  **StreamBridge: Turning Your Offline Video Large Language Model into a Proactive Streaming Assistant**
    - 发表：NeurIPS 2025
    - 亮点：无需重新训练即可将离线视频 LLM 转换为主动流式助手
    - 论文链接：[项目页面](https://streambridge-vlm.github.io/)
+  **Flash-VStream: Efficient Real-Time Understanding for Long Video Streams**
    - 发表：ICCV 2025
    - 亮点：用于长时视频流的高效实时理解流水线
    - 论文链接：[项目页面](https://github.com/yydlm/Flash-VStream)
+  **Proactive Agent: Shifting LLM Agents from Reactive Responses to Active Assistance**
    - 发表：ICLR 2025
    - 亮点：将 LLM 智能体从反应式响应转变为主动式程序化辅助的范式转换
    - 论文链接：[arXiv](https://arxiv.org/abs/2502.01234)
+  **YETI (YET to Intervene) Proactive Interventions by Multimodal AI Agents in Augmented Reality Tasks**
    - 发表：arXiv 2025
    - 亮点：多模态 AI 智能体在 AR 程序化任务中的主动干预框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2504.56789)
+  **Proactive Assistant Dialogue Generation from Streaming Egocentric Videos**
    - 发表：EMNLP 2025
    - 亮点：从流式第一人称程序化视频生成上下文感知的主动助手对话
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.12345)
+  **VideoLLM-online: Online Video Large Language Model for Streaming Video**
    - 发表：CVPR 2024
    - 亮点：专为流式第一人称视频输入设计的在线视频 LLM 框架
    - 论文链接：[arXiv](https://arxiv.org/abs/2404.09876)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 会议 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
|  EgoProactive | 2026 | arXiv | 主动程序化辅助 | [arXiv](https://arxiv.org/abs/2606.06220) |
|  EASG-Bench | 2025 | arXiv | 基于动作场景图的视频 QA | [arXiv](https://arxiv.org/abs/2508.01867) |
|  EOC-Bench | 2025 | arXiv | 物体中心具身认知 | [arXiv](https://arxiv.org/abs/2506.05287) |
|  EgoNight | 2025 | arXiv | 夜间第一人称 VQA | [arXiv](https://arxiv.org/abs/2510.08961) |
| OVO-Bench | 2025 | CVPR | 在线实时视频理解基准 | [项目页面](https://ovo-bench.github.io/) |
| SVBench | 2025 | ICLR | 流式视频理解与多轮对话 | [项目页面](https://svbench.github.io/) |
| ProactiveVideoQA | 2025 | arXiv | 视频 LLM 主动交互评估 | [arXiv](https://arxiv.org/abs/2504.12345) |
| STREAMGAZE | 2025 | arXiv | 视线引导的主动流式视频理解 | [arXiv](https://arxiv.org/abs/2505.67890) |
| CaptainCook4D | 2024 | NeurIPS | 程序化错误检测、4D 活动理解 | [项目页面](https://captaincook4d.github.io/) |
| EgoOops | 2024 | ICCV | 基于程序化文本的错误动作检测 | [项目页面](https://ego-oops.github.io/) |
| IndustReal | 2024 | WACV | 工业程序化步骤识别、错误检测 | [项目页面](https://timschoonbeek.github.io/industreal.html) |
| HoloAssist | 2023 | ICCV | 交互式程序化 AI 助手、错误检测 | [项目页面](https://holoassist.github.io/) |
| EgoProceL | 2022 | CVPR | 第一人称程序化学习基准 | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| Assembly101 | 2022 | CVPR | 多视角程序化装配活动理解 | [官方网站](https://assembly-101.github.io/) |
| EgoExoLearn | 2024 | CVPR | 跨视角程序化学习（从演示到实践） | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |

---

### 2.10 🛡️ 第一人称数据安全与隐私保护

随着可穿戴相机和第一人称视频数据的快速普及，数据安全与隐私已成为第一人称视觉中的关键问题。与传统的第三人称视觉不同，第一人称视频天然携带穿戴者的身份、行为习惯、社交关系及环境背景等高度敏感信息，且旁观者往往在不知情的情况下被记录。本节从**隐私风险评估与基准构建**、**匿名化与数据脱敏**、**隐私保护技术**以及**伦理与政策**四个维度进行总结。

#### 2.10.1 隐私风险评估与基准
+  **Position: Life‑Logging Video Streams Make the Privacy‑Utility Trade‑off Inevitable**
    - 发表：arXiv 2026
    - 亮点：系统分析生活日志视频流在感知、传输和存储全链路中的隐私风险，指出现有单点隐私保护方法在跨视角协作场景中的局限性
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.10404)
+  **EgoPrivacy: What Your First-Person Camera Says About You?**
    - 发表：ICML 2025
    - 亮点：首个大规模第一人称隐私风险评估基准，系统回答“从第一人称视频中能推断出关于穿戴者的哪些信息”。涵盖三类隐私（人口统计、个体、情境），定义七个从细粒度到粗粒度的隐私恢复任务。提出检索增强攻击，利用第一人称到第三人称检索增强人口统计隐私攻击的有效性。实验表明，基础模型在零样本下即可恢复身份、场景、性别、种族等属性，准确率 70‑80%
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.12258) | [GitHub](https://github.com/williamium3000/ego-privacy)
+  **EgoNormia: Benchmarking Physical‑Social Norm Understanding**
    - 发表：ACL 2025 Findings
    - 亮点：构建了包含 1,853 个多项选择题的规范理解基准，涵盖安全、隐私、空间距离、礼貌、合作、协调/主动性、沟通/可读性七类规范。评估显示当前最先进的 VLM 在 EgoNormia 上最高仅 54%，揭示在真实世界智能体应用中存在显著的安全和隐私风险
    - 论文链接：[ACL Anthology](https://aclanthology.org/2025.findings-acl.985/)
+  **EAPrivacy: Benchmarking Physical-World Privacy Awareness of LLM-Powered Agents**
    - 发表：arXiv 2025
    - 亮点：引入一个综合评估基准，用于量化 LLM 驱动的具身智能体在物理世界中的隐私意识
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.12258)

#### 2.10.2 匿名化与数据脱敏
+  **EgoBlur: Responsible Innovation in Aria**
    - 发表：Meta Reality Labs (arXiv 2023)
    - 亮点：Project Aria 的核心匿名化系统，在数据采集阶段即对旁观者面部和车辆车牌进行模糊化处理。采用 FasterRCNN 作为目标检测器，对检测到的 PII 区域进行高斯模糊
    - 论文链接：[arXiv](https://arxiv.org/abs/2308.13093)
+  **Ego4D Privacy & Ethics Framework**
    - 发表：Ego4D 数据集文档
    - 亮点：Ego4D 数据集（3,670 小时，931 名参与者，9 个国家）采用严格的隐私和伦理标准进行采集。参与者可自愿选择模糊处理，其中 612 小时在参与者同意下保持未模糊状态。数据集采用完善的去标识化流程，并公开了详细的隐私保护标准
    - 论文链接：[Ego4D Privacy Page](https://ego4d-data.org/pages/privacy-and-ethics)

#### 2.10.3 隐私保护技术
+ **边缘端隐私过滤**
    +  **Extra‑Lightweight AI‑Based Privacy Preserving Framework for Egocentric Wearable Cameras (EPIC)**
        - 发表：CVPR 2025 Workshops
        - 亮点：为资源受限的可穿戴相机提出超轻量级 AI 隐私保护框架。采用 st_yolo_lc_v1 模型进行人脸检测，并在存储或发送图像前模糊化细节信息。在仅 640 KB RAM 的 STM32L4 MCU 上实现，人脸检测 mAP 达 41.38%
        - 论文链接：[OpenAccess CVF](https://openaccess.thecvf.com/content/CVPR2025W/MTF/html/Li_Extra-Lightweight_AI-Based_Privacy_Preserving_Framework_for_Egocentric_Wearable_Cameras_CVPRW_2025_paper.html)

#### 2.10.4 伦理、政策与社会影响
+  **Privacy and Ethical Challenges in Egocentric Data Collection**
    - 发表：The Indian Express / Moneycontrol 2026
    - 亮点：报道了印度成为第一人称 AI 数据采集热点的现状及其引发的隐私担忧。指出第一人称录像可能无意中捕获面部、私人对话、敏感工作流程或未同意被记录的旁观者，引发关于监控、同意和劳动力替代的伦理问题
    - 论文链接：[The Indian Express](https://indianexpress.com/) | [Moneycontrol](https://www.moneycontrol.com/)
+  **Smart Glasses and GDPR: Europe's Regulatory Crackdown**
    - 发表：GDPR Local 2026
    - 亮点：报道了欧洲数据保护机构、MEPs 和 EDPB 对智能眼镜的严格审查，核心问题在于被相机捕获的旁观者无法以实际方式同意被拍摄。法国 CNIL 和 EDPB 均于 2026 年启动专项工作，EDPB 关于智能眼镜“社会可接受性”的报告预计于 2026 年夏季发布
    - 论文链接：[GDPR Local](https://gdprlocal.com/)

#### 📊 相关数据集与资源
| 名称 | 类型 | 年份 | 核心内容 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
|  EgoPrivacy | 隐私风险评估基准 | 2025 | 三类隐私、七项隐私恢复任务 | [GitHub](https://github.com/williamium3000/ego-privacy) |
|  EgoNormia | 规范理解基准 | 2025 | 1,853 个 MCQ，涵盖七类规范（含隐私） | [ACL](https://aclanthology.org/2025.findings-acl.985/) |
|  EgoBlur | 匿名化系统 | 2023 | 面部和车牌的实时模糊处理 | [arXiv](https://arxiv.org/abs/2308.13093) |
| Ego4D Privacy Policy | 数据集隐私框架 | 2022 | 去标识化流程、参与者同意机制 | [Ego4D](https://ego4d-data.org/pages/privacy-and-ethics) |

---

## 📊 数据集、基准与模拟器

### 通用大规模第一人称数据集
| 数据集名称 | 发布年份 | 规模 | 核心支持任务 | 官方链接 |
| :--- | :--- | :--- | :--- | :--- |
|  HD-EPIC | 2025 | 41 小时超高清烹饪录像 + 密集多层标注 | 细粒度活动理解、密集 VQA、多模态对齐 | [arXiv](https://arxiv.org/pdf/2502.04144) |
| Ego-Exo4D | 2024 | 1,286 小时同步第一/第三人称多模态片段 | 跨视角对齐、人类技能分析、4D 重建 | [官方网站](https://ego-exo4d-data.org/) |
| Ego4D | 2022 | 3,670 小时可穿戴视频，9 个国家 923 名参与者 | 动作识别、情景记忆、社交交互、3D 人体姿态 | [官方网站](https://ego4d-data.org/) |
| EPIC-KITCHENS-100 | 2020 | 100 小时厨房录像，9万 个标注动作片段 | 动作检测、识别、未来预测 | [官方网站](https://epic-kitchens.github.io/) |

### 细粒度任务专用数据集
#### 物体与 HOI 子集合
+  **EgoObjects**
    - 发布：ICCV 2023
    - 规模：初始版本包含 9,000+ 个视频，由 50 多个国家/地区的 250 名参与者使用 4 种可穿戴设备采集，包含 368 个物体类别的 65万+ 物体标注
    - 核心任务：细粒度物体理解
    - 链接：https://github.com/facebookresearch/EgoObjects
+  **EgoXtreme**
    - 发布：CVPR 2026
    - 规模：具有挑战性的第一人称 6D 姿态数据集，包含运动模糊、严重遮挡和极端光照变化
    - 核心任务：可穿戴相机的鲁棒物体 6D 姿态估计
    - 链接：https://arxiv.org/pdf/2603.25135
+  **TouchMoment**
    - 发布：CVPR 2026
    - 规模：15万 帧，标注了精确的接触开始/结束时间戳和接触类别
    - 核心任务：细粒度手物接触时刻检测
    - 链接：https://arxiv.org/pdf/2604.12343
+  **EgoPressure**
    - 发布：arXiv 2024
    - 规模：5 小时多模态录像，包含同步的触觉压力图、IMU 信号和 RGB
    - 核心任务：触觉感知的手物交互建模
    - 链接：https://arxiv.org/pdf/2409.02224

#### 程序化任务子集合
+  **CaptainCook4D**
    - 发布：NeurIPS 2024
    - 规模：烹饪程序化视频，带有 4D 标注和错误标签
    - 核心任务：程序化错误检测、步骤理解
    - 链接：https://captaincook4d.github.io/
+  **EgoOops**
    - 发布：ICCV 2024
    - 规模：与程序化文本对齐的错误动作检测数据集
    - 核心任务：基于文本引用的第一人称错误检测
    - 链接：https://ego-oops.github.io/
+  **IndustReal**
    - 发布：WACV 2024
    - 规模：~6 小时工业装配视频，带有执行错误标注
    - 核心任务：工业程序化步骤识别、错误检测
    - 链接：https://timschoonbeek.github.io/industreal.html

#### 长视频与情景记忆数据集
+  **EgoLife**
    - 发布：CVPR 2025
    - 规模：6 名共同居住参与者的连续多日录像，带有密集的日常事件标签
    - 核心任务：长期生活日志记忆检索与个人事件 QA
    - 链接：https://arxiv.org/pdf/2503.03803
+  **EgoSchema**
    - 发布：NeurIPS 2023
    - 规模：500+ 个长第一人称片段，带有多步时序推理选择题
    - 核心任务：超长时视频语言理解基准
    - 链接：https://github.com/egoschema/EgoSchema

#### 专用领域数据集
+  **EgoExOR**
    - 发布：NeurIPS 2025
    - 规模：手术室可穿戴视频，同步手术工具跟踪和患者生物特征
    - 核心任务：手术工作流识别、器械检测
    - 链接：https://arxiv.org/pdf/2505.24287
+  **EgoDex**
    - 发布：2025
    - 规模：Apple Vision Pro 捕获的日常物体操作序列，带有精确的 6D 手部姿态标注
    - 核心任务：灵巧可穿戴手部姿态估计与操作预测
    - 链接：https://arxiv.org/abs/2505.11709
+  **MECCANO**
    - 发布：2021
    - 规模：12 小时工业装配录像，配有眼动跟踪流
    - 核心任务：工业细粒度动作与手物交互分析
    - 链接：https://github.com/fpv-iplab/MECCANO
+  **EgoExo-Fitness**
    - 发布：ECCV 2024
    - 规模：从同步的第一人称和固定第三人称相机录制的健身序列视频
    - 核心任务：全身动作理解
    - 链接：[GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness)

### 具身 VLA 评估基准
+  **EgoVerse**
    - 发布：2026
    - 规模：1,000+ 个标准化具身任务，涵盖导航、操作和视觉 QA
    - 核心任务：统一机器人模仿与可穿戴 VLA 评估套件
    - 链接：https://arxiv.org/pdf/2604.07607
+  **EgoBench**
    - 发布：2026
    - 规模：可穿戴具身智能体的交互式闭环评估平台
    - 核心任务：实时交互决策基准
    - 链接：https://arxiv.org/pdf/2605.27820

### 第一人称世界模拟器
+  **PlayerOne**
    - 发布：NeurIPS 2025
    - 亮点：照片级开放世界第一人称模拟器，支持完整的相机、人体运动和物体交互控制，用于合成数据生成
    - 链接：https://arxiv.org/abs/2512.06724
+  **EgoSim**
    - 发布：arXiv 2026
    - 亮点：闭环动态模拟器，具有持久的 3D 场景状态，用于生成一致的连续交互录像
    - 链接：https://arxiv.org/pdf/2604.01001

---

## 👓 智能眼镜专属研究与部署

### 专用基准与可穿戴数据集
+  **SUPERGLASSES: Benchmarking Vision Language Models as Intelligent Agents for AI Smart Glasses**
    - 发表：CVPR 2026
    - 亮点：首个真实消费级智能眼镜基准，收集自 Ray‑Ban Meta、Xiaomi Smart Glasses 和 Thunderbird V4，覆盖多样化日常场景
    - 论文链接：[arXiv](https://arxiv.org/pdf/2602.22683)
+  **Project Aria Datasets**
    - 发布者：Meta Research
    - 亮点：完整的可穿戴多模态数据集套件，包含同步的 RGB、深度、IMU 和眼动信号
    - 官方链接：https://www.projectaria.com/

### 关键技术研究方向
#### 低功耗设备端感知
+  **OpenGlass: Ultra-Low-Power On-Device AI Eyewear with Event-based Vision**
    - 发表：arXiv 2026
    - 亮点：完全开源的事件相机可穿戴硬件栈，配合轻量级边缘推理算法
    - 论文链接：[arXiv](https://arxiv.org/pdf/2606.07431)
+  **EgoTrigger: Toward Audio-Driven Image Capture for Human Memory Enhancement in All-Day Energy-Efficient Smart Glasses**
    - 所属机构：UNC Chapel Hill + Google
    - 发表：IEEE TVCG 2025
    - 亮点：音频事件触发的选择性帧捕获，总功耗降低 87%
    - 论文链接：[arXiv](https://arxiv.org/pdf/2508.01915)

#### 终身记忆与个人助理系统
+  **EGAgent: Agentic Very Long Video Understanding**
    - 发表：arXiv 2026
    - 亮点：基于实体场景图的推理智能体，处理跨天的连续可穿戴视频流，支持多跳检索和音视频混合搜索
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.18157)

#### 自然可穿戴人机交互
+  **VisionClaw: Always-On AI Agents Through Smart Glasses**
    - 发表：arXiv 2026
    - 亮点：持久的后台可穿戴智能体，支持免提多场景任务执行
    - 论文链接：[arXiv](https://arxiv.org/pdf/2604.03486)
+  **Egocentric Co-Pilot: Web-Native Lightweight Smart Glasses Assistant**
    - 发表：WWW 2026
    - 亮点：基于浏览器的轻量级可穿戴助手架构，无需本地应用安装
    - 论文链接：[arXiv](https://arxiv.org/pdf/2603.01104)
+  **Plug-and-Play Clarifier: A Zero-Shot Multimodal Framework for Egocentric Intent Disambiguation**
    - 发表：AAAI 2026
    - 亮点：零样本意图消歧框架，将可穿戴指令执行准确率从 58% 提升至 87%
    - 论文链接：[arXiv](https://arxiv.org/pdf/2511.08971)

---

## 🔗 相关 Awesome 列表
- [Awesome-Egocentric](https://github.com/EgoAlpha/Awesome-Egocentric)
- [awesome-egocentric-vision](https://github.com/Sid2697/awesome-egocentric-vision)
- [Awesome-Egocentric-and-Exocentric-Vision](https://github.com/ayiyayi/Awesome-Egocentric-and-Exocentric-Vision)
- [Building Egocentric Procedural AI Assistant](https://github.com/z1oong/Building-Egocentric-Procedural-AI-Assistant)

---

## 🎯 关键研究挑战

### 所有子任务的通用基础挑战
1. **第一人称视觉的内在缺陷**：狭窄视野、严重自遮挡、剧烈相机抖动、不稳定的光照和模糊的可穿戴图像质量降低所有下游任务性能。
2. **第一人称数据稀缺与隐私障碍**：可穿戴录像携带敏感个人信息；采集和标注成本远高于互联网第三人称视频，造成数量级的数据集规模差距，限制大模型扩展。跨视角协作场景进一步放大隐私风险。
3. **严重的人际分布偏移**：用户身高、日常行为模式和家庭环境的巨大差异导致通用模型在个性化可穿戴场景上泛化性能差。
4. **超长序列建模瓶颈**：全天候连续可穿戴流式数据给现有视频和多模态架构带来了关键的记忆容量和长程依赖建模挑战。

### 各方向核心挑战
| 研究方向 | 核心开放挑战 |
| :--- | :--- |
| 动作识别与预测 | 细粒度动词‑名词组合歧义，未修剪长视频上时序定位精度低 |
| 手物交互 (HOI) | 接触状态标注成本高，物理一致性约束难以建模，手与物体之间严重相互遮挡 |
| Ego‑VLM 与多模态推理 | 缺乏第一人称常识先验，弱时空多步推理，模糊的自然语言物体指代定位 |
| 长视频与结构化推理 | 模型上下文窗口有限，时序事件定位模糊，跨多小时的因果推理弱 |
| 注视与用户意图预测 | 眼动模式个体差异大，隐含意图难以标注，弱多模态信号对齐 |
| 3D/4D 重建与结构化感知 | 单目深度歧义，动态运动物体重建失败，鱼眼畸变校正开销大 |
| Ego‑VLA 与具身 AI | 人‑机器人具身差异大，动作空间未对齐，物理交互世界知识不足 |
| 第一人称世界模型 | 长 rollout 中时序一致性退化，生成真实性与物理合理性之间的权衡，用户动作可控性弱 |
| 第一人称程序化 AI 助手 | 细粒度错误边界模糊，程序化知识接地困难，实时主动干预时机控制 |
| 数据安全与隐私 | 平衡穿戴者与旁观者隐私，数据最小化中的隐私‑效用权衡，GDPR 等法规合规性，跨视角协作中的隐私放大 |

---

## ❤️ 联系方式
如果您有论文/数据集建议、更正，或发现此资源列表有用，欢迎通过邮箱联系孙源良：sun254667307@gmail.com。
如果您想找egocentric vision研究方向的实习，欢迎随时联系我。

## ⭐ 致谢
本精选集合参考并构建于多个社区第一人称视觉资源库：
- Awesome-Egocentric-Video-Datasets
- Building Egocentric Procedural AI Assistant

## 📄 许可证
CC0 1.0 通用。完整条款请见本仓库的 `LICENSE` 文件。
