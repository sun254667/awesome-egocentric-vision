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

> A curated, learning-friendly list of egocentric (first-person) vision & embodied AI resources: papers, datasets, code, models, toolkits, challenges and tutorials, covering both classic foundational works and cutting-edge advances, catering to research initiation and industrial落地.
>

✅ **Inclusion Criteria**

+ Prioritize high-quality works from top conferences and journals such as CVPR / ICCV / ECCV / NeurIPS / ICLR / AAAI / TPAMI / TVCG
+ Cover core cutting-edge directions: Ego-VLM/LLM, Ego-VLA Embodied Intelligence, 3D/4D Reconstruction, Hand-Object Interaction, Gaze Estimation, Long Video Understanding, World Models

---

## 📑 Table of Contents
1. [📚 Surveys & Overviews](#-surveys--overviews)
2. [🔬 Core Research Topics](#-core-research-topics)
    - 2.1 Action Recognition, Detection & Anticipation
    - 2.2 Hand-Object Interaction & Fine-grained Activity
    - 2.3 Egocentric Vision-Language Models (Ego-VLM / Ego-LLM)
    - 2.4 Long-form Video Understanding & QA
    - 2.5 Gaze, Attention & Intention Prediction
    - 2.6 3D/4D Reconstruction & Spatial Perception
    - 2.7 Vision-Language-Action & Embodied AI (Ego-VLA)
    - 2.8 Egocentric World Models
3. [📊 Datasets, Benchmarks & Simulators](#-datasets-benchmarks--simulators)
4. [👓 Smart Glasses Exclusive Research & Deployment](#-smart-glasses-exclusive-research--deployment)
5. [🔗 Related Awesome Lists](#-related-awesome-lists)
6. [🎯 Key Research Challenges](#-key-research-challenges)

---

## 📚 Surveys & Overviews
> The preferred materials for getting started in the field, helping to quickly establish a global understanding, sort out the development context, core tasks and key challenges.
>

+ **Challenges and Trends in Egocentric Vision: A Survey**
    - Publication: arXiv 2025
    - Highlights: The latest panoramic survey of the field, systematically classifying four major task directions: subject understanding, object understanding, environment understanding, and hybrid understanding, comprehensively summarizing challenges and trends
    - Paper Link: [https://arxiv.org/abs/2503.15275](https://arxiv.org/abs/2503.15275)
+ **Building Egocentric Procedural AI Assistant: Methods, Benchmarks, and Challenges**
    - Publication: arXiv 2025
    - Highlights: For the first time, systematically proposes a complete technical framework for first-person procedural AI assistants, defining three core tasks: error detection, procedural learning, and visual question answering, as well as two supporting dimensions: real-time stream processing and active interaction
    - Paper Link: [https://arxiv.org/pdf/2511.13261](https://arxiv.org/pdf/2511.13261)
+ **An Outlook into the Future of Egocentric Vision**
    - Publication: arXiv 2023
    - Highlights: Co-authored by authoritative scholars in the field, combining future scenarios of wearable computing, sorting out research shortcomings and directions to be broken through
    - Paper Link: [https://arxiv.org/abs/2308.07123](https://arxiv.org/abs/2308.07123)
+ **Bridging Perspectives: A Survey on Cross-view Collaborative Intelligence with Egocentric-Exocentric Vision**
    - Publication: arXiv 2025
    - Highlights: Systematically sorts out the direction of egocentric-exocentric collaborative learning, covering three paradigms: exocentric-assisted egocentric, egocentric-assisted exocentric, and joint learning
    - Paper Link: [https://arxiv.org/abs/2506.06253](https://arxiv.org/abs/2506.06253)
+ **First-Person Vision**
    - Publication: Proceedings of the IEEE 2012
    - Highlights: Foundational survey of the field, formally defining the research scope, core challenges and application directions of first-person vision for the first time
    - Paper Link: [https://ieeexplore.ieee.org/document/6232429](https://ieeexplore.ieee.org/document/6232429)
+ **HD-EPIC: A Highly-Detailed Egocentric Video Dataset**
    - Publication: arXiv 2025
    - Highlights: Constructs the current highest annotation density unscripted first-person dataset of real household scenes, containing 41 hours of kitchen cooking videos, covering multi-level linked annotations such as recipe steps, fine-grained actions, ingredient nutrition, 3D digital twin scenes, eye movement data, and audio events
    - Paper Link: [https://arxiv.org/pdf/2502.04144](https://arxiv.org/pdf/2502.04144)
+ **Ego-Exo4D: Understanding Skilled Human Activity from First- and Third-Person Perspectives** 
    - Publication: CVPR 2024
    - Highlights: Currently the world's largest multimodal dataset with synchronously collected first/third-person perspective videos, containing 1286 hours of paired videos covering professional skill scenarios such as sports, music, dance, and equipment maintenance
    - Paper Link: [https://arxiv.org/pdf/2311.18259](https://arxiv.org/pdf/2311.18259)
+ **EgoExoLearn: A Dataset for Bridging Asynchronous Ego- and Exo-centric View of Procedural Activities in Real World** 
    - Publication: CVPR 2024
    - Highlights: The first asynchronous cross-view dataset simulating the human learning process of "watching third-person demonstrations - first-person practice", containing 120 hours of paired demonstration videos and first-person practice videos covering daily life and professional laboratory scenarios
    - Paper Link: [https://arxiv.org/pdf/2403.16182](https://arxiv.org/pdf/2403.16182)
+ **EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding** 
    - Publication: ICCV 2023
    - Highlights: Proposes a diagnostic benchmark for language understanding of ultra-long temporal first-person videos, introducing the "temporal certificate" quantitative indicator to measure the intrinsic temporal reasoning difficulty of tasks
    - Paper Link: [https://arxiv.org/pdf/2308.09126](https://arxiv.org/pdf/2308.09126)
+ **Ego4D: Around the World in 3,000 Hours of Egocentric Video** 
    - Publication: CVPR 2022
    - Highlights: To date, the world's largest first-person perspective video dataset, containing 3670 hours of daily life activity videos collected from 923 participants in 74 locations across 9 countries worldwide
    - Paper Link: [https://arxiv.org/pdf/2110.07058](https://arxiv.org/pdf/2110.07058)
+ **Rescaling Egocentric Vision**
    - Publication: IJCV 2021
    - Highlights: Releases the classic large-scale first-person kitchen action dataset EPIC-KITCHENS-100, containing 100 hours of video, 90,000+ fine-grained action segments, and proposes an innovative annotation pipeline of "pause - narrate", significantly improving annotation density and accuracy
    - Paper Link: [https://arxiv.org/pdf/2006.13256](https://arxiv.org/pdf/2006.13256)
+ **Charades-Ego: A Large-Scale Dataset of Paired Third and First Person Videos**
    - Publication: CVPR 2018
    - Highlights: Constructs the first large-scale paired first/third-person daily action dataset, covering diverse household scenes and daily activity categories
    - Paper Link: [https://arxiv.org/pdf/1804.09626](https://arxiv.org/pdf/1804.09626)
+ **Position: Life-Logging Video Streams Make the Privacy-Utility Trade-off Inevitable**
    - Publication: arXiv 2026
    - Highlights: Systematically analyzes the privacy risks of life-logging video streams in the entire link of perception, transmission, and storage, pointing out the limitations of existing single-point privacy protection methods in cross-view collaborative scenarios
    - Paper Link: [https://arxiv.org/pdf/2605.10404](https://arxiv.org/pdf/2605.10404)

---

## 🔬 Core Research Topics
### 2.1 Action Recognition, Detection & Anticipation
> The most fundamental and mature direction of Egocentric vision, studying the recognition, detection and prediction of human actions from first-person videos.
>

#### Action Recognition & Detection
+ **EgoAction: Egocentric Action Composition with Reliability-Aware Temporal Fusion**
    - Publication: CVPR 2026 EPIC-KITCHENS Challenge Champion Solution
    - Highlights: Proposes a decoupled verb-noun detection + dynamic weighted fusion strategy, achieving SOTA accuracy for long untrimmed videos based on VideoMAE-L features
    - Paper Link: [https://arxiv.org/abs/2605.24496](https://arxiv.org/abs/2605.24496)
+ **Ego-Only: Egocentric Action Detection without Exocentric Transferring**
    - Publication: ICCV 2023
    - Highlights: Proves for the first time that models trained with pure first-person data can surpass methods relying on third-person transfer
    - Paper Link: [https://openaccess.thecvf.com/content/ICCV2023/papers/Wang_Ego-Only_Egocentric_Action_Detection_without_Exocentric_Transferring_ICCV_2023_paper.pdf](https://openaccess.thecvf.com/content/ICCV2023/papers/Wang_Ego-Only_Egocentric_Action_Detection_without_Exocentric_Transferring_ICCV_2023_paper.pdf)
+ **MM-CDFSL: Multimodal Cross-Domain Few-Shot Learning for Egocentric Action Recognition**
    - Publication: ECCV 2024
    - Highlights: Systematically studies the cross-domain few-shot scenario of egocentric action recognition for the first time, proposing a multimodal distillation framework
    - Paper Link: [https://arxiv.org/pdf/2405.19917](https://arxiv.org/pdf/2405.19917)

#### Action Anticipation
+ **GANO: Enhancing Next Active Object-Based Egocentric Action Anticipation with Guided Attention**
    - Publication: arXiv 2023
    - Highlights: Aims at the next active object prediction task, proposing a guided attention mechanism
    - Paper Link: [https://arxiv.org/abs/2305.12953](https://arxiv.org/abs/2305.12953)
+ **PALM: Predicting Actions through Language Models**
    - Publication: arXiv 2023
    - Highlights: Introduces large language models into long temporal action anticipation for the first time
    - Paper Link: [https://arxiv.org/abs/2311.17944](https://arxiv.org/abs/2311.17944)
+ **INSIGHT: Intention-Guided Cognitive Reasoning for Egocentric Long-Term Action Anticipation**
    - Publication: AAAI 2026
    - Highlights: Proposes a two-stage framework of "HOI semantic recognition + intention reasoning"
    - Paper Link: [https://arxiv.org/pdf/2508.01742](https://arxiv.org/pdf/2508.01742)
+ **Ego4OOD: Rethinking Egocentric Video Domain Generalization via Covariate Shift Scoring**
    - Publication: arXiv 2026
    - Highlights: Proposes the Ego4OOD domain generalization benchmark, containing 8 geographically different domains, and introduces a clustering-based covariate shift metric
    - Paper Link: [https://arxiv.org/abs/2601.17056](https://arxiv.org/abs/2601.17056)
+ **Cross-Modal Action Recognition in Egocentric Video Using Mamba: Integrating RGB and Hand Skeleton Streams via CLS Token Fusion Strategies**
    - Publication: EgoVis@CVPR 2026
    - Highlights: A cross-modal architecture based on the Mamba framework, fusing RGB video and temporal hand skeleton data, and proposing four CLS Token mixing strategies
    - Paper Link: [https://arxiv.org/abs/2605.24302](https://arxiv.org/abs/2605.24302)
+ **Egocentric Hand Activity Video Dataset and Bidirectional Motion-Priors for Hand Action Recognition**
    - Publication: IEEE Access 2026, Vol.14
    - Highlights: Releases the Ego-Bi large-scale first-person RGB video dataset (1,223 sequences, 622,737 frames), proposing a bidirectional motion prior module
    - Paper Link: [https://ksp.etri.re.kr/ksp/article/read?id=72508](https://ksp.etri.re.kr/ksp/article/read?id=72508)
+ **Ego-METAS: Egocentric online Multimodal Energy-efficient Temporal Action Segmentation benchmark**
    - Publication: arXiv 2026
    - Highlights: The first online multimodal temporal action segmentation benchmark for energy awareness, containing 100+ hours of untrimmed videos, covering 5 modalities
    - Paper Link: [https://arxiv.org/abs/2606.02246](https://arxiv.org/abs/2606.02246)
+ **Continual Multimodal Egocentric Activity Recognition via Modality-Aware Novel Detection**
    - Publication: arXiv 2026
    - Highlights: Proposes the MAND modality-aware framework, improving the novel activity detection AUC by 10%
    - Paper Link: [https://arxiv.org/abs/2603.16970](https://arxiv.org/abs/2603.16970)
+ **EgoFusion: unified semantic and scale-aware prompt fusion for egocentric action recognition**
    - Publication: Multimedia Systems 2026
    - Highlights: Proposes the EgoFusion prompt learning framework, enhancing verb-noun semantic alignment through a component semantic interaction module
    - Paper Link: [https://dl.acm.org/doi/10.1007/s00530-026-02282-1](https://dl.acm.org/doi/10.1007/s00530-026-02282-1)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| --- | --- | --- | --- | --- |
| ⭐ Ego4D | 2022 | ~3,670 h | AR, VQA, forecasting, many | [Official Website](https://ego4d-data.org/) |
| ⭐ EPIC-KITCHENS-100 | 2021 | 100 h / 90K segments | Action Recognition, Detection, Anticipation | [Official Website](https://epic-kitchens.github.io/) |
| ChildLens | 2026 | 108.58 h / 354 videos | Children's Daily Activity Analysis | [Data](https://doi.org/10.17617/4.fe) |
| EgoScale | 2026 | 20k+ h labeled manipulation | Action, Dexterity Transfer | [Paper](https://arxiv.org/abs/2602.16710) |
| CogDrive (EyeCue) | 2026 | Multi-scenario Driving | Driver Cognitive Distraction Detection | [Paper](https://arxiv.org/abs/2605.07859) |
| Ego-METAS | 2026 | 100+ h / 5 modalities | Online Action Segmentation, Sensor Routing | [HF](https://huggingface.co/datasets/Ego-METAS/Ego-METAS) |
| Furhat Egocentric Dataset | 2026 | 20 seq. / ~25 min | Robot-Self Face/Body Tracking | [Paper](https://arxiv.org/abs/2606.03694) |
| World In Your Hands | 2025 | 1000+ h labeled manipulation | Action, VLA Training | [GitHub](https://github.com/tars-robotics/World-In-Your-Hands) |
| EgoCampus | 2025 | ~32 h | Gaze, Pedestrian Egocentric | [GitHub](https://github.com/ComputerVisionRutgers/EgoCampus) |
| AEA | 2024 | 143 seq. / ~7.3 h | Daily Activities (Aria) | [Aria](https://www.projectaria.com/datasets/aea/) |
| EgoSurgery | 2024 | Open Surgery Videos | Surgical Phase, Tool Detection | [GitHub](https://github.com/Fujiry0/EgoSurgery) |
| EgoExo-Fitness | 2024 | 32 h / 1,276 seq. | Full-Body Action, Quality Assessment | [GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness) |
| E³ (Exploring Embodied Emotion) | 2024 | 50+ h | Emotion Recognition, Multimodal | [GitHub](https://github.com/Exploring-Embodied-Emotion-official/E3) |
| EGOFALLS | 2023 | Fall Samples | Fall Detection | [Dataverse](https://www.dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/HO5GE3) |
| Epic-Sounding-Object | 2023 | 3.2K short clips | Audiovisual Object Localization | [GitHub](https://github.com/WikiChao/Ego-AV-Loc) |
| HoloAssist | 2023 | 169 h | Interactive Assistant | [Official Website](https://holoassist.github.io/) |
| WEAR | 2023 | ~19 h outdoor sports | Activity + IMU | [Official Website](https://mariusbock.github.io/wear/) |
| N-EPIC-KITCHENS | 2022 | Event+RGB Subset | Neuromorphic Action Recognition | [GitHub](https://github.com/EgocentricVision/N-EPIC-Kitchens) |
| Ego-Deliver | 2021 | 5,360 videos | Delivery Behavior Analysis | [Official Website](https://egodeliver.github.io/) |
| HOMAGE | 2021 | 30 h | Household Activity Composition Understanding | [GitHub](https://github.com/nishantrai18/homage) |
| MECCANO | 2021 | ~55 h industrial | Hand-Object Interaction, Industrial | [Official Website](https://iplab.dmi.unict.it/MECCANO/) |
| EGO-CH | 2020 | 27+ h | Tourist Behavior, POI Tasks | [Paper](https://arxiv.org/abs/2002.00899) |
| EgoCom | 2020 | 38.5 h conversation | Multi-person Egocentric Dialogue | [GitHub](https://github.com/facebookresearch/EgoCom-Dataset) |
| LEMMA | 2020 | Multi-view Activity | Multi-agent Tasks | [GitHub](https://github.com/Buzz-Beater/LEMMA) |
| Charades-Ego | 2018 | Paired Egocentric/Exocentric | Alignment, Action | [Official Website](https://prior.allenai.org/projects/charades-ego) |
| EGTEA Gaze+ | 2018 | 28 h cooking | Gaze+Action Recognition | [Official Website](https://cbs.ic.gatech.edu/fpv/) |
| EgoGesture | 2017 | 2K+ videos / 24K samples | Gesture Recognition | [Official Website](https://nlpr.ia.ac.cn/iva/yfzhang/datasets/egogesture.html) |
| Stanford ECM | 2017 | 31 h | Daily Activity Classification | [Paper](https://openaccess.thecvf.com/content_cvpr_2017/html/Nakamura_Jointly_Learning_Energy_CVPR_2017_paper.html) |
| THU-READ | 2017 | 1,920 clips | Helmet RGB-D Action | [Official Website](https://ivg.au.tsinghua.edu.cn/dataset/THU_READ.php) |
| PEV | 2016 | 1,226 pairs | Dyadic Dialogue Micro-actions | [Paper](https://openaccess.thecvf.com/content_cvpr_2016/html/Yonetani_Recognizing_Micro-Actions_and_CVPR_2016_paper.html) |
| FPPA | 2015 | 5 subjects | Daily Actions + Hand/Gaze | [Paper](https://openaccess.thecvf.com/content_iccv_2015/html/Zhou_Temporal_Perception_and_ICCV_2015_paper.html) |
| JPL-Interaction | 2013 | 84 videos | First-Person Activity Recognition | [Official Website](http://michaelryoo.com/jpl-interaction.html) |
| ADL | 2012 | ~10 h | Daily Activity Recognition | [Official Website](https://www.csee.umbc.edu/~hpirsiav/papers/ADLdataset/) |
| Social Interactions | 2012 | ~60 h | Social Activities | [Official Website](https://cbs.ic.gatech.edu/fpv/) |
| EgoAction | 2011 | First-Person Sports Videos | Action Recognition | [Paper](https://doi.org/10.1109/CVPR.2011.5995406) |


---

### 2.2 Hand-Object Interaction & Fine-grained Activity
> Studies the interaction process between hands and objects from the first-person perspective, which is the core foundation of embodied intelligence and robot imitation learning.
>

+ **Glove2Hand: Synthesizing Natural Hand-Object Interaction from Multi-Modal Sensing Gloves**
    - Publication: CVPR 2026 (Highlight)
    - Highlights: Generates realistic bare-hand HOI videos from multi-modal sensing glove data, with accompanying HandSense dataset
    - Paper Link: [https://arxiv.org/pdf/2603.20850](https://arxiv.org/pdf/2603.20850)
+ **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - Publication: arXiv 2026
    - Highlights: The first egocentric HOI world model, embedding physical priors into generative diffusion models
    - Paper Link: [https://arxiv.org/abs/2603.13615](https://arxiv.org/abs/2603.13615)
+ **TOUCH: Text-guided Controllable Generation of Free-Form Hand-Object Interactions**
    - Publication: ICLR 2026
    - Highlights: Free-form HOI generation task, constructing the WildO2 large-scale 3D HOI dataset
    - Paper Link: [https://openreview.net/forum?id=4VW9HVCRw0](https://openreview.net/forum?id=4VW9HVCRw0)
+ **Do Egocentric Video-Language Models Truly Understand Hand-Object Interactions?**
    - Publication: ICLR 2025
    - Highlights: Systematically evaluates the fine-grained HOI understanding ability of egocentric VLMs for the first time, proposing EgoHOIBench
    - Paper Link: [https://arxiv.org/abs/2405.17719](https://arxiv.org/abs/2405.17719)
+ **Get a Grip: Reconstructing Hand-Object Stable Grasps in Egocentric Videos**
    - Publication: arXiv 2023
    - Highlights: Reconstructs hand-object stable grasping states from monocular egocentric videos for the first time
    - Paper Link: [https://arxiv.org/abs/2312.15719](https://arxiv.org/abs/2312.15719)
+ **HOI-Ref: Hand-Object Interaction Referral in Egocentric Vision**
    - Publication: arXiv 2024
    - Highlights: Defines a new task of HOI referral in egocentric scenarios, with accompanying HOI-QA evaluation benchmark
    - Paper Link: [https://arxiv.org/pdf/2404.09933](https://arxiv.org/pdf/2404.09933)
+ **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - Publication: NeurIPS 2025
    - Highlights: Proposes a two-layer architecture framework, using VLM to infer motion priors at the high level, and flow matching strategy based on DiT to generate fine-grained trajectories at the low level
    - Paper Link: [https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)
+ **Leveraging Synthetic Data for Enhancing Egocentric Hand-Object Interaction Detection**
    - Publication: IJCV 2026, Vol.134
    - Highlights: Using only a small amount of real annotated data combined with synthetic data, AP is improved by 11.69% on VISOR, and the HOI-Synth synthetic data generation pipeline is open-sourced
    - Paper Link: [https://rd.springer.com/article/10.1007/s11263-026-02838-8](https://rd.springer.com/article/10.1007/s11263-026-02838-8)
+ **Hand Trajectory Fusion for Egocentric Natural Language Query Grounding**
    - Publication: EgoVis@CVPR 2026
    - Highlights: Integrates hand motion cues into the NLQ grounding task for the first time, improving R1@IoU=0.3 by 2.54% for hand-object interaction queries
    - Paper Link: [https://arxiv.org/abs/2606.02962](https://arxiv.org/abs/2606.02962)
+ **TouchAnything: A Dataset and Framework for Bimanual Tactile Estimation from Egocentric Video**
    - Publication: arXiv 2026
    - Highlights: The EgoTouch dataset contains 1,891 manipulation segments, synchronized multi-view RGB, 3D pose of both hands, and continuous tactile pressure maps
    - Paper Link: [https://arxiv.org/abs/2605.13083](https://arxiv.org/abs/2605.13083)
+ **EgoAERO: Learning Dexterous Manipulation from a Single Egocentric Video without Object Assets**
    - Publication: arXiv 2026
    - Highlights: A dexterous manipulation learning framework without pre-scanned object assets, constructing the EgoDex-R large-scale dataset (4.3M RGB-D frames)
    - Paper Link: [https://arxiv.org/abs/2606.08057](https://arxiv.org/abs/2606.08057)
+ **EgoInteract: Synthetic Egocentric Videos Generation for Interaction Understanding and Anticipation**
    - Publication: arXiv 2026
    - Highlights: A controllable egocentric video generation simulator, achieving precise control over cameras, human actions, and object manipulations
    - Paper Link: [https://arxiv.org/abs/2605.18214](https://arxiv.org/abs/2605.18214)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| --- | --- | --- | --- | --- |
| ⭐ HOI4D | 2022 | 2.4M frames / 4K seq. | 4D HOI | [Official Website](https://hoi4d.github.io/) |
| ⭐ EgoDex | 2025 | 829 h / 30K trajectories | Dexterous Manipulation, Pose | [GitHub](https://github.com/apple/ml-egodex) |
| EventEgoHands | 2026 | 48 clips / 129.6K frames | RGB+Event Hand Detection | [GitHub](https://github.com/SynthSyntax/EventEgoHands) |
| EgoTactile | 2026 | ~6 h / 768 clips | Grasp Pressure Estimation | [Official Website](https://egotactile.github.io/) |
| EgoDex-R | 2026 | 4.3M RGB-D frames / 5.6K seq. | Dexterous Manipulation, Hand-Object Pose | [Paper](https://arxiv.org/abs/2606.08057) |
| HA-Ego-1K | 2026 | ~24 h / 484 multi-view clips | Dexterous Manipulation | [HF](https://huggingface.co/datasets/humanarchive/HA-Ego-1K) |
| DexGloveHOI | 2026 | 3.5 h / 100K+ samples | Visual-IMU 3D Hand Tracking | [Paper](https://arxiv.org/abs/2605.21714) |
| EgoTouch | 2026 | 1,891 episodes / 208 tasks | Tactile HOI | [HF](https://huggingface.co/datasets/zhenyuxie-zhzh/EgoTouch_hdf5) |
| EgoEVHands | 2026 | 5,419 annotated seq. | Stereo Event 3D Gesture | [GitHub](https://github.com/ZJUWang01/EgoEV-HandPose) |
| EgoEMG | 2026 | 41 participants / 10+ h | EMG+Visual Hand Pose | [GitHub](https://github.com/zhenqis123/EgoEMG) |
| HRDexDB | 2026 | 1.4K grasping trials | Dexterous Grasping, Tactile | [HF](https://huggingface.co/datasets/hahahataeyun/hrdexdb) |
| TouchMoment | 2026 | 4,021 videos / 8,456 touch moments | Touch Moment Detection | [Paper](https://arxiv.org/abs/2604.12343) |
| EgoFun3D | 2026 | 271 egocentric videos | Interactive 3D Objects | [Official Website](https://3dlg-hcvc.github.io/EgoFun3D/) |
| SHOW3D | 2026 | Wild Egocentric-Exocentric HOI | 3D Hand-Object Annotation | [Paper](https://arxiv.org/abs/2603.28760) |
| FEEL | 2026 | Force-Synchronized Kitchen Videos | Physical Action Understanding | [Official Website](https://www.cs.umd.edu/~edessale/feel) |
| EgoPoints | 2025 | Point Trajectories + Synthetic | Egocentric Video Tracking | [GitHub](https://github.com/AhmadDarKhalil/EgoPoints) |
| AssemblyHands | 2023 | 3M images | 3D Hand Pose | [Official Website](https://assemblyhands.github.io/) |
| EgoObjects | 2023 | 9.2K+ videos | Detection, Instance Segmentation | [GitHub](https://github.com/facebookresearch/EgoObjects) |
| ENIGMA-51 | 2023 | 22 h industrial | Fine-grained Behavior | [Official Website](https://fpv-iplab.github.io/ENIGMA-51/) |
| POV-Surgery | 2023 | ~88K frames (Synthetic) | Surgical Hand-Tool Pose | [Official Website](https://batfacewayne.github.io/POV_Surgery_io/) |
| VOST | 2023 | 713 videos | Video Object Segmentation | [Official Website](https://www.vostdataset.org/) |
| EgoBody | 2022 | 125 seq. | Body Pose, Interaction | [Official Website](https://egobody.ethz.ch/) |
| EgoHOS | 2022 | 11K+ images | Hand-Object Segmentation | [GitHub](https://github.com/owenzlz/EgoHOS) |
| EgoPAT3D | 2022 | 1M+ frames RGB-D | 3D Action Target Prediction | [GitHub](https://github.com/ai4ce/EgoPAT3D) |
| Touch and Go | 2022 | 12K+ vis–tactile frames | Visual+Tactile | [Official Website](https://touch-and-go.github.io/) |
| VISOR | 2022 | EPIC + masks | Segmentation, HOI | [Official Website](https://epic-kitchens.github.io/VISOR) |
| H2O | 2021 | 100K+ frames | Bimanual Interaction | [Official Website](https://h2odataset.ethz.ch/) |
| TREK-150 | 2021 | 150 EPIC seq. | Object Tracking | [Official Website](https://machinelearning.uniud.it/datasets/trek150/) |
| You2Me | 2020 | 14 seq. | Infer Body Pose via Egocentric-Exocentric | [GitHub](https://github.com/facebookresearch/you2me) |
| FPHA | 2018 | 1.2K seq. | Hand Pose + Action | [Official Website](https://guiggh.github.io/publications/first-person-hands/) |
| EgoDexter | 2017 | ~3.2K frames | Hand Tracking under Occlusion | [Official Website](https://handtracker.mpi-inf.mpg.de/projects/OccludedHands/EgoDexter.htm) |
| EgoHands | 2015 | 4.8K labeled frames | Hand Detection | [Official Website](http://vision.soic.indiana.edu/projects/egohands/) |
| BEOID | 2014 | 58 videos | Hand-Object Interaction | [Official Website](https://data.bris.ac.uk/data/dataset/3wats8ruq1sp52hq3bo8dkzul3) |
| EDSH | 2013 | 2 videos | Pixel-level Hand Segmentation | [Official Website](http://www.cs.cmu.edu/~kkitani/datasets/) |
| Handled Objects | 2009 | 11 categories | Grasp Sequences | [Paper](https://doi.org/10.1109/CVPRW.2009.5204360) |


---

### 2.3 Egocentric Vision-Language Models (Ego-VLM / Ego-LLM)
> Combining large language models with first-person vision to achieve advanced cognitive capabilities such as video question answering, content description, and reasoning, which is the current hottest direction.
>

#### Pre-trained Foundation Models
+ **Egocentric Video-Language Pretraining (EgoVLP)**
    - Publication: CVPR 2022
    - Highlights: The first video-language pre-training framework specifically for egocentric scenarios
    - Paper Link: [https://arxiv.org/abs/2206.01670](https://arxiv.org/abs/2206.01670)
+ **EgoVLPv2: Egocentric Video-Language Pre-training with Fusion in the Backbone**
    - Publication: ICCV 2023
    - Highlights: Improved VLP with fusion in the backbone network
    - Paper Link: [https://arxiv.org/pdf/2307.05463](https://arxiv.org/pdf/2307.05463)

#### Advanced Reasoning & Cutting-Edge Advances
+ **EgoThinker: Unveiling Egocentric Reasoning with Spatio-Temporal CoT**
    - Publication: NeurIPS 2025
    - Highlights: Introduces Chain of Thought (CoT) into egocentric video understanding, proposing a spatio-temporal chain of thought framework
    - Paper Link: [https://arxiv.org/abs/2510.23569](https://arxiv.org/abs/2510.23569)
+ **CLiViS: Unleashing Cognitive Map through Linguistic-Visual Synergy for Embodied Visual Reasoning**
    - Publication: arXiv 2025
    - Highlights: Constructs cognitive maps through linguistic-visual synergy, breaking through the bottleneck of long video reasoning
    - Paper Link: [https://arxiv.org/abs/2506.17629](https://arxiv.org/abs/2506.17629)
+ **PhysBrain: Human Egocentric Data as a Bridge from Vision Language Models to Physical Intelligence**
    - Publication: arXiv 2025
    - Highlights: Converts human first-person videos into embodied supervision data
    - Paper Link: [https://arxiv.org/abs/2512.16793](https://arxiv.org/abs/2512.16793)
+ **Vinci: A Real-time Smart Assistant based on Egocentric Vision-Language Model**
    - Publication: ACM 2025 (arXiv 2024)
    - Highlights: A lightweight Ego-VLM for wearable devices, supporting long video memory and action generation, and can run in real-time on edge devices
    - Paper Link: [https://arxiv.org/abs/2412.21080](https://arxiv.org/abs/2412.21080)
+ **EgoMotion: Hierarchical Reasoning and Diffusion for Egocentric Vision-Language Motion Generation**
    - Publication: arXiv 2026
    - Highlights: Proposes a hierarchical reasoning and diffusion framework to generate language-described 3D human motion from first-person videos
    - Paper Link: [https://arxiv.org/abs/2604.19105](https://arxiv.org/abs/2604.19105)
+ **The Right Inference Strategy Is All You Need: Nearly Training-Free Domain-Wise Inference for EgoCross Challenge**
    - Publication: arXiv 2026
    - Highlights: EgoCross Challenge solution, domain-aware inference strategy achieves 66.98% accuracy with only 20 training samples
    - Paper Link: [https://arxiv.org/abs/2606.00829](https://arxiv.org/abs/2606.00829)
+ **Decoding Pedestrian Crossing Intention from Egocentric Vision via Vision Language Models**
    - Publication: arXiv 2026
    - Highlights: Uses VLM to decode pedestrian crossing intention for the first time, with accuracy improved by 14.5% after fusing eye movement and ego-motion
    - Paper Link: [https://arxiv.org/abs/2606.09142](https://arxiv.org/abs/2606.09142)
+ **Allocentric Perceiver: Disentangling Allocentric Reasoning from Egocentric Visual Priors via Frame Instantiation**
    - Publication: arXiv 2026
    - Highlights: A training-agnostic allocentric perception strategy, recovering metric 3D states from single or multiple images, improving by about 10% on allocentric tasks
    - Paper Link: [https://arxiv.org/abs/2602.05789](https://arxiv.org/abs/2602.05789)
+ **EgoBabyVLM: Benchmarking Cross-Modal Learning from Naturalistic Egocentric Video Data**
    - Publication: arXiv 2026
    - Highlights: The first systematic benchmark test, finding that current VLMs rely on tight semantic alignment and cannot utilize weakly aligned natural signals
    - Paper Link: [https://arxiv.org/abs/2605.19130](https://arxiv.org/abs/2605.19130)
+ **EgoTL: Egocentric Think-Aloud Chains for Long-Horizon Tasks**
    - Publication: arXiv 2026
    - Highlights: Records step-by-step goals and verbal reasoning using the "think aloud before acting" protocol, covering 100+ daily household tasks
    - Paper Link: [https://arxiv.org/abs/2604.09535](https://arxiv.org/abs/2604.09535)
+ **Gaze-Regularized VLMs for Ego-Centric Behavior Understanding**
    - Publication: arXiv 2026
    - Highlights: Integrates eye movement information into VLM training, making the model focus on gaze-highlighted regions through gaze regularization mechanism, improving semantic scores by nearly 13%
    - Paper Link: [https://arxiv.org/abs/2603.23190](https://arxiv.org/abs/2603.23190)
+ **Towards Comprehensive Scene Understanding: Integrating First and Third-Person Views for LVLMs**
    - Publication: NeurIPS 2025
    - Highlights: Proposes the E3VQA multi-view question answering benchmark (4K high-quality QA pairs) and M3CoT prompt technology, improving by 4.84% on GPT-4o
    - Paper Link: [https://proceedings.neurips.cc/paper_files/paper/2025/hash/1af83ab66b4f07a3f55788e67dab5782-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/1af83ab66b4f07a3f55788e67dab5782-Abstract-Conference.html)
+ **Exo2Ego: Exocentric Knowledge Guided MLLM for Egocentric Video Understanding**
    - Publication: AAAI 2026
    - Highlights: Constructs the Ego-ExoClip pre-training dataset (1.1 million synchronized egocentric-exocentric clip-text pairs), proposing a three-stage progressive mapping learning pipeline
    - Paper Link: [https://ojs.aaai.org/index.php/AAAI/article/view/38244](https://ojs.aaai.org/index.php/AAAI/article/view/38244)
+ **Spatial Reasoning with Vision-Language Models in Ego-Centric Multi-View Scenes**
    - Publication: ICLR 2026
    - Highlights: Proposes the Ego3D-Bench spatial reasoning benchmark (8,600+ QA pairs), and the Ego3D-VLM post-training framework
    - Paper Link: [https://iclr.cc/virtual/2026/poster/10008200](https://iclr.cc/virtual/2026/poster/10008200)
+ **Personal Visual Context Learning in Large Multimodal Models**
    - Publication: arXiv 2026
    - Highlights: Proposes Personal VCL, building benchmarks based on EgoLife/Ego4D/CaptainCook4D, containing 2,255 personal visual queries
    - Paper Link: [https://vision.cs.utexas.edu/projects/PersonalVCL/](https://vision.cs.utexas.edu/projects/PersonalVCL/)
+ **EgoCoT-Bench: Benchmarking Grounded and Verifiable Operation-Centric Chain of Thought Reasoning for MLLMs**
    - Publication: arXiv 2026
    - Highlights: Contains 3,172 verifiable QA pairs, constructed through a spatio-temporal scene graph-guided generation framework, covering 12 subtasks
    - Paper Link: [https://arxiv.org/abs/2605.19559](https://arxiv.org/abs/2605.19559)
+ **Benchmarking Egocentric Multimodal Goal Inference for Assistive Wearable Agents**
    - Publication: NeurIPS 2025 Datasets and Benchmarks Track
    - Highlights: Goal inference benchmark dataset, containing 363 participants, 3,482 records, human upper limit 93% accuracy, best VLM only 84%
    - Paper Link: [https://papers.nips.cc/paper_files/paper/2025/hash/23ab960082db936f874b171822e0d097-Abstract-Datasets_and_Benchmarks_Track.html](https://papers.nips.cc/paper_files/paper/2025/hash/23ab960082db936f874b171822e0d097-Abstract-Datasets_and_Benchmarks_Track.html)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| --- | --- | --- | --- | --- |
| HD-EPIC | 2025 | ~41 h / dense labels | Fine-grained Kitchen, VQA | [Official Website](https://hd-epic.github.io/) |
| EgoClip | 2022 | 3.8M clip–text pairs | Video-Language Pre-training | [GitHub](https://github.com/showlab/EgoVLP) |
| EgoTL | 2026 | 100+ daily household tasks | Long-Horizon Reasoning, Spatial QA | [Official Website](https://ego-tl.github.io/) |
| MM-Conv | 2026 | 6.7 h / 4,211 expressions | Contextual 3D Dialogue Referring | [Paper](https://arxiv.org/abs/2605.21796) |
| Minerva-Ego | 2026 | 1,160 QA / 156 videos | Spatio-Temporal Reasoning Trajectory | [GitHub](https://github.com/google-deepmind/neptune) |
| EgoEverything | 2026 | 100+ h / 5K+ MCQs | Long-Context AR Video QA | [Paper](https://arxiv.org/abs/2604.08342) |
| EgoEsportsQA | 2026 | 1,745 QA pairs | Esports Video QA, Reasoning | [Paper](https://arxiv.org/abs/2604.12320) |
| MyEgo | 2026 | 541 long videos / 5K QA | Personalized Video QA | [GitHub](https://github.com/Ryougetsu3606/MyEgo) |
| LifeDialBench / EgoMem | 2026 | Life Logging Memory | Online Evaluation | [GitHub](https://github.com/qys77714/LifeDialBench) |
| Ego2Web | 2026 | 500 video-instruction pairs | Egocentric Video Grounded Web Agent | [HF](https://huggingface.co/datasets/Shoubin/Ego2Web) |
| NoRA | 2026 | 1,420 clips | Normative Action Reasoning | [Paper](https://arxiv.org/abs/2606.04806) |
| Causal-Plan-1M | 2026 | 1M QA / 22.2K clips | Physically Grounded Planning QA | [HF](https://huggingface.co/datasets/anonymous-causal-plan/Causal_Plan) |
| Pause-and-Think | 2026 | 10K QA clips + 300 benchmark | Assistive Action Suggestion | [GitHub](https://github.com/sssshivvvv/pause-and-think) |
| EgoCoT-Bench | 2026 | 351 videos / 3,172 QA | Grounded Operation-Centric CoT QA | [Official Website](https://dstardust.github.io/EgoCoT/) |
| EgoEMS | 2025 | 20+ h emergency scenarios | First Aid QA, Multimodal | [GitHub](https://github.com/UVA-DSA/EgoEMS) |
| HowToDIV | 2025 | ~24 h instructional | Dialogue, Procedural QA | [GitHub](https://github.com/google/howtodiv) |
| InterVLA | 2025 | 11.4 h interactions | Instruction, Egocentric-Exocentric Action Capture | [Official Website](https://liangxuy.github.io/InterVLA/) |
| AssistQ | 2022 | 100 long videos / 529 QA | Instructional QA | [GitHub](https://github.com/showlab/AssistQ) |
| EgoTaskQA | 2022 | ~2K videos / 40K QA | Causal & Task QA | [Official Website](https://sites.google.com/view/egotaskqa) |
| EgoVQA | 2019 | 600+ QAs | Video QA | [ICCVW 2019](https://openaccess.thecvf.com/content_ICCVW_2019/html/EPIC/Fan_EgoVQA_-_An_Egocentric_Video_Question_Answering_Benchmark_Dataset_ICCVW_2019_paper.html) |


---

### 2.4 Long-form Video Understanding & QA
> Processing ultra-long first-person videos at the hour-level or even day-level, with core challenges of long temporal dependency modeling, memory retrieval and information summarization.
>

+ **EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding**
    - Publication: NeurIPS 2023
    - Highlights: Authoritative diagnostic benchmark for ultra-long egocentric video understanding
    - Paper Link: [https://arxiv.org/pdf/2308.09126](https://arxiv.org/pdf/2308.09126)
+ **OSGNet: Champion Solution for Ego4D Episodic Memory Challenge 2025**
    - Publication: CVPR 2025 Challenge All-Track Champion
    - Highlights: Proposes an early fusion temporal localization architecture, winning three tasks of the Ego4D Episodic Memory Challenge
    - Paper Link: [https://arxiv.org/abs/2506.03710](https://arxiv.org/abs/2506.03710)
+ **EgoMemory: Memory-Augmented Personalized Retrieval for Long-Context Egocentric Video**
    - Publication: ACL 2026
    - Highlights: Proposes a lifelong memory framework for continuous streaming first-person videos
    - Paper Link: [https://www.microsoft.com/en-us/research/publication/egomemory-memory-augmented-personalized-retrieval-for-long-context-egocentric-video/](https://www.microsoft.com/en-us/research/publication/egomemory-memory-augmented-personalized-retrieval-for-long-context-egocentric-video/)
+ **Unique Lives, Shared World: Learning from Single-Life Egocentric Videos**
    - Publication: arXiv 2025
    - Highlights: Studies the learning problem of ultra-long life-cycle videos of a single individual
    - Paper Link: [https://arxiv.org/abs/2512.04085](https://arxiv.org/abs/2512.04085)
+ **MyEgo: Ego-Grounding for Personalized Question-Answering in Egocentric Videos**
    - Publication: CVPR 2026
    - Highlights: Large-scale personalized first-person video dataset
    - Paper Link: [https://arxiv.org/pdf/2604.01966](https://arxiv.org/pdf/2604.01966)
+ **EGAgent: Agentic Very Long Video Understanding**
    - Publication: arXiv 2026
    - Highlights: An agent-based reasoning framework based on entity scene graphs, capable of processing continuous video streams at the cross-day level, supporting structured multi-hop reasoning and audio-visual hybrid retrieval
    - Paper Link: [https://arxiv.org/abs/2601.18157](https://arxiv.org/abs/2601.18157)
+ **EgoMemReason: A Memory-Driven Reasoning Benchmark for Long-Horizon Egocentric Video Understanding**
    - Publication: arXiv 2026
    - Highlights: A benchmark for evaluating week-level egocentric video memory-driven reasoning, containing 500 questions, with the best model only achieving 39.6% accuracy
    - Paper Link: [https://arxiv.org/abs/2605.09874](https://arxiv.org/abs/2605.09874)
+ **Semantic and Visual Evidence for Efficient Long-Video Reasoning: A Solution for the HD-EPIC VQA Challenge**
    - Publication: arXiv 2026
    - Highlights: Decouples long video reasoning into semantic evidence and visual evidence, achieving efficient long video understanding via query-conditioned retrieval integration
    - Paper Link: [https://arxiv.org/abs/2605.29402](https://arxiv.org/abs/2605.29402)
+ **Bridging Modalities, Spanning Time: Structured Memory for Ultra-Long Agentic Video Reasoning**
    - Publication: arXiv 2026
    - Highlights: Proposes modality-interleaved narrative chain and multi-modal memory graph based MAGIC-Video framework, outperforms prior state-of-the-art agent systems by 10.1 points on EgoLifeQA
    - Paper Link: [https://arxiv.org/abs/2605.08271](https://arxiv.org/abs/2605.08271)
+ **MA-EgoQA: Question Answering over Egocentric Videos from Multiple Embodied Agents**
    - Publication: arXiv 2026
    - Highlights: First definition of multi-agent egocentric video QA task, providing 1,700+ questions across five scene categories
    - Paper Link: [https://arxiv.org/abs/2603.09827](https://arxiv.org/abs/2603.09827)
+ **Spatial-Conditioned Reasoning in Long-Egocentric Videos**
    - Publication: arXiv 2026
    - Highlights: Explores explicit spatial signals' impact on long-form VLM reasoning, introduces finely re-annotated Sanpo-D dataset
    - Paper Link: [https://arxiv.org/abs/2601.18100](https://arxiv.org/abs/2601.18100)
+ **FocusGraph: Graph-Structured Frame Selection for Embodied Long Video Question Answering**
    - Publication: arXiv 2026
    - Highlights: Graph-based frame filtering pipeline, leverages Scene-Caption LLM selector to retrieve query-relevant frames
    - Paper Link: [https://arxiv.org/abs/2603.04349](https://arxiv.org/abs/2603.04349)
+ **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - Publication: ICLR 2026
    - Highlights: Benchmark assessing embodied cognition via egocentric world modeling, reveals VLMs perform better on inverse tasks than forward prediction
    - Paper Link: [https://iclr.cc/virtual/2026/10013240](https://iclr.cc/virtual/2026/10013240)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| --- | --- | --- | --- | --- |
| EgoLife | 2025 | ~266–300 h daily footage | Long-term personal assistant, episodic memory | [Official Website](https://egolife-ai.github.io/) |
| EgoSchema | 2023 | 250+ h / 5K MCQs | Ultra-long video reasoning & QA | [Official Website](https://egoschema.github.io/) |
| SuperMemory-VQA | 2026 | 52.9 h / 4,853 QA pairs | Long-duration memory QA | [Hugging Face](https://huggingface.co/datasets/OSU-AIoT-MLSys-Lab/SuperMemory-VQA) |
| EgoMemReason | 2026 | 500 weekly-level MCQs | Week-scale memory reasoning evaluation | [Hugging Face](https://huggingface.co/datasets/Ted412/EgoMemReason) |
| EgoExoMem | 2026 | 2.6K MCQs / 390 clips | Cross-view episodic memory reasoning | [GitHub](https://github.com/RuipingL/EgoExoMem) |
| EgoIntrospect | 2026 | 180 h / 60 subjects | Internal user state inference, long-term memory | [Official Website](https://ego-introspect.github.io/) |
| MA-EgoQA | 2026 | 1,741 QA / 7-day multi-agent footage | Multi-agent egocentric video QA | [Official Website](https://ma-egoqa.github.io/) |
| EgoStream | 2026 | 2,250 evaluation queries | Streaming episodic memory benchmark | [Official Website](https://saroo25.github.io/Egostream/) |
| VidChapters-7M | 2023 | 817K videos / 7M chapter annotations | Long video segmentation & summarization | [Official Website](https://antoyang.github.io/vidchapters.html) |
| Multi-Ego | 2022 | ~12 h / 41 multi-wearer sequences | Cross-user video summarization | [GitHub](https://github.com/M-Elfeki/Multi-DPP) |
| DoMSEV | 2018 | 80 h / 48 long videos | Semantic video time-lapse & skimming | [Official Website](https://www.verlab.dcc.ufmg.br/semantic-hyperlapse/cvpr2018-dataset/) |
| HUJI-EgoSeg | 2014 | 29 untrimmed long videos | Temporal activity segmentation | [Official Website](http://www.cs.huji.ac.il/~yedMDpid/egoseg/) |
| UT Ego | 2012 | ~17 h / 4 full-length recordings | Long video summarization & life logging | [Official Website](http://vision.cs.utexas.edu/projects/egocentric_data/UT_Egocentric_Dataset.html) |
| VINST / Visual Diaries | 2011 | 31 daily log videos | Event segmentation, timeline extraction | [Official Website](https://csc.kth.se/cvap/vinst/NovEgoMotion.html) |

---

### 2.5 Gaze, Attention & Intention Prediction
> Predict human gaze points, attention distribution and underlying intent from first-person footage, core technology for wearable interactive assistants.
>
+ **Ego-PMOVE: Prompt-aware Mixture of View Experts Network for Egocentric Gaze Prediction**
    - Publication: AAAI 2026
    - Highlights: First method exploring cross-view gaze correlations, prompt-driven multi-view expert mixture architecture
    - Paper Link: [https://ojs.aaai.org/index.php/AAAI/article/view/37808](https://ojs.aaai.org/index.php/AAAI/article/view/37808)
+ **Gaze Beyond the Frame: Forecasting Egocentric 3D Visual Span**
    - Publication: NeurIPS 2025
    - Highlights: Proposes novel 3D visual span forecasting task, EgoSpanLift lifts 2D gaze predictions into full 3D scene space
    - Paper Link: [https://proceedings.neurips.cc/paper_files/paper/2025/hash/bf649dbcf4eaaba4fc68ccaee25a7f9e-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/bf649dbcf4eaaba4fc68ccaee25a7f9e-Abstract-Conference.html)
+ **Gaze-Regularized VLMs for Ego-Centric Behavior Understanding**
    - Publication: arXiv 2026
    - Highlights: Embeds eye-tracking signals into VLM training pipeline, gaze regularization forces models to prioritize fixated regions, semantic metric gain ~13%
    - Paper Link: [https://arxiv.org/abs/2603.23190](https://arxiv.org/abs/2603.23190)
+ **Learning from Human Gaze: Human-like Robot Social Navigation in Dense Crowds**
    - Publication: AAAI 2026
    - Highlights: Releases GazeNav dataset with synchronized wearable eye-tracking, RGB footage and robot navigation trajectories
    - Paper Link: [https://ojs.aaai.org/index.php/AAAI/article/view/38941](https://ojs.aaai.org/index.php/AAAI/article/view/38941)
+ **In the Eye of MLLM: Benchmarking Egocentric Video Intent Understanding with Gaze-Guided Prompting**
    - Publication: NeurIPS 2025 Dataset & Benchmark Track
    - Highlights: EgoGazeVQA benchmark systematically evaluates multimodal LLM ability to infer user intent via eye movement signals
    - Paper Link: [https://proceedings.neurips.cc/paper_files/paper/2025/hash/9df42a5f6d1397e46e2cdca80a1a7903-Abstract-Datasets_and_Benchmarks_Track.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/9df42a5f6d1397e46e2cdca80a1a7903-Abstract-Datasets_and_Benchmarks_Track.html)
+ **egoEMOTION: Egocentric Vision and Physiological Signals for Emotion and Personality Recognition in Real-World Tasks**
    - Publication: NeurIPS 2025
    - Highlights: Multi-modal dataset collected via Meta Project Aria glasses combining video, eye tracking and biometric signals for real-life emotion analysis
    - Paper Link: [https://arxiv.org/pdf/2510.22129](https://arxiv.org/pdf/2510.22129)

---

### 2.6 3D/4D Reconstruction & Spatial Perception
> Recover 3D human meshes, depth maps and dynamic 4D scene structures from monocular first-person video, foundational for AR/VR and robotic spatial awareness.
>
#### Human Pose & Mesh Recovery
+ **AG-EgoPose: Leveraging Action-Guided Motion and Kinematic Joint Encoding for Egocentric 3D Pose Estimation**
    - Publication: arXiv 2026
    - Highlights: Action-conditioned motion modeling plus kinematic joint embedding for robust wearable camera pose estimation
    - Paper Link: [https://arxiv.org/pdf/2603.25175](https://arxiv.org/pdf/2603.25175)
+ **Fish2Mesh Transformer: 3D Human Mesh Recovery from Egocentric Vision**
    - Publication: arXiv 2025
    - Highlights: First mesh recovery pipeline optimized for wide fisheye head-mounted cameras
    - Paper Link: [https://arxiv.org/pdf/2503.06089](https://arxiv.org/pdf/2503.06089)

#### Event Camera-based Perception
+ **D-EventEgo: Event-Based Egocentric Human Pose Estimation in Dynamic Environments**
    - Publication: arXiv 2025
    - Highlights: Pioneering event-stream pipeline for egocentric human pose tracking under fast motion and high dynamic range
    - Paper Link: [https://arxiv.org/pdf/2505.22007](https://arxiv.org/pdf/2505.22007)

#### Scene Reconstruction & Egocentric SLAM
+ **EventEgo3D: 3D Human Motion Capture from Egocentric Event Streams**
    - Publication: CVPR 2024
    - Highlights: High-speed human motion capture system leveraging asynchronous event camera footage
    - Paper Link: [https://arxiv.org/pdf/2404.08640](https://arxiv.org/pdf/2404.08640)
+ **EventEgo3D++: 3D Human Motion Capture from a Head-Mounted Event Camera**
    - Publication: arXiv 2025
    - Highlights: End-to-end pipeline for fisheye event-based wearable full-body motion capture
    - Paper Link: [https://arxiv.org/pdf/2502.07869](https://arxiv.org/pdf/2502.07869)
+ **Bringing a Personal Point of View: Evaluating Dynamic 3D Gaussian Splatting for Egocentric Scene Reconstruction**
    - Publication: EgoVis@CVPR 2026
    - Highlights: Systematic benchmark of dynamic 3DGS on egocentric vs exocentric footage, confirms consistent quality degradation for wearable viewpoints
    - Paper Link: [https://arxiv.org/abs/2604.23803](https://arxiv.org/abs/2604.23803)
+ **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - Publication: SIGGRAPH 2026
    - Highlights: Differentiable forearm representation and unified arm-hand Transformer, MPJPE reduced by 28% on HOT3D across all lens types
    - Paper Link: [https://arxiv.org/abs/2605.12498](https://arxiv.org/abs/2605.12498)
+ **FunRec: Reconstructing Functional 3D Scenes from Egocentric Interaction Videos**
    - Publication: CVPR 2026
    - Highlights: Generates interactive household digital twins from RGB-D wearable clips, automatically detects articulated joints and kinematic parameters
    - Paper Link: [https://arxiv.org/abs/2604.05621](https://arxiv.org/abs/2604.05621)
+ **OmniEgoCap: Camera-Agnostic Sequence-Level Egocentric Motion Reconstruction**
    - Publication: arXiv 2026
    - Highlights: Diffusion-based reconstruction generalized across all wearable camera hardware, geometric visibility augmentation module
    - Paper Link: [https://arxiv.org/abs/2512.19283](https://arxiv.org/abs/2512.19283)
+ **Towards Learning a Generalizable 3D Scene Representation from 2D Observations**
    - Publication: ESANN 2026
    - Highlights: Generalized NeRF architecture predicting workspace occupancy from egocentric robot frames, reconstruction error ~26mm across 40 real scenes
    - Paper Link: [https://arxiv.org/abs/2602.10943](https://arxiv.org/abs/2602.10943)
+ **Ego-1K: A Large-Scale Multiview Video Dataset for Egocentric Vision**
    - Publication: CVPR 2026
    - Highlights: Nearly 1,000 multi-view egocentric clips captured by 12 synchronized cameras surrounding a 4-camera VR headset rig
    - Paper Link: [https://arxiv.org/abs/2603.13741](https://arxiv.org/abs/2603.13741)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| --- | --- | --- | --- | --- |
| ⭐ Ego-Exo4D | 2024 | 1,286+ hours paired ego/exo footage | Multi-view skill analysis, 3D reconstruction | [Official Website](https://ego-exo4d-data.org/) |
| ⭐ ADT (Aria Digital Twin) | 2023 | 200 multi-modal sequences, 2 indoor scenes | Egocentric 3D scene & body perception | [Official Website](https://www.projectaria.com/datasets/adt/) |
| PRISM | 2026 | 270K samples / 11.8M frames | Retail embodied VLM, spatial reasoning | [Hugging Face](https://huggingface.co/datasets/DreamVu/PRISM-100K) |
| EgoTraj | 2026 | 10.7 h / 1.15M frames | Egocentric camera trajectory forecasting | [GitHub](https://github.com/yehiahmad/EgoTraj) |
| AIST-Living | 2026 | Egocentric video + ground-truth 3D scene maps | Global camera localization, human pose tracking | [Official Website](https://deguchihiroyuki.github.io/Map-Mono-Ego-Project/) |
| OVO-S-Bench | 2026 | 348 videos / 1,680 spatial QA pairs | Streaming spatial embodied reasoning | [Official Website](https://internlm.github.io/OVO-S-Bench/) |
| PVSG | 2023 | 400 panoramic clips / ~150K frames | Egocentric panoramic scene graph construction | [GitHub](https://jingkang50.github.io/PVSG/) |
| DR(eye)VE | 2018 | ~6 h driving footage / 555K frames | Driver gaze prediction, automotive egocentric perception | [Official Website](http://aimagelab.ing.unimore.it/dreyeve) |
| EgoCart | 2018 | 9 retail RGB-D sequences | Indoor shopping cart localization | [Official Website](https://iplab.dmi.unict.it/EgocentricShoppingCartLocalization/) |
| IU ShareView | 2018 | 9 paired egocentric video sets | Cross-wearer instance segmentation & re-identification | [Official Website](http://vision.soic.indiana.edu/firstthird-eccv2018/) |
| OST | 2017 | 57 indoor sequences | Object search, wearable gaze tracking | [GitHub](https://github.com/Mengmi/deepfuturegaze_gan) |

---

### 2.7 Vision-Language-Action & Embodied AI (Ego-VLA)
> Align vision, language and action signals from human first-person footage, transfer human manipulation knowledge to robotic agents, core pipeline for embodied intelligence.
>
+ **EgoBridge: Domain Adaptation for Generalizable Imitation from Egocentric Human Videos**
    - Publication: NeurIPS 2025
    - Highlights: Optimal transport alignment between human visual-action distributions, imitation success rate improved by 44% over standard baselines
    - Paper Link: [https://arxiv.org/pdf/2509.19626](https://arxiv.org/pdf/2509.19626)
+ **EgoAgent: A Joint Predictive Agent Model in Egocentric Worlds**
    - Publication: ICCV 2025
    - Highlights: Unified Transformer architecture integrating egocentric vision, language, world modeling and action decision heads
    - Paper Link: [https://arxiv.org/abs/2502.05857](https://arxiv.org/abs/2502.05857)
+ **Ego-Pi: VLA Fine-Tuning for Egocentric Human and Robot Data**
    - Publication: arXiv 2026
    - Highlights: Targeted fine-tuning pipeline for dual-arm dexterous manipulation VLA models trained on wearable human footage
    - Paper Link: [https://arxiv.org/pdf/2606.08107](https://arxiv.org/pdf/2606.08107)
+ **ViterbiPlanNet: Injecting Procedural Knowledge via Differentiable Viterbi for Egocentric Task Planning**
    - Publication: CVPR 2026
    - Highlights: Differentiable Viterbi algorithm to inject step-by-step procedural priors into VLA planning modules
    - Paper Link: [https://arxiv.org/abs/2603.04265](https://arxiv.org/abs/2603.04265)
+ **Co-training with Ego-centric Video and Demonstration for Robot Navigation Task**
    - Publication: arXiv 2026
    - Highlights: Cross-domain co-training converting human egocentric walking footage into mobile robot imitation datasets
    - Paper Link: [https://arxiv.org/abs/2606.01951](https://arxiv.org/abs/2606.01951)
+ **OSCAR: Omni-Embodiment Skeleton-Conditioned World Action Model for Robotics**
    - Publication: arXiv 2026
    - Highlights: Universal skeleton-conditioned world-action model learning multi-robot policies from human first-person demonstrations
    - Paper Link: [https://arxiv.org/abs/2606.04463](https://arxiv.org/abs/2606.04463)

#### 📊 Related Datasets & Benchmarks (Procedural Skill Learning)
| Dataset Name | Year | Scale | Core Tasks | Link |
| --- | --- | --- | --- | --- |
| ⭐ EgoExoLearn | 2024 | 120 h asynchronous ego/exo paired clips | Human procedural learning simulation, robot imitation | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |
| ⭐ Assembly101 | 2022 | 513 h multi-view assembly footage | Step-wise industrial procedural manipulation | [Official Website](https://assembly-101.github.io/) |
| EgoVerse | 2026 | 1,362 h / ~80K task episodes | General robot manipulation pre-training, embodied benchmarking | [Official Website](https://egoverse.ai/) |
| EgoLive | 2026 | Large-scale real-world daily task recordings | Unstructured robotic skill transfer | [Paper](https://arxiv.org/abs/2604.23570) |
| EgoMAGIC | 2026 | 3,355 medical task videos / 50 clinical workflows | Surgical action detection & procedural assistance | [Zenodo](https://doi.org/10.5281/zenodo.19239154) |
| HumanEgo | 2026 | Short Aria wearable demonstration sequences | Human-to-robot policy distillation | [Official Website](https://humanego-ai.github.io/) |
| EgoSPT | 2026 | 11,515 operation episodes / 112 task folders | Spatial prompt-conditioned manipulation trajectory generation | [Hugging Face](https://huggingface.co/datasets/JackYFL233/EgoSPT) |
| Ego-EXTRA | 2026 | 50 h / 15K+ instructional VQA pairs | Expert-novice wearable assistance scenarios | [Official Website](https://fpv-iplab.github.io/Ego-EXTRA/) |
| GM-100 | 2026 | 100+ manipulation tasks / 13K trajectories | General robot skill evaluation benchmark | [Official Website](https://rhos.ai/research/gm-100) |
| SABER | 2026 | 100+ h / 44.8K retail samples | Embodied VLA domain adaptation for shopping robots | [Official Website](https://dreamvu.ai/saber/) |
| EgoProactive / Pro²Bench | 2026 | 700 wearable recordings / 42K evaluation samples | Proactive procedural wearable assistant benchmark | [Hugging Face](https://huggingface.co/datasets/facebook/wearable-ai) |
| EgoYC2 / Exo2EgoDVC | 2025 | ~43 h cooking footage with dense step captions | Household procedural alignment cross-view | [GitHub](https://github.com/ut-vision/Exo2EgoDVC) |
| IndustReal | 2024 | ~6 h factory operation sequences | Industrial step detection & error recognition | [Official Website](https://timschoonbeek.github.io/industreal.html) |
| EgoProceL | 2022 | 62 wearable videos / 16 household tasks | Daily procedural learning baseline | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| EPIC-Tent | 2019 | 7+ h dual HMD tent assembly footage + eye tracking | Multi-modal procedural activity analysis | [Data Repository](https://data.bris.ac.uk/data/dataset/2ite3tu1u53n42hjfh3886sa86) |
| CMU-MMAC | 2011 | 25 participants / 5 cooking recipes | Kitchen procedural activity recognition | [Official Website](http://kitchen.cs.cmu.edu/) |
| GTEA Gaze | 2011 | 17 cooking sessions | Fine-grained procedural action + gaze prediction | [Official Website](https://cbs.ic.gatech.edu/fpv/) |

---

### 2.8 Egocentric World Models
> Learn temporal evolution rules of environments from first-person observations, enabling future frame forecasting, synthetic interaction video generation, and long-horizon task planning.
>
+ **AnchorWorld: Embodied Egocentric World Simulation with View-based Evolution Customization**
    - Publication: arXiv 2026
    - Highlights: Anchor-keyframe constrained controllable egocentric simulator, anchor matching accuracy reaches 89%
    - Paper Link: [https://arxiv.org/abs/2606.07326](https://arxiv.org/abs/2606.07326)
+ **WEM: World-Ego Modeling for Long-Horizon Evolution in Hybrid Embodied Tasks**
    - Publication: arXiv 2026
    - Highlights: Disentangled static scene & dynamic self-branch world modeling architecture for long sequential forecasting
    - Paper Link: [https://arxiv.org/abs/2605.19957](https://arxiv.org/abs/2605.19957)
+ **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - Publication: ICLR 2026
    - Highlights: First benchmark quantifying embodied reasoning capability via egocentric world model simulation
    - Paper Link: [https://openreview.net/forum?id=Patx6MRipw](https://openreview.net/forum?id=Patx6MRipw)
+ **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - Publication: arXiv 2026
    - Highlights: Pioneering HOI-focused egocentric diffusion world model embedding physical interaction priors
    - Paper Link: [https://arxiv.org/abs/2603.13615](https://arxiv.org/abs/2603.13615)
+ **Walk through Paintings: Egocentric World Models from Internet Priors**
    - Publication: arXiv 2026
    - Highlights: Repurposes pre-trained video diffusion models into action-conditioned egocentric world models via web video priors
    - Paper Link: [https://arxiv.org/abs/2601.15284](https://arxiv.org/abs/2601.15284)
+ **EgoExo-WM: Unlocking Exo Video for Ego World Models**
    - Publication: arXiv 2026
    - Highlights: Cross-view knowledge transfer pipeline leveraging abundant third-person footage to augment egocentric world model training
    - Paper Link: [https://arxiv.org/pdf/2605.15477](https://arxiv.org/pdf/2605.15477)
+ **PlayerOne: Egocentric World Simulator**
    - Publication: NeurIPS 2025
    - Highlights: First photorealistic open-world egocentric simulator supporting unlimited free exploration and full motion control
    - Paper Link: [https://arxiv.org/abs/2506.09995](https://arxiv.org/abs/2506.09995)
+ **EgoSim: Egocentric World Simulator for Embodied Interaction Generation**
    - Publication: arXiv 2026
    - Highlights: Closed-loop interactive simulator with persistent dynamic 3D scene state updates for continuous synthetic video generation
    - Paper Link: [https://arxiv.org/abs/2604.01001](https://arxiv.org/abs/2604.01001)
+ **EgoForge: Goal-Directed Egocentric World Simulator**
    - Publication: arXiv 2026
    - Highlights: Target-conditioned generative simulator producing future egocentric sequences matching user-specified task objectives
    - Paper Link: [https://arxiv.org/abs/2603.20169](https://arxiv.org/abs/2603.20169)
+ **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - Publication: NeurIPS 2025
    - Highlights: Generalizable HOI world model with two-stage VLM prior inference + DiT flow matching trajectory generation
    - Paper Link: [https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)

#### 📊 Related Datasets & Benchmarks (World Model Pre-training & Video Generation)
| Dataset Name | Year | Scale | Core Tasks | Link |
| --- | --- | --- | --- | --- |
| ⭐ Ropedia Xperience-10M | 2026 | 10M multi-modal human experience clips | Large-scale egocentric world model pre-training | [Hugging Face](https://huggingface.co/datasets/ropedia-ai/xperience-10m) |
| DreamDojo-HV | 2026 | Massive first-person synthetic footage | Generative world model training | [Paper](https://arxiv.org/abs/2602.06949) |
| Ego-1K | 2026 | Multi-view egocentric video fragments | Neural 3D/4D dynamic scene synthesis | [Hugging Face](https://huggingface.co/datasets/facebook/ego-1k) |
| In-lab | 2026 | Desktop manipulation trajectory sequences | Small-scale skill world model fine-tuning | [Paper](https://arxiv.org/abs/2602.06949) |
| HumanNet | 2026 | ~1M hours human-centric video corpus | General VLA & world model pre-training | [Paper](https://arxiv.org/abs/2605.06747) |
| MobileEgo Anywhere | 2026 | 200 h smartphone egocentric daily footage | Lightweight long-form world model training | [Paper](https://arxiv.org/abs/2605.05945) |
| EgoEdit | 2025 | 100K egocentric video editing pairs | Conditional egocentric video generation benchmark | [Official Website](https://snap-research.github.io/EgoEdit) |
| EgoVid-5M | 2024 | 5M diverse first-person video clips | Foundation generative egocentric video dataset | [Official Website](https://egovid.github.io/) |

---

## 📊 Datasets, Benchmarks & Simulators
### General Large-Scale Egocentric Datasets
| Dataset Name | Release Year | Scale | Core Supported Tasks | Official Link |
| --- | --- | --- | --- | --- |
| Ego4D | 2022 | 3,670 hours wearable video, 923 participants across 9 countries | Action recognition, episodic memory, social interaction, 3D human pose | [Official Website](https://ego4d-data.org/) |
| EPIC-KITCHENS-100 | 2020 | 100 h kitchen footage, 90K annotated action segments | Action detection, recognition, future action forecasting | [Official Website](https://epic-kitchens.github.io/) |
| Ego-Exo4D | 2024 | 1,286 hours synchronized first/third-person multi-modal clips | Cross-view alignment, human skill analysis, 4D reconstruction | [Official Website](https://ego-exo4d-data.org/) |
| HD-EPIC | 2025 | 41 h ultra-high resolution cooking footage with dense multi-layer labels | Fine-grained activity understanding, dense VQA, multi-modal alignment | [Paper](https://arxiv.org/pdf/2502.04144) |

### Fine-Grained Task-Specific Datasets
#### EPIC-KITCHENS Object & HOI Sub-collections
+ **EgoObjects**
    - Release: Meta AI
    - Scale: 14K egocentric videos, 2M annotated frames, 900+ object categories
    - Core Task: First-person object detection, instance tracking
    - Link: [https://github.com/facebookresearch/EgoObjects](https://github.com/facebookresearch/EgoObjects)
+ **EgoXtreme**
    - Release: CVPR 2026
    - Scale: Challenging egocentric 6D pose dataset with motion blur, heavy occlusion and extreme lighting shifts
    - Core Task: Robust object 6D pose estimation for wearable cameras
    - Link: [https://arxiv.org/pdf/2603.25135](https://arxiv.org/pdf/2603.25135)
+ **EgoPressure**
    - Release: arXiv 2024
    - Scale: 5 h multi-modal footage with synchronized tactile pressure maps, IMU signals and RGB
    - Core Task: Tactile-aware hand-object interaction modeling
    - Link: [https://arxiv.org/pdf/2409.02224](https://arxiv.org/pdf/2409.02224)
+ **TouchMoment**
    - Release: CVPR 2026
    - Scale: 150K frames annotated with precise contact start/end timestamps & contact categories
    - Core Task: Fine-grained hand-object contact moment detection
    - Link: [https://arxiv.org/pdf/2604.12343](https://arxiv.org/pdf/2604.12343)

#### Long Video & Episodic Memory Datasets
+ **EgoSchema**
    - Release: NeurIPS 2023
    - Scale: 500+ long egocentric clips with multi-step temporal reasoning MCQs
    - Core Task: Ultra-long temporal video language understanding benchmark
    - Link: [https://github.com/egoschema/EgoSchema](https://github.com/egoschema/EgoSchema)
+ **EgoLife**
    - Release: CVPR 2025
    - Scale: Continuous multi-day footage from 6 co-living participants with dense daily event labels
    - Core Task: Long-term life-log memory retrieval & personal event QA
    - Link: [https://arxiv.org/pdf/2503.03803](https://arxiv.org/pdf/2503.03803)

#### Specialized Domain Datasets
+ **EgoExOR**
    - Release: NeurIPS 2025
    - Scale: Operating room wearable video synchronized with surgical tool tracking & patient biometrics
    - Core Task: Surgical workflow recognition, instrument detection
    - Link: [https://arxiv.org/pdf/2505.24287](https://arxiv.org/pdf/2505.24287)
+ **MECCANO**
    - Release: 2021
    - Scale: 12 h industrial assembly footage paired with eye-tracking streams
    - Core Task: Industrial fine-grained action & hand-object interaction analysis
    - Link: [https://github.com/fpv-iplab/MECCANO](https://github.com/fpv-iplab/MECCANO)
+ **EgoDex**
    - Release: 2025
    - Scale: Apple Vision Pro captured daily object manipulation sequences with precise 6D hand pose annotations
    - Core Task: Dexterous wearable hand pose estimation & manipulation forecasting
    - Link: [https://arxiv.org/abs/2505.11709](https://arxiv.org/abs/2505.11709)

### Embodied VLA Evaluation Benchmarks
+ **EgoVerse**
    - Release: 2026
    - Scale: 1,000+ standardized embodied tasks covering navigation, manipulation and visual QA
    - Core Task: Unified robotic imitation & wearable VLA evaluation suite
    - Link: [https://arxiv.org/pdf/2604.07607](https://arxiv.org/pdf/2604.07607)
+ **EgoBench**
    - Release: 2026
    - Scale: Interactive closed-loop evaluation platform for wearable embodied agents
    - Core Task: Real-time interactive decision-making benchmark
    - Link: [https://arxiv.org/pdf/2605.27820](https://arxiv.org/pdf/2605.27820)

### Egocentric World Simulators
+ **PlayerOne**
    - Release: NeurIPS 2025
    - Highlights: Photorealistic open-world egocentric simulator with full camera, human motion and object interaction control for synthetic data generation
    - Link: [https://arxiv.org/abs/2506.09995](https://arxiv.org/abs/2506.09995)
+ **EgoSim**
    - Release: arXiv 2026
    - Highlights: Closed-loop dynamic simulator maintaining persistent 3D scene states to generate consistent sequential interaction footage
    - Link: [https://arxiv.org/pdf/2604.01001](https://arxiv.org/pdf/2604.01001)

---

## 👓 Smart Glasses Exclusive Research & Deployment
### Specialized Benchmarks & Wearable Datasets
+ **SUPERGLASSES: Benchmarking Vision Language Models as Intelligent Agents for AI Smart Glasses**
    - Publication: CVPR 2026
    - Highlights: First real consumer smart glasses benchmark collected across Ray-Ban Meta, Xiaomi Smart Glasses and Thunderbird V3 with diverse daily scenarios
    - Paper Link: [https://arxiv.org/pdf/2602.22683](https://arxiv.org/pdf/2602.22683)
+ **Project Aria Datasets**
    - Publisher: Meta Research
    - Highlights: Full multi-modal wearable dataset suite with synchronized RGB, depth, IMU and eye-tracking signals
    - Official Link: [https://www.projectaria.com/](https://www.projectaria.com/)

### Key Technical Research Directions
#### Low-Power On-Device Perception
+ **EgoTrigger: Toward Audio-Driven Image Capture for Human Memory Enhancement in All-Day Energy-Efficient Smart Glasses**
    - Affiliation: UNC Chapel Hill + Google
    - Publication: IEEE TVCG 2025
    - Highlights: Audio-event triggered selective frame capture reducing total power consumption by 87%
    - Paper Link: [https://arxiv.org/pdf/2508.01915](https://arxiv.org/pdf/2508.01915)
+ **OpenGlass: Ultra-Low-Power On-Device AI Eyewear with Event-based Vision**
    - Publication: arXiv 2026
    - Highlights: Fully open-source event camera wearable hardware stack paired with lightweight edge inference algorithms
    - Paper Link: [https://arxiv.org/pdf/2606.07431](https://arxiv.org/pdf/2606.07431)

#### Lifelong Memory & Personal Assistant Systems
+ **EGAgent: Agentic Very Long Video Understanding**
    - Publication: arXiv 2026
    - Highlights: Entity scene graph based reasoning agent handling cross-day continuous wearable video streams with multi-hop retrieval
    - Paper Link: [https://arxiv.org/abs/2601.18157](https://arxiv.org/abs/2601.18157)

#### Natural Wearable Human-Computer Interaction
+ **Egocentric Co-Pilot: Web-Native Lightweight Smart Glasses Assistant**
    - Publication: WWW 2026
    - Highlights: Browser-based lightweight wearable assistant architecture without native app installation requirements
    - Paper Link: [https://arxiv.org/pdf/2603.01104](https://arxiv.org/pdf/2603.01104)
+ **Plug-and-Play Clarifier: A Zero-Shot Multimodal Framework for Egocentric Intent Disambiguation**
    - Publication: AAAI 2026
    - Highlights: Zero-shot intent resolution framework boosting wearable instruction execution accuracy from 58% to 87%
    - Paper Link: [https://arxiv.org/pdf/2511.08971](https://arxiv.org/pdf/2511.08971)
+ **VisionClaw: Always-On AI Agents Through Smart Glasses**
    - Publication: arXiv 2026
    - Highlights: Persistent background wearable agent enabling touch-free multi-scenario task execution
    - Paper Link: [https://arxiv.org/pdf/2604.03486](https://arxiv.org/pdf/2604.03486)

---

## 🔗 Related Awesome Resource Lists
+ [Awesome-Egocentric](https://github.com/EgoAlpha/Awesome-Egocentric)
+ [awesome-egocentric-vision](https://github.com/Sid2697/awesome-egocentric-vision)
+ [Awesome-Egocentric-and-Exocentric-Vision](https://github.com/ayiyayi/Awesome-Egocentric-and-Exocentric-Vision)
+ [Awesome-Egocentric-Video-Datasets](https://github.com/player0718/awesome-ego-video-datasets)

---

## 🎯 Key Research Challenges
### Universal Foundational Challenges Across All Subtasks
1. **Intrinsic Egocentric Visual Defects**: Narrow field-of-view, severe self-occlusion, violent camera jitter, unstable lighting and blurry wearable imagery degrade all downstream tasks.
2. **Egocentric Data Scarcity & Privacy Barriers**: Wearable footage carries sensitive personal information; collection and annotation costs are drastically higher than internet third-person video, creating an order-of-magnitude dataset size gap limiting large model scaling.
3. **Severe Inter-Person Distribution Shift**: Large variance in user height, daily behavior patterns, household environments leads to poor generalization of generic models on personalized wearable scenarios.
4. **Ultra-Long Sequential Modeling Bottlenecks**: Continuous all-day wearable streaming poses critical memory capacity and long-range dependency modeling challenges for existing video and multimodal architectures.

### Domain-Specific Core Challenges
| Research Direction | Core Open Challenges |
| --- | --- |
| Action Recognition & Anticipation | Fine-grained verb-noun compositional ambiguity, low temporal localization precision on untrimmed long footage |
| Hand-Object Interaction (HOI) | High annotation cost for contact states, physical consistency constraints hard to model, heavy mutual occlusion between hands and objects |
| Ego-VLM Multimodal Reasoning | Lack of first-person commonsense priors, weak spatio-temporal multi-step reasoning, ambiguous natural language object reference grounding |
| Long-Form Video Memory QA | Limited model context windows, fuzzy temporal event localization, weak causal reasoning across multi-hour footage |
| Gaze & User Intention Prediction | High inter-individual variance in eye movement patterns, implicit human intent difficult to label, weak multi-modal signal alignment |
| 3D/4D Spatial Reconstruction | Monocular depth ambiguity, dynamic moving object reconstruction failure, heavy fisheye lens distortion correction overhead |
| Ego-VLA Embodied Imitation | Large human-robot embodiment domain gap, misaligned action spaces, insufficient physical interaction world knowledge |
| Egocentric World Models | Temporal consistency degradation over long rollouts, trade-off between generation realism and physical plausibility, weak user action controllability |

---

## ❤️ Contact
If you have paper/dataset suggestions, corrections or find this resource list useful, feel free to reach Yuanliang Sun via email: sun254667307@gmail.com.

## ⭐ Acknowledgements
This curated collection cross-references and builds upon multiple community egocentric vision repositories:
+ [Awesome-Egocentric-Video-Datasets](https://github.com/player0718/awesome-ego-video-datasets)

## License
CC0 1.0 Universal. Full terms available in the `LICENSE` file of this repository.
