<div align="center">

# 🎥 Awesome Egocentric Vision（优秀第一人称视觉资源精选）

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

> 一份精心策划、面向学习的**第一人称（egocentric）视觉与具身AI**资源列表：涵盖论文、数据集、代码、模型、工具包、挑战赛和教程，既包括经典基础工作，也包含前沿进展，适合研究入门和工业部署。

✅ **收录标准**
+ 优先收录来自 CVPR / ICCV / ECCV / NeurIPS / ICLR / AAAI / TPAMI / TVCG 等顶级会议和期刊的高质量工作。
+ 覆盖核心前沿方向：Ego‑VLM/LLM、Ego‑VLA 具身智能、3D/4D 重建、手‑物交互、视线估计、长视频理解、世界模型。

---

## 📑 目录
1. [📚 综述与概述](#-综述与概述)
2. [🔬 核心研究主题](#-核心研究主题)
    - 2.1 动作识别、检测与预测
    - 2.2 手‑物交互与细粒度活动
    - 2.3 第一人称视觉‑语言模型与多模态推理
    - 2.4 长视频理解与结构化推理
    - 2.5 视线、注意力与意图预测
    - 2.6 3D/4D 重建与结构化感知
    - 2.7 具身AI与视觉‑语言‑动作（Ego‑VLA）
    - 2.8 第一人称世界模型
    - 2.9 第一人称程序化AI助手
    - 2.10 第一人称数据安全与隐私保护
3. [📊 数据集、基准与模拟器](#-数据集基准与模拟器)
4. [👓 智能眼镜专项研究与部署](#-智能眼镜专项研究与部署)
5. [🔗 相关Awesome列表](#-相关awesome列表)
6. [🎯 关键研究挑战](#-关键研究挑战)

---

## 📚 综述与概述
适合入门该领域的首选材料，帮助快速建立全局认识，梳理发展脉络、核心任务和关键挑战。

+  **Challenges and Trends in Egocentric Vision: A Survey（第一人称视觉的挑战与趋势综述）**
    - 发表：arXiv 2025
    - 亮点：该领域最新的全景综述，系统划分四大任务方向：主体理解、客体理解、环境理解和混合理解，全面总结了挑战与趋势。
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.15275)
    - 微信文章：https://mp.weixin.qq.com/s/Nm1UOZ8wa3VnXNNeAQMiHw

+  **Building Egocentric Procedural AI Assistant: Methods, Benchmarks, and Challenges（构建第一人称程序化AI助手：方法、基准与挑战）**
    - 发表：arXiv 2025
    - 亮点：首次系统提出了第一人称程序化AI助手的完整技术框架，定义了三大核心任务（错误检测、程序化学习、视觉问答）以及两个支撑维度（实时流处理和主动交互）。
    - 论文链接：[arXiv](https://arxiv.org/abs/2511.13261)

+  **Bridging Perspectives: A Survey on Cross-view Collaborative Intelligence with Egocentric-Exocentric Vision（跨视角协同智能综述：第一人称与第三人称视觉的桥梁）**
    - 发表：arXiv 2025
    - 亮点：系统梳理了第一人称‑第三人称协同学习方向，涵盖三种范式：第三人称辅助第一人称、第一人称辅助第三人称、以及联合学习。
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.06253)

+ **An Outlook into the Future of Egocentric Vision（第一人称视觉的未来展望）**
    - 发表：IJCV 2024
    - 亮点：由该领域权威学者合著，结合可穿戴计算的未来场景，梳理了研究不足和待突破的方向。
    - 论文链接：[arXiv](https://arxiv.org/abs/2308.07123)

+ **First-Person Vision（第一人称视觉）**
    - 发表：Proceedings of the IEEE 2012
    - 亮点：该领域的奠基性综述，首次正式定义了第一人称视觉的研究范围、核心挑战和应用方向。
    - 论文链接：[IEEE Xplore](https://ieeexplore.ieee.org/document/6232429)

---

## 🔬 核心研究主题

### 2.1 动作识别、检测与预测
这是第一人称视觉中最基础、最成熟的方向，研究从第一人称视角识别、检测和预测人类动作。

#### 动作识别与检测
+  **UNIEGO: Proxies as Mediators for Unified Egocentric Video Representation Learning**
    - 发表：arXiv 2026
    - 亮点：一种分层多教师蒸馏框架，生成统一的egocentric编码器，通过9个教师（涵盖ego‑exo视角、RGB、深度和骨骼模态）进行训练，在动作识别、视频检索和动作分割上达到SOTA。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.20559)

+  **Divide, Deliberate, Decide: A Multi-Agent Framework for Fine-Grained Egocentric Action Recognition**
    - 发表：arXiv 2026
    - 亮点：一种完全本地化、零样本的多智能体框架，VLM专家通过结构化商议和同行评审，提升零样本动作识别性能。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.17627)

+  **From Frames to Temporal Graphs: In-Context Egocentric Action Recognition with Vision-Language Models**
    - 发表：arXiv 2026
    - 亮点：提出将视频转换为时序动作图，配合多阶段提示管道，在11个开源VLM（2B～235B参数）上实现高效的上下文少样本学习。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.15417)

+  **Cross-Modal Action Recognition in Egocentric Video Using Mamba: Integrating RGB and Hand Skeleton Streams via CLS Token Fusion Strategies**
    - 发表：EgoVis@CVPR 2026
    - 亮点：基于Mamba框架的跨模态架构，融合RGB视频和时序手部骨架数据，提出四种CLS token融合策略。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.24302)

+  **EgoAction: Egocentric Action Composition with Reliability-Aware Temporal Fusion**
    - 发表：CVPR 2026（EPIC‑KITCHENS挑战赛冠军方案）
    - 亮点：提出解耦的动词‑名词检测 + 动态加权融合策略，基于VideoMAE‑L特征在长未裁剪视频上达到SOTA准确率。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.24496)

+  **ENIGMA-360: An Ego-Exo Dataset for Human Behavior Understanding in Industrial Scenarios**
    - 发表：arXiv 2026
    - 亮点：为三项基础任务（时序动作分割、关键步骤识别、第一人称人‑物交互检测）提供基线实验。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.14327)

+  **Ego4OOD: Rethinking Egocentric Video Domain Generalization via Covariate Shift Scoring**
    - 发表：arXiv 2026
    - 亮点：提出Ego4OOD域泛化基准，包含8个地理上不同的域，并引入基于聚类的协变量偏移度量。
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.17056)

+  **Continual Multimodal Egocentric Activity Recognition via Modality-Aware Novelty Detection**
    - 发表：arXiv 2026
    - 亮点：提出MAND模态感知框架，将新活动检测的AUC提升了10%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.16970)

+  **Ego-METAS: Egocentric online Multimodal Energy-efficient Temporal Action Segmentation benchmark**
    - 发表：arXiv 2026
    - 亮点：首个面向能效感知的在线多模态时序动作分割基准，包含100+小时未裁剪视频，覆盖5种模态。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.02246)

+  **MM-CDFSL: Multimodal Cross-Domain Few-Shot Learning for Egocentric Action Recognition**
    - 发表：ECCV 2024
    - 亮点：首次系统研究第一人称动作识别的跨域少样本场景，提出多模态蒸馏框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2405.19917)

+ **Ego-Only: Egocentric Action Detection without Exocentric Transferring**
    - 发表：ICCV 2023
    - 亮点：首次证明仅用第一人称数据训练的模型可以超越依赖第三人称迁移的方法。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Ego-Only_Egocentric_Action_Detection_without_Exocentric_Transferring_ICCV_2023_paper.html)

#### 动作预测
+  **JFAA: Technical Report for the EPIC-KITCHENS-100 Action Anticipation Challenge at EgoVis 2026**
    - 发表：arXiv 2026
    - 亮点：基于JEPA的未来动作预测方法，在EgoVis 2026 EK‑100动作预测挑战赛中荣获第一名。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.20904)

+  **TAP-JEPA: Frozen Future-Latent Probing and Two-Stage Score Fusion for EPIC-KITCHENS-100 Action Anticipation**
    - 发表：arXiv 2026
    - 亮点：EgoVis 2026 EK‑100动作预测挑战赛的亚军方案。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.00662)

+  **INSIGHT: Intention-Guided Cognitive Reasoning for Egocentric Long-Term Action Anticipation**
    - 发表：AAAI 2026
    - 亮点：提出“HOI语义识别 + 意图推理”两阶段框架，用于长期动作预测。
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.01742)

