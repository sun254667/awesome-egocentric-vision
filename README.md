

> 精心整理的第一人称视觉（Egocentric Vision）领域资源清单，涵盖论文、数据集、开源工具、预训练模型、挑战赛、学习路线等内容，兼顾经典奠基工作与前沿进展，面向科研入门与产业落地。
>
> A curated, learning-friendly list of egocentric (first-person) vision & embodied AI resources: papers, datasets, code, models, toolkits, challenges and tutorials.
>

✅ **收录标准 Inclusion Criteria**

+ 优先收录 CVPR / ICCV / ECCV / NeurIPS / ICLR / AAAI / TPAMI / TVCG 等顶会顶刊高质量工作
+ 覆盖核心前沿方向：Ego-VLM/LLM、Ego-VLA具身智能、3D/4D重建、手物交互、视线估计、长视频理解、世界模型

---

## 📑 目录 Table of Contents
1. [📚 综述与领域概览 Surveys & Overviews](#-综述与领域概览-surveys--overviews)
2. [🔬 核心研究方向 Core Research Topics](#-核心研究方向-core-research-topics)
    - 2.1 动作识别、检测与预判 Action Recognition, Detection & Anticipation
    - 2.2 手物交互与细粒度活动 Hand-Object Interaction & Fine-grained Activity
    - 2.3 第一人称视觉语言模型 Ego-VLM / Ego-LLM
    - 2.4 长时序视频理解与问答 Long-form Video Understanding & QA
    - 2.5 视线、注意力与意图预测 Gaze, Attention & Intention Prediction
    - 2.6 3D/4D重建与空间感知 3D/4D Reconstruction & Spatial Perception
    - 2.7 视觉-语言-动作与具身智能 Ego-VLA & Embodied AI
    - 2.8 第一人称世界模型 Egocentric World Models
3. [📊 数据集、基准与模拟器 Datasets, Benchmarks & Simulators](#-数据集基准与模拟器-datasets-benchmarks--simulators)
4. [👓 智能眼镜专属研究与落地 Smart Glasses Exclusive Research](#-智能眼镜专属研究与落地-smart-glasses-exclusive-research)
5. [🔗 相关资源列表 Related Awesome Lists](#-相关资源列表-related-awesome-lists)
6. [🎯 核心研究挑战 Key Research Challenges](#-核心研究挑战-key-research-challenges)

---

## 📚 综述与领域概览 Surveys & Overviews
> 入门领域的首选材料，帮助快速建立全局认知，梳理发展脉络、核心任务与关键挑战。
>

+ **Challenges and Trends in Egocentric Vision: A Survey**
    - 发布：arXiv 2025
    - 亮点：领域最新全景综述，系统分类主体理解、物体理解、环境理解、混合理解四大任务方向，全面总结挑战与趋势
    - 论文链接：[https://arxiv.org/abs/2503.15275](https://arxiv.org/abs/2503.15275)
+ **Building Egocentric Procedural AI Assistant: Methods, Benchmarks, and Challenges**
    - 发布：arXiv 2025
    - 亮点：首次系统提出第一视角程序化 AI 助手的完整技术框架，定义错误检测、程序化学习、视觉问答三大核心任务，以及实时流处理、主动交互两大支撑维度
    - 论文链接：[https://arxiv.org/pdf/2511.13261](https://arxiv.org/pdf/2511.13261)
+ **An Outlook into the Future of Egocentric Vision**
    - 发布：arXiv 2023
    - 亮点：领域权威学者联合撰写，结合可穿戴计算未来场景，梳理研究短板与待突破方向
    - 论文链接：[https://arxiv.org/abs/2308.07123](https://arxiv.org/abs/2308.07123)
+ **Bridging Perspectives: A Survey on Cross-view Collaborative Intelligence with Egocentric-Exocentric Vision**
    - 发布：arXiv 2025
    - 亮点：系统梳理主视角-外视角协同学习方向，涵盖外视角辅助主视角、主视角辅助外视角、联合学习三类范式
    - 论文链接：[https://arxiv.org/abs/2506.06253](https://arxiv.org/abs/2506.06253)
+ **First-Person Vision**
    - 发布：Proceedings of the IEEE 2012
    - 亮点：领域奠基性综述，首次正式定义第一人称视觉的研究范畴、核心挑战与应用方向
    - 论文链接：[https://ieeexplore.ieee.org/document/6232429](https://ieeexplore.ieee.org/document/6232429)
+ **HD-EPIC: A Highly-Detailed Egocentric Video Dataset**
    - 发布：arXiv 2025
    - 亮点：构建了当前标注密度最高的真实家庭场景无脚本第一视角数据集，包含 41 小时厨房烹饪视频，覆盖食谱步骤、细粒度动作、食材营养、3D 数字孪生场景、眼动数据、音频事件等多层级联动标注
    - 论文链接：[https://arxiv.org/pdf/2502.04144](https://arxiv.org/pdf/2502.04144)
+ **Ego-Exo4D: Understanding Skilled Human Activity from First- and Third-Person Perspectives** 
    - 发布：CVPR 2024
    - 亮点：目前全球规模最大的同步采集第一 / 第三视角多模态数据集，包含 1286 小时覆盖运动、音乐、舞蹈、器械维修等专业技能场景的配对视频
    - 论文链接：[https://arxiv.org/pdf/2311.18259](https://arxiv.org/pdf/2311.18259)
+ **EgoExoLearn: A Dataset for Bridging Asynchronous Ego- and Exo-centric View of Procedural Activities in Real World** 
    - 发布：CVPR 2024
    - 亮点：首个模拟人类 "观看第三人称演示 - 第一人称实操" 学习过程的异步跨视角数据集，包含 120 小时覆盖日常生活与专业实验室场景的演示视频与实操第一视角视频配对数据
    - 论文链接：[https://arxiv.org/pdf/2403.16182](https://arxiv.org/pdf/2403.16182)
+ **EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding** 
    - 发布：ICCV 2023
    - 亮点：提出面向超长时序第一视角视频的语言理解诊断基准，引入 "时间证书" 量化指标来衡量任务的内在时间推理难度
    - 论文链接：[https://arxiv.org/pdf/2308.09126](https://arxiv.org/pdf/2308.09126)
+ **Ego4D: Around the World in 3,000 Hours of Egocentric Video** 
    - 发布：CVPR 2022
    - 亮点：迄今为止全球规模最大的第一人称视角视频数据集，包含来自全球 9 个国家 74 个地点、923 名参与者采集的 3670 小时日常生活活动视频
    - 论文链接：[https://arxiv.org/pdf/2110.07058](https://arxiv.org/pdf/2110.07058)
+ **Rescaling Egocentric Vision**
    - 发布：IJCV 2021
    - 亮点：发布经典大规模第一视角厨房动作数据集 EPIC-KITCHENS-100，包含 100 小时视频、9 万 + 细粒度动作片段，提出 "暂停 - 讲述" 的创新标注流水线，显著提升了标注密度与准确性
    - 论文链接：[https://arxiv.org/pdf/2006.13256](https://arxiv.org/pdf/2006.13256)
+ **Charades-Ego: A Large-Scale Dataset of Paired Third and First Person Videos**
    - 发布：CVPR 2018
    - 亮点：构建了首个大规模配对的第一 / 第三视角日常动作数据集，覆盖多样家庭场景与日常活动类别
    - 论文链接：[https://arxiv.org/pdf/1804.09626](https://arxiv.org/pdf/1804.09626)
+ **Position: Life-Logging Video Streams Make the Privacy-Utility Trade-off Inevitable**
    - 发布：arXiv 2026
    - 亮点：系统剖析了生活日志类视频流在感知、传输、存储全链路的隐私风险，指出现有单点式隐私保护方法在跨视角协同场景下的局限性
    - 论文链接：[https://arxiv.org/pdf/2605.10404](https://arxiv.org/pdf/2605.10404)

---

## 🔬 核心研究方向 Core Research Topics
### 2.1 动作识别、检测与预判 Action Recognition, Detection & Anticipation
> Egocentric视觉最基础、最成熟的方向，研究从第一人称视频中识别、检测、预测人类动作。
>

#### 动作识别与检测
+ **EgoAction: Egocentric Action Composition with Reliability-Aware Temporal Fusion**
    - 发布：CVPR 2026 EPIC-KITCHENS 挑战赛冠军方案
    - 亮点：提出解耦式动词-名词检测+动态加权融合策略，基于VideoMAE-L特征实现长未修剪视频SOTA精度
    - 论文链接：[https://arxiv.org/abs/2605.24496](https://arxiv.org/abs/2605.24496)
+ **Ego-Only: Egocentric Action Detection without Exocentric Transferring**
    - 发布：ICCV 2023
    - 亮点：首次证明纯第一人称数据训练的模型可以超越依赖第三人称迁移的方法
    - 论文链接：[https://openaccess.thecvf.com/content/ICCV2023/papers/Wang_Ego-Only_Egocentric_Action_Detection_without_Exocentric_Transferring_ICCV_2023_paper.pdf](https://openaccess.thecvf.com/content/ICCV2023/papers/Wang_Ego-Only_Egocentric_Action_Detection_without_Exocentric_Transferring_ICCV_2023_paper.pdf)
+ **MM-CDFSL: Multimodal Cross-Domain Few-Shot Learning for Egocentric Action Recognition**
    - 发布：ECCV 2024
    - 亮点：首次系统研究egocentric动作识别的跨域少样本场景，提出多模态蒸馏框架
    - 论文链接：[https://arxiv.org/pdf/2405.19917](https://arxiv.org/pdf/2405.19917)

#### 动作预判
+ **GANO: Enhancing Next Active Object-Based Egocentric Action Anticipation with Guided Attention**
    - 发布：arXiv 2023
    - 亮点：针对下一活跃物体预测任务，提出引导式注意力机制
    - 论文链接：[https://arxiv.org/abs/2305.12953](https://arxiv.org/abs/2305.12953)
+ **PALM: Predicting Actions through Language Models**
    - 发布：arXiv 2023
    - 亮点：首次将大语言模型引入长时序动作预判
    - 论文链接：[https://arxiv.org/abs/2311.17944](https://arxiv.org/abs/2311.17944)
+ **INSIGHT: Intention-Guided Cognitive Reasoning for Egocentric Long-Term Action Anticipation**
    - 发布：AAAI 2026
    - 亮点：提出「HOI语义识别+意图推理」两阶段框架
    - 论文链接：[https://arxiv.org/pdf/2508.01742](https://arxiv.org/pdf/2508.01742)
+ **Ego4OOD: Rethinking Egocentric Video Domain Generalization via Covariate Shift Scoring**
    - 发布：arXiv 2026
    - 亮点：提出Ego4OOD领域泛化基准，包含8个地理上不同的域，引入基于聚类的协变量偏移度量
    - 论文链接：[https://arxiv.org/abs/2601.17056](https://arxiv.org/abs/2601.17056)
+ **Cross-Modal Action Recognition in Egocentric Video Using Mamba: Integrating RGB and Hand Skeleton Streams via CLS Token Fusion Strategies**
    - 发布：EgoVis@CVPR 2026
    - 亮点：基于Mamba框架的跨模态架构，融合RGB视频和时间手部骨架数据，提出四种CLS Token混合策略
    - 论文链接：[https://arxiv.org/abs/2605.24302](https://arxiv.org/abs/2605.24302)
+ **Egocentric Hand Activity Video Dataset and Bidirectional Motion-Priors for Hand Action Recognition**
    - 发布：IEEE Access 2026, Vol.14
    - 亮点：发布Ego-Bi大规模第一人称RGB视频数据集（1,223个序列，622,737帧），提出双向运动先验模块
    - 论文链接：[https://ksp.etri.re.kr/ksp/article/read?id=72508](https://ksp.etri.re.kr/ksp/article/read?id=72508)
+ **Ego-METAS: Egocentric online Multimodal Energy-efficient Temporal Action Segmentation benchmark**
    - 发布：arXiv 2026
    - 亮点：首个面向能量感知的在线多模态时间动作分割基准，包含100+小时未修剪视频，覆盖5种模态
    - 论文链接：[https://arxiv.org/abs/2606.02246](https://arxiv.org/abs/2606.02246)
+ **Continual Multimodal Egocentric Activity Recognition via Modality-Aware Novel Detection**
    - 发布：arXiv 2026
    - 亮点：提出MAND模态感知框架，新颖活动检测AUC提升10%
    - 论文链接：[https://arxiv.org/abs/2603.16970](https://arxiv.org/abs/2603.16970)
+ **EgoFusion: unified semantic and scale-aware prompt fusion for egocentric action recognition**
    - 发布：Multimedia Systems 2026
    - 亮点：提出EgoFusion提示学习框架，通过成分语义交互模块增强动词-名词语义对齐
    - 论文链接：[https://dl.acm.org/doi/10.1007/s00530-026-02282-1](https://dl.acm.org/doi/10.1007/s00530-026-02282-1)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| --- | --- | --- | --- | --- |
| ⭐ Ego4D | 2022 | ~3,670 h | AR, VQA, forecasting, many | [官网](https://ego4d-data.org/) |
| ⭐ EPIC-KITCHENS-100 | 2021 | 100 h / 90K segments | 动作识别、检测、预判 | [官网](https://epic-kitchens.github.io/) |
| ChildLens | 2026 | 108.58 h / 354 videos | 儿童日常活动分析 | [Data](https://doi.org/10.17617/4.fe) |
| EgoScale | 2026 | 20k+ h labeled manipulation | 动作、灵巧迁移 | [论文](https://arxiv.org/abs/2602.16710) |
| CogDrive (EyeCue) | 2026 | 多场景驾驶 | 驾驶员认知分心检测 | [论文](https://arxiv.org/abs/2605.07859) |
| Ego-METAS | 2026 | 100+ h / 5 modalities | 在线动作分割、传感器路由 | [HF](https://huggingface.co/datasets/Ego-METAS/Ego-METAS) |
| Furhat Egocentric Dataset | 2026 | 20 seq. / ~25 min | 机器人-自我人脸/身体跟踪 | [论文](https://arxiv.org/abs/2606.03694) |
| World In Your Hands | 2025 | 1000+ h labeled manipulation | 动作、VLA训练 | [GitHub](https://github.com/tars-robotics/World-In-Your-Hands) |
| EgoCampus | 2025 | ~32 h | 注视、行人自我 | [GitHub](https://github.com/ComputerVisionRutgers/EgoCampus) |
| AEA | 2024 | 143 seq. / ~7.3 h | 日常活动（Aria） | [Aria](https://www.projectaria.com/datasets/aea/) |
| EgoSurgery | 2024 | 开放手术视频 | 手术阶段、工具检测 | [GitHub](https://github.com/Fujiry0/EgoSurgery) |
| EgoExo-Fitness | 2024 | 32 h / 1,276 seq. | 全身动作、质量评估 | [GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness) |
| E³ (Exploring Embodied Emotion) | 2024 | 50+ h | 情绪识别、多模态 | [GitHub](https://github.com/Exploring-Embodied-Emotion-official/E3) |
| EGOFALLS | 2023 | 跌倒样本 | 跌倒检测 | [Dataverse](https://www.dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/HO5GE3) |
| Epic-Sounding-Object | 2023 | 3.2K short clips | 视听物体定位 | [GitHub](https://github.com/WikiChao/Ego-AV-Loc) |
| HoloAssist | 2023 | 169 h | 交互式助手 | [官网](https://holoassist.github.io/) |
| WEAR | 2023 | ~19 h outdoor sports | 活动 + IMU | [官网](https://mariusbock.github.io/wear/) |
| N-EPIC-KITCHENS | 2022 | 事件+RGB子集 | 神经形态动作识别 | [GitHub](https://github.com/EgocentricVision/N-EPIC-Kitchens) |
| Ego-Deliver | 2021 | 5,360 videos | 配送行为分析 | [官网](https://egodeliver.github.io/) |
| HOMAGE | 2021 | 30 h | 家庭活动组合理解 | [GitHub](https://github.com/nishantrai18/homage) |
| MECCANO | 2021 | ~55 h industrial | 手物交互、工业 | [官网](https://iplab.dmi.unict.it/MECCANO/) |
| EGO-CH | 2020 | 27+ h | 游客行为、POI任务 | [论文](https://arxiv.org/abs/2002.00899) |
| EgoCom | 2020 | 38.5 h conversation | 多人自我对话 | [GitHub](https://github.com/facebookresearch/EgoCom-Dataset) |
| LEMMA | 2020 | 多视角活动 | 多智能体任务 | [GitHub](https://github.com/Buzz-Beater/LEMMA) |
| Charades-Ego | 2018 | 配对自我/外部 | 对齐、动作 | [官网](https://prior.allenai.org/projects/charades-ego) |
| EGTEA Gaze+ | 2018 | 28 h cooking | 注视+动作识别 | [官网](https://cbs.ic.gatech.edu/fpv/) |
| EgoGesture | 2017 | 2K+ videos / 24K samples | 手势识别 | [官网](https://nlpr.ia.ac.cn/iva/yfzhang/datasets/egogesture.html) |
| Stanford ECM | 2017 | 31 h | 日常活动分类 | [论文](https://openaccess.thecvf.com/content_cvpr_2017/html/Nakamura_Jointly_Learning_Energy_CVPR_2017_paper.html) |
| THU-READ | 2017 | 1,920 clips | 头盔RGB-D动作 | [官网](https://ivg.au.tsinghua.edu.cn/dataset/THU_READ.php) |
| PEV | 2016 | 1,226 pairs | 双人对话微动作 | [论文](https://openaccess.thecvf.com/content_cvpr_2016/html/Yonetani_Recognizing_Micro-Actions_and_CVPR_2016_paper.html) |
| FPPA | 2015 | 5 subjects | 日常动作+手部/注视 | [论文](https://openaccess.thecvf.com/content_iccv_2015/html/Zhou_Temporal_Perception_and_ICCV_2015_paper.html) |
| JPL-Interaction | 2013 | 84 videos | 第一人称活动识别 | [官网](http://michaelryoo.com/jpl-interaction.html) |
| ADL | 2012 | ~10 h | 日常活动识别 | [官网](https://www.csee.umbc.edu/~hpirsiav/papers/ADLdataset/) |
| Social Interactions | 2012 | ~60 h | 社交活动 | [官网](https://cbs.ic.gatech.edu/fpv/) |
| EgoAction | 2011 | 第一人称运动视频 | 动作识别 | [论文](https://doi.org/10.1109/CVPR.2011.5995406) |


---

### 2.2 手物交互与细粒度活动 Hand-Object Interaction & Fine-grained Activity
> 研究第一人称视角下手与物体的交互过程，是具身智能、机器人模仿学习的核心基础。
>

+ **Glove2Hand: Synthesizing Natural Hand-Object Interaction from Multi-Modal Sensing Gloves**
    - 发布：CVPR 2026 (Highlight)
    - 亮点：从多模态传感手套数据生成逼真裸手HOI视频，配套HandSense数据集
    - 论文链接：[https://arxiv.org/pdf/2603.20850](https://arxiv.org/pdf/2603.20850)
+ **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - 发布：arXiv 2026
    - 亮点：首个egocentric HOI世界模型，将物理先验嵌入生成式扩散模型
    - 论文链接：[https://arxiv.org/abs/2603.13615](https://arxiv.org/abs/2603.13615)
+ **TOUCH: Text-guided Controllable Generation of Free-Form Hand-Object Interactions**
    - 发布：ICLR 2026
    - 亮点：自由式HOI生成任务，构建WildO2大规模3D HOI数据集
    - 论文链接：[https://openreview.net/forum?id=4VW9HVCRw0](https://openreview.net/forum?id=4VW9HVCRw0)
+ **Do Egocentric Video-Language Models Truly Understand Hand-Object Interactions?**
    - 发布：ICLR 2025
    - 亮点：首次系统评测egocentric VLM的细粒度HOI理解能力，提出EgoHOIBench
    - 论文链接：[https://arxiv.org/abs/2405.17719](https://arxiv.org/abs/2405.17719)
+ **Get a Grip: Reconstructing Hand-Object Stable Grasps in Egocentric Videos**
    - 发布：arXiv 2023
    - 亮点：首次从单目egocentric视频重建手-物体稳定抓取状态
    - 论文链接：[https://arxiv.org/abs/2312.15719](https://arxiv.org/abs/2312.15719)
+ **HOI-Ref: Hand-Object Interaction Referral in Egocentric Vision**
    - 发布：arXiv 2024
    - 亮点：定义egocentric场景下HOI指代新任务，配套HOI-QA评测基准
    - 论文链接：[https://arxiv.org/pdf/2404.09933](https://arxiv.org/pdf/2404.09933)
+ **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - 发布：NeurIPS 2025
    - 亮点：提出双层架构框架，高层利用VLM推断运动先验，低层使用基于DiT的流匹配策略生成细粒度轨迹
    - 论文链接：[https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)
+ **Leveraging Synthetic Data for Enhancing Egocentric Hand-Object Interaction Detection**
    - 发布：IJCV 2026, Vol.134
    - 亮点：仅使用少量真实标注数据结合合成数据，在VISOR上AP提升11.69%，开源HOI-Synth合成数据生成流水线
    - 论文链接：[https://rd.springer.com/article/10.1007/s11263-026-02838-8](https://rd.springer.com/article/10.1007/s11263-026-02838-8)
+ **Hand Trajectory Fusion for Egocentric Natural Language Query Grounding**
    - 发布：EgoVis@CVPR 2026
    - 亮点：首次将手部运动线索融入NLQ定位任务，针对手物交互查询R1@IoU=0.3提升2.54%
    - 论文链接：[https://arxiv.org/abs/2606.02962](https://arxiv.org/abs/2606.02962)
+ **TouchAnything: A Dataset and Framework for Bimanual Tactile Estimation from Egocentric Video**
    - 发布：arXiv 2026
    - 亮点：EgoTouch数据集含1,891个操作片段、同步多视角RGB、双手3D姿态和连续触觉压力图
    - 论文链接：[https://arxiv.org/abs/2605.13083](https://arxiv.org/abs/2605.13083)
+ **EgoAERO: Learning Dexterous Manipulation from a Single Egocentric Video without Object Assets**
    - 发布：arXiv 2026
    - 亮点：无需预扫描物体资产的灵巧操作学习框架，构建EgoDex-R大规模数据集（4.3M RGB-D帧）
    - 论文链接：[https://arxiv.org/abs/2606.08057](https://arxiv.org/abs/2606.08057)
+ **EgoInteract: Synthetic Egocentric Videos Generation for Interaction Understanding and Anticipation**
    - 发布：arXiv 2026
    - 亮点：可控自中心视频生成模拟器，实现对摄像机、人体动作、物体操作的精确控制
    - 论文链接：[https://arxiv.org/abs/2605.18214](https://arxiv.org/abs/2605.18214)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| --- | --- | --- | --- | --- |
| ⭐ HOI4D | 2022 | 2.4M frames / 4K seq. | 4D HOI | [官网](https://hoi4d.github.io/) |
| ⭐ EgoDex | 2025 | 829 h / 30K trajectories | 灵巧操作、姿态 | [GitHub](https://github.com/apple/ml-egodex) |
| EventEgoHands | 2026 | 48 clips / 129.6K frames | RGB+事件手部检测 | [GitHub](https://github.com/SynthSyntax/EventEgoHands) |
| EgoTactile | 2026 | ~6 h / 768 clips | 抓取压力估计 | [官网](https://egotactile.github.io/) |
| EgoDex-R | 2026 | 4.3M RGB-D frames / 5.6K seq. | 灵巧操作、手物姿态 | [论文](https://arxiv.org/abs/2606.08057) |
| HA-Ego-1K | 2026 | ~24 h / 484 multi-view clips | 灵巧操作 | [HF](https://huggingface.co/datasets/humanarchive/HA-Ego-1K) |
| DexGloveHOI | 2026 | 3.5 h / 100K+ samples | 视觉-IMU 3D手部跟踪 | [论文](https://arxiv.org/abs/2605.21714) |
| EgoTouch | 2026 | 1,891 episodes / 208 tasks | 触觉HOI | [HF](https://huggingface.co/datasets/zhenyuxie-zhzh/EgoTouch_hdf5) |
| EgoEVHands | 2026 | 5,419 annotated seq. | 立体事件3D手势 | [GitHub](https://github.com/ZJUWang01/EgoEV-HandPose) |
| EgoEMG | 2026 | 41 participants / 10+ h | EMG+视觉手部姿态 | [GitHub](https://github.com/zhenqis123/EgoEMG) |
| HRDexDB | 2026 | 1.4K grasping trials | 灵巧抓取、触觉 | [HF](https://huggingface.co/datasets/hahahataeyun/hrdexdb) |
| TouchMoment | 2026 | 4,021 videos / 8,456 touch moments | 接触时刻检测 | [论文](https://arxiv.org/abs/2604.12343) |
| EgoFun3D | 2026 | 271 egocentric videos | 交互式3D物体 | [官网](https://3dlg-hcvc.github.io/EgoFun3D/) |
| SHOW3D | 2026 | 野外自我-外部HOI | 3D手物标注 | [论文](https://arxiv.org/abs/2603.28760) |
| FEEL | 2026 | 力同步厨房视频 | 物理动作理解 | [官网](https://www.cs.umd.edu/~edessale/feel) |
| EgoPoints | 2025 | 点轨迹+合成 | 自我视频跟踪 | [GitHub](https://github.com/AhmadDarKhalil/EgoPoints) |
| AssemblyHands | 2023 | 3M images | 3D手部姿态 | [官网](https://assemblyhands.github.io/) |
| EgoObjects | 2023 | 9.2K+ videos | 检测、实例分割 | [GitHub](https://github.com/facebookresearch/EgoObjects) |
| ENIGMA-51 | 2023 | 22 h industrial | 细粒度行为 | [官网](https://fpv-iplab.github.io/ENIGMA-51/) |
| POV-Surgery | 2023 | ~88K frames (合成) | 手术手-工具姿态 | [官网](https://batfacewayne.github.io/POV_Surgery_io/) |
| VOST | 2023 | 713 videos | 视频物体分割 | [官网](https://www.vostdataset.org/) |
| EgoBody | 2022 | 125 seq. | 身体姿态、交互 | [官网](https://egobody.ethz.ch/) |
| EgoHOS | 2022 | 11K+ images | 手-物体分割 | [GitHub](https://github.com/owenzlz/EgoHOS) |
| EgoPAT3D | 2022 | 1M+ frames RGB-D | 3D动作目标预测 | [GitHub](https://github.com/ai4ce/EgoPAT3D) |
| Touch and Go | 2022 | 12K+ vis–tactile frames | 视觉+触觉 | [官网](https://touch-and-go.github.io/) |
| VISOR | 2022 | EPIC + masks | 分割、HOI | [官网](https://epic-kitchens.github.io/VISOR) |
| H2O | 2021 | 100K+ frames | 双手交互 | [官网](https://h2odataset.ethz.ch/) |
| TREK-150 | 2021 | 150 EPIC seq. | 物体跟踪 | [官网](https://machinelearning.uniud.it/datasets/trek150/) |
| You2Me | 2020 | 14 seq. | 通过自我-外部推断身体姿态 | [GitHub](https://github.com/facebookresearch/you2me) |
| FPHA | 2018 | 1.2K seq. | 手部姿态+动作 | [官网](https://guiggh.github.io/publications/first-person-hands/) |
| EgoDexter | 2017 | ~3.2K frames | 遮挡下手部跟踪 | [官网](https://handtracker.mpi-inf.mpg.de/projects/OccludedHands/EgoDexter.htm) |
| EgoHands | 2015 | 4.8K labeled frames | 手部检测 | [官网](http://vision.soic.indiana.edu/projects/egohands/) |
| BEOID | 2014 | 58 videos | 手物交互 | [官网](https://data.bris.ac.uk/data/dataset/3wats8ruq1sp52hq3bo8dkzul3) |
| EDSH | 2013 | 2 videos | 像素级手部分割 | [官网](http://www.cs.cmu.edu/~kkitani/datasets/) |
| Handled Objects | 2009 | 11 categories | 抓取序列 | [论文](https://doi.org/10.1109/CVPRW.2009.5204360) |


---

### 2.3 第一人称视觉语言模型 Ego-VLM / Ego-LLM
> 将大语言模型与第一人称视觉结合，实现视频问答、内容描述、推理等高级认知能力，是当前最火热的方向。
>

#### 预训练基础模型
+ **Egocentric Video-Language Pretraining (EgoVLP)**
    - 发布：CVPR 2022
    - 亮点：首个专门针对egocentric场景的视频-语言预训练框架
    - 论文链接：[https://arxiv.org/abs/2206.01670](https://arxiv.org/abs/2206.01670)
+ **EgoVLPv2: Egocentric Video-Language Pre-training with Fusion in the Backbone**
    - 发布：ICCV 2023
    - 亮点：骨干网络内融合的改进版VLP
    - 论文链接：[https://arxiv.org/pdf/2307.05463](https://arxiv.org/pdf/2307.05463)

#### 高级推理与前沿进展
+ **EgoThinker: Unveiling Egocentric Reasoning with Spatio-Temporal CoT**
    - 发布：NeurIPS 2025
    - 亮点：将思维链引入egocentric视频理解，提出时空思维链框架
    - 论文链接：[https://arxiv.org/abs/2510.23569](https://arxiv.org/abs/2510.23569)
+ **CLiViS: Unleashing Cognitive Map through Linguistic-Visual Synergy for Embodied Visual Reasoning**
    - 发布：arXiv 2025
    - 亮点：语言-视觉协同构建认知地图，突破长视频推理瓶颈
    - 论文链接：[https://arxiv.org/abs/2506.17629](https://arxiv.org/abs/2506.17629)
+ **PhysBrain: Human Egocentric Data as a Bridge from Vision Language Models to Physical Intelligence**
    - 发布：arXiv 2025
    - 亮点：将人类第一人称视频转化为具身监督数据
    - 论文链接：[https://arxiv.org/abs/2512.16793](https://arxiv.org/abs/2512.16793)
+ **Vinci: A Real-time Smart Assistant based on Egocentric Vision-Language Model**
    - 发布：ACM 2025 (arXiv 2024)
    - 亮点：面向可穿戴设备的轻量级Ego-VLM，支持长视频记忆与动作生成，可在端侧实时运行
    - 论文链接：[https://arxiv.org/abs/2412.21080](https://arxiv.org/abs/2412.21080)
+ **EgoMotion: Hierarchical Reasoning and Diffusion for Egocentric Vision-Language Motion Generation**
    - 发布：arXiv 2026
    - 亮点：提出层级推理与扩散框架，从第一人称视频生成语言描述的3D人体运动
    - 论文链接：[https://arxiv.org/abs/2604.19105](https://arxiv.org/abs/2604.19105)
+ **The Right Inference Strategy Is All You Need: Nearly Training-Free Domain-Wise Inference for EgoCross Challenge**
    - 发布：arXiv 2026
    - 亮点：EgoCross挑战赛方案，领域感知推理策略在仅20个训练样本下达到66.98%准确率
    - 论文链接：[https://arxiv.org/abs/2606.00829](https://arxiv.org/abs/2606.00829)
+ **Decoding Pedestrian Crossing Intention from Egocentric Vision via Vision Language Models**
    - 发布：arXiv 2026
    - 亮点：首次用VLM解码行人过街意图，融合眼动和自运动后准确率达14.5%提升
    - 论文链接：[https://arxiv.org/abs/2606.09142](https://arxiv.org/abs/2606.09142)
+ **Allocentric Perceiver: Disentangling Allocentric Reasoning from Egocentric Visual Priors via Frame Instantiation**
    - 发布：arXiv 2026
    - 亮点：训练无关的离中心感知策略，从单张或多张图像恢复度量3D状态，在离中心任务上提升约10%
    - 论文链接：[https://arxiv.org/abs/2602.05789](https://arxiv.org/abs/2602.05789)
+ **EgoBabyVLM: Benchmarking Cross-Modal Learning from Naturalistic Egocentric Video Data**
    - 发布：arXiv 2026
    - 亮点：首个系统基准测试，发现当前VLM依赖紧密语义对齐，无法利用弱对齐的自然信号
    - 论文链接：[https://arxiv.org/abs/2605.19130](https://arxiv.org/abs/2605.19130)
+ **EgoTL: Egocentric Think-Aloud Chains for Long-Horizon Tasks**
    - 发布：arXiv 2026
    - 亮点：用"说在行动前"协议记录逐步目标和口头推理，覆盖100+日常家务任务
    - 论文链接：[https://arxiv.org/abs/2604.09535](https://arxiv.org/abs/2604.09535)
+ **Gaze-Regularized VLMs for Ego-Centric Behavior Understanding**
    - 发布：arXiv 2026
    - 亮点：将眼动信息融入VLM训练，通过注视正则化机制使模型关注注视高亮区域，语义得分提升近13%
    - 论文链接：[https://arxiv.org/abs/2603.23190](https://arxiv.org/abs/2603.23190)
+ **Towards Comprehensive Scene Understanding: Integrating First and Third-Person Views for LVLMs**
    - 发布：NeurIPS 2025
    - 亮点：提出E3VQA多视角问答基准（4K高质量问答对）和M3CoT提示技术，在GPT-4o上提升4.84%
    - 论文链接：[https://proceedings.neurips.cc/paper_files/paper/2025/hash/1af83ab66b4f07a3f55788e67dab5782-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/1af83ab66b4f07a3f55788e67dab5782-Abstract-Conference.html)
+ **Exo2Ego: Exocentric Knowledge Guided MLLM for Egocentric Video Understanding**
    - 发布：AAAI 2026
    - 亮点：构建Ego-ExoClip预训练数据集（110万同步自中心-外中心片段-文本对），提出三阶段渐进映射学习流水线
    - 论文链接：[https://ojs.aaai.org/index.php/AAAI/article/view/38244](https://ojs.aaai.org/index.php/AAAI/article/view/38244)
+ **Spatial Reasoning with Vision-Language Models in Ego-Centric Multi-View Scenes**
    - 发布：ICLR 2026
    - 亮点：提出Ego3D-Bench空间推理基准（8,600+QA对），及Ego3D-VLM后训练框架
    - 论文链接：[https://iclr.cc/virtual/2026/poster/10008200](https://iclr.cc/virtual/2026/poster/10008200)
+ **Personal Visual Context Learning in Large Multimodal Models**
    - 发布：arXiv 2026
    - 亮点：提出Personal VCL，基于EgoLife/Ego4D/CaptainCook4D构建基准，包含2,255个个人视觉查询
    - 论文链接：[https://vision.cs.utexas.edu/projects/PersonalVCL/](https://vision.cs.utexas.edu/projects/PersonalVCL/)
+ **EgoCoT-Bench: Benchmarking Grounded and Verifiable Operation-Centric Chain of Thought Reasoning for MLLMs**
    - 发布：arXiv 2026
    - 亮点：包含3,172个可验证QA对，通过时空场景图引导生成框架构建，涵盖12个子任务
    - 论文链接：[https://arxiv.org/abs/2605.19559](https://arxiv.org/abs/2605.19559)
+ **Benchmarking Egocentric Multimodal Goal Inference for Assistive Wearable Agents**
    - 发布：NeurIPS 2025数据集与基准赛道
    - 亮点：目标推断基准数据集，含363名参与者、3,482条记录，人类上限93%准确率，最佳VLM仅84%
    - 论文链接：[https://papers.nips.cc/paper_files/paper/2025/hash/23ab960082db936f874b171822e0d097-Abstract-Datasets_and_Benchmarks_Track.html](https://papers.nips.cc/paper_files/paper/2025/hash/23ab960082db936f874b171822e0d097-Abstract-Datasets_and_Benchmarks_Track.html)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| --- | --- | --- | --- | --- |
| HD-EPIC | 2025 | ~41 h / dense labels | 细粒度厨房、VQA | [官网](https://hd-epic.github.io/) |
| EgoClip | 2022 | 3.8M clip–text pairs | 视频-语言预训练 | [GitHub](https://github.com/showlab/EgoVLP) |
| EgoTL | 2026 | 100+ daily household tasks | 长时推理、空间问答 | [官网](https://ego-tl.github.io/) |
| MM-Conv | 2026 | 6.7 h / 4,211 expressions | 上下文3D对话指代 | [论文](https://arxiv.org/abs/2605.21796) |
| Minerva-Ego | 2026 | 1,160 QA / 156 videos | 时空推理轨迹 | [GitHub](https://github.com/google-deepmind/neptune) |
| EgoEverything | 2026 | 100+ h / 5K+ MCQs | 长上下文AR视频问答 | [论文](https://arxiv.org/abs/2604.08342) |
| EgoEsportsQA | 2026 | 1,745 QA pairs | 电竞视频问答、推理 | [论文](https://arxiv.org/abs/2604.12320) |
| MyEgo | 2026 | 541 long videos / 5K QA | 个性化视频问答 | [GitHub](https://github.com/Ryougetsu3606/MyEgo) |
| LifeDialBench / EgoMem | 2026 | 生活日志记忆 | 在线评估 | [GitHub](https://github.com/qys77714/LifeDialBench) |
| Ego2Web | 2026 | 500 video-instruction pairs | 自我视频接地网络智能体 | [HF](https://huggingface.co/datasets/Shoubin/Ego2Web) |
| NoRA | 2026 | 1,420 clips | 规范性动作推理 | [论文](https://arxiv.org/abs/2606.04806) |
| Causal-Plan-1M | 2026 | 1M QA / 22.2K clips | 物理接地规划问答 | [HF](https://huggingface.co/datasets/anonymous-causal-plan/Causal_Plan) |
| Pause-and-Think | 2026 | 10K QA clips + 300 benchmark | 辅助动作建议 | [GitHub](https://github.com/sssshivvvv/pause-and-think) |
| EgoCoT-Bench | 2026 | 351 videos / 3,172 QA | 接地操作思维链问答 | [官网](https://dstardust.github.io/EgoCoT/) |
| EgoEMS | 2025 | 20+ h emergency scenarios | 急救问答、多模态 | [GitHub](https://github.com/UVA-DSA/EgoEMS) |
| HowToDIV | 2025 | ~24 h instructional | 对话、程序性问答 | [GitHub](https://github.com/google/howtodiv) |
| InterVLA | 2025 | 11.4 h interactions | 指令、自我-外部动作捕捉 | [官网](https://liangxuy.github.io/InterVLA/) |
| AssistQ | 2022 | 100 long videos / 529 QA | 教学性问答 | [GitHub](https://github.com/showlab/AssistQ) |
| EgoTaskQA | 2022 | ~2K videos / 40K QA | 因果与任务问答 | [官网](https://sites.google.com/view/egotaskqa) |
| EgoVQA | 2019 | 600+ QAs | 视频问答 | [ICCVW 2019](https://openaccess.thecvf.com/content_ICCVW_2019/html/EPIC/Fan_EgoVQA_-_An_Egocentric_Video_Question_Answering_Benchmark_Dataset_ICCVW_2019_paper.html) |


---

### 2.4 长时序视频理解与问答 Long-form Video Understanding & QA
> 处理小时级甚至天级的超长第一人称视频，核心挑战是长时序依赖建模、记忆检索与信息摘要。
>

+ **EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding**
    - 发布：NeurIPS 2023
    - 亮点：超长egocentric视频理解的权威诊断基准
    - 论文链接：[https://arxiv.org/pdf/2308.09126](https://arxiv.org/pdf/2308.09126)
+ **OSGNet: Champion Solution for Ego4D Episodic Memory Challenge 2025**
    - 发布：CVPR 2025 挑战赛全赛道冠军
    - 亮点：提出早期融合的时序定位架构，包揽Ego4D情景记忆三项任务冠军
    - 论文链接：[https://arxiv.org/abs/2506.03710](https://arxiv.org/abs/2506.03710)
+ **EgoMemory: Memory-Augmented Personalized Retrieval for Long-Context Egocentric Video**
    - 发布：ACL 2026
    - 亮点：提出面向持续流式第一人称视频的终身记忆框架
    - 论文链接：[https://www.microsoft.com/en-us/research/publication/egomemory-memory-augmented-personalized-retrieval-for-long-context-egocentric-video/](https://www.microsoft.com/en-us/research/publication/egomemory-memory-augmented-personalized-retrieval-for-long-context-egocentric-video/)
+ **Unique Lives, Shared World: Learning from Single-Life Egocentric Videos**
    - 发布：arXiv 2025
    - 亮点：研究单一个体超长生命周期视频的学习问题
    - 论文链接：[https://arxiv.org/abs/2512.04085](https://arxiv.org/abs/2512.04085)
+ **MyEgo: Ego-Grounding for Personalized Question-Answering in Egocentric Videos**
    - 发布：CVPR 2026
    - 亮点：大规模个性化第一人称视频数据集
    - 论文链接：[https://arxiv.org/pdf/2604.01966](https://arxiv.org/pdf/2604.01966)
+ **EGAgent: Agentic Very Long Video Understanding**
    - 发布：arXiv 2026
    - 亮点：基于实体场景图的智能体推理框架，可处理跨天级别的连续视频流，支持结构化多跳推理、音视频混合检索
    - 论文链接：[https://arxiv.org/abs/2601.18157](https://arxiv.org/abs/2601.18157)
+ **EgoMemReason: A Memory-Driven Reasoning Benchmark for Long-Horizon Egocentric Video Understanding**
    - 发布：arXiv 2026
    - 亮点：评估周级自中心视频记忆驱动推理的基准，含500个问题，最佳模型仅39.6%准确率
    - 论文链接：[https://arxiv.org/abs/2605.09874](https://arxiv.org/abs/2605.09874)
+ **Semantic and Visual Evidence for Efficient Long-Video Reasoning: A Solution for the HD-EPIC VQA Challenge**
    - 发布：arXiv 2026
    - 亮点：将长视频推理解耦为语义证据和视觉证据，通过查询条件检索集成实现高效长视频理解
    - 论文链接：[https://arxiv.org/abs/2605.29402](https://arxiv.org/abs/2605.29402)
+ **Bridging Modalities, Spanning Time: Structured Memory for Ultra-Long Agentic Video Reasoning**
    - 发布：arXiv 2026
    - 亮点：提出MAGIC-Video训练无关框架，基于多模态记忆图与交错叙事链，在EgoLifeQA上超越此前最佳智能体系统10.1点
    - 论文链接：[https://arxiv.org/abs/2605.08271](https://arxiv.org/abs/2605.08271)
+ **MA-EgoQA: Question Answering over Egocentric Videos from Multiple Embodied Agents**
    - 发布：arXiv 2026
    - 亮点：首个多智能体自中心视频理解问题定义，提供1.7k个横跨五类场景的问题
    - 论文链接：[https://arxiv.org/abs/2603.09827](https://arxiv.org/abs/2603.09827)
+ **Spatial-Conditioned Reasoning in Long-Egocentric Videos**
    - 发布：arXiv 2026
    - 亮点：研究显式空间信号对VLM长视频理解的影响，引入Sanpo-D细粒度重标注数据集
    - 论文链接：[https://arxiv.org/abs/2601.18100](https://arxiv.org/abs/2601.18100)
+ **FocusGraph: Graph-Structured Frame Selection for Embodied Long Video Question Answering**
    - 发布：arXiv 2026
    - 亮点：基于图的帧选择框架，使用Scene-Caption LLM Selector选择查询相关片段
    - 论文链接：[https://arxiv.org/abs/2603.04349](https://arxiv.org/abs/2603.04349)
+ **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - 发布：ICLR 2026
    - 亮点：通过世界建模评估具身认知的基准，实验揭示VLM求解逆问题优于正向问题
    - 论文链接：[https://iclr.cc/virtual/2026/10013240](https://iclr.cc/virtual/2026/10013240)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| --- | --- | --- | --- | --- |
| EgoLife | 2025 | ~266–300 h daily life | 长时助手、记忆 | [官网](https://egolife-ai.github.io/) |
| EgoSchema | 2023 | 250+ h / 5K QA | 长时视频问答 | [官网](https://egoschema.github.io/) |
| SuperMemory-VQA | 2026 | 52.9 h / 4,853 QA | 长时记忆视频问答 | [HF](https://huggingface.co/datasets/OSU-AIoT-MLSys-Lab/SuperMemory-VQA) |
| EgoMemReason | 2026 | 500 MCQs over EgoLife | 周级记忆推理 | [HF](https://huggingface.co/datasets/Ted412/EgoMemReason) |
| EgoExoMem | 2026 | 2.6K MCQs / 390 videos | 跨视角记忆推理 | [GitHub](https://github.com/RuipingL/EgoExoMem) |
| EgoIntrospect | 2026 | 180 h / 60 subjects | 内部状态推理、记忆 | [官网](https://ego-introspect.github.io/) |
| MA-EgoQA | 2026 | 1,741 QA / 6 agents / 7 days | 多智能体自我问答 | [官网](https://ma-egoqa.github.io/) |
| EgoStream | 2026 | 2,250 Q / 8,528 evals | 流式情景记忆 | [官网](https://saroo25.github.io/Egostream/) |
| VidChapters-7M | 2023 | 817K videos / 7M chapters | 视频章节化 | [官网](https://antoyang.github.io/vidchapters.html) |
| Multi-Ego | 2022 | ~12 h / 41 seq. | 多佩戴者、摘要 | [GitHub](https://github.com/M-Elfeki/Multi-DPP) |
| DoMSEV | 2018 | 80 h, 48 seq. | 语义快进 | [官网](https://www.verlab.dcc.ufmg.br/semantic-hyperlapse/cvpr2018-dataset/) |
| HUJI-EgoSeg | 2014 | 29 long videos | 时间分割 | [官网](http://www.cs.huji.ac.il/~yedMDpid/egoseg/) |
| UT Ego | 2012 | ~17 h, 4 long videos | 摘要、长时自我 | [官网](http://vision.cs.utexas.edu/projects/egocentric_data/UT_Egocentric_Dataset.html) |
| VINST / Visual Diaries | 2011 | 31 videos | 时间分割、摘要 | [官网](https://www.csc.kth.se/cvap/vinst/NovEgoMotion.html) |


---

### 2.5 视线、注意力与意图预测 Gaze, Attention & Intention Prediction
> 预测第一人称视角下用户的注视点、注意力分布与潜在意图，是智能交互、辅助系统的核心技术。
>

+ **Ego-PMOVE: Prompt-aware Mixture of View Experts Network for Egocentric Gaze Prediction**
    - 发布：AAAI 2026
    - 亮点：首个探索跨视角注视关系的方法，提出提示感知的多视角专家混合网络
    - 论文链接：[https://ojs.aaai.org/index.php/AAAI/article/view/37808](https://ojs.aaai.org/index.php/AAAI/article/view/37808)
+ **Gaze Beyond the Frame: Forecasting Egocentric 3D Visual Span**
    - 发布：NeurIPS 2025
    - 亮点：提出3D视觉跨度预测新任务，EgoSpanLift方法将2D注视预测提升到3D场景
    - 论文链接：[https://proceedings.neurips.cc/paper_files/paper/2025/hash/bf649dbcf4eaaba4fc68ccaee25a7f9e-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/bf649dbcf4eaaba4fc68ccaee25a7f9e-Abstract-Conference.html)
+ **Gaze-Regularized VLMs for Ego-Centric Behavior Understanding**
    - 发布：arXiv 2026
    - 亮点：将眼动信息融入VLM训练，通过注视正则化机制使模型关注注视高亮区域，语义得分提升近13%
    - 论文链接：[https://arxiv.org/abs/2603.23190](https://arxiv.org/abs/2603.23190)
+ **Learning from Human Gaze: Human-like Robot Social Navigation in Dense Crowds**
    - 发布：AAAI 2026
    - 亮点：引入GazeNav数据集（佩戴式眼动追踪仪同步视频、注视和轨迹）
    - 论文链接：[https://ojs.aaai.org/index.php/AAAI/article/view/38941](https://ojs.aaai.org/index.php/AAAI/article/view/38941)
+ **In the Eye of MLLM: Benchmarking Egocentric Video Intent Understanding with Gaze-Guided Prompting**
    - 发布：NeurIPS 2025数据集与基准赛道
    - 亮点：提出EgoGazeVQA基准，系统评估MLLM利用眼动信息理解用户意图的能力
    - 论文链接：[https://proceedings.neurips.cc/paper_files/paper/2025/hash/9df42a5f6d1397e46e2cdca80a1a7903-Abstract-Datasets_and_Benchmarks_Track.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/9df42a5f6d1397e46e2cdca80a1a7903-Abstract-Datasets_and_Benchmarks_Track.html)
+ **egoEMOTION: Egocentric Vision and Physiological Signals for Emotion and Personality Recognition in Real-World Tasks**
    - 发布：NeurIPS 2025
    - 亮点：基于Meta Project Aria科研眼镜的情绪与人格识别数据集
    - 论文链接：[https://arxiv.org/pdf/2510.22129](https://arxiv.org/pdf/2510.22129)

---

### 2.6 3D/4D重建与空间感知 3D/4D Reconstruction & Spatial Perception
> 从第一人称单目视频中恢复3D人体姿态、网格、场景深度与4D动态结构，是AR/VR、机器人的核心感知能力。
>

#### 人体姿态与网格重建
+ **AG-EgoPose: Leveraging Action-Guided Motion and Kinematic Joint Encoding for Egocentric 3D Pose Estimation**
    - 发布：arXiv 2026
    - 亮点：动作引导的运动建模+运动学关节编码框架
    - 论文链接：[https://arxiv.org/pdf/2603.25175](https://arxiv.org/pdf/2603.25175)
+ **Fish2Mesh Transformer: 3D Human Mesh Recovery from Egocentric Vision**
    - 发布：arXiv 2025
    - 亮点：首个针对头戴鱼眼相机的人体网格恢复方法
    - 论文链接：[https://arxiv.org/pdf/2503.06089](https://arxiv.org/pdf/2503.06089)

#### 事件相机与极端场景
+ **D-EventEgo: Event-Based Egocentric Human Pose Estimation in Dynamic Environments**
    - 发布：arXiv 2025
    - 亮点：首次研究基于事件相机的egocentric人体姿态估计
    - 论文链接：[https://arxiv.org/pdf/2505.22007](https://arxiv.org/pdf/2505.22007)

#### 场景重建与SLAM
+ **EventEgo3D: 3D Human Motion Capture from Egocentric Event Streams**
    - 发布：CVPR 2024
    - 亮点：基于事件流的高速3D人体动作捕捉方案
    - 论文链接：[https://arxiv.org/pdf/2404.08640](https://arxiv.org/pdf/2404.08640)
+ **EventEgo3D++: 3D Human Motion Capture from a Head-Mounted Event Camera**
    - 发布：arXiv 2025
    - 亮点：首个基于头戴鱼眼事件相机的3D人体动作捕捉方案
    - 论文链接：[https://arxiv.org/pdf/2502.07869](https://arxiv.org/pdf/2502.07869)
+ **Bringing a Personal Point of View: Evaluating Dynamic 3D Gaussian Splatting for Egocentric Scene Reconstruction**
    - 发布：EgoVis@CVPR 2026
    - 亮点：首次系统评估动态3DGS在自中心和外中心视频上的表现，发现自中心视图重建质量系统性地较低
    - 论文链接：[https://arxiv.org/abs/2604.23803](https://arxiv.org/abs/2604.23803)
+ **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - 发布：SIGGRAPH 2026
    - 亮点：可微前臂表示和统一臂-手Transformer架构，跨鱼眼、透视和畸变广角相机模型统一网络，在HOT3D上MPJPE降低28%
    - 论文链接：[https://arxiv.org/abs/2605.12498](https://arxiv.org/abs/2605.12498)
+ **FunRec: Reconstructing Functional 3D Scenes from Egocentric Interaction Videos**
    - 发布：CVPR 2026
    - 亮点：从野外RGB-D交互视频重建可交互3D场景数字孪生，自动发现关节部件并估计运动学参数
    - 论文链接：[https://arxiv.org/abs/2604.05621](https://arxiv.org/abs/2604.05621)
+ **OmniEgoCap: Camera-Agnostic Sequence-Level Egocentric Motion Reconstruction**
    - 发布：arXiv 2026
    - 亮点：扩散框架将自中心重建扩展到多种采集设备，引入几何感知可见性增强策略
    - 论文链接：[https://arxiv.org/abs/2512.19283](https://arxiv.org/abs/2512.19283)
+ **Towards Learning a Generalizable 3D Scene Representation from 2D Observations**
    - 发布：ESANN 2026
    - 亮点：从机器人自中心观测预测3D工作空间占据率的广义NeRF方法，在40个真实场景上训练达26mm重建误差
    - 论文链接：[https://arxiv.org/abs/2602.10943](https://arxiv.org/abs/2602.10943)
+ **Ego-1K: A Large-Scale Multiview Video Dataset for Egocentric Vision**
    - 发布：CVPR 2026
    - 亮点：近1,000个自中心多视角短视频，12台同步相机围绕4摄像机VR头戴式设备
    - 论文链接：[https://arxiv.org/abs/2603.13741](https://arxiv.org/abs/2603.13741)

#### 📊 相关数据集与基准
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| --- | --- | --- | --- | --- |
| ⭐ Ego-Exo4D | 2024 | 1,286+ h ego+exo | 技能活动、多任务 | [官网](https://ego-exo4d-data.org/) |
| ⭐ ADT (Aria Digital Twin) | 2023 | 200 seq., 2 scenes | 自我3D感知 | [官网](https://www.projectaria.com/datasets/adt/) |
| PRISM | 2026 | 270K samples / 11.8M frames | 零售具身VLM、空间推理 | [HF](https://huggingface.co/datasets/DreamVu/PRISM-100K) |
| EgoTraj | 2026 | 10.7 h / 1.15M frames | 自我轨迹预测 | [GitHub](https://github.com/yehiahmad/EgoTraj) |
| AIST-Living | 2026 | 自我视频+3D场景GT | 全局姿态、定位 | [官网](https://deguchihiroyuki.github.io/Map-Mono-Ego-Project/) |
| OVO-S-Bench | 2026 | 348 videos / 1,680 Q | 流式空间智能问答 | [官网](https://internlm.github.io/OVO-S-Bench/) |
| PVSG | 2023 | 400 vids, ~150K frames | 全景视频场景图 | [官网](https://jingkang50.github.io/PVSG/) |
| DR(eye)VE | 2018 | ~6 h driving, 555K frames | 注视预测、驾驶自我 | [官网](http://aimagelab.ing.unimore.it/dreyeve) |
| EgoCart | 2018 | 零售RGB-D, 9 videos | 室内/购物车定位 | [官网](https://iplab.dmi.unict.it/EgocentricShoppingCartLocalization/) |
| IU ShareView | 2018 | 9 paired ego video sets | 跨佩戴者分割/ID | [官网](http://vision.soic.indiana.edu/firstthird-eccv2018/) |
| OST | 2017 | 57 sequences | 物体搜索、眼动 | [GitHub](https://github.com/Mengmi/deepfuturegaze_gan) |


---

### 2.7 视觉-语言-动作与具身智能 Ego-VLA & Embodied AI
> 基于人类第一人称视频学习视觉-语言-动作对齐，将人类行为知识迁移到机器人，是具身智能的核心技术路径。
>

+ **EgoBridge: Domain Adaptation for Generalizable Imitation from Egocentric Human Videos**
    - 发布：NeurIPS 2025
    - 亮点：基于最优传输对齐视觉特征-动作联合分布，成功率比基线提升44%
    - 论文链接：[https://arxiv.org/pdf/2509.19626](https://arxiv.org/pdf/2509.19626)
+ **EgoAgent: A Joint Predictive Agent Model in Egocentric Worlds**
    - 发布：ICCV 2025
    - 亮点：单个统一Transformer架构融合视觉、语言、世界模型与动作决策
    - 论文链接：[https://arxiv.org/abs/2502.05857](https://arxiv.org/abs/2502.05857)
+ **Ego-Pi: VLA Fine-Tuning for Egocentric Human and Robot Data**
    - 发布：arXiv 2026
    - 亮点：面向双臂灵巧操作的VLA微调方案
    - 论文链接：[https://arxiv.org/pdf/2606.08107](https://arxiv.org/pdf/2606.08107)
+ **ViterbiPlanNet: Injecting Procedural Knowledge via Differentiable Viterbi for Egocentric Task Planning**
    - 发布：CVPR 2026
    - 亮点：通过可微维特比算法将步骤式先验知识注入VLA
    - 论文链接：[https://arxiv.org/abs/2603.04265](https://arxiv.org/abs/2603.04265)
+ **Co-training with Ego-centric Video and Demonstration for Robot Navigation Task**
    - 发布：arXiv 2026
    - 亮点：将第一人称行走视频转换为移动机器人模仿学习数据集
    - 论文链接：[https://arxiv.org/abs/2606.01951](https://arxiv.org/abs/2606.01951)
+ **OSCAR: Omni-Embodiment Skeleton-Conditioned World Action Model for Robotics**
    - 发布：arXiv 2026
    - 亮点：全具身骨架条件世界动作模型，支持从第一人称视频学习多种机器人的动作策略
    - 论文链接：[https://arxiv.org/abs/2606.04463](https://arxiv.org/abs/2606.04463)

#### 📊 相关数据集与基准（程序性活动与技能学习）
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| --- | --- | --- | --- | --- |
| ⭐ EgoExoLearn | 2024 | 120 h ego+exo | 程序性、异步视角 | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |
| ⭐ Assembly101 | 2022 | 513 h multiview | 组装、程序 | [官网](https://assembly-101.github.io/) |
| EgoVerse | 2026 | 1,362 h / ~80K episodes | 机器人学习、操作技能 | [官网](https://egoverse.ai/) |
| EgoLive | 2026 | 大规模真实任务例程 | 机器人操作学习 | [论文](https://arxiv.org/abs/2604.23570) |
| EgoMAGIC | 2026 | 3,355 videos / 50 medical tasks | 现场医疗动作检测 | [Zenodo](https://doi.org/10.5281/zenodo.19239154) |
| HumanEgo | 2026 | 分钟级Aria演示 | 人-机器人策略学习 | [官网](https://humanego-ai.github.io/) |
| EgoSPT | 2026 | 11,515 episodes / 112 task folders | 空间提示操作轨迹 | [HF](https://huggingface.co/datasets/JackYFL233/EgoSPT) |
| Ego-EXTRA | 2026 | 50 h / 15K+ VQA | 专家-学员协助 | [官网](https://fpv-iplab.github.io/Ego-EXTRA/) |
| GM-100 | 2026 | 100+ tasks / 13K+ trajectories | 机器人操作评估 | [官网](https://www.rhos.ai/research/gm-100) |
| SABER | 2026 | 100+ h / 44.8K samples | 零售VLA适应 | [官网](https://dreamvu.ai/saber/) |
| EgoProactive / Pro²Bench | 2026 | 700 recordings / 42K eval | 主动程序性协助 | [HF](https://huggingface.co/datasets/facebook/wearable-ai) |
| EgoYC2 / Exo2EgoDVC | 2025 | ~43 h cooking | 密集字幕、程序性 | [GitHub](https://github.com/ut-vision/Exo2EgoDVC) |
| IndustReal | 2024 | ~6 h industrial | 程序步骤、错误 | [官网](https://timschoonbeek.github.io/industreal.html) |
| EgoProceL | 2022 | 62 videos / 16 tasks | 程序学习 | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| EPIC-Tent | 2019 | 7+ h, tent assembly | 程序性、双HMD+注视 | [官网](https://data.bris.ac.uk/data/dataset/2ite3tu1u53n42hjfh3886sa86) |
| CMU-MMAC | 2011 | 25 subjects, 5 recipes | 程序性活动 | [官网](http://kitchen.cs.cmu.edu/) |
| GTEA Gaze | 2011 | 17 sessions | 程序性活动、注视 | [官网](https://cbs.ic.gatech.edu/fpv/) |


---

### 2.8 第一人称世界模型 Egocentric World Models
> 学习第一人称视角下环境的演化规律，可预测未来状态、生成交互场景，是长时序规划、数据增强的核心基础。
>

+ **AnchorWorld: Embodied Egocentric World Simulation with View-based Evolution Customization**
    - 发布：arXiv 2026
    - 亮点：支持关键帧作为锚点约束的可控世界模拟，锚点准确率达89%
    - 论文链接：[https://arxiv.org/abs/2606.07326](https://arxiv.org/abs/2606.07326)
+ **WEM: World-Ego Modeling for Long-Horizon Evolution in Hybrid Embodied Tasks**
    - 发布：arXiv 2026
    - 亮点：世界-自我解耦建模架构，将隐状态分为静态场景分支与动态自我分支
    - 论文链接：[https://arxiv.org/abs/2605.19957](https://arxiv.org/abs/2605.19957)
+ **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - 发布：ICLR 2026
    - 亮点：首个从世界建模角度评测具身认知能力的基准
    - 论文链接：[https://openreview.net/forum?id=Patx6MRipw](https://openreview.net/forum?id=Patx6MRipw)
+ **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - 发布：arXiv 2026
    - 亮点：首个egocentric HOI世界模型，无需未来状态的物理先验生成
    - 论文链接：[https://arxiv.org/abs/2603.13615](https://arxiv.org/abs/2603.13615)
+ **Walk through Paintings: Egocentric World Models from Internet Priors**
    - 发布：arXiv 2026
    - 亮点：EgoWM利用互联网视频先验，将预训练视频扩散模型转化为动作条件世界模型
    - 论文链接：[https://arxiv.org/abs/2601.15284](https://arxiv.org/abs/2601.15284)
+ **<font style="color:rgb(40, 121, 22) !important;background-color:rgb(238, 255, 232) !important;">EgoExo</font>****<font style="color:rgb(45, 45, 45);">-</font>****<font style="color:rgb(40, 121, 22) !important;background-color:rgb(238, 255, 232) !important;">WM</font>****<font style="color:rgb(45, 45, 45);">: Unlocking Exo Video for Ego World Models</font>**
    - 发布：arXiv 2026
    - 亮点：利用第三视角数据补充第一视角数据
    - 论文链接：[https://arxiv.org/pdf/2605.15477](https://arxiv.org/pdf/2605.15477)
+ **PlayerOne: Egocentric World Simulator**
    - 发布：NeurIPS 2025
    - 亮点：首个自中心真实感世界模拟器，支持沉浸式和无限制探索
    - 论文链接：[https://arxiv.org/abs/2506.09995](https://arxiv.org/abs/2506.09995)
+ **EgoSim: Egocentric World Simulator for Embodied Interaction Generation**
    - 发布：arXiv 2026
    - 亮点：闭环自中心世界模拟器，生成空间一致交互视频并持续更新3D场景状态
    - 论文链接：[https://arxiv.org/abs/2604.01001](https://arxiv.org/abs/2604.01001)
+ **EgoForge: Goal-Directed Egocentric World Simulator**
    - 发布：arXiv 2026
    - 亮点：目标导向的自中心世界模拟器，支持生成符合特定目标约束的未来帧序列
    - 论文链接：[https://arxiv.org/abs/2603.20169](https://arxiv.org/abs/2603.20169)
+ **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - 发布：NeurIPS 2025
    - 亮点：可推广到新物体的多模态HOI世界模型，VLM推断运动先验，DiT流匹配生成轨迹
    - 论文链接：[https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)

#### 📊 相关数据集与基准（视频生成与世界模型预训练）
| 数据集名称 | 年份 | 规模 | 核心任务 | 链接 |
| --- | --- | --- | --- | --- |
| ⭐ Ropedia Xperience-10M | 2026 | 10M multimodal experiences | 多模态自我预训练 | [HF](https://huggingface.co/datasets/ropedia-ai/xperience-10m) |
| DreamDojo-HV | 2026 | 非常大FP视频 | 世界模型、预训练 | [论文](https://arxiv.org/abs/2602.06949) |
| Ego-1K | 2026 | 多视角片段 | 神经3D/4D合成 | [HF](https://huggingface.co/datasets/facebook/ego-1k) |
| In-lab | 2026 | 实验室桌面轨迹 | 技能、世界模型 | [论文](https://arxiv.org/abs/2602.06949) |
| HumanNet | 2026 | ~1M h human-centric video | VLA/具身预训练 | [论文](https://arxiv.org/abs/2605.06747) |
| MobileEgo Anywhere | 2026 | 200 h smartphone ego | 长时自我数据、VLA | [论文](https://arxiv.org/abs/2605.05945) |
| EgoEdit | 2025 | 100K editing pairs | 自我视频编辑 | [官网](https://snap-research.github.io/EgoEdit) |
| EgoVid-5M | 2024 | 5M clips | 视频生成 | [官网](https://egovid.github.io/) |


---

## 📊 数据集、基准与模拟器 Datasets, Benchmarks & Simulators
### 通用大规模数据集
| 数据集名称 | 发布年份 | 数据规模 | 核心任务 | 官方链接 |
| --- | --- | --- | --- | --- |
| Ego4D | 2022 | 3670小时视频，931名佩戴者，74个采集地点 | 动作识别、情景记忆、社交理解、3D姿态 | [官网](https://ego4d-data.org/) |
| EPIC-KITCHENS-100 | 2020 | 100小时视频，9万个动作片段，45个厨房场景 | 动作识别、动作检测、动作预判 | [官网](https://epic-kitchens.github.io/) |
| Ego-Exo4D | 2024 | 1286小时同步主视角+外视角多模态数据 | 跨视角学习、技能分析、3D重建 | [官网](https://ego-exo4d-data.org/) |
| HD-EPIC | 2025 | 4K高分辨率第一人称厨房数据集 | 细粒度动作理解、高分辨率视觉任务 | [论文](https://arxiv.org/pdf/2502.04144) |


### 细粒度任务数据集
#### EPIC-KITCHENS-100物体与交互类
+ **EgoObjects**：Meta AI发布的大规模第一人称物体检测数据集，1.4万视频，200万帧，900+物体类别，支持实例级跟踪
    - 链接：[https://github.com/facebookresearch/EgoObjects](https://github.com/facebookresearch/EgoObjects)
+ **EgoXtreme**：CVPR 2026发布的极端场景egocentric 6D物体位姿数据集，包含运动模糊、遮挡、光照剧变等挑战场景
    - 链接：[https://arxiv.org/pdf/2603.25135](https://arxiv.org/pdf/2603.25135)
+ **EgoPressure**：配套触觉信号的手物交互数据集，5小时视频，同步压力分布、IMU、手部姿态多模态数据
    - 链接：[https://arxiv.org/pdf/2409.02224](https://arxiv.org/pdf/2409.02224)
+ **TouchMoment**：CVPR 2026发布的细粒度接触时刻检测数据集，标注15万帧的接触开始、结束时刻与接触类型
    - 链接：[https://arxiv.org/pdf/2604.12343](https://arxiv.org/pdf/2604.12343)

#### 长视频与记忆类
+ **EgoSchema**：NeurIPS 2023长视频问答诊断基准，500+多步推理选择题，平均视频时长3分钟
    - 链接：[https://github.com/egoschema/EgoSchema](https://github.com/egoschema/EgoSchema)
+ **EgoLife**：CVPR 2025连续7天共同居住生活数据集，6名参与者，密集标注身份、事件、日常活动
    - 链接：[https://arxiv.org/pdf/2503.03803](https://arxiv.org/pdf/2503.03803)

#### 特殊场景类
+ **EgoExOR**：NeurIPS 2025手术室第一人称数据集，智能眼镜采集，同步手术器械、动作、生理信号标注
    - 链接：[https://arxiv.org/pdf/2505.24287](https://arxiv.org/pdf/2505.24287)
+ **MECCANO**：工业装配场景第一人称数据集，12小时视频，61类动作，24类物体，配套眼动数据
    - 链接：[https://github.com/fpv-iplab/MECCANO](https://github.com/fpv-iplab/MECCANO)
+ **EgoDex**：灵巧操作第一人称数据集，Apple Vision Pro采集，包含30类日常物体操作，配套6D手部姿态
    - 链接：[https://arxiv.org/abs/2505.11709](https://arxiv.org/abs/2505.11709)

### 具身智能与VLA基准
+ **EgoVerse**：通用egocentric具身智能评测基准，覆盖1000+任务，包含导航、操作、问答三大类
    - 链接：[https://arxiv.org/pdf/2604.07607](https://arxiv.org/pdf/2604.07607)
+ **EgoBench**：交互式具身智能评测基准，支持智能体与环境实时交互，评估闭环决策能力
    - 链接：[https://arxiv.org/pdf/2605.27820](https://arxiv.org/pdf/2605.27820)

### 模拟器
+ **PlayerOne**：首个照片级真实感egocentric世界模拟器，支持无限合成数据生成，精确控制人体运动与视角
    - 链接：[https://arxiv.org/abs/2506.09995](https://arxiv.org/abs/2506.09995)
+ **EgoSim**：闭环egocentric交互模拟器，支持3D场景状态持久化更新，可生成连续交互视频
    - 链接：[https://arxiv.org/pdf/2604.01001](https://arxiv.org/pdf/2604.01001)

---

## 👓 智能眼镜专属研究与落地 Smart Glasses Exclusive Research
### 专属基准与数据集
+ **SUPERGLASSES: Benchmarking Vision Language Models as Intelligent Agents for AI Smart Glasses**
    - 发布：CVPR 2026
    - 亮点：首个真实消费级眼镜采集的多场景VLM智能体基准，覆盖Ray-Ban Meta、小米智能眼镜、雷鸟V3三款设备
    - 论文链接：[https://arxiv.org/pdf/2602.22683](https://arxiv.org/pdf/2602.22683)
+ **Project Aria Datasets**：Meta发布的科研级智能眼镜数据集，包含眼动、IMU、深度、音频多模态同步数据
    - 链接：[https://www.projectaria.com/](https://www.projectaria.com/)

### 关键技术方向
#### 低功耗感知
+ **EgoTrigger: Toward Audio-Driven Image Capture for Human Memory Enhancement in All-Day Energy-Efficient Smart Glasses**
    - 单位：北卡罗来纳大学教堂山分校 + Google
    - 发布：IEEE TVCG 2025
    - 亮点：音频事件驱动的自适应拍照方案，功耗降低87%
    - 论文链接：[https://arxiv.org/pdf/2508.01915](https://arxiv.org/pdf/2508.01915)
+ **OpenGlass: Ultra-Low-Power On-Device AI Eyewear with Event-based Vision**
    - 发布：arXiv 2026
    - 亮点：完全开源的事件相机智能眼镜硬件方案，配套端侧算法栈
    - 论文链接：[https://arxiv.org/pdf/2606.07431](https://arxiv.org/pdf/2606.07431)

#### 记忆与辅助系统
+ **EGAgent: Agentic Very Long Video Understanding**
    - 发布：arXiv 2026
    - 亮点：基于实体场景图的智能体推理框架，可处理跨天级别的连续视频流
    - 论文链接：[https://arxiv.org/abs/2601.18157](https://arxiv.org/abs/2601.18157)

#### 自然交互
+ **Egocentric Co-Pilot: Web-Native Lightweight Smart Glasses Assistant**
    - 发布：WWW 2026
    - 亮点：基于Web技术的轻量级眼镜副驾架构，无需安装APP
    - 论文链接：[https://arxiv.org/pdf/2603.01104](https://arxiv.org/pdf/2603.01104)
+ **Plug-and-Play Clarifier: A Zero-Shot Multimodal Framework for Egocentric Intent Disambiguation**
    - 发布：AAAI 2026
    - 亮点：零样本意图消歧框架，指令执行准确率从58%提升到87%
    - 论文链接：[https://arxiv.org/pdf/2511.08971](https://arxiv.org/pdf/2511.08971)
+ **VisionClaw: Always-On AI Agents Through Smart Glasses**
    - 发布：arXiv 2026
    - 亮点：常在线AI代理系统，支持免触屏操作多类场景任务
    - 论文链接：[https://arxiv.org/pdf/2604.03486](https://arxiv.org/pdf/2604.03486)

---

## 🔗 相关资源列表 Related Awesome Lists
+ [Awesome-Egocentric](https://github.com/EgoAlpha/Awesome-Egocentric)
+ [awesome-egocentric-vision](https://github.com/Sid2697/awesome-egocentric-vision)
+ [Awesome-Egocentric-and-Exocentric-Vision](https://github.com/ayiyayi/Awesome-Egocentric-and-Exocentric-Vision)
+ [Awesome-Egocentric-Video-Datasets](https://github.com/player0718/awesome-ego-video-datasets)
---

## 🎯 核心研究挑战 Key Research Challenges
### 底层共性挑战
1. **第一人称固有缺陷**：视野有限、自遮挡严重、运动剧烈、成像质量不稳定，是所有任务都面临的基础难题
2. **数据规模瓶颈**：相比互联网海量第三人称数据，第一人称数据采集成本高、隐私敏感，规模差距达两个数量级，严重制约大模型训练效果
3. **个体差异巨大**：不同用户身高、行为习惯、居住环境差异极大，通用模型在个性化场景下泛化能力差
4. **长时序建模困难**：真实穿戴场景是连续数小时甚至数天的流式数据，现有模型难以处理超长时序依赖与记忆管理

### 各方向专属挑战
| 研究方向 | 核心挑战 |
| --- | --- |
| 动作理解 | 细粒度动作区分难、动词-名词组合爆炸、长视频时序定位精度低 |
| 手物交互 | 接触状态标注成本高、物理真实性难以保证、遮挡严重 |
| Ego-VLM | 第一人称常识缺失、时空推理能力弱、指代消歧困难 |
| 长视频理解 | 记忆容量有限、时序定位模糊、因果推理能力不足 |
| 视线与意图 | 个体眼动习惯差异大、隐式意图难以标注、多模态对齐难 |
| 3D重建 | 单目深度歧义性大、动态场景重建难、鱼眼畸变校正复杂 |
| Ego-VLA | 人-机器人域差距大、动作空间对齐难、物理交互常识缺失 |
| 世界模型 | 长时序一致性差、物理合理性不足、可控性与生成质量矛盾 |


## ❤️ Contact
If you have suggestions, or find this project useful, feel free to contact Yuanliang Sun at sun254667307@gmail.com.

## License
CC0 1.0 Universal. See LICENSE.