+  **PALM: Predicting Actions through Language Models**
    - 发表：arXiv 2023
    - 亮点：首次将大语言模型引入长期时序动作预测。
    - 论文链接：[arXiv](https://arxiv.org/abs/2311.17944)

+  **GANO: Gaze-Augmented Next Active Object-Based Egocentric Action Anticipation**
    - 发表：arXiv 2023
    - 亮点：针对下一个主动对象预测任务，提出视线引导的注意力机制。
    - 论文链接：[arXiv](https://arxiv.org/abs/2305.12953)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| EgoScale | 2026 | 2万+小时标注操作 | 动作识别、灵巧迁移 | [arXiv](https://arxiv.org/abs/2602.16710) |
| Ego-METAS | 2026 | 100+小时 / 5种模态 | 在线动作分割、传感器路由 | [Hugging Face](https://huggingface.co/datasets/Ego-METAS/Ego-METAS) |
| ChildLens | 2026 | 108.58小时 / 354个视频 | 儿童日常活动分析 | [数据](https://doi.org/10.17617/4.fe) |
| CogDrive (EyeCue) | 2026 | 多场景驾驶 | 驾驶员认知分心检测 | [arXiv](https://arxiv.org/abs/2605.07859) |
| Furhat Egocentric Dataset | 2026 | 20个序列 / 约25分钟 | 机器人‑自我人脸/身体跟踪 | [arXiv](https://arxiv.org/abs/2606.03694) |
| World In Your Hands | 2025 | 1000+小时标注操作 | 动作识别、VLA训练 | [GitHub](https://github.com/tars-robotics/World-In-Your-Hands) |
| EgoCampus | 2025 | 约32小时 | 视线、行人第一人称 | [GitHub](https://github.com/ComputerVisionRutgers/EgoCampus) |
| AEA | 2024 | 143个序列 / 约7.3小时 | 日常活动（Aria） | [Project Aria](https://www.projectaria.com/datasets/aea/) |
| EgoSurgery | 2024 | 开放手术视频 | 手术阶段、工具检测 | [GitHub](https://github.com/Fujiry0/EgoSurgery) |
| EgoExo-Fitness | 2024 | 32小时 / 1,276个序列 | 全身运动、质量评估 | [GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness) |
| E³（探索具身情感） | 2024 | 50+小时 | 情感识别、多模态 | [GitHub](https://github.com/Exploring-Embodied-Emotion-official/E3) |
| ⭐ Ego4D | 2022 | 约3,670小时 | 动作识别、VQA、预测等 | [官方网站](https://ego4d-data.org/) |
| ⭐ EPIC-KITCHENS-100 | 2021 | 100小时 / 9万个片段 | 动作识别、检测、预测 | [官方网站](https://epic-kitchens.github.io/) |
| EGOFALLS | 2023 | 跌倒样本 | 跌倒检测 | [Dataverse](https://www.dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/HO5GE3) |
| Epic-Sounding-Object | 2023 | 3.2K短片段 | 视听物体定位 | [GitHub](https://github.com/WikiChao/Ego-AV-Loc) |
| HoloAssist | 2023 | 169小时 | 交互式助手 | [官方网站](https://holoassist.github.io/) |
| WEAR | 2023 | 约19小时户外运动 | 活动 + IMU | [官方网站](https://mariusbock.github.io/wear/) |
| N-EPIC-KITCHENS | 2022 | 事件 + RGB子集 | 神经形态动作识别 | [GitHub](https://github.com/EgocentricVision/N-EPIC-Kitchens) |
| Ego-Deliver | 2021 | 5,360个视频 | 配送行为分析 | [官方网站](https://egodeliver.github.io/) |
| HOMAGE | 2021 | 30小时 | 家庭活动组合理解 | [GitHub](https://github.com/nishantrai18/homage) |
| MECCANO | 2021 | 约55小时工业 | 手‑物交互、工业 | [官方网站](https://iplab.dmi.unict.it/MECCANO/) |
| EGO-CH | 2020 | 27+小时 | 游客行为、POI任务 | [arXiv](https://arxiv.org/abs/2002.00899) |
| EgoCom | 2020 | 38.5小时对话 | 多人第一人称对话 | [GitHub](https://github.com/facebookresearch/EgoCom-Dataset) |
| LEMMA | 2020 | 多视角活动 | 多智能体任务 | [GitHub](https://github.com/Buzz-Beater/LEMMA) |
| Charades-Ego | 2018 | ego/exo配对 | 对齐、动作 | [官方网站](https://prior.allenai.org/projects/charades-ego) |
| EGTEA Gaze+ | 2018 | 28小时烹饪 | 视线 + 动作识别 | [官方网站](https://cbs.ic.gatech.edu/fpv/) |
| EgoGesture | 2017 | 2K+视频 / 2.4万样本 | 手势识别 | [官方网站](https://nlpr.ia.ac.cn/iva/yfzhang/datasets/egogesture.html) |
| Stanford ECM | 2017 | 31小时 | 日常活动分类 | [CVF](https://openaccess.thecvf.com/content_cvpr_2017/html/Nakamura_Jointly_Learning_Energy_CVPR_2017_paper.html) |
| THU-READ | 2017 | 1,920个片段 | 头盔RGB‑D动作 | [官方网站](https://ivg.au.tsinghua.edu.cn/dataset/THU_READ.php) |
| PEV | 2016 | 1,226对 | 双人对话微动作 | [CVF](https://openaccess.thecvf.com/content_cvpr_2016/html/Yonetani_Recognizing_Micro-Actions_and_CVPR_2016_paper.html) |
| FPPA | 2015 | 5名受试者 | 日常动作 + 手/视线 | [CVF](https://openaccess.thecvf.com/content_iccv_2015/html/Zhou_Temporal_Perception_and_ICCV_2015_paper.html) |
| JPL-Interaction | 2013 | 84个视频 | 第一人称活动识别 | [官方网站](http://michaelryoo.com/jpl-interaction.html) |
| ADL | 2012 | 约10小时 | 日常活动识别 | [官方网站](https://www.csee.umbc.edu/~hpirsiav/papers/ADLdataset/) |
| Social Interactions | 2012 | 约60小时 | 社交活动 | [官方网站](https://cbs.ic.gatech.edu/fpv/) |
| EgoAction (Sports) | 2011 | 第一人称运动视频 | 动作识别 | [IEEE](https://doi.org/10.1109/CVPR.2011.5995406) |

---

### 2.2 手‑物交互与细粒度活动
研究第一人称视角下手与物体的交互过程，是具身智能和机器人模仿学习的核心基础。

+  **Hand-4DGS: Feed-Forward 3D Gaussian Splatting for 4D Hand Reconstruction from Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：从第一人称视频中进行动态3D手部重建，应对快速头部运动、快速手部动态、严重遮挡和单视角模糊问题，对AR/VR和AI眼镜至关重要。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16930)

+  **Wh0: Generative World Models as Scalable Sources of Egocentric Human Hand Manipulation Data**
    - 发表：arXiv 2026
    - 亮点：利用生成式视频世界模型作为可扩展、可控的第一人称人手操作数据源，释放预训练灵巧VLA模型的操作能力，并生成包含5万集数据的WM‑H数据集。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.22136)

+  **Hand Trajectory Fusion for Egocentric Natural Language Query Grounding**
    - 发表：EgoVis@CVPR 2026
    - 亮点：首次将手部运动线索整合到自然语言查询定位任务中，在手‑物交互查询上R@1, IoU=0.3提升了2.54%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.02962)

+  **TouchAnything: A Dataset and Framework for Bimanual Tactile Estimation from Egocentric Video**
    - 发表：arXiv 2026
    - 亮点：提出了EgoTouch，一个大规模多视角第一人称数据集，包含密集触觉监督的双手手‑物交互，涵盖208个操作任务，共1,891个片段。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.13083)

+  **IMPACT-HOI: Supervisory Control for Onset-Anchored Partial HOI Event Construction**
    - 发表：arXiv 2026
    - 亮点：一种混合主动式框架，用于标注第一人称程序化视频，通过构建结构化事件图来表示人‑物交互，旨在从人类示教中学习机器人操作。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.17639)

+  **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - 发表：SIGGRAPH 2026
    - 亮点：可微分前臂表示 + 统一手臂‑手Transformer，在HOT3D上所有镜头类型下MPJPE降低28%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.12498)

+  **EgoGrasp: World-Space Hand-Object Interaction Estimation from Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：首次从动态第一人称视频中重建世界空间手‑物交互（W‑HOI），支持开放词汇物体。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.12255)

+  **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - 发表：arXiv 2026
    - 亮点：首个第一人称HOI世界模型，将物理先验嵌入生成式扩散模型，从3D估计中蒸馏几何和运动学先验到物理感知嵌入中。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.13615)

+  **Glove2Hand: Synthesizing Natural Hand-Object Interaction from Multi-Modal Sensing Gloves**
    - 发表：CVPR 2026（亮点论文）
    - 亮点：从多模态传感手套数据生成逼真的裸手HOI视频，并附带HandSense数据集。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.20850)

+  **TOUCH: Text-Guided Controllable Generation of Free-Form Hand-Object Interactions**
    - 发表：ICLR 2026
    - 亮点：提出自由形式HOI生成任务，构建大规模WildO2 3D HOI数据集。
    - 论文链接：[OpenReview](https://openreview.net/forum?id=4VW9HVCRw0)

+  **Leveraging Synthetic Data for Enhancing Egocentric Hand-Object Interaction Detection**
    - 发表：IJCV 2026, Vol.134
    - 亮点：仅用少量真实标注数据结合合成数据，在VISOR上AP提升11.69%，并开源HOI‑Synth合成数据生成流程。
    - 论文链接：[Springer](https://link.springer.com/article/10.1007/s11263-026-02838-8)

+  **ECHO: Ego-Centric modeling of Human-Object interactions**
    - 发表：arXiv 2025
    - 亮点：首个统一框架，仅通过头部和手腕跟踪联合恢复人体姿态、物体运动和接触动力学，采用新颖的三变量扩散过程。
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.21556)

+  **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - 发表：NeurIPS 2025
    - 亮点：提出双层架构框架，高层使用VLM推断运动先验，低层基于DiT流匹配生成细粒度轨迹。
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)

+  **EgoAERO: Learning Dexterous Manipulation from a Single Egocentric Video without Object Assets**
    - 发表：arXiv 2026
    - 亮点：无需预先扫描物体资产的灵巧操作学习框架，构建大规模EgoDex‑R数据集（430万RGB‑D帧）。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.08057)

+  **EgoInteract: Synthetic Egocentric Videos Generation for Interaction Understanding and Anticipation**
    - 发表：arXiv 2026
    - 亮点：可控的第一人称视频生成模拟器，可精确控制相机、人体动作和物体操作。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.18214)

+  **EgoHandICL: Egocentric 3D Hand Reconstruction with In-Context Learning**
    - 发表：arXiv 2026
    - 亮点：应对深度模糊、自遮挡和复杂手‑物交互的鲁棒3D手部重建，提升EgoVLM的手‑物交互推理能力。
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.09806)

+  **Do Egocentric Video-Language Models Truly Understand Hand-Object Interactions?**
    - 发表：ICLR 2025
    - 亮点：首次系统评估第一人称VLM的细粒度HOI理解能力，提出EgoHOIBench基准。
    - 论文链接：[arXiv](https://arxiv.org/abs/2405.17719)

+  **HOI-Ref: Hand-Object Interaction Referral in Egocentric Vision**
    - 发表：arXiv 2024
    - 亮点：定义第一人称场景下的HOI指向新任务，并附带HOI‑QA评估基准。
    - 论文链接：[arXiv](https://arxiv.org/abs/2404.09933)

+  **Get a Grip: Reconstructing Hand-Object Stable Grasps in Egocentric Videos**
    - 发表：arXiv 2023
    - 亮点：首次从单目第一人称视频中重建稳定的手‑物抓取状态。
    - 论文链接：[arXiv](https://arxiv.org/abs/2312.15719)

+ **EgoPCA: A New Framework for Egocentric Hand-Object Interaction Understanding**
    - 发表：ICCV 2023
    - 亮点：提出新框架作为基础设施，通过“探测、整理和适应”（EgoPCA）推进Ego‑HOI识别。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/ICCV2023/html/EgoPCA_A_New_Framework_for_Egocentric_Hand-Object_Interaction_Understanding_ICCV_2023_paper.html)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| ⭐ EgoDex | 2025 | 829小时 / 3万条轨迹 | 灵巧操作、手部姿态 | [GitHub](https://github.com/apple/ml-egodex) |
| EgoDex-R | 2026 | 430万RGB‑D帧 / 5,600个序列 | 灵巧操作、手‑物姿态 | [arXiv](https://arxiv.org/abs/2606.08057) |
| EgoTouch | 2026 | 1,891个片段 / 208个任务 | 触觉HOI | [Hugging Face](https://huggingface.co/datasets/zhenyuxie-zhzh/EgoTouch_hdf5) |
| EgoTactile | 2026 | 约6小时 / 768个片段 | 抓握压力估计 | [官方网站](https://egotactile.github.io/) |
| EventEgoHands | 2026 | 48个片段 / 12.96万帧 | RGB+事件手部检测 | [GitHub](https://github.com/SynthSyntax/EventEgoHands) |
| HA-Ego-1K | 2026 | 约24小时 / 484个多视角片段 | 灵巧操作 | [Hugging Face](https://huggingface.co/datasets/humanarchive/HA-Ego-1K) |
| DexGloveHOI | 2026 | 3.5小时 / 10万+样本 | 视觉‑IMU 3D手部跟踪 | [arXiv](https://arxiv.org/abs/2605.21714) |
| EgoEVHands | 2026 | 5,419个标注序列 | 立体事件3D手部姿态 | [GitHub](https://github.com/ZJUWang01/EgoEV-HandPose) |
| EgoEMG | 2026 | 41名参与者 / 10+小时 | EMG+视觉手部姿态 | [GitHub](https://github.com/zhenqis123/EgoEMG) |
| HRDexDB | 2026 | 1,400次抓握试验 | 灵巧抓握、触觉 | [Hugging Face](https://huggingface.co/datasets/hahahataeyun/hrdexdb) |
| TouchMoment | 2026 | 4,021个视频 / 8,456个接触时刻 | 接触时刻检测 | [arXiv](https://arxiv.org/abs/2604.12343) |
| EgoFun3D | 2026 | 271个第一人称视频 | 交互式3D物体 | [官方网站](https://3dlg-hcvc.github.io/EgoFun3D/) |
| SHOW3D | 2026 | 野外ego‑exo HOI | 3D手‑物标注 | [arXiv](https://arxiv.org/abs/2603.28760) |
| FEEL | 2026 | 力同步厨房视频 | 物理动作理解 | [官方网站](https://www.cs.umd.edu/~edessale/feel) |
| EgoPoints | 2025 | 点轨迹 + 合成 | 第一人称视频跟踪 | [GitHub](https://github.com/AhmadDarKhalil/EgoPoints) |
| ⭐ HOI4D | 2022 | 240万帧 / 4,000个序列 | 4D HOI | [官方网站](https://hoi4d.github.io/) |
| AssemblyHands | 2023 | 300万张图像 | 3D手部姿态 | [官方网站](https://assemblyhands.github.io/) |
| EgoObjects | 2023 | 9,200+个视频 | 检测、实例分割 | [GitHub](https://github.com/facebookresearch/EgoObjects) |
| ENIGMA-51 | 2023 | 22小时工业 | 细粒度行为 | [官方网站](https://fpv-iplab.github.io/ENIGMA-51/) |
| POV-Surgery | 2023 | 约8.8万帧（合成） | 手术手‑工具姿态 | [官方网站](https://batfacewayne.github.io/POV_Surgery_io/) |
| VOST | 2023 | 713个视频 | 视频物体分割 | [官方网站](https://www.vostdataset.org/) |
| EgoBody | 2022 | 125个序列 | 身体姿态、交互 | [官方网站](https://egobody.ethz.ch/) |
| EgoHOS | 2022 | 1.1万+张图像 | 手‑物分割 | [GitHub](https://github.com/owenzlz/EgoHOS) |
| EgoPAT3D | 2022 | 100万+帧RGB‑D | 3D动作目标预测 | [GitHub](https://github.com/ai4ce/EgoPAT3D) |
| Touch and Go | 2022 | 1.2万+视觉‑触觉帧 | 视觉 + 触觉 | [官方网站](https://touch-and-go.github.io/) |
| VISOR | 2022 | EPIC + 掩码 | 分割、HOI | [官方网站](https://epic-kitchens.github.io/VISOR/) |
| H2O | 2021 | 10万+帧 | 双手交互 | [官方网站](https://h2odataset.ethz.ch/) |
| TREK-150 | 2021 | 150个EPIC序列 | 物体跟踪 | [官方网站](https://machinelearning.uniud.it/datasets/trek150/) |
| You2Me | 2020 | 14个序列 | 通过ego‑exo推理身体姿态 | [GitHub](https://github.com/facebookresearch/you2me) |
| FPHA | 2018 | 1,200个序列 | 手部姿态 + 动作 | [官方网站](https://guiggh.github.io/publications/first-person-hands/) |
| EgoDexter | 2017 | 约3,200帧 | 遮挡下手部跟踪 | [官方网站](https://handtracker.mpi-inf.mpg.de/projects/OccludedHands/EgoDexter.htm) |
| EgoHands | 2015 | 4,800张标注帧 | 手部检测 | [官方网站](http://vision.soic.indiana.edu/projects/egohands/) |
| BEOID | 2014 | 58个视频 | 手‑物交互 | [官方网站](https://data.bris.ac.uk/data/dataset/3wats8ruq1sp52hq3bo8dkzul3) |
| EDSH | 2013 | 2个视频 | 像素级手部分割 | [官方网站](http://www.cs.cmu.edu/~kkitani/datasets/) |
| Handled Objects | 2009 | 11个类别 | 抓取序列 | [IEEE](https://doi.org/10.1109/CVPRW.2009.5204360) |

---

### 2.3 第一人称视觉‑语言模型与多模态推理
结合大语言模型与第一人称视觉，实现视频问答、内容描述和推理等高级认知能力。本节还涵盖RGB、深度、IMU、音频和视线信号的多模态融合方法。

#### 预训练基础模型
+  **EgoM2P: Egocentric Multimodal Multitask Pretraining**
    - 发表：ICCV 2025
    - 亮点：统一设计支持多种第一人称感知和合成任务，包括视线预测、第一人称相机跟踪和单目深度估计，同时作为条件第一人称视频生成的生成模型。
    - 论文链接：[ICCV](https://openaccess.thecvf.com/content/ICCV2025/html/EgoM2P_Egocentric_Multimodal_Multitask_Pretraining_ICCV_2025_paper.html)

+  **EgoAdapt: Adaptive Multisensory Distillation and Policy Learning for Efficient Egocentric Perception**
    - 发表：ICCV 2025
    - 亮点：自适应执行跨模态蒸馏和策略学习，实现高效的第一人称感知推理，覆盖动作识别、主动说话人定位和行为预测。GMACs降低最多89.09%，参数量降低82.02%，能耗降低9.6倍。
    - 论文链接：[ICCV](https://www.openaccess.thecvf.com/content/ICCV2025/html/Chowdhury_EgoAdapt_Adaptive_Multisensory_Distillation_and_Policy_Learning_for_Efficient_Egocentric_ICCV_2025_paper.html) | [arXiv](https://arxiv.org/abs/2506.21080)

+ **EgoVLPv2: Egocentric Video-Language Pre-training with Fusion in the Backbone**
    - 发表：ICCV 2023
    - 亮点：改进的VLP，骨干网络级融合架构。
    - 论文链接：[arXiv](https://arxiv.org/abs/2307.05463)

+ **Egocentric Video-Language Pretraining (EgoVLP)**
    - 发表：CVPR 2022
    - 亮点：首个专为第一人称场景设计的视频‑语言预训练框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2206.01670)

#### 高级推理与前沿进展
+  **EgoSAT: A Comprehensive Benchmark of Egocentric Streaming Interaction Understanding**
    - 发表：ECCV 2026
    - 亮点：首个针对第一人称视频流式交互理解的综合基准，包含1,997个独特视频，总时长165小时，约4,800个QA对。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.24422)

+  **PROSE: Training-Free Egocentric Scene Registration with Vision-Language Models**
    - 发表：arXiv 2026
    - 亮点：利用预训练VLM作为场景理解和跨扫描匹配的来源，用于第一人称场景配准，性能优于几何和学习的场景图基线。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16569)

+  **EgoSafetyBench: A Diagnostic Egocentric Video Benchmark for Evaluating Embodied VLMs as Runtime Safety Guards**
    - 发表：arXiv 2026
    - 亮点：包含1,200个机器人视角场景的第一人称视频基准，以半秒粒度标注，用于评估VLM作为流式安全守卫。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.00218)

+  **Decoding Pedestrian Crossing Intention from Egocentric Vision via Vision Language Models**
    - 发表：arXiv 2026
    - 亮点：首次利用VLM解码行人过街意图，融合眼动和自我运动后准确率提升14.5%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.09142)

+  **The Right Inference Strategy Is All You Need: Nearly Training-Free Domain-Wise Inference for EgoCross Challenge**
    - 发表：arXiv 2026
    - 亮点：EgoCross挑战赛解决方案，域感知推理策略仅用20个训练样本达到66.98%准确率。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.00829)

+  **EgoProx: Evaluating MLLMs on Egocentric 3D Proximity Reasoning Across a Cognitive Hierarchy**
    - 发表：arXiv 2026
    - 亮点：引入EgoProx，首个评估MLLM是否能够从第一人称视角建模3D感知‑动作耦合的基准。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.24456)

+  **EgoBabyVLM: Benchmarking Cross-Modal Learning from Naturalistic Egocentric Video Data**
    - 发表：arXiv 2026
    - 亮点：在语义对齐程度不同的数据集（包括自然主义婴儿和成人第一人称视频）上训练VLM。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.19130)

+  **Minerva-Ego: Spatiotemporal Hints for Egocentric Video Understanding**
    - 发表：arXiv 2026
    - 亮点：评估复杂第一人称视觉推理的基准，包含密集时空人工标注推理轨迹。向前沿模型提示“看哪里”和“何时看”可显著提升性能。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.15342)

+  **Spatial Reasoning with Vision-Language Models in Ego-Centric Multi-View Scenes**
    - 发表：ICLR 2026
    - 亮点：提出Ego3D‑Bench空间推理基准（8,600+ QA对）和Ego3D‑VLM后训练框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2509.06266)

+  **EgoMotion: Hierarchical Reasoning and Diffusion for Egocentric Vision-Language Motion Generation**
    - 发表：arXiv 2026
    - 亮点：提出分层推理与扩散框架，从第一人称视频生成语言描述的3D人体运动。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.19105)

+  **EgoReasoner: Learning Egocentric 4D Reasoning via Task-Adaptive Structured Thinking**
    - 发表：arXiv 2026
    - 亮点：针对第一人称4D推理任务的两阶段框架，采用任务自适应思考模板和奖励函数，在复杂时空推理上性能提升。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.06561)

+  **Exo2Ego: Exocentric Knowledge Guided Multimodal LLMs for Egocentric Video Understanding**
    - 发表：AAAI 2026
    - 亮点：构建Ego‑ExoClip预训练数据集（110万同步的第一人称‑第三人称片段‑文本对），提出三阶段渐进式映射学习流程。
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/38244)

+  **Egocentric Bias in Vision-Language Models**
    - 发表：arXiv 2026
    - 亮点：提出FlipSet诊断基准，用于评估VLM的二级视觉观点采择能力。评估103个VLM发现系统性自我中心偏差：绝大多数模型表现低于随机水平。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.03953)

+  **Allocentric Perceiver: Disentangling Allocentric Reasoning from Egocentric Visual Priors via Frame Instantiation**
    - 发表：arXiv 2026
    - 亮点：一种免训练的异中心感知策略，从单张或多张图像中恢复度量3D状态，在异中心任务上提升约10%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.05789)

+  **Cognitively-Inspired Tokens Overcome Egocentric Bias in Multimodal Models**
    - 发表：arXiv 2026
    - 亮点：多模态语言模型在语义视觉‑语言任务上表现良好，但在需要采用他人视觉视角的空间推理上失败，反映了持续的自我中心偏差。
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.15849)

+  **EgoThinker: Unveiling Egocentric Reasoning with Spatio-Temporal Chain of Thought**
    - 发表：NeurIPS 2025
    - 亮点：将思维链引入第一人称视频理解，提出时空思维链框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.23569)

+  **Towards Comprehensive Scene Understanding: Integrating First and Third-Person Views for LVLMs**
    - 发表：NeurIPS 2025
    - 亮点：提出E3VQA多视角问答基准（4,000个高质量QA对）和M3CoT提示技术，在GPT‑4o上提升4.84%。
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/1af83ab66b4f07a3f55788e67dab5782-Abstract-Conference.html)

+  **Benchmarking Egocentric Multimodal Goal Inference for Assistive Wearable Agents**
    - 发表：NeurIPS 2025 数据集与基准轨道
    - 亮点：目标推理基准数据集，包含363名参与者、3,482条记录，人类上限准确率93%，最佳VLM仅84%。
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/23ab960082db936f874b171822e0d097-Abstract-Datasets_and_Benchmarks.html)

+  **ECBench: Can Multi-modal Foundation Models Understand the Egocentric World? A Holistic Embodied Cognition Benchmark**
    - 发表：CVPR 2025
    - 亮点：高质量基准，系统评估LVLM的具身认知能力，包含多样场景视频源、开放式问题格式和30个具身认知维度。
    - 论文链接：[CVF](https://www.openaccess.thecvf.com/content/CVPR2025/html/Dang_ECBench_Can_Multi-modal_Foundation_Models_Understand_the_Egocentric_World_A_CVPR_2025_paper.html) | [arXiv](https://arxiv.org/abs/2501.05031)

+  **MM-Ego: Towards Building Egocentric Multimodal LLMs for Video QA**
    - 发表：ICLR 2025
    - 亮点：提出MM‑Ego，一个在第一人称视频理解上表现强大的多模态LLM。
    - 论文链接：[arXiv](https://arxiv.org/abs/2410.07177) | [OpenReview](https://openreview.net/forum?id=7k9a8b7s9d)

+  **CLiViS: Unleashing Cognitive Map through Linguistic-Visual Synergy for Embodied Visual Reasoning**
    - 发表：arXiv 2025
    - 亮点：通过语言‑视觉协同构建认知地图，突破长视频推理瓶颈。
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.17629)

+  **PhysBrain: Human Egocentric Data as a Bridge from Vision Language Models to Physical Intelligence**
    - 发表：arXiv 2025
    - 亮点：将第一人称人类视频转换为具身监督数据。
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.16793)
    - 微信文章：https://mp.weixin.qq.com/s/Eydrv6aj3q6Km6TRmfnBBQ

+  **Vinci: A Real-time Smart Assistant based on Egocentric Vision-language Model**
    - 发表：ACM 2025
    - 亮点：用于可穿戴设备的轻量级Ego‑VLM，支持长视频记忆和动作生成，可在边缘设备上实时运行。
    - 论文链接：[arXiv](https://arxiv.org/abs/2412.21080)

+  **OmniView-Space: Reinforcing Spatial Reasoning via Multi-Perspective Spatial Mapping**
    - 发表：arXiv 2026
    - 亮点：通过多模态第一人称证据维持空间一致性的框架，包含三个核心组件：多视角空间映射、工具引导的第一人称推理和认知地图蒸馏。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.00881)

+  **EgoThink: Evaluating First-Person Perspective Thinking Capability of Vision-Language Models**
    - 发表：CVPR 2024
    - 亮点：新颖的视觉问答基准，涵盖6种核心能力、12个细粒度维度，基于第一人称视频片段和人工标注QA对构建。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/EgoThink_Evaluating_First-Person_Perspective_Thinking_Capability_of_Vision-Language_Models_CVPR_2024_paper.html)

+  **VidEgoThink: A Comprehensive Benchmark for Egocentric Video Understanding**
    - 发表：arXiv 2024
    - 亮点：在EgoThink基础上扩展，提出综合基准评估第一人称视频理解能力，设计四个相互关联的任务：视频问答、层级规划、视觉定位和奖励建模。
    - 论文链接：[arXiv](https://arxiv.org/abs/2405.17719)

+  **Binocular Egocentric-360 Multi-modal Scene Understanding in the Wild**
    - 发表：ICCV 2025 Workshop
    - 亮点：聚焦双目/立体第一人称和360°全景视角的多模态场景理解与感知，同时度量第一人称视角和第三人称全视视角。
    - 论文链接：[Workshop Official Site](https://x360dataset.github.io/BinEgo-360/)

+  **D3Net: Dual-Path Decoupling-Distillation for Adaptive Fusion in Continual Egocentric Learning**
    - 发表：IEEE 2025
    - 亮点：提出双路径解耦‑蒸馏网络，通过动态门控机制显式分离模态的共享和私有特征，实现更有效的模态信息动态融合和知识迁移，在UESTC MMEA CL数据集上达到83.97%准确率。
    - 论文链接：[IEEE Xplore](https://ieeexplore.ieee.org/document/11324280)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| EgoSAT | 2026 | 165小时 / 约4,800 QA | 流式交互理解 | [arXiv](https://arxiv.org/abs/2606.24422) |
| EgoTL | 2026 | 100+日常家务任务 | 长时推理、空间QA | [官方网站](https://ego-tl.github.io/) |
| EgoCoT-Bench | 2026 | 351个视频 / 3,172个QA | 接地操作中心化CoT QA | [官方网站](https://dstardust.github.io/EgoCoT/) |
| MM-Conv | 2026 | 6.7小时 / 4,211个表述 | 上下文3D对话定位 | [arXiv](https://arxiv.org/abs/2605.21796) |
| Minerva-Ego | 2026 | 1,160个QA / 156个视频 | 时空推理轨迹 | [GitHub](https://github.com/google-deepmind/neptune) |
| EgoEverything | 2026 | 100+小时 / 5K+ MCQ | 长上下文AR视频QA | [arXiv](https://arxiv.org/abs/2604.08342) |
| EgoEsportsQA | 2026 | 1,745个QA对 | 电竞视频QA、推理 | [arXiv](https://arxiv.org/abs/2604.12320) |
| MyEgo | 2026 | 541个长视频 / 5K个QA | 个性化视频QA | [GitHub](https://github.com/Ryougetsu3606/MyEgo) |
| LifeDialBench / EgoMem | 2026 | 生活日志记忆 | 在线评估 | [GitHub](https://github.com/qys77714/LifeDialBench) |
| Ego2Web | 2026 | 500个视频‑指令对 | 第一人称视频接地网络代理 | [Hugging Face](https://huggingface.co/datasets/Shoubin/Ego2Web) |
| NoRA | 2026 | 1,420个片段 | 规范性动作推理 | [arXiv](https://arxiv.org/abs/2606.04806) |
| Causal-Plan-1M | 2026 | 100万QA / 2.22万个片段 | 物理接地规划QA | [Hugging Face](https://huggingface.co/datasets/anonymous-causal-plan/Causal_Plan) |
| Pause-and-Think | 2026 | 1万个QA片段 + 300个基准 | 辅助动作建议 | [GitHub](https://github.com/sssshivvvv/pause-and-think) |
| HD-EPIC | 2025 | 约41小时 / 密集标注 | 细粒度厨房、VQA | [官方网站](https://hd-epic.github.io/) |
| EgoEMS | 2025 | 20+小时急救场景 | 急救QA、多模态 | [GitHub](https://github.com/UVA-DSA/EgoEMS) |
| HowToDIV | 2025 | 约24小时教学 | 对话、程序化QA | [GitHub](https://github.com/google/howtodiv) |
| InterVLA | 2025 | 11.4小时交互 | 指令、ego‑exo动作捕捉 | [官方网站](https://liangxuy.github.io/InterVLA/) |
| EgoClip | 2022 | 380万个片段‑文本对 | 视频‑语言预训练 | [GitHub](https://github.com/showlab/EgoVLP) |
| AssistQ | 2022 | 100个长视频 / 529个QA | 教学QA | [GitHub](https://github.com/showlab/AssistQ) |
| EgoTaskQA | 2022 | 约2,000个视频 / 4万个QA | 因果与任务QA | [官方网站](https://sites.google.com/view/egotaskqa) |
| EgoVQA | 2019 | 600+个QA | 视频QA | [ICCVW 2019](https://openaccess.thecvf.com/content_ICCVW_2019/html/EPIC/Fan_EgoVQA_-_An_Egocentric_Video_Question_Answering_Benchmark_Dataset_ICCVW_2019_paper.html) |

---

### 2.4 长视频理解与结构化推理
处理小时甚至天级别的超长第一人称视频，核心挑战包括长程依赖建模、记忆检索和信息摘要。本节还涵盖基于场景图的结构化长视频推理表示。

+  **LongEgoRefer: A Benchmark for Long-Form Egocentric Video Referring Expression Comprehension**
    - 发表：arXiv 2026
    - 亮点：基于长时Ego4D视频构建的基准，包含1,498个指代表达，平均视频时长45分钟，呈现极端目标稀疏性和复杂人‑物交互。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.02096)

+  **Imprint: Online Memory Compression for Long-Horizon Egocentric QA**
    - 发表：arXiv 2026
    - 亮点：一种交互中心的内存框架，将长时第一人称记忆形式化为在线内存压缩。在EgoLifeQA上将QA准确率从31.0%提升至35.8%，内存占用减少2.3倍。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.00696)

+  **Keep It in Mind: User Centric Continual Spatial Intelligence Reasoning in Egocentric Video Streams**
    - 发表：ICML 2026
    - 亮点：引入UCS‑Bench数据集，涵盖170+小时和8,100+个带时间戳的问题，用于用户中心的持续空间智能。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.15200)

+  **Graph it first! Enabling Reasoning on Long-form Egocentric Videos through Scene Graphs**
    - 发表：arXiv 2026
    - 亮点：提出第一人称场景图（EgoSG）以克服MLLM输入限制，通过将视频表示为紧凑的基于文本的场景图，在HD‑EPIC VQA上取得SOTA。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.25842)

+  **EXPLORE-Bench: Egocentric Scene Prediction with Long-Horizon Reasoning**
    - 发表：arXiv 2026
    - 亮点：用于长时推理的第一人称场景预测基准：给定初始场景图像和动作序列，模型预测最终场景，揭示了MLLM与人类之间的显著性能差距。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.09731)

+  **Bridging Modalities, Spanning Time: Structured Memory for Ultra-Long Agentic Video Reasoning**
    - 发表：arXiv 2026
    - 亮点：提出MAGIC‑Video，包含多模态记忆图和交错叙事链，在EgoLifeQA上比之前最好的智能体系统高出10.1个百分点。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.08271)

+  **EgoMemReason: A Memory-Driven Reasoning Benchmark for Long-Horizon Egocentric Video Understanding**
    - 发表：arXiv 2026
    - 亮点：评估周级第一人称视频记忆驱动推理的基准，包含500个问题，最佳模型仅达到39.6%准确率。
    - 论文链接：[Hugging Face](https://huggingface.co/datasets/Ted412/EgoMemReason)

+  **Semantic and Visual Evidence for Efficient Long-Video Reasoning: A Solution for the HD-EPIC VQA Challenge**
    - 发表：arXiv 2026
    - 亮点：将长视频推理解耦为语义证据和视觉证据，通过查询引导的检索集成实现高效长视频理解。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.29402)

+  **EgoEverything: A Benchmark for Human Behavior Inspired Long Context Egocentric Video Understanding in AR Environment**
    - 发表：arXiv 2026
    - 亮点：一个显式考虑人类行为的基准，在生成问题时利用视线数据抽象出的人类注意力信号。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.08342)

+  **MA-EgoQA: Question Answering over Egocentric Videos from Multiple Embodied Agents**
    - 发表：arXiv 2026
    - 亮点：首次定义多智能体第一人称视频QA任务，提供5个场景类别的1,700+个问题。
    - 论文链接：[官方网站](https://ma-egoqa.github.io/)

+  **Static Scene Reconstruction from Dynamic Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：提出一种鲁棒流程，将静态重建主干适应到长时第一人称视频，并采用掩码感知重建机制。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.18090)

+  **From Pixels to Graphs: using Scene and Knowledge Graphs for HD-EPIC VQA Challenge**
    - 发表：arXiv 2025
    - 亮点：提出融合两种互补神经符号抽象（场景图和常识知识图）的框架，分别通过SceneNet和KnowledgeNet实例化。
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.01867)

+  **Action Scene Graphs for Long-Form Understanding of Egocentric Videos**
    - 发表：arXiv 2024
    - 亮点：提出动作场景图用于长时第一人称视频理解，实现可穿戴设备捕捉的人类活动结构化分析。
    - 论文链接：[arXiv](https://arxiv.org/abs/2409.01600)

+  **EgoMemory: Memory-Augmented Personalized Retrieval for Long-Context Egocentric Video**
    - 发表：ACL 2026
    - 亮点：为连续流式第一人称视频提出终身记忆框架。
    - 论文链接：[Microsoft Research](https://www.microsoft.com/en-us/research/publication/egomemory-memory-augmented-personalized-retrieval-for-long-context-egocentric-video/)

+  **MyEgo: Ego-Grounding for Personalized Question-Answering in Egocentric Videos**
    - 发表：CVPR 2026
    - 亮点：用于长时QA的大规模个性化第一人称视频数据集。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.01966)

+  **EGAgent: Agentic Very Long Video Understanding**
    - 发表：arXiv 2026
    - 亮点：基于实体场景图的智能体推理框架，可处理跨天连续视频流，支持结构化多跳推理和音视频混合检索。
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.18157)

+  **Spatial-Conditioned Reasoning in Long-Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：探索显式空间信号对长时VLM推理的影响，引入精细重新标注的Sanpo‑D数据集。
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.18100)

+  **FocusGraph: Graph-Structured Frame Selection for Embodied Long Video Question Answering**
    - 发表：arXiv 2026
    - 亮点：基于图的帧过滤流程，使用场景‑描述LLM选择器检索查询相关帧。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.04349)

+  **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - 发表：ICLR 2026
    - 亮点：通过第一人称交互世界建模评估具身认知的基准，揭示VLM在反向任务上表现优于前向预测。
    - 论文链接：[OpenReview](https://openreview.net/forum?id=Patx6MRipw)

+  **OSGNet: Champion Solution for Ego4D Episodic Memory Challenge 2025**
    - 发表：CVPR 2025 挑战赛全赛道冠军
    - 亮点：提出早期融合时序定位架构，赢得Ego4D情景记忆挑战赛全部三个赛道。
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.03710)

+  **Unique Lives, Shared World: Learning from Single-Life Egocentric Videos**
    - 发表：arXiv 2025
    - 亮点：研究来自单一个体的超长生命周期视频的学习问题。
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.04085)

+  **EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding**
    - 发表：NeurIPS 2023
    - 亮点：超长第一人称视频理解的权威诊断基准。
    - 论文链接：[arXiv](https://arxiv.org/abs/2308.09126)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| UCS-Bench | 2026 | 170+小时 / 8.1K+ QA | 用户中心持续空间智能 | [arXiv](https://arxiv.org/abs/2606.15200) |
| LongEgoRefer | 2026 | 1,498个指代表达 / 平均45分钟 | 长时视频指代表达理解 | [arXiv](https://arxiv.org/abs/2607.02096) |
| SuperMemory-VQA | 2026 | 52.9小时 / 4,853个QA对 | 长时记忆QA | [Hugging Face](https://huggingface.co/datasets/OSU-AIoT-MLSys-Lab/SuperMemory-VQA) |
| EgoMemReason | 2026 | 500个周级多选题 | 周尺度记忆推理评估 | [Hugging Face](https://huggingface.co/datasets/Ted412/EgoMemReason) |
| EgoExoMem | 2026 | 2,600个多选题 / 390个片段 | 跨视角情景记忆推理 | [GitHub](https://github.com/RuipingL/EgoExoMem) |
| EgoIntrospect | 2026 | 180小时 / 60名受试者 | 内部用户状态推断、长期记忆 | [官方网站](https://ego-introspect.github.io/) |
| MA-EgoQA | 2026 | 1,741个QA / 7天多智能体录像 | 多智能体第一人称视频QA | [官方网站](https://ma-egoqa.github.io/) |
| EgoStream | 2026 | 2,250个评估查询 | 流式情景记忆基准 | [官方网站](https://saroo25.github.io/Egostream/) |
| EgoLife | 2025 | 约266–300小时日常录像 | 长期个人助手、情景记忆 | [官方网站](https://egolife-ai.github.io/) |
| EgoSchema | 2023 | 250+小时 / 5,000个多选题 | 超长视频推理与QA | [官方网站](https://egoschema.github.io/) |
| VidChapters-7M | 2023 | 81.7万个视频 / 700万章节 | 长视频分割与摘要 | [官方网站](https://antoyang.github.io/vidchapters.html) |
| Multi-Ego | 2022 | 约12小时 / 41个多佩戴者序列 | 跨用户视频摘要 | [GitHub](https://github.com/M-Elfeki/Multi-DPP) |
| DoMSEV | 2018 | 80小时，48个序列 | 语义视频快进与略读 | [官方网站](https://www.verlab.dcc.ufmg.br/semantic-hyperlapse/cvpr2018-dataset/) |
| HUJI-EgoSeg | 2014 | 29个未裁剪长视频 | 时序活动分割 | [官方网站](http://www.cs.huji.ac.il/~yedMDpid/egoseg/) |
| UT Ego | 2012 | 约17小时，4个完整录像 | 长视频摘要与生活日志 | [官方网站](http://vision.cs.utexas.edu/projects/egocentric_data/UT_Egocentric_Dataset.html) |
| VINST / Visual Diaries | 2011 | 31个日常日志视频 | 事件分割、时间线提取 | [官方网站](https://www.csc.kth.se/cvap/vinst/NovEgoMotion.html) |

---

### 2.5 视线、注意力与意图预测
从第一人称视频中预测人类注视点、注意力分布和潜在意图，是可穿戴交互助手的核心技术。

+  **EPIC: A System Framework for Efficient Egocentric Perception on Embodied AR Glasses**
    - 发表：arXiv 2026
    - 亮点：面向智能AR眼镜上具身智能的高效第一人称感知系统，利用视线、姿态和惯性信号推断用户意图，仅保留最相关的感知输入。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.14282)

+  **Gaze Beyond the Frame: Forecasting Egocentric 3D Visual Span**
    - 发表：NeurIPS 2025
    - 亮点：提出新颖的3D视觉跨度预测任务，EgoSpanLift将2D视线预测提升到完整3D场景空间。
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/bf649dbcf4eaaba4fc68ccaee25a7f9e-Abstract-Conference.html)

+  **SkillSight: Efficient First-Person Skill Assessment with Gaze**
    - 发表：arXiv 2026
    - 亮点：探索在资源受限的智能眼镜上部署高能效、保护隐私的第一人称技能评估。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.01645)

+  **Gaze-Regularized VLMs for Ego-Centric Behavior Understanding**
    - 发表：arXiv 2026
    - 亮点：将眼动追踪信号嵌入VLM训练流程，视线正则化强制模型优先注视注视区域，语义指标提升近13%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.23190)

+  **Real Eyes Realize Faster: Gaze Stability and Pupil Novelty for Efficient Egocentric Learning**
    - 发表：arXiv 2026
    - 亮点：利用眼动追踪作为免训练辅助通道：注视稳定性捕捉视觉稳定性，瞳孔响应捕捉唤醒相关新颖性。双重标准帧筛选器在10%预算下匹配全流性能。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.04098)

+  **EgoCampus: Egocentric Pedestrian Eye Gaze Model and Dataset**
    - 发表：arXiv 2026
    - 亮点：引入EgoCampus数据集，涵盖25条独特户外路径，使用Project Aria眼镜记录了80多名行人的录像。
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.07668)

+  **Eyes on Target: Gaze-Aware Object Detection in Egocentric Video**
    - 发表：arXiv 2026
    - 亮点：将视线派生特征注入ViT注意力机制，使空间特征选择偏向人类关注的区域。
    - 论文链接：[arXiv](https://arxiv.org/abs/2511.01237)

+  **Beyond Scanpaths: Graph-Based Gaze Simulation in Dynamic Scenes**
    - 发表：arXiv 2026
    - 亮点：引入物体密度网络（ODN）预测下一步视线分布，并发布Focus100数据集，包含30名参与者观看第一人称驾驶录像的原始视线数据。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.23750)

+  **Ego-PMOVE: Prompt-aware Mixture of View Experts Network for Egocentric Gaze Prediction**
    - 发表：AAAI 2026
    - 亮点：首次探索跨视角视线相关性，提出提示驱动的多视角专家混合架构。
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/37808)

+  **Learning from Human Gaze: Human-like Robot Social Navigation in Dense Crowds**
    - 发表：AAAI 2026
    - 亮点：发布GazeNav数据集，包含同步的可穿戴眼动追踪、RGB录像和机器人导航轨迹。
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/38941)

+  **In the Eye of MLLM: Benchmarking Egocentric Video Intent Understanding with Gaze-Guided Prompting**
    - 发表：NeurIPS 2025 数据集与基准轨道
    - 亮点：EgoGazeVQA基准系统评估多模态LLM通过眼动信号推断用户意图的能力。
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/9df42a5f6d1397e46e2cdca80a1a7903-Abstract-Datasets_and_Benchmarks.html)

+  **egoEMOTION: Egocentric Vision and Physiological Signals for Emotion and Personality Recognition in Real-World Tasks**
    - 发表：NeurIPS 2025
    - 亮点：通过Meta Project Aria眼镜收集的多模态数据集，结合视频、眼动追踪和生物信号进行真实环境情感分析。
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.22129)

+  **EgoIntention: Visual Intention Grounding for Egocentric Assistants**
    - 发表：ICCV 2025
    - 亮点：引入首个第一人称视觉意图定位数据集，挑战多模态LLM理解和忽略非意图上下文物体，并推理不常见物体功能。
    - 论文链接：[arXiv](https://arxiv.org/abs/2504.13621) | [ICCV补充材料](https://openaccess.thecvf.com/content/ICCV2025/supplemental/Sun_Visual_Intention_Grounding_ICCV_2025_supplemental.pdf)

+  **How Much Future Helps? A Controlled Study of Future-Privileged Supervision for Causal Egocentric Gaze Estimation**
    - 发表：GAZE 2026 @ CVPR 2026
    - 亮点：一项控制研究，考察未来特权监督在因果第一人称视线估计中的作用。最优性能对应约1.7–3.3秒的未来上下文。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.01437)

+  **EyeCue: Driver Cognitive Distraction Detection via Gaze-Empowered Egocentric Video Understanding**
    - 发表：arXiv 2026
    - 亮点：一种利用视线增强的第一人称视频理解框架，用于检测驾驶员认知分心。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.07859)

---

### 2.6 3D/4D 重建与结构化感知
从单目第一人称视频中恢复3D人体网格、深度图和动态4D场景结构，是AR/VR和机器人空间感知的基础技术。本节还涵盖基于场景图的结构化3D感知。

#### 人体姿态与网格恢复
+  **Whareformer: Learning to Track What is Where in Long Egocentric Videos**
    - 发表：ECCV 2026
    - 亮点：首个针对“视野外但未遗忘”（OSNOM）任务的学习型解决方案。基于Transformer的模型，具备可更新的已建立轨迹记忆和轨迹分配模块。在56个视频上训练，在EPIC‑KITCHENS‑100、IT3DEgo和HD‑EPIC的260个长测试视频上达到SOTA。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.08537) | [项目页面](https://jacobchalk.github.io/Whareformer/)

+  **TSR-Ego: Temporally Guided Stereo Refinement Framework for Egocentric 3D Human Pose Estimation**
    - 发表：arXiv 2026
    - 亮点：一种时序引导的立体框架，结合短期运动证据和投影引导的特征采样，在UnrealEgo2和UnrealEgo‑RW上达到SOTA。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.09169)

+  **R3D: Quantitative 3D Spatial Reasoning for Egocentric Wearables**
    - 发表：arXiv 2026
    - 亮点：提出R3D‑Bench，包含基于Aria Digital Twin构建的3,033个定量空间推理问题（15种类型），并提出模型无关的空间工具调用框架R3D，平均相对准确率达73.5%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.02921)

+  **Hand-4DGS: Feed-Forward 3D Gaussian Splatting for 4D Hand Reconstruction from Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：应对快速头部运动、快速手部动态、严重遮挡和单视角模糊的动态3D手部重建。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16930)

+  **RoboAtlas: Contextual Active SLAM**
    - 发表：arXiv 2026
    - 亮点：通过上下文多臂赌博机整合边界探索、全局语义地图推理和第一人称VLM推理。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.19378)

+  **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - 发表：SIGGRAPH 2026
    - 亮点：可微分前臂表示 + 统一手臂‑手Transformer，在HOT3D上MPJPE降低28%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.12498)

+  **Bringing a Personal Point of View: Evaluating Dynamic 3D Gaussian Splatting for Egocentric Scene Reconstruction**
    - 发表：EgoVis@CVPR 2026
    - 亮点：动态3DGS在第一人称与第三人称视角上的系统基准测试，确认第一人称视角下质量持续下降。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.23803)

+  **FunRec: Reconstructing Functional 3D Scenes from Egocentric Interaction Videos**
    - 发表：CVPR 2026
    - 亮点：直接从第一人称RGB‑D交互视频重建室内场景的功能性3D数字孪生，发现关节部件并估计运动学参数。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.05621)

+  **OmniEgoCap: Camera-Agnostic Sequence-Level Egocentric Motion Reconstruction**
    - 发表：arXiv 2026
    - 亮点：基于扩散的重建，泛化至所有可穿戴相机硬件，配备几何感知可见性增强模块。
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.19283)

+  **EgoGrasp: World-Space Hand-Object Interaction Estimation from Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：首次从动态第一人称视频中重建世界空间手‑物交互，支持开放词汇物体。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.12255)

+  **AG-EgoPose: Leveraging Action-Guided Motion and Kinematic Joint Encoding for Egocentric 3D Pose Estimation**
    - 发表：arXiv 2026
    - 亮点：动作条件运动建模 + 运动学关节嵌入，用于鲁棒的可穿戴相机姿态估计。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.25175)

+  **Pandora: Articulated 3D Scene Graphs from Egocentric Vision**
    - 发表：BMVC 2025
    - 亮点：利用人类自然探索场景时佩戴Project Aria眼镜捕获的第一人称数据，恢复关节物体部件模型。证明关节3D场景图可增强机器人执行移动操作任务的能力。
    - 论文链接：[BMVC](https://bmvc2025.bmva.org/proceedings/548/)

+  **Lost & Found: Updating Dynamic 3D Scene Graphs from Egocentric Observations**
    - 发表：arXiv 2024
    - 亮点：仅基于第一人称录像及对应手部位置和相机姿态估计，在检测到的交互间隔内跟踪移动物体的6DoF姿态。在平移和方向误差上分别比第二好方法提升34%和56%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2411.19162)

+  **Fish2Mesh Transformer: 3D Human Mesh Recovery from Egocentric Vision**
    - 发表：arXiv 2025
    - 亮点：首个针对广角鱼眼头戴相机优化的网格恢复流程。
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.06089)

+  **Single-to-Dual-View Adaptation for Egocentric 3D Hand Pose Estimation**
    - 发表：CVPR 2024
    - 亮点：提出新颖的单视角到双视角适配（S2DHand）方案，将预训练的单视角估计器适配到双视角。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content_CVPR2024/html/Single-to-Dual-View_Adaptation_for_Egocentric_3D_Hand_Pose_Estimation_CVPR_2024_paper.html)

+ **Ego-Humans: An Ego-Centric 3D Multi-Human Benchmark**
    - 发表：ICCV 2023
    - 亮点：提出EgoHumans，一个新的多视角多人视频基准，用于推进第一人称人体3D姿态估计和跟踪。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/ICCV2023/html/Ego-Humans_An_Ego-Centric_3D_Multi-Human_Benchmark_ICCV_2023_paper.html)

#### 事件相机感知
+  **D-EventEgo: Event-Based Egocentric Human Pose Estimation in Dynamic Environments**
    - 发表：arXiv 2025
    - 亮点：开创性的事件流流程，用于快速运动和高动态范围下的第一人称人体姿态跟踪。
    - 论文链接：[arXiv](https://arxiv.org/abs/2505.22007)

+  **EventEgo3D++: 3D Human Motion Capture from a Head-Mounted Event Camera**
    - 发表：arXiv 2025
    - 亮点：头戴鱼眼事件相机的端到端全身动作捕捉流程。
    - 论文链接：[arXiv](https://arxiv.org/abs/2502.07869)

#### 场景重建与第一人称SLAM
+  **Ego-1K: A Large-Scale Multiview Video Dataset for Egocentric Vision**
    - 发表：CVPR 2026
    - 亮点：近1,000个多视角第一人称片段，由围绕4相机VR头显设备的12个同步相机捕获。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.13741)

+  **EgoLifter: Open-World 3D Segmentation for Egocentric Perception**
    - 发表：ECCV 2024
    - 亮点：面向第一人称感知的开放世界3D分割方法。
    - 论文链接：[Springer](https://link.springer.com/chapter/10.1007/978-3-031-72912-6_22)

+  **EgoSG: Learning 3D Scene Graphs from Egocentric RGB-D Sequences**
    - 发表：CVPR 2024
    - 亮点：提出EgoSG，直接从第一人称帧序列估计3D场景图。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/EgoSG_Learning_3D_Scene_Graphs_from_Egocentric_RGB-D_Sequences_CVPR_2024_paper.html)

+  **Generalizable Dynamic Radiance Field in Egocentric View**
    - 发表：ICLR 2024
    - 亮点：一种新颖的通用动态辐射场框架，基于单目视频预测给定时刻物理世界的3D表示，无需测试时训练。
    - 论文链接：[OpenReview](https://openreview.net/forum?id=Generalizable_Dynamic_Radiance_Field_in_Egocentric_View)

+  **EventEgo3D: 3D Human Motion Capture from Egocentric Event Streams**
    - 发表：CVPR 2024
    - 亮点：利用异步事件相机视频的高效人体运动捕捉系统。
    - 论文链接：[arXiv](https://arxiv.org/abs/2404.08640)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| Oxford Day-and-Night | 2026 | 大规模第一人称 | 新视角合成、挑战光照下的视觉重定位 | [NeurIPS 2026] |
| ⭐ Ego-Exo4D | 2024 | 1,286+小时配对的ego/exo录像 | 多视角技能分析、3D重建 | [官方网站](https://ego-exo4d-data.org/) |
| PRISM | 2026 | 27万样本 / 1,180万帧 | 零售具身VLM、空间推理 | [Hugging Face](https://huggingface.co/datasets/DreamVu/PRISM-100K) |
| EgoTraj | 2026 | 10.7小时 / 115万帧 | 第一人称相机轨迹预测 | [GitHub](https://github.com/yehiahmad/EgoTraj) |
| AIST-Living | 2026 | 第一人称视频 + GT 3D场景地图 | 全局相机定位、人体姿态跟踪 | [官方网站](https://deguchihiroyuki.github.io/Map-Mono-Ego-Project/) |
| OVO-S-Bench | 2026 | 348个视频 / 1,680个空间QA对 | 流式空间具身推理 | [官方网站](https://internlm.github.io/OVO-S-Bench/) |
| ⭐ ADT (Aria Digital Twin) | 2023 | 200个多模态序列，2个室内场景 | 第一人称3D场景与身体感知 | [官方网站](https://www.projectaria.com/datasets/adt/) |
| PVSG | 2023 | 400个全景片段 / 约15万帧 | 第一人称全景场景图构建 | [GitHub](https://github.com/jingkang50/PVSG) |
| DR(eye)VE | 2018 | 约6小时驾驶录像 / 55.5万帧 | 驾驶员视线预测、汽车第一人称感知 | [官方网站](http://aimagelab.ing.unimore.it/dreyeve) |
| EgoCart | 2018 | 9个零售RGB‑D序列 | 室内/购物车定位 | [官方网站](https://iplab.dmi.unict.it/EgocentricShoppingCartLocalization/) |
| IU ShareView | 2018 | 9组配对的第一人称视频集 | 跨佩戴者实例分割与重识别 | [官方网站](http://vision.soic.indiana.edu/firstthird-eccv2018/) |
| OST | 2017 | 57个室内序列 | 物体搜索、可穿戴视线跟踪 | [GitHub](https://github.com/Mengmi/deepfuturegaze_gan) |

---

### 2.7 具身AI与视觉‑语言‑动作（Ego‑VLA）
将第一人称人类视频中的视觉、语言和动作信号对齐，将人类操作知识迁移到机器人智能体，是具身智能的核心流程。本节还涵盖具身AI基准和从人类示教中学习机器人。

+  **EgoSteer: A Full-Stack System Towards Steerable Dexterous Manipulation from Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：一个全栈系统，将第一人称人类视频的灵巧VLA预训练扩展到9,600小时高质量预训练数据。集成了EgoSmith数据流程、统一机器人栈和世界模型增强的VLA。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.09701)

+  **EgoWAM: World Action Models Beyond Pixels with In-the-Wild Egocentric Human Data**
    - 发表：arXiv 2026
    - 亮点：受控的人‑机共训练框架，比较像素、DINO和3D运动流作为世界预测目标。DINO将分布外泛化提升最多4倍，3D流将领域内性能提升20‑30%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.08436) | [项目页面](https://gatech-rl2.github.io/egowam.github.io)

+  **HumanScale: Egocentric Human Video Can Outperform Real-Robot Data for Embodied Pretraining**
    - 发表：arXiv 2026
    - 亮点：系统比较第一人称人类视频和遥操作真实机器人轨迹作为预训练数据源。在ego数据上预训练的模型验证损失降低24%，分布内和分布外任务成功率分别高出52.5%和90%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.20521)
    - 微信文章：https://mp.weixin.qq.com/s/l4XY2I2I8BYCxphstKcbvQ

+  **HumanoidArena: Benchmarking Egocentric Hierarchical Whole-body Learning**
    - 发表：arXiv 2026
    - 亮点：首个面向第一人称分层全身学习的仿真优先基准，将策略学习形式化为分层决策问题，包含7个腿部关键的HOI/HSI任务。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.17833)

+  **ACE-Ego-0: Unifying Egocentric Human and Robotic Data for VLA Pretraining**
    - 发表：arXiv 2026
    - 亮点：统一VLA预训练框架，联合利用异构数据源，通过可扩展的第一人称视频到动作流程将原始人类视频转换为机器人格式的伪动作轨迹。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.17200)
    - 微信文章：https://mp.weixin.qq.com/s/w4OS_vk1n3KTs5c4lawjPw

+  **VEGA: Learning Navigation VLAs from In-the-Wild Egocentric Video with Geometric Trajectory Supervision**
    - 发表：arXiv 2026
    - 亮点：从无标注的第一人称导航视频中训练导航VLA的方法。重建局部场景几何，采样导航目标，生成障碍物感知轨迹，碰撞减少33.0%，障碍物避让提升17.9%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.18426)

+  **Motion-Focused Latent Action Enables Cross-Embodiment VLA Training from Human EgoVideos**
    - 发表：arXiv 2026
    - 亮点：解决第一人称人类操作视频中缺乏动作标签用于VLA训练的问题。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16251)

+  **ActiveMimic: Egocentric Video Pretraining with Active Perception**
    - 发表：arXiv 2026
    - 亮点：一个预训练框架，从单个穿戴式RGB相机恢复同步的相机和手腕轨迹，以解决第一人称视频与机器人数据预训练之间的性能差距。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.06194)

+  **EgoPhys: Learning Generalizable Physics Models of Deformable Objects from Egocentric Video**
    - 发表：arXiv 2026
    - 亮点：从第一人称RGB视频中利用通用先验构建可变形物体的物理数字孪生，实现对未知物体密集弹簧刚度场的预测。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16202)

+  **EgoGuide: Egocentric Guidance for Efficient Robot-Free Demonstration Collection and Learning**
    - 发表：arXiv 2026
    - 亮点：一个采集界面，记录同步的手腕和头部/第一人称观测，并带有在线视觉‑几何数据质量指导。提出门控第一人称残差策略以实现鲁棒学习。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.14665)

+  **EgoAERO: Learning Dexterous Manipulation from a Single Egocentric Video without Object Assets**
    - 发表：arXiv 2026
    - 亮点：首个从单张第一人称RGB‑D人类示教中学习灵巧操作而无需物体资产的框架，构建EgoDex‑R数据集（430万RGB‑D帧）。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.08057)

+  **EgoPriMo: Egocentric Motion Generation for Interactive Humanoid Control**
    - 发表：arXiv 2026
    - 亮点：从第一人称人类示教学习全身运动先验的统一框架。给定第一人称观测和文本提示，重建、生成和预测基于SMPL的全身运动。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.08495)

+  **EgoTSR: From Perception to Planning: Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning**
    - 发表：ICML 2026
    - 亮点：基于课程学习的任务导向时空推理框架。构建EgoTSR‑Data，包含4,600万个样本，分三个阶段组织，在长时逻辑推理任务上达到92.4%准确率。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.10517) | [ICML Poster](https://icml.cc/virtual/2026/poster/64173)

+  **EARL: Towards a Unified Analysis-Guided Reinforcement Learning Framework for Egocentric Interaction Reasoning and Pixel Grounding**
    - 发表：ICML 2026
    - 亮点：采用组相对策略优化（GRPO）增强MLLM在第一人称视觉中的交互理解。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.14742)

+  **Ego3S: Select, Strengthen, and Synchronize for Efficient Egocentric Reasoning**
    - 发表：ICML 2026
    - 亮点：提出新颖的三阶段Ego3S框架，将模型推理锚定在交互证据上，应对第一人称推理相比第三人称理解的独特挑战。
    - 论文链接：[ICML Poster](https://icml.cc/virtual/2026/poster/63931)

+  **Embodied VideoAgent: Persistent Memory from Egocentric Videos and Embodied Sensors Enables Dynamic Scene Understanding**
    - 发表：ICCV 2025
    - 亮点：基于LLM的智能体，从第一人称视频和具身传感器输入（深度和姿态感知）构建场景记忆，在Ego4D‑VQ3D上提升6.5%，OpenEQA上提升2.6%，EnvQA上提升15.3%。
    - 论文链接：[ICCV](https://www.openaccess.thecvf.com/content/ICCV2025/html/Fan_Embodied_VideoAgent_Persistent_Memory_from_Egocentric_Videos_and_Embodied_Sensors_ICCV_2025_paper.html) | [arXiv](https://arxiv.org/abs/2501.00358)

+  **Minerva-Ego: Spatiotemporal Hints for Egocentric Video Understanding**
    - 发表：CVPR 2025
    - 亮点：评估复杂第一人称视觉推理的基准，扩展高质量视频数据源，包含挑战性的多步多模态问题和密集时空人工标注推理轨迹。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2025/html/Minerva-Ego_Spatiotemporal_Hints_for_Egocentric_Video_Understanding_CVPR_2025_paper.html)

+  **JoyAI-RA 0.1: A Foundation Model for Robotic Autonomy**
    - 发表：arXiv 2026
    - 亮点：VLA具身基础模型，多源多层次预训练整合网络数据、大规模第一人称人类操作视频、仿真轨迹和真实机器人数据。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.13863)

+  **EgoPush: Learning End-to-End Egocentric Multi-Object Rearrangement for Mobile Robots**
    - 发表：arXiv 2026
    - 亮点：策略学习框架，使移动机器人能够进行第一人称、感知驱动的重排，无需依赖显式全局状态估计。使用物体中心潜空间编码相对空间关系。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.18071)

+  **EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data**
    - 发表：arXiv 2026
    - 亮点：在超过20,854小时的动作标注第一人称人类视频上训练VLA模型，揭示人类数据规模与验证损失之间的对数线性缩放律。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.16710)
    - 微信文章：https://mp.weixin.qq.com/s/OpH-3oQRHNpiOSVsyuH0fA

+  **Ego-Pi: VLA Fine-Tuning for Egocentric Human and Robot Data**
    - 发表：arXiv 2026
    - 亮点：针对在可穿戴人类录像上训练的双臂灵巧操作VLA的微调流程。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.08107)

+  **ViterbiPlanNet: Injecting Procedural Knowledge via Differentiable Viterbi for Egocentric Task Planning**
    - 发表：CVPR 2026
    - 亮点：可微分Viterbi算法将逐步程序化先验注入VLA规划模块。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.04265)

+  **OSCAR: Omni-Embodiment Skeleton-Conditioned World Action Model for Robotics**
    - 发表：arXiv 2026
    - 亮点：通用骨架条件世界‑动作模型，从第一人称人类示教学习多机器人策略。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.04463)

+  **Co-training with Ego-centric Video and Demonstration for Robot Navigation Task**
    - 发表：arXiv 2026
    - 亮点：跨领域共训练将第一人称行走视频转换为移动机器人模仿数据集。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.01951)

+  **In-N-On: Scaling Egocentric Manipulation with in-the-wild and on-task Data**
    - 发表：arXiv 2025
    - 亮点：策划PHSD数据集，包含直接与目标操作任务对齐的第一人称数据和任务内数据。
    - 论文链接：[arXiv](https://arxiv.org/abs/2511.12643)

+  **EgoBridge: Domain Adaptation for Generalizable Imitation from Egocentric Human Videos**
    - 发表：NeurIPS 2025
    - 亮点：人类视觉‑动作分布的最优传输对齐，相比标准基线将模仿成功率提升44%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2509.19626)

+  **EgoAgent: A Joint Predictive Agent Model in Egocentric Worlds**
    - 发表：ICCV 2025
    - 亮点：统一Transformer架构，集成第一人称视觉、语言、世界建模和动作决策头。
    - 论文链接：[arXiv](https://arxiv.org/abs/2502.05857)

+  **Wh0: Generative World Models as Scalable Sources of Egocentric Human Hand Manipulation Data**
    - 发表：arXiv 2026
    - 亮点：利用生成式视频世界模型作为可扩展、可控的第一人称人手操作数据源，释放预训练灵巧VLA模型的操作能力。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.22136)

+  **HumanEgo: Zero-Shot Robot Learning from Minutes of Human Egocentric Videos**
    - 发表：arXiv 2026
    - 亮点：通过将每次人类示教提升到手‑物交互的实体级表示来弥合具身差距。每任务仅需30分钟人类视频，在四个真实世界任务上平均成功率达92.5%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.24934)

+  **Ego2World: Compiling Egocentric Cooking Videos into Executable Worlds for Belief-State Planning**
    - 发表：arXiv 2026
    - 亮点：将第一人称烹饪视频转换为由图‑转移规则支配的可执行符号世界。强制智能体在不观察真实世界状态的情况下更新记忆并重新规划。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.13335)

+  **LOME: Learning Human-Object Manipulation with Action-Conditioned Egocentric World Model**
    - 发表：arXiv 2026
    - 亮点：一个第一人称世界模型，以输入图像、文本提示和每帧人体动作（包括身体姿态和手势）为条件，生成逼真的人‑物交互视频。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.27449)

+  **EgoActor: Grounding Task Planning into Spatial-aware Egocentric Actions for Humanoid Robots via Visual-Language Models**
    - 发表：arXiv 2026
    - 亮点：提出EgoActing任务，要求将高层指令接地到空间感知的人形动作中。EgoActor VLM实时预测运动基元、头部运动和操作命令。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.04515)

+  **Act, Sense, Act: Learning Non-Markovian Active Perception Strategies from Large-Scale Egocentric Human Data**
    - 发表：arXiv 2026
    - 亮点：提出CoMe‑VLA，一种认知和记忆感知的VLA框架，利用大规模人类第一人称数据学习通用的探索和操作先验。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.04600)

+  **Legs Over Arms: On the Predictive Value of Lower-Body Pose for Human Trajectory Prediction from Egocentric Robot Perception**
    - 发表：arXiv 2026
    - 亮点：发现机器人可通过观察腿部高效预测人类移动，为社交导航的感知设计提供可操作见解。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.09076)

+  **Seeing Together: Multi-Robot Cooperative Egocentric Spatial Reasoning with Multimodal Large Language Models**
    - 发表：arXiv 2026
    - 亮点：多机器人协作的第一人称空间推理，使用多模态大语言模型。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.18431)

+  **Spatially Prompted Visual Trajectory Prediction for Egocentric Manipulation**
    - 发表：arXiv 2026
    - 亮点：首次形式化空间提示视觉轨迹预测（SP‑VTP），收集EgoSPT数据集，包含第一人称空间提示操作轨迹。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.20085)

#### 📊 相关数据集与基准（程序化技能学习）
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| In-N-On (PHSD) | 2025 | 第一人称 + 任务内数据 | 操作策略学习 | [arXiv](https://arxiv.org/abs/2511.12643) |
| EgoVerse | 2026 | 1,362小时 / 约8万个任务片段 | 通用机器人操作预训练、具身基准测试 | [官方网站](https://egoverse.ai/) |
| EgoLive | 2026 | 大规模真实世界日常任务录像 | 非结构化机器人技能迁移 | [arXiv](https://arxiv.org/abs/2604.23570) |
| EgoMAGIC | 2026 | 3,355个医疗任务视频 / 50个临床工作流 | 手术动作检测与程序化辅助 | [Zenodo](https://doi.org/10.5281/zenodo.19239154) |
| HumanEgo | 2026 | 短Aria可穿戴示教序列 | 人类到机器人的策略蒸馏 | [官方网站](https://humanego-ai.github.io/) |
| EgoSPT | 2026 | 11,515个操作片段 / 112个任务文件夹 | 空间提示条件操作轨迹生成 | [Hugging Face](https://huggingface.co/datasets/JackYFL233/EgoSPT) |
| Ego-EXTRA | 2026 | 50小时 / 1.5万+教学VQA对 | 专家‑新手可穿戴辅助场景 | [官方网站](https://fpv-iplab.github.io/Ego-EXTRA/) |
| GM-100 | 2026 | 100+操作任务 / 1.3万条轨迹 | 通用机器人技能评估基准 | [官方网站](https://www.rhos.ai/research/gm-100) |
| SABER | 2026 | 100+小时 / 4.48万个零售样本 | 购物机器人的具身VLA域适应 | [官方网站](https://dreamvu.ai/saber/) |
| EgoProactive / Pro²Bench | 2026 | 700个可穿戴录像 / 4.2万个评估样本 | 主动式程序化可穿戴助手基准 | [Hugging Face](https://huggingface.co/datasets/facebook/wearable-ai) |
| EgoYC2 / Exo2EgoDVC | 2025 | 约43小时烹饪录像，密集步骤描述 | 家庭程序化跨视角对齐 | [GitHub](https://github.com/ut-vision/Exo2EgoDVC) |
| ⭐ EgoExoLearn | 2024 | 120小时异步ego/exo配对片段 | 人类程序化学习模拟、机器人模仿 | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |
| ⭐ Assembly101 | 2022 | 513小时多视角组装录像 | 逐步工业程序化操作 | [官方网站](https://assembly-101.github.io/) |
| IndustReal | 2024 | 约6小时工厂操作序列 | 工业步骤检测与错误识别 | [官方网站](https://timschoonbeek.github.io/industreal.html) |
| EgoProceL | 2022 | 62个可穿戴视频 / 16个家务任务 | 日常程序化学习基线 | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| EPIC-Tent | 2019 | 7+小时双HMD帐篷组装录像 + 眼动追踪 | 多模态程序化活动分析 | [数据仓库](https://data.bris.ac.uk/data/dataset/2ite3tu1u53n42hjfh3886sa86) |
| CMU-MMAC | 2011 | 25名参与者 / 5个烹饪食谱 | 厨房程序化活动识别 | [官方网站](http://kitchen.cs.cmu.edu/) |
| GTEA Gaze | 2011 | 17个烹饪会话 | 细粒度程序化动作 + 视线预测 | [官方网站](https://cbs.ic.gatech.edu/fpv/) |

---

### 2.8 第一人称世界模型
从第一人称观测中学习环境的演化规律，实现未来帧预测、合成交互视频生成和长时任务规划。

+  **EgoWAM: World Action Models Beyond Pixels with In-the-Wild Egocentric Human Data**
    - 发表：arXiv 2026
    - 亮点：研究世界动作模型（WAM）是否比行为克隆提供更好的训练信号，要求策略不仅预测动作，还预测场景如何演化。引入EgoWAM，一个受控的人‑机共训练框架，比较像素、DINO和3D运动流作为世界预测目标。DINO将分布外物体和场景泛化提升最多4倍，3D流将领域内性能提升20‑30%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.08436) | [项目页面](https://gatech-rl2.github.io/egowam.github.io)

+  **EgoCS-400K: An Egocentric Gameplay Dataset for World Models**
    - 发表：arXiv 2026
    - 亮点：一个大规模基于回放的第一人称Counter‑Strike数据集，用于世界模型，从公开的职业CS比赛录像中构建，保留了人类游戏轨迹。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.16186)

+  **AnchorWorld: Embodied Egocentric World Simulation with View-based Evolution Customization**
    - 发表：arXiv 2026
    - 亮点：锚定关键帧约束的可控第一人称模拟器，锚匹配准确率达89%。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.07326)

+  **World-Language-Action Model for Unified World Modeling, Language Reasoning, and Action Synthesis**
    - 发表：arXiv 2026
    - 亮点：提出世界‑语言‑动作（WLA）模型作为一类新的具身基础模型。WLA以文本指令、图像和机器人状态为输入，联合预测文本子任务、子目标图像和机器人动作。利用大量第一人称视频进行世界建模和语言推理能力，处理复杂长时任务。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.05979)

+  **PlayerOne: Egocentric World Simulator**
    - 发表：NeurIPS 2025
    - 亮点：首个逼真的开放世界第一人称模拟器，支持无限制自由探索和完全运动控制。
    - 论文链接：[arXiv](https://arxiv.org/abs/2512.06724)

+  **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - 发表：arXiv 2026
    - 亮点：开创性的面向HOI的第一人称扩散世界模型，嵌入物理先验。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.13615)

+  **WEM: World-Ego Modeling for Long-Horizon Evolution in Hybrid Embodied Tasks**
    - 发表：arXiv 2026
    - 亮点：解耦静态场景 + 动态自身分支的世界建模架构，用于长序列预测。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.19957)

+  **EgoExo-WM: Unlocking Exo Video for Ego World Models**
    - 发表：arXiv 2026
    - 亮点：跨视角知识迁移流程，利用丰富的第三人称录像增强第一人称世界模型训练。
    - 论文链接：[arXiv](https://arxiv.org/pdf/2605.15477)
    - 微信文章：https://mp.weixin.qq.com/s/S9LkbbBgD3EU6DYPAvUhmA

+  **EgoSim: Egocentric World Simulator for Embodied Interaction Generation**
    - 发表：arXiv 2026
    - 亮点：闭环交互模拟器，具有持久动态3D场景状态，用于连续合成交互视频生成。
    - 论文链接：[arXiv](https://arxiv.org/abs/2604.01001)

+  **LOME: Learning Human-Object Manipulation with Action-Conditioned Egocentric World Model**
    - 发表：arXiv 2026
    - 亮点：一个第一人称世界模型，以输入图像、文本提示和每帧人体动作为条件，生成逼真的人‑物交互视频，为逼真AR/VR体验和可扩展机器人训练铺平道路。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.27449)

+  **EgoForge: Goal-Directed Egocentric World Simulator**
    - 发表：arXiv 2026
    - 亮点：目标条件生成模拟器，生成匹配用户指定任务目标的未来第一人称序列。
    - 论文链接：[arXiv](https://arxiv.org/abs/2603.20169)

+  **Walk through Paintings: Egocentric World Models from Internet Priors**
    - 发表：arXiv 2026
    - 亮点：利用网络视频先验，将预训练视频扩散模型重新用作动作条件第一人称世界模型。
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.15284)

+  **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - 发表：ICLR 2026
    - 亮点：首个通过第一人称交互世界建模量化具身认知的基准，揭示VLM在反向任务上优于前向预测。
    - 论文链接：[OpenReview](https://openreview.net/forum?id=Patx6MRipw)

+  **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - 发表：NeurIPS 2025
    - 亮点：通用HOI世界模型，两阶段VLM先验推理 + DiT流匹配轨迹生成。
    - 论文链接：[NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)

+  **Hand2World: Autoregressive Egocentric Interaction Generation via Free-Space Hand Gestures**
    - 发表：arXiv 2026
    - 亮点：研究在自由空间手势下从单张场景图像生成第一人称交互。提出Hand2World，一个统一的自回归框架，解决分布偏移、手与相机运动模糊以及任意长度视频生成问题。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.09600)

#### 📊 相关数据集与基准（世界模型预训练与视频生成）
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| ⭐ Ropedia Xperience-10M | 2026 | 1,000万个多模态人类体验片段 | 大规模第一人称世界模型预训练 | [Hugging Face](https://huggingface.co/datasets/ropedia-ai/xperience-10m) |
| DreamDojo-HV | 2026 | 大规模第一人称合成录像 | 生成式世界模型训练 | [arXiv](https://arxiv.org/abs/2602.06949) |
| Ego-1K | 2026 | 多视角第一人称视频片段 | 神经3D/4D动态场景合成 | [Hugging Face](https://huggingface.co/datasets/facebook/ego-1k) |
| In-lab | 2026 | 桌面操作轨迹序列 | 小规模技能世界模型微调 | [arXiv](https://arxiv.org/abs/2602.06949) |
| HumanNet | 2026 | 约100万小时以人为中心的视频语料 | 通用VLA与世界模型预训练 | [arXiv](https://arxiv.org/abs/2605.06747) |
| MobileEgo Anywhere | 2026 | 200小时智能手机第一人称日常录像 | 轻量级长时世界模型训练 | [arXiv](https://arxiv.org/abs/2605.05945) |
| EgoEdit | 2025 | 10万个第一人称视频编辑对 | 条件第一人称视频生成基准 | [官方网站](https://snap-research.github.io/EgoEdit) |
| EgoVid-5M | 2024 | 500万个多样化第一人称视频片段 | 基础生成式第一人称视频数据集 | [官方网站](https://egovid.github.io/) |

---

### 2.9 第一人称程序化AI助手
专注于构建逐步指导用户完成日常和专业程序化任务的第一人称AI助手。该方向围绕三个核心能力组织——程序化错误检测、程序化学习和程序化问答，并由两个支撑维度（实时流感知和主动交互）提供支持。

#### 2.9.1 程序化错误检测
+  **Plan, Watch, Recover: A Benchmark and Architectures for Proactive Procedural Assistance**
    - 发表：arXiv 2026
    - 亮点：发布EgoProactive，一个大规模可穿戴第一人称数据集，用于主动式程序化辅助，包含显式的“偏离计划”标注和恢复步骤；提出解耦的规划器‑交互架构，专用于程序化状态跟踪和恢复注入。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.04970)

+  **Modeling Multiple Normal Action Representations for Error Detection in Procedural Tasks**
    - 发表：CVPR 2025
    - 亮点：提出自适应多正常动作表示（AMNAR）框架，预测所有有效下一步动作并重建对应的正常表示，以检测程序化任务中的细粒度执行偏差。
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.22405) | [CVPR 2025 Official](https://openaccess.thecvf.com/content/CVPR2025/html/Huang_Modeling_Multiple_Normal_Action_Representations_for_Error_Detection_in_Procedural_Tasks_CVPR_2025_paper.html)

+  **Gazing Into Missteps: Leveraging Eye-Gaze for Unsupervised Mistake Detection in Egocentric Videos of Skilled Human Activities**
    - 发表：CVPR 2025
    - 亮点：首次利用眼动信号进行无监督错误检测，用于熟练程序化活动。
    - 论文链接：[arXiv](https://arxiv.org/abs/2504.07892)

+  **Transparent and Coherent Procedural Mistake Detection**
    - 发表：EMNLP 2025
    - 亮点：为检测到的程序化错误生成透明、连贯的自然语言解释。
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.08765)

+  **PREGO: Online Mistake Detection in PRocedural EGOcentric Videos**
    - 发表：CVPR 2024
    - 亮点：专为第一人称程序化视频定制的在线实时错误检测框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2404.01688)

+  **TI-PREGO: Chain of Thought and In-Context Learning for Online Mistake Detection in PRocedural EGOcentric Videos**
    - 发表：arXiv 2024
    - 亮点：通过思维链和上下文学习增强PREGO，提升在线错误检测能力。
    - 论文链接：[arXiv](https://arxiv.org/abs/2410.05678)

+  **EgoOops: A Dataset for Mistake Action Detection from Egocentric Videos Referring to Procedural Texts**
    - 发表：ICCV 2024
    - 亮点：首个与程序化文本指令对齐的第一人称错误动作检测数据集。
    - 论文链接：[项目页面](https://ego-oops.github.io/)

+  **Error Detection in Egocentric Procedural Task Videos**
    - 发表：CVPR 2024
    - 亮点：第一人称程序化错误检测的系统基准和基线框架。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2024/html/Li_Error_Detection_in_Egocentric_Procedural_Task_Videos_CVPR_2024_paper.html)

+  **Understanding-Enhanced Model Collaboration for Long-Tailed Egocentric Mistake Detection**
    - 发表：arXiv 2026
    - 亮点：提出UE‑MCM，结合高效的粗粒度视频理解和精确的细粒度动作推理，处理错误实例的长尾分布，采用互补优化目标。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.02120)

#### 2.9.2 程序化学习
+  **Task Graph Maximum Likelihood Estimation for Procedural Activity Understanding in Egocentric Videos**
    - 发表：arXiv 2025
    - 亮点：引入基于梯度的任务图学习方法，通过最大似然优化边权重。
    - 论文链接：[arXiv](https://arxiv.org/abs/2502.08123)

+  **HiERO: Understanding the Hierarchy of Human Behavior Enhances Reasoning on Egocentric Videos**
    - 发表：ICCV 2025
    - 亮点：分层行为理解框架，显著提升第一人称程序化推理性能。
    - 论文链接：[项目页面](https://github.com/facebookresearch/hiero)

+  **Procedure Learning via Regularized Gromov-Wasserstein Optimal Transport**
    - 发表：arXiv 2025
    - 亮点：基于正则化Gromov‑Wasserstein最优传输的程序化学习方法。
    - 论文链接：[arXiv](https://arxiv.org/abs/2507.15540)

+  **OPEL: Optimal Transport Guided ProcedurE Learning**
    - 发表：NeurIPS 2024
    - 亮点：最优传输引导的无监督程序化学习框架。
    - 论文链接：[OpenReview](https://openreview.net/forum?id=5806637acc87823d00dc8ff1945b86c1c0462612)

+  **United We Stand, Divided We Fall: UnityGraph for Unsupervised Procedure Learning from Videos**
    - 发表：WACV 2024
    - 亮点：基于UnityGraph的无监督程序化学习，从无标签教学视频中学习。
    - 论文链接：[arXiv](https://arxiv.org/abs/2311.04567)

+  **STEPs: Self-Supervised Key Step Extraction and Localization from Unlabeled Procedural Videos**
    - 发表：ICCV 2023
    - 亮点：从无标签程序化视频中自监督提取和定位关键步骤。
    - 论文链接：[项目页面](https://steps-procedural.github.io/)

+  **My View is the Best View: Procedure Learning from Egocentric Videos**
    - 发表：ECCV 2022
    - 亮点：首个专为第一人称视角设计的程序化学习框架。
    - 论文链接：[项目页面](https://github.com/ShyamNarasimhan/Procedure-Learning-from-Egocentric-Videos)

+  **Learning To Recognize Procedural Activities with Distant Supervision**
    - 发表：CVPR 2022
    - 亮点：基于远程监督的程序化活动识别框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2204.02345)

#### 2.9.3 程序化问答
+  **EgoCoT-Bench: Benchmarking Grounded and Verifiable Operation-Centric Chain of Thought Reasoning for MLLMs**
    - 发表：arXiv 2026
    - 亮点：一个细粒度的第一人称基准，包含351个第一人称视频上的3,172个可验证QA对，覆盖12个子任务组。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.19559)

+  **Grounded Multi-Hop VideoQA in Long-Form Egocentric Videos**
    - 发表：AAAI 2025
    - 亮点：研究长时第一人称视频中的多跳视频问答问题。
    - 论文链接：[AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/33925)

+  **EASG-Bench: Video Q&A Benchmark with Egocentric Action Scene Graphs**
    - 发表：arXiv 2025
    - 亮点：一个问答基准，QA对由时空接地动态场景图创建，捕捉演员、动作和物体之间的关系。
    - 论文链接：[arXiv](https://arxiv.org/abs/2508.01867)

+  **EOC-Bench: Can MLLMs Identify, Recall, and Forecast Objects in an Egocentric World?**
    - 发表：arXiv 2025
    - 亮点：一个旨在系统评估动态第一人称场景中物体中心具身认知的基准。
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.05287)

+  **EgoNight: Towards Egocentric Vision Understanding at Night with a Challenging Benchmark**
    - 发表：arXiv 2025
    - 亮点：首个以VQA为核心任务的夜间第一人称视觉综合基准。
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.08961)

+  **EgoLife: Towards Egocentric Life Assistant**
    - 发表：CVPR 2025
    - 亮点：开发第一人称生活助手的项目，通过AI驱动的可穿戴眼镜陪伴用户并提升个人效率。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content/CVPR2025/html/EgoLife_Towards_Egocentric_Life_Assistant_CVPR_2025_paper.html)

+  **RAVEN: Query-Guided Representation Alignment for Question Answering over Audio, Video, Embedded Sensors, and Natural Language**
    - 发表：arXiv 2025
    - 亮点：多模态QA框架，对齐音频、视频、嵌入式传感器和自然语言，用于程序化场景。
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.06789)

+  **EgoTextVQA: Towards Egocentric Scene-Text Aware Video Question Answering**
    - 发表：CVPR 2025
    - 亮点：首个融合场景文本信息的第一人称视频QA基准，用于程序化任务。
    - 论文链接：[项目页面](https://egotextvqa.github.io/)

+  **Omnia de Egotempo: Benchmarking Temporal Understanding of Multi-Modal LLMs in Egocentric Videos**
    - 发表：CVPR 2025
    - 亮点：多模态LLM在第一人称程序化视频上时序推理能力的基准。
    - 论文链接：[arXiv](https://arxiv.org/abs/2503.13646) | [GitHub](https://github.com/google-research-datasets/egotempo)

+  **Vinci: A Real-time Smart Assistant Based on Egocentric Vision-language Model for Portable Devices**
    - 发表：ACM 2025
    - 亮点：可部署在边缘的轻量级Ego‑VLM，用于程序化助手场景。
    - 论文链接：[arXiv](https://arxiv.org/abs/2412.21080)

+  **Grounded Question-Answering in Long Egocentric Videos**
    - 发表：CVPR 2024
    - 亮点：长时第一人称程序化视频的接地QA框架。
    - 论文链接：[CVF](https://openaccess.thecvf.com/content_CVPR2024/html/Wang_Grounded_Question-Answering_in_Long_Egocentric_Videos_CVPR_2024_paper.html)

#### 2.9.4 实时流处理与主动交互
+  **Vinci2: Providing Proactive Assistance in Continuous Egocentric Videos**
    - 发表：ECCV 2026
    - 亮点：将端侧助手Vinci从被动响应推进到主动，提出EgoServe，首个大规模主动辅助基准，包含10个类别的3,000+个服务实例。提出EgoMemo，一个免训练的记忆增强智能体。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.11523)

+  **Dispider: Enabling Video LLMs with Active Real-Time Interaction via Disentangled Perception, Decision, and Reaction**
    - 发表：CVPR 2025
    - 亮点：解耦的感知‑决策‑反应框架，用于实时交互视频LLM。
    - 论文链接：[项目页面](https://dispider.github.io/)

+  **StreamBridge: Turning Your Offline Video Large Language Model into a Proactive Streaming Assistant**
    - 发表：NeurIPS 2025
    - 亮点：无需重新训练即可将离线视频LLM转换为主动流式助手。
    - 论文链接：[项目页面](https://streambridge-vlm.github.io/)

+  **Flash-VStream: Efficient Real-Time Understanding for Long Video Streams**
    - 发表：ICCV 2025
    - 亮点：长时视频流的高效实时理解流程。
    - 论文链接：[项目页面](https://github.com/yydlm/Flash-VStream)

+  **Proactive Agent: Shifting LLM Agents from Reactive Responses to Active Assistance**
    - 发表：ICLR 2025
    - 亮点：将LLM智能体从被动响应转变为主动程序化辅助的范式转变。
    - 论文链接：[arXiv](https://arxiv.org/abs/2410.12361)

+  **YETI (YET to Intervene) Proactive Interventions by Multimodal AI Agents in Augmented Reality Tasks**
    - 发表：arXiv 2025
    - 亮点：多模态AI智能体在AR程序化任务中的主动干预框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2501.09355)

+  **Proactive Assistant Dialogue Generation from Streaming Egocentric Videos**
    - 发表：EMNLP 2025
    - 亮点：从流式第一人称程序化视频生成上下文感知的主动助手对话。
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.05904)

+  **VideoLLM-online: Online Video Large Language Model for Streaming Video**
    - 发表：CVPR 2024
    - 亮点：专为流式第一人称视频输入设计的在线视频LLM框架。
    - 论文链接：[arXiv](https://arxiv.org/abs/2406.11816) | [项目页面](https://showlab.github.io/videollm-online/)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 会议 | 核心任务 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| EgoProactive | 2026 | arXiv | 主动式程序化辅助 | [arXiv](https://arxiv.org/abs/2606.06220) |
| EASG-Bench | 2025 | arXiv | 带动作场景图的视频QA | [arXiv](https://arxiv.org/abs/2508.01867) |
| EOC-Bench | 2025 | arXiv | 物体中心具身认知 | [arXiv](https://arxiv.org/abs/2506.05287) |
| EgoNight | 2025 | arXiv | 夜间第一人称VQA | [arXiv](https://arxiv.org/abs/2510.08961) |
| OVO-Bench | 2025 | CVPR | 在线实时视频理解基准 | [项目页面](https://ovo-bench.github.io/) |
| SVBench | 2025 | ICLR | 多轮对话流式视频理解 | [项目页面](https://svbench.github.io/) |
| STREAMGAZE | 2025 | arXiv | 视线引导的主动流式视频理解 | [arXiv](https://arxiv.org/abs/2512.01707) |
| ProactiveVideoQA | 2025 | arXiv | 视频LLM主动交互评估 | [arXiv](https://arxiv.org/abs/2504.12345) |
| CaptainCook4D | 2024 | NeurIPS | 程序化错误检测、4D活动理解 | [项目页面](https://captaincook4d.github.io/) |
| EgoOops | 2024 | ICCV | 带程序化文本引用的错误动作检测 | [项目页面](https://ego-oops.github.io/) |
| IndustReal | 2024 | WACV | 工业程序化步骤识别、错误检测 | [项目页面](https://timschoonbeek.github.io/industreal.html) |
| HoloAssist | 2023 | ICCV | 交互式程序化AI助手、错误检测 | [项目页面](https://holoassist.github.io/) |
| EgoProceL | 2022 | CVPR | 第一人称程序化学习基准 | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| Assembly101 | 2022 | CVPR | 多视角程序化组装活动理解 | [官方网站](https://assembly-101.github.io/) |
| EgoExoLearn | 2024 | CVPR | 从示范到实践的跨视角程序化学习 | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |

---

### 2.10 🛡️ 第一人称数据安全与隐私保护
随着可穿戴相机和第一人称视频数据的迅速普及，数据安全和隐私已成为第一人称视觉中的关键问题。与传统的第三人称视觉不同，第一人称视频天生携带佩戴者的身份、行为、社交关系和环境的敏感信息，同时旁观者经常在未经同意的情况下被记录。本节总结了**隐私风险评估与基准**、**匿名化与数据去标识化**、**隐私保护技术**以及**伦理与政策考量**方面的代表性工作。

#### 2.10.1 隐私风险评估与基准
+  **Position: Life‑Logging Video Streams Make the Privacy‑Utility Trade‑off Inevitable**
    - 发表：arXiv 2026
    - 亮点：系统分析生活日志视频流在感知、传输和存储整个流程中的隐私风险，指出现有单点隐私保护方法在跨视角协同场景中的局限性。
    - 论文链接：[arXiv](https://arxiv.org/abs/2605.10404)

+  **EgoPrivacy: What Your First-Person Camera Says About You?**
    - 发表：ICML 2025
    - 亮点：首个大规模第一人称隐私风险评估基准，系统回答“从第一人称视频中可以推断出佩戴者的哪些信息？”。涵盖三类隐私（人口统计、个体、上下文），定义七个不同粒度的隐私恢复任务。提出利用ego‑to‑exo检索的**检索增强攻击**。实验表明，基础模型在零样本设置下以**70‑80%的准确率**恢复身份、场景、性别、种族等属性。
    - 论文链接：[arXiv](https://arxiv.org/abs/2506.12258) | [GitHub](https://github.com/williamium3000/ego-privacy)

+  **EgoNormia: Benchmarking Physical‑Social Norm Understanding**
    - 发表：ACL 2025 Findings
    - 亮点：构建一个规范理解基准，包含**1,853个多选题**，涵盖七类规范（安全、隐私、近体空间、礼貌、合作、协调/主动性、沟通/可读性）。评估表明，最先进的VLM在EgoNormia上仅达到**54%**，揭示了真实世界智能体应用中显著的**安全与隐私风险**。
    - 论文链接：[ACL Anthology](https://aclanthology.org/2025.findings-acl.985/)

+  **EAPrivacy: Benchmarking Physical-World Privacy Awareness of LLM-Powered Agents**
    - 发表：arXiv 2025
    - 亮点：引入一个综合评估基准，旨在量化LLM驱动的具身智能体对物理世界隐私的感知能力。
    - 论文链接：[arXiv](https://arxiv.org/abs/2510.02356) | [GitHub](https://github.com/Graph-COM/EAPrivacy)

#### 2.10.2 匿名化与数据去标识化
+  **EgoBlur: Responsible Innovation in Aria**
    - 发表：Meta Reality Labs 2023
    - 亮点：**Project Aria**的核心匿名化系统，旨在数据采集阶段模糊**旁观者面部和车辆牌照**。使用FasterRCNN作为检测器，并对检测到的PII区域应用高斯模糊。
    - 论文链接：[arXiv](https://arxiv.org/abs/2308.13093)

+  **Ego4D Privacy & Ethics Framework**
    - 发表：Ego4D数据集文档
    - 亮点：Ego4D数据集（3,670小时，931名参与者，9个国家）在采集过程中采用**严格的隐私和伦理标准**。参与者可选择模糊处理，**612小时**在明确同意下保持未模糊。数据集使用全面的**去标识化流程**，并发布详细的隐私和伦理指南。
    - 论文链接：[Ego4D Privacy Page](https://ego4d-data.org/pages/privacy-and-ethics)

#### 2.10.3 隐私保护技术
+ **边缘隐私过滤**
    +  **Extra‑Lightweight AI‑Based Privacy Preserving Framework for Egocentric Wearable Cameras (EPIC)**
        - 发表：CVPR 2025 Workshops
        - 亮点：为资源受限的可穿戴相机提出超轻量级AI隐私保护框架。采用st_yolo_lc_v1模型进行人脸检测，在存储或发送图像前模糊细节信息。在仅640 KB RAM的STM32L4 MCU上实现，人脸检测mAP达到41.38%。
        - 论文链接：[OpenAccess CVF](https://openaccess.thecvf.com/content/CVPR2025W/MTF/html/Li_Extra-Lightweight_AI-Based_Privacy_Preserving_Framework_for_Egocentric_Wearable_Cameras_CVPRW_2025_paper.html)

#### 2.10.4 伦理、政策与社会影响
+  **Privacy and Ethical Challenges in Egocentric Data Collection**
    - 发表：The Indian Express / Moneycontrol 2026
    - 亮点：报道印度成为第一人称AI数据采集热点及其引发的隐私担忧。指出第一人称录像可能**无意中捕捉到面部、私人对话、敏感工作流程或未经同意的旁观者**，引发**监控、同意和劳动力替代**等伦理问题。
    - 论文链接：[The Indian Express](https://indianexpress.com/) | [Moneycontrol](https://www.moneycontrol.com/)

+  **Smart Glasses and GDPR: Europe's Regulatory Crackdown**
    - 发表：GDPR Local 2026
    - 亮点：报道欧洲数据保护机构、欧洲议会议员和EDPB对**智能眼镜**的严格审查；核心问题是**相机捕捉到的旁观者无法有意义地表示同意**。法国CNIL和EDPB均于2026年启动专项工作，EDPB关于智能眼镜“社会可接受性”的报告预计于2026年夏季发布。
    - 论文链接：[GDPR Local](https://gdprlocal.com/)

#### 📊 相关数据集与资源
| 名称 | 类型 | 年份 | 核心内容 | 链接 |
| :--- | :--- | :--- | :--- | :--- |
| EgoPrivacy | 隐私风险评估基准 | 2025 | 三类隐私、七项隐私恢复任务 | [GitHub](https://github.com/williamium3000/ego-privacy) |
| EgoNormia | 规范理解基准 | 2025 | 1,853个多选题，覆盖七类规范（含隐私） | [ACL](https://aclanthology.org/2025.findings-acl.985/) |
| EgoBlur | 匿名化系统 | 2023 | 实时模糊人脸和车牌 | [arXiv](https://arxiv.org/abs/2308.13093) |
| Ego4D Privacy Policy | 数据集隐私框架 | 2022 | 去标识化流程、参与者同意机制 | [Ego4D](https://ego4d-data.org/pages/privacy-and-ethics) |

---

## 📊 数据集、基准与模拟器

### 通用大规模第一人称数据集
| 数据集名称 | 发布年份 | 规模 | 核心支持任务 | 官方链接 |
| :--- | :--- | :--- | :--- | :--- |
| HD-EPIC | 2025 | 41小时超高分辨率烹饪录像，密集多层标注 | 细粒度活动理解、密集VQA、多模态对齐 | [arXiv](https://arxiv.org/pdf/2502.04144) |
| Ego-Exo4D | 2024 | 1,286小时同步第一/第三人称多模态片段 | 跨视角对齐、人类技能分析、4D重建 | [官方网站](https://ego-exo4d-data.org/) |
| Ego4D | 2022 | 3,670小时可穿戴视频，9个国家923名参与者 | 动作识别、情景记忆、社交交互、3D人体姿态 | [官方网站](https://ego4d-data.org/) |
| EPIC-KITCHENS-100 | 2020 | 100小时厨房录像，9万个标注动作片段 | 动作检测、识别、未来预测 | [官方网站](https://epic-kitchens.github.io/) |

### 细粒度任务专用数据集
#### 物体与HOI子集
+  **EgoObjects**
    - 发布：ICCV 2023
    - 规模：试点版本包含9K+视频，由来自50+国家的250名参与者使用4种可穿戴设备采集，包含368个物体类别的65万+个物体标注。
    - 核心任务：细粒度物体理解
    - 链接：https://github.com/facebookresearch/EgoObjects

+  **EgoXtreme**
    - 发布：CVPR 2026
    - 规模：挑战性第一人称6D姿态数据集，包含运动模糊、严重遮挡和极端光照变化。
    - 核心任务：可穿戴相机的鲁棒物体6D姿态估计
    - 链接：https://arxiv.org/pdf/2603.25135

+  **TouchMoment**
    - 发布：CVPR 2026
    - 规模：15万帧标注了精确接触开始/结束时间戳和接触类别。
    - 核心任务：细粒度手‑物接触时刻检测
    - 链接：https://arxiv.org/pdf/2604.12343

+  **EgoPressure**
    - 发布：arXiv 2024
    - 规模：5小时多模态录像，同步触觉压力图、IMU信号和RGB。
    - 核心任务：触觉感知手‑物交互建模
    - 链接：https://arxiv.org/pdf/2409.02224

#### 程序化任务子集
+  **CaptainCook4D**
    - 发布：NeurIPS 2024
    - 规模：烹饪程序化视频，包含4D标注和错误标签。
    - 核心任务：程序化错误检测、步骤理解
    - 链接：https://captaincook4d.github.io/

+  **EgoOops**
    - 发布：ICCV 2024
    - 规模：与程序化文本对齐的错误动作检测数据集。
    - 核心任务：文本引用第一人称错误检测
    - 链接：https://ego-oops.github.io/

+  **IndustReal**
    - 发布：WACV 2024
    - 规模：约6小时工业组装视频，含执行错误标注。
    - 核心任务：工业程序化步骤识别、错误检测
    - 链接：https://timschoonbeek.github.io/industreal.html

#### 长视频与情景记忆数据集
+  **EgoLife**
    - 发布：CVPR 2025
    - 规模：来自6位共居参与者的连续多日录像，密集日常事件标注。
    - 核心任务：长期生活日志记忆检索与个人事件QA
    - 链接：https://arxiv.org/pdf/2503.03803

+  **EgoSchema**
    - 发布：NeurIPS 2023
    - 规模：500+个长第一人称片段，含多步时序推理多选题。
    - 核心任务：超长时序视频语言理解基准
    - 链接：https://github.com/egoschema/EgoSchema

#### 专用领域数据集
+  **EgoExOR**
    - 发布：NeurIPS 2025
    - 规模：手术室可穿戴视频，同步手术工具跟踪和患者生物特征。
    - 核心任务：手术工作流识别、器械检测
    - 链接：https://arxiv.org/pdf/2505.24287

+  **EgoDex**
    - 发布：2025
    - 规模：Apple Vision Pro捕获的日常物体操作序列，含精确6D手部姿态标注。
    - 核心任务：灵巧可穿戴手部姿态估计与操作预测
    - 链接：https://arxiv.org/abs/2505.11709

+  **MECCANO**
    - 发布：2021
    - 规模：12小时工业组装录像，配眼动追踪流。
    - 核心任务：工业细粒度动作与手‑物交互分析
    - 链接：https://github.com/fpv-iplab/MECCANO

+  **EgoExo-Fitness**
    - 发布：ECCV 2024
    - 规模：从同步的第一人称和固定第三人称相机记录的健身序列视频。
    - 核心任务：全身动作理解
    - 链接：[GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness)

### 具身VLA评估基准
+  **EgoVerse**
    - 发布：2026
    - 规模：1,000+标准化具身任务，涵盖导航、操作和视觉QA。
    - 核心任务：统一机器人模仿与可穿戴VLA评估套件
    - 链接：https://arxiv.org/pdf/2604.07607

+  **EgoBench**
    - 发布：2026
    - 规模：可穿戴具身智能体的交互式闭环评估平台。
    - 核心任务：实时交互决策基准
    - 链接：https://arxiv.org/pdf/2605.27820

### 第一人称世界模拟器
+  **PlayerOne**
    - 发布：NeurIPS 2025
    - 亮点：逼真开放世界第一人称模拟器，支持完全相机、人体运动和物体交互控制，用于合成数据生成。
    - 链接：https://arxiv.org/abs/2512.06724

+  **EgoSim**
    - 发布：arXiv 2026
    - 亮点：闭环动态模拟器，具有持久3D场景状态，用于生成一致的顺序交互录像。
    - 链接：https://arxiv.org/pdf/2604.01001

---

## 👓 智能眼镜专项研究与部署

### 专项基准与可穿戴数据集
+  **SUPERGLASSES: Benchmarking Vision Language Models as Intelligent Agents for AI Smart Glasses**
    - 发表：CVPR 2026
    - 亮点：首个在Ray‑Ban Meta、小米智能眼镜和Thunderbird V4等真实消费级智能眼镜上采集的基准，涵盖多样日常场景。
    - 论文链接：[arXiv](https://arxiv.org/pdf/2602.22683)

+  **Project Aria Datasets**
    - 发布方：Meta Research
    - 亮点：完整的多模态可穿戴数据集套件，含同步RGB、深度、IMU和眼动追踪信号。
    - 官方链接：https://www.projectaria.com/

### 关键技术研究方向
#### 低功耗端侧感知
+  **OpenGlass: Ultra-Low-Power On-Device AI Eyewear with Event-based Vision**
    - 发表：arXiv 2026
    - 亮点：完全开源的事件相机可穿戴硬件栈，配合轻量级边缘推理算法。
    - 论文链接：[arXiv](https://arxiv.org/pdf/2606.07431)

+  **EgoTrigger: Toward Audio-Driven Image Capture for Human Memory Enhancement in All-Day Energy-Efficient Smart Glasses**
    - 所属机构：UNC Chapel Hill + Google
    - 发表：IEEE TVCG 2025
    - 亮点：音频事件触发的选择性帧捕获，总功耗降低87%。
    - 论文链接：[arXiv](https://arxiv.org/pdf/2508.01915)

#### 终身记忆与个人助手系统
+  **EGAgent: Agentic Very Long Video Understanding**
    - 发表：arXiv 2026
    - 亮点：基于实体场景图的推理智能体，处理跨天连续可穿戴视频流，支持多跳检索和音视频混合搜索。
    - 论文链接：[arXiv](https://arxiv.org/abs/2601.18157)

+  **LightMem-Ego: Your AI Memory for Everyday Life**
    - 发表：arXiv 2026
    - 亮点：将轻量级智能手机或AI眼镜风格客户端与后端连接，摄取第一人称视听流作为日常生活的记忆伴侣。
    - 论文链接：[arXiv](https://arxiv.org/abs/2607.11487)

#### 自然可穿戴人机交互
+  **VisionClaw: Always-On AI Agents Through Smart Glasses**
    - 发表：arXiv 2026
    - 亮点：持久后台可穿戴智能体，支持免提多场景任务执行。
    - 论文链接：[arXiv](https://arxiv.org/pdf/2604.03486)

+  **Egocentric Co-Pilot: Web-Native Lightweight Smart Glasses Assistant**
    - 发表：WWW 2026
    - 亮点：基于浏览器的轻量级可穿戴助手架构，无需安装原生应用。
    - 论文链接：[arXiv](https://arxiv.org/pdf/2603.01104)

+  **Plug-and-Play Clarifier: A Zero-Shot Multimodal Framework for Egocentric Intent Disambiguation**
    - 发表：AAAI 2026
    - 亮点：零样本意图消歧框架，将可穿戴指令执行准确率从58%提升至87%。
    - 论文链接：[arXiv](https://arxiv.org/pdf/2511.08971)

+  **Face versus Body Tracking for Human-Robot Interaction: An Egocentric Dataset**
    - 发表：arXiv 2026
    - 亮点：新颖的第一人称数据集和优化跟踪流程，通过应对遮挡和复杂社交动态减少社交机器人中的身份切换。
    - 论文链接：[arXiv](https://arxiv.org/abs/2606.03694)

#### 数据采集基础设施
+  **AoE: Always-on Egocentric Human Video Collection for Embodied AI**
    - 发表：arXiv 2026 (Mar 2026)
    - 亮点：一种经济高效、可扩展的系统，利用人类智能体和智能手机技术采集真实世界交互数据。
    - 论文链接：[arXiv](https://arxiv.org/abs/2602.23893)

---

## 🔗 相关Awesome列表
- [Awesome-Egocentric](https://github.com/EgoAlpha/Awesome-Egocentric)
- [awesome-egocentric-vision](https://github.com/Sid2697/awesome-egocentric-vision)
- [Awesome-Egocentric-and-Exocentric-Vision](https://github.com/ayiyayi/Awesome-Egocentric-and-Exocentric-Vision)
- [Building Egocentric Procedural AI Assistant](https://github.com/z1oong/Building-Egocentric-Procedural-AI-Assistant)

---

## 🎯 关键研究挑战

### 所有子任务的通用基础挑战
1. **内在的第一人称视觉缺陷**：窄视野、严重自遮挡、剧烈相机抖动、不稳定光照和模糊的可穿戴图像降低了所有下游任务的性能。
2. **第一人称数据稀缺与隐私壁垒**：可穿戴录像携带敏感个人信息；采集和标注成本远高于互联网第三人称视频，造成数量级数据集规模差距，限制了大型模型扩展。跨视角协同场景进一步放大了隐私风险。
3. **严重的人际分布偏移**：用户身高、日常行为模式和生活环境的巨大差异导致通用模型在个性化可穿戴场景上泛化能力差。
4. **超长序列建模瓶颈**：全天候连续可穿戴流对现有视频和多模态架构提出了严峻的内存容量和长程依赖建模挑战。

### 领域特定核心挑战
| 研究方向 | 核心开放挑战 | 近期进展（2026） |
| :--- | :--- | :--- |
| **动作识别与预测** | 细粒度动词‑名词组合歧义；未裁剪长视频上的时序定位精度低。 | **UNIEGO** 通过多教师蒸馏统一ego‑exo、RGB、深度和骨骼模态，在识别、检索和分割上达到SOTA。**Divide, Deliberate, Decide** 实现零样本多智能体VLM商议，用于细粒度识别。 |
| **手‑物交互（HOI）** | 接触状态标注成本高；物理一致性建模困难；手与物体之间严重相互遮挡。 | **EgoHOI** 将物理先验嵌入扩散世界模型。**Hand‑4DGS** 实现单视角第一人称视频的端到端4D手部重建。**EgoGrasp** 从动态第一人称视频重建世界空间HOI。 |
| **Ego‑VLM与多模态推理** | 缺乏第一人称常识先验；时空多步推理弱；跨模态对齐与同步；缺失模态处理。 | **EgoSAT** 揭示流式设置中模型的严重校准偏差。**Egocentric Bias in VLMs** 显示103个VLM中91.3%表现出系统性自我中心偏差。**EgoReasoner** 使用任务自适应结构化思维进行4D推理。 |
| **长视频与结构化推理** | 模型上下文窗口有限；时序事件定位模糊；长视频可扩展场景图构建。 | **Imprint** 以2.3倍内存占用缩减压缩长时记忆。**Graph it first!** 使用第一人称场景图克服MLLM输入限制。**LongEgoRefer** 提供45分钟视频指代理解的基准。 |
| **视线与用户意图预测** | 眼动模式个体差异大；隐性意图难以标注；多模态信号对齐弱。 | **EPIC** 利用视线/姿态/惯性信号在AR眼镜上减少内存27.5倍、能耗24.3倍。**Ego‑PMOVE** 通过MoE探索跨视角视线相关性。**EyeCue** 通过视线增强的第一人称视频检测驾驶员认知分心。 |
| **3D/4D重建与结构化感知** | 单目深度模糊；动态移动物体重建失败；动态场景图更新。 | **Whareformer** 引入首个基于学习的OSNOM长视频跟踪器。**TSR‑Ego** 通过时序引导立体细化在UnrealEgo2上达到SOTA。**R3D‑Bench** 在Aria Digital Twin上提供3,033个定量3D空间推理QA对。 |
| **Ego‑VLA与具身AI** | 人‑机器人具身差距大；动作空间未对齐；策略从人到机器人迁移；仿真到真实泛化；主动感知建模。 | **HumanScale** 显示第一人称人类视频**优于真实机器人数据**进行预训练（成功率高出52.5%）。**ACE‑Ego‑0** 通过可扩展视频到动作流程统一人类/机器人数据用于VLA预训练。**ActiveMimic** 将相机运动建模为视点动作以实现主动感知。**EgoWAM** 比较像素/DINO/3D流作为世界预测目标——DINO将OOD泛化提升**4倍**，3D流将领域内性能提升20‑30%。**EgoSteer** 将灵巧VLA预训练扩展到9,600小时。**HumanEgo** 每任务30分钟人类视频实现92.5%零样本成功率。 |
| **第一人称世界模型** | 长展开中时序一致性退化；生成真实感与物理合理性权衡；用户动作可控性弱；跨视角数据利用；隐式与像素级预测。 | **Walk through Paintings** 通过轻量级适配器将预训练视频扩散模型重新用作动作条件世界模型——SCS提升**80%**，延迟降低**6倍**。**EgoExo‑WM** 通过姿态提取和视角转换解锁第三人称视频用于第一人称世界模型训练。**EgoSim** 实现带持久3D场景状态的**闭环**第一人称模拟。**EgoForge** 使用轨迹级奖励引导扩散实现目标导向生成。**WLA模型** 在单一基础模型中统一世界建模、语言推理和动作合成（RoboTwin2.0上92.94%成功率）。**Hand2World** 实现自由空间手势驱动的第一人称交互生成。**Being‑H0.7** 探索隐式世界‑动作模型，避免显式帧生成以提高效率。 |
| **第一人称程序化AI助手** | 细粒度错误边界模糊；程序化知识接地困难；实时主动干预时机控制。 | **Vinci2** 从被动响应推进到主动辅助，附带**EgoServe**基准（3,000+服务实例）。**Plan, Watch, Recover** 引入**EgoProactive**数据集，含显式“偏离计划”标注。**EgoCoT‑Bench** 提供3,172个可验证QA对，用于操作中心化CoT推理。 |
| **数据安全与隐私** | 佩戴者与旁观者隐私平衡；数据最小化中的隐私‑效用权衡；同意与法规遵从（GDPR）；跨视角协作中的隐私放大。 | **EgoPrivacy**（2025）提供首个大规模第一人称隐私风险评估基准。**EgoNormia**（2025）揭示VLM在物理‑社会规范理解上仅达到54%，存在显著安全/隐私风险。 |

---

## ❤️ 联系方式
如果您有新增论文或数据集建议、发现任何不准确之处，或觉得本资源列表对您有帮助，欢迎通过邮件联系孙源良：sun254667307@gmail.com。
关于第一人称视觉的研究实习机会咨询，也欢迎随时联系。

## ⭐ 致谢
本精选集参考并借鉴了多个社区第一人称视觉仓库：
- Awesome-Egocentric-Video-Datasets
- Building Egocentric Procedural AI Assistant

## 📄 许可证
CC0 1.0 通用版。完整条款见本仓库的 `LICENSE` 文件。
