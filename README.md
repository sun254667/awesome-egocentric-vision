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

> A curated, learning-friendly list of egocentric (first-person) vision & embodied AI resources: papers, datasets, code, models, toolkits, challenges and tutorials, covering both classic foundational works and cutting-edge advances, catering to research initiation and industrial deployment.
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
    - 2.3 Egocentric Vision-Language Models & Multimodal Reasoning
    - 2.4 Long-form Video Understanding & Structured Reasoning
    - 2.5 Gaze, Attention & Intention Prediction
    - 2.6 3D/4D Reconstruction & Structured Perception
    - 2.7 Embodied AI & Vision-Language-Action (Ego-VLA)
    - 2.8 Egocentric World Models
    - 2.9 Egocentric Procedural AI Assistant
    - 2.10 Egocentric Data Security & Privacy Protection
3. [📊 Datasets, Benchmarks & Simulators](#-datasets-benchmarks--simulators)
4. [👓 Smart Glasses Exclusive Research & Deployment](#-smart-glasses-exclusive-research--deployment)
5. [🔗 Related Awesome Lists](#-related-awesome-lists)
6. [🎯 Key Research Challenges](#-key-research-challenges)

---

## 📚 Surveys & Overviews
The preferred materials for getting started in the field, helping to quickly establish a global understanding, sort out the development context, core tasks and key challenges.

+  **Challenges and Trends in Egocentric Vision: A Survey**
    - Publication: arXiv 2025 (v1: Mar 2025, v2: Apr 2025)
    - Highlights: The latest panoramic survey of the field, systematically classifying four major task directions: subject understanding, object understanding, environment understanding, and hybrid understanding, comprehensively summarizing challenges and trends
    - Paper Link: [arXiv](https://arxiv.org/abs/2503.15275)
+  **Building Egocentric Procedural AI Assistant: Methods, Benchmarks, and Challenges**
    - Publication: arXiv 2025
    - Highlights: For the first time, systematically proposes a complete technical framework for first-person procedural AI assistants, defining three core tasks: error detection, procedural learning, and visual question answering, as well as two supporting dimensions: real-time stream processing and active interaction
    - Paper Link: [arXiv](https://arxiv.org/abs/2511.13261)
+  **Bridging Perspectives: A Survey on Cross-view Collaborative Intelligence with Egocentric-Exocentric Vision**
    - Publication: arXiv 2025
    - Highlights: Systematically sorts out the direction of egocentric-exocentric collaborative learning, covering three paradigms: exocentric-assisted egocentric, egocentric-assisted exocentric, and joint learning
    - Paper Link: [arXiv](https://arxiv.org/abs/2506.06253)
+ **An Outlook into the Future of Egocentric Vision**
    - Publication: IJCV 2024
    - Highlights: Co-authored by authoritative scholars in the field, combined with future scenarios of wearable computing, sorting out research shortcomings and directions to be broken through
    - Paper Link: [arXiv](https://arxiv.org/abs/2308.07123)
+ **First-Person Vision**
    - Publication: Proceedings of the IEEE 2012
    - Highlights: A foundational survey in the field, formally defining the research scope, core challenges and application directions of first-person vision for the first time
    - Paper Link: [IEEE Xplore](https://ieeexplore.ieee.org/document/6232429)

---

## 🔬 Core Research Topics

### 2.1 Action Recognition, Detection & Anticipation
The most fundamental and mature direction of egocentric vision, studying the recognition, detection and prediction of human actions from a first-person perspective.

#### Action Recognition & Detection
+  **Divide, Deliberate, Decide: A Multi-Agent Framework for Fine-Grained Egocentric Action Recognition**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: A fully-local, zero-shot multi-agent framework where VLM specialists engage in structured deliberation with peer consultation, improving zero-shot action recognition performance
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.17627)
+  **From Frames to Temporal Graphs: In-Context Egocentric Action Recognition with Vision-Language Models**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Proposes converting videos into Temporal Action Graphs with a multi-stage prompting pipeline, enabling efficient in-context few-shot learning across 11 open-weight VLMs from 2B to 235B parameters
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.15417)
+  **Cross-Modal Action Recognition in Egocentric Video Using Mamba: Integrating RGB and Hand Skeleton Streams via CLS Token Fusion Strategies**
    - Publication: EgoVis@CVPR 2026 (arXiv May 2026)
    - Highlights: A cross-modal architecture based on the Mamba framework, fusing RGB video and temporal hand skeleton data, and proposes four CLS token fusion strategies
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.24302)
+  **EgoAction: Egocentric Action Composition with Reliability-Aware Temporal Fusion**
    - Publication: CVPR 2026 (EPIC-KITCHENS Challenge Champion Solution)
    - Highlights: Proposes a decoupled verb-noun detection + dynamic weighted fusion strategy, achieving SOTA accuracy on long untrimmed videos based on VideoMAE-L features
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.24496)
+  **ENIGMA-360: An Ego-Exo Dataset for Human Behavior Understanding in Industrial Scenarios**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Provides baseline experiments for three foundational tasks: Temporal Action Segmentation, Keystep Recognition, and Egocentric Human-Object Interaction Detection
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.14327)
+  **Ego4OOD: Rethinking Egocentric Video Domain Generalization via Covariate Shift Scoring**
    - Publication: arXiv 2026 (Jan 2026)
    - Highlights: Proposes the Ego4OOD domain generalization benchmark, containing 8 geographically distinct domains, and introduces a clustering-based covariate shift metric
    - Paper Link: [arXiv](https://arxiv.org/abs/2601.17056)
+  **Continual Multimodal Egocentric Activity Recognition via Modality-Aware Novelty Detection**
    - Publication: arXiv 2026
    - Highlights: Proposes the MAND modality-aware framework, improving the AUC of novel activity detection by 10%
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.16970)
+  **Ego-METAS: Egocentric online Multimodal Energy-efficient Temporal Action Segmentation benchmark**
    - Publication: arXiv 2026
    - Highlights: The first online multimodal temporal action segmentation benchmark for energy awareness, containing 100+ hours of untrimmed videos covering 5 modalities
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.02246)
+  **MM-CDFSL: Multimodal Cross-Domain Few-Shot Learning for Egocentric Action Recognition**
    - Publication: ECCV 2024
    - Highlights: Systematically studies the cross-domain few-shot scenario of egocentric action recognition for the first time, proposing a multimodal distillation framework
    - Paper Link: [arXiv](https://arxiv.org/abs/2405.19917)
+ **Ego-Only: Egocentric Action Detection without Exocentric Transferring**
    - Publication: ICCV 2023
    - Highlights: Proves for the first time that models trained with pure first-person data can outperform methods relying on third-person transfer
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/ICCV2023/html/Wang_Ego-Only_Egocentric_Action_Detection_without_Exocentric_Transferring_ICCV_2023_paper.html)

#### Action Anticipation
+  **INSIGHT: Intention-Guided Cognitive Reasoning for Egocentric Long-Term Action Anticipation**
    - Publication: AAAI 2026
    - Highlights: Proposes a two-stage framework of "HOI semantic recognition + intention reasoning" for long-term action anticipation
    - Paper Link: [arXiv](https://arxiv.org/abs/2508.01742)
+  **PALM: Predicting Actions through Language Models**
    - Publication: arXiv 2023
    - Highlights: Introduces large language models into long-term temporal action anticipation for the first time
    - Paper Link: [arXiv](https://arxiv.org/abs/2311.17944)
+  **GANO: Gaze-Augmented Next Active Object-Based Egocentric Action Anticipation**
    - Publication: arXiv 2023
    - Highlights: Aims at the next active object prediction task, proposing a gaze-guided attention mechanism
    - Paper Link: [arXiv](https://arxiv.org/abs/2305.12953)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
| EgoScale | 2026 | 20k+ h labeled manipulation | Action Recognition, Dexterous Transfer | [arXiv](https://arxiv.org/abs/2602.16710) |
| Ego-METAS | 2026 | 100+ h / 5 modalities | Online Action Segmentation, Sensor Routing | [Hugging Face](https://huggingface.co/datasets/Ego-METAS/Ego-METAS) |
| ChildLens | 2026 | 108.58 h / 354 videos | Children's daily activity analysis | [Data](https://doi.org/10.17617/4.fe) |
| CogDrive (EyeCue) | 2026 | Multi-scenario driving | Driver cognitive distraction detection | [arXiv](https://arxiv.org/abs/2605.07859) |
| Furhat Egocentric Dataset | 2026 | 20 seq. / ~25 min | Robot-ego face/body tracking | [arXiv](https://arxiv.org/abs/2606.03694) |
| World In Your Hands | 2025 | 1000+ h labeled manipulation | Action Recognition, VLA Training | [GitHub](https://github.com/tars-robotics/World-In-Your-Hands) |
| EgoCampus | 2025 | ~32 h | Gaze, Pedestrian Egocentric | [GitHub](https://github.com/ComputerVisionRutgers/EgoCampus) |
| AEA | 2024 | 143 seq. / ~7.3 h | Daily Activities (Aria) | [Project Aria](https://www.projectaria.com/datasets/aea/) |
| EgoSurgery | 2024 | Open surgery videos | Surgical phase, Tool detection | [GitHub](https://github.com/Fujiry0/EgoSurgery) |
| EgoExo-Fitness | 2024 | 32 h / 1,276 seq. | Full-body motion, Quality assessment | [GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness) |
| E³ (Exploring Embodied Emotion) | 2024 | 50+ h | Emotion Recognition, Multimodal | [GitHub](https://github.com/Exploring-Embodied-Emotion-official/E3) |
| ⭐ Ego4D | 2022 | ~3,670 h | Action Recognition, VQA, Anticipation, etc. | [Official Website](https://ego4d-data.org/) |
| ⭐ EPIC-KITCHENS-100 | 2021 | 100 h / 90K segments | Action Recognition, Detection, Anticipation | [Official Website](https://epic-kitchens.github.io/) |
| EGOFALLS | 2023 | Fall samples | Fall Detection | [Dataverse](https://www.dataverse.nl/dataset.xhtml?persistentId=doi:10.34894/HO5GE3) |
| Epic-Sounding-Object | 2023 | 3.2K short clips | Audio-visual object localization | [GitHub](https://github.com/WikiChao/Ego-AV-Loc) |
| HoloAssist | 2023 | 169 h | Interactive Assistant | [Official Website](https://holoassist.github.io/) |
| WEAR | 2023 | ~19 h outdoor sports | Activity + IMU | [Official Website](https://mariusbock.github.io/wear/) |
| N-EPIC-KITCHENS | 2022 | Event + RGB subset | Neuromorphic Action Recognition | [GitHub](https://github.com/EgocentricVision/N-EPIC-Kitchens) |
| Ego-Deliver | 2021 | 5,360 videos | Delivery Behavior Analysis | [Official Website](https://egodeliver.github.io/) |
| HOMAGE | 2021 | 30 h | Home activity compositional understanding | [GitHub](https://github.com/nishantrai18/homage) |
| MECCANO | 2021 | ~55 h industrial | Hand-object interaction, Industrial | [Official Website](https://iplab.dmi.unict.it/MECCANO/) |
| EGO-CH | 2020 | 27+ h | Tourist behavior, POI tasks | [arXiv](https://arxiv.org/abs/2002.00899) |
| EgoCom | 2020 | 38.5 h conversation | Multi-person egocentric dialogue | [GitHub](https://github.com/facebookresearch/EgoCom-Dataset) |
| LEMMA | 2020 | Multi-view activities | Multi-agent tasks | [GitHub](https://github.com/Buzz-Beater/LEMMA) |
| Charades-Ego | 2018 | Paired ego/exo | Alignment, Action | [Official Website](https://prior.allenai.org/projects/charades-ego) |
| EGTEA Gaze+ | 2018 | 28 h cooking | Gaze + Action Recognition | [Official Website](https://cbs.ic.gatech.edu/fpv/) |
| EgoGesture | 2017 | 2K+ videos / 24K samples | Gesture Recognition | [Official Website](https://nlpr.ia.ac.cn/iva/yfzhang/datasets/egogesture.html) |
| Stanford ECM | 2017 | 31 h | Daily activity classification | [CVF](https://openaccess.thecvf.com/content_cvpr_2017/html/Nakamura_Jointly_Learning_Energy_CVPR_2017_paper.html) |
| THU-READ | 2017 | 1,920 clips | Helmet RGB-D action | [Official Website](https://ivg.au.tsinghua.edu.cn/dataset/THU_READ.php) |
| PEV | 2016 | 1,226 pairs | Two-person dialogue micro-actions | [CVF](https://openaccess.thecvf.com/content_cvpr_2016/html/Yonetani_Recognizing_Micro-Actions_and_CVPR_2016_paper.html) |
| FPPA | 2015 | 5 subjects | Daily action + hand/gaze | [CVF](https://openaccess.thecvf.com/content_iccv_2015/html/Zhou_Temporal_Perception_and_ICCV_2015_paper.html) |
| JPL-Interaction | 2013 | 84 videos | First-person activity recognition | [Official Website](http://michaelryoo.com/jpl-interaction.html) |
| ADL | 2012 | ~10 h | Daily activity recognition | [Official Website](https://www.csee.umbc.edu/~hpirsiav/papers/ADLdataset/) |
| Social Interactions | 2012 | ~60 h | Social Activities | [Official Website](https://cbs.ic.gatech.edu/fpv/) |
| EgoAction (Sports) | 2011 | First-person sports videos | Action Recognition | [IEEE](https://doi.org/10.1109/CVPR.2011.5995406) |

---

### 2.2 Hand-Object Interaction & Fine-grained Activity
Studies the interaction process between hands and objects from a first-person perspective, which is the core foundation of embodied intelligence and robot imitation learning.

+  **Hand-4DGS: Feed-Forward 3D Gaussian Splatting for 4D Hand Reconstruction from Egocentric Videos**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Dynamic 3D hand reconstruction from egocentric videos essential for AR/VR and AI glasses, addressing fast head motion, rapid hand dynamics, severe occlusions, and single-view ambiguity
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.16930)
+  **Hand Trajectory Fusion for Egocentric Natural Language Query Grounding**
    - Publication: EgoVis@CVPR 2026 (arXiv Jun 2026)
    - Highlights: Integrates hand motion cues into the NLQ grounding task for the first time, improving R@1, IoU=0.3 by 2.54% for hand-object interaction queries
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.02962)
+  **Wh0: Generative World Models as Scalable Sources of Egocentric Human Hand Manipulation Data**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Uses generative video world models as scalable and controllable sources of egocentric human-hand manipulation data to unlock manipulation capabilities of pretrained dexterous VLA models
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.22136)
+  **TouchAnything: A Dataset and Framework for Bimanual Tactile Estimation from Egocentric Video**
    - Publication: arXiv 2026 (May 2026)
    - Highlights: Introduces EgoTouch, a large-scale multi-view egocentric dataset with dense tactile supervision for bimanual hand-object interaction, comprising 208 manipulation tasks spanning 1,891 episodes
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.13083)
+  **IMPACT-HOI: Supervisory Control for Onset-Anchored Partial HOI Event Construction**
    - Publication: arXiv 2026 (May 2026)
    - Highlights: A mixed-initiative framework for annotating egocentric procedural video by constructing structured event graphs for Human-Object Interactions, motivated by learning robot manipulation from human demonstration
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.17639)
+  **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - Publication: SIGGRAPH 2026 (arXiv May 2026)
    - Highlights: Differentiable forearm representation + unified arm-hand Transformer. MPJPE reduced by 28% on HOT3D across all lens types
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.12498)
+  **EgoGrasp: World-Space Hand-Object Interaction Estimation from Egocentric Videos**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: The first method to reconstruct world-space hand-object interactions (W-HOI) from dynamic egoview videos, supporting open-vocabulary objects
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.12255)
+  **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: The first egocentric HOI world model, embedding physical priors into generative diffusion models, distilling geometric and kinematic priors from 3D estimates into physics-informed embeddings
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.13615)
+  **Glove2Hand: Synthesizing Natural Hand-Object Interaction from Multi-Modal Sensing Gloves**
    - Publication: CVPR 2026 (Highlight)
    - Highlights: Generates realistic bare-hand HOI videos from multi-modal sensing glove data, accompanied by the HandSense dataset
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.20850)
+  **TOUCH: Text-Guided Controllable Generation of Free-Form Hand-Object Interactions**
    - Publication: ICLR 2026
    - Highlights: Proposes the free-form HOI generation task, constructing the large-scale WildO2 3D HOI dataset
    - Paper Link: [OpenReview](https://openreview.net/forum?id=4VW9HVCRw0)
+  **Leveraging Synthetic Data for Enhancing Egocentric Hand-Object Interaction Detection**
    - Publication: IJCV 2026, Vol.134
    - Highlights: Using only a small amount of real annotated data combined with synthetic data, AP is improved by 11.69% on VISOR, and the HOI-Synth synthetic data generation pipeline is open-sourced
    - Paper Link: [Springer](https://link.springer.com/article/10.1007/s11263-026-02838-8)
+  **ECHO: Ego-Centric modeling of Human-Object interactions**
    - Publication: arXiv 2025 (v1: Aug 2025, v2: Mar 2026)
    - Highlights: The first unified framework to jointly recover human pose, object motion, and contact dynamics solely from head and wrist tracking, using a novel tri-variate diffusion process with independent noise schedules
    - Paper Link: [arXiv](https://arxiv.org/abs/2508.21556)
+  **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - Publication: NeurIPS 2025
    - Highlights: Proposes a two-layer architecture framework, using VLM to infer motion priors at the high level, and generating fine-grained trajectories based on DiT flow matching at the low level
    - Paper Link: [NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)
+  **EgoAERO: Learning Dexterous Manipulation from a Single Egocentric Video without Object Assets**
    - Publication: arXiv 2026
    - Highlights: A dexterous manipulation learning framework without pre-scanned object assets, constructing the large-scale EgoDex-R dataset (4.3M RGB-D frames)
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.08057)
+  **EgoInteract: Synthetic Egocentric Videos Generation for Interaction Understanding and Anticipation**
    - Publication: arXiv 2026
    - Highlights: A controllable egocentric video generation simulator, achieving precise control over cameras, human actions and object manipulations
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.18214)
+  **EgoHandICL: Egocentric 3D Hand Reconstruction with In-Context Learning**
    - Publication: arXiv 2026 (Jan 2026)
    - Highlights: Robust 3D hand reconstruction in egocentric vision addressing depth ambiguity, self-occlusion, and complex hand-object interactions; improves EgoVLM hand-object interaction reasoning
    - Paper Link: [arXiv](https://arxiv.org/abs/2601.09806)
+  **Do Egocentric Video-Language Models Truly Understand Hand-Object Interactions?**
    - Publication: ICLR 2025
    - Highlights: Systematically evaluates the fine-grained HOI understanding ability of egocentric VLMs for the first time, proposing the EgoHOIBench benchmark
    - Paper Link: [arXiv](https://arxiv.org/abs/2405.17719)
+  **HOI-Ref: Hand-Object Interaction Referral in Egocentric Vision**
    - Publication: arXiv 2024
    - Highlights: Defines a new task of HOI referral in egocentric scenarios, accompanied by the HOI-QA evaluation benchmark
    - Paper Link: [arXiv](https://arxiv.org/abs/2404.09933)
+  **Get a Grip: Reconstructing Hand-Object Stable Grasps in Egocentric Videos**
    - Publication: arXiv 2023
    - Highlights: Reconstructs stable hand-object grasping states from monocular egocentric videos for the first time
    - Paper Link: [arXiv](https://arxiv.org/abs/2312.15719)
+ **EgoPCA: A New Framework for Egocentric Hand-Object Interaction Understanding**
    - Publication: ICCV 2023
    - Highlights: Proposes a new framework as an infrastructure to advance Ego-HOI recognition by Probing, Curation and Adaption (EgoPCA)
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/ICCV2023/html/EgoPCA_A_New_Framework_for_Egocentric_Hand-Object_Interaction_Understanding_ICCV_2023_paper.html)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
| ⭐ EgoDex | 2025 | 829 h / 30K trajectories | Dexterous manipulation, Hand pose | [GitHub](https://github.com/apple/ml-egodex) |
| EgoDex-R | 2026 | 4.3M RGB-D frames / 5.6K seq. | Dexterous manipulation, Hand-object pose | [arXiv](https://arxiv.org/abs/2606.08057) |
| EgoTouch | 2026 | 1,891 episodes / 208 tasks | Tactile HOI | [Hugging Face](https://huggingface.co/datasets/zhenyuxie-zhzh/EgoTouch_hdf5) |
| EgoTactile | 2026 | ~6 h / 768 clips | Grasp pressure estimation | [Official Website](https://egotactile.github.io/) |
| EventEgoHands | 2026 | 48 clips / 129.6K frames | RGB+event hand detection | [GitHub](https://github.com/SynthSyntax/EventEgoHands) |
| HA-Ego-1K | 2026 | ~24 h / 484 multi-view clips | Dexterous manipulation | [Hugging Face](https://huggingface.co/datasets/humanarchive/HA-Ego-1K) |
| DexGloveHOI | 2026 | 3.5 h / 100K+ samples | Visual-IMU 3D hand tracking | [arXiv](https://arxiv.org/abs/2605.21714) |
| EgoEVHands | 2026 | 5,419 annotated seq. | Stereo event 3D hand pose | [GitHub](https://github.com/ZJUWang01/EgoEV-HandPose) |
| EgoEMG | 2026 | 41 participants / 10+ h | EMG+visual hand pose | [GitHub](https://github.com/zhenqis123/EgoEMG) |
| HRDexDB | 2026 | 1.4K grasping trials | Dexterous grasping, Tactile | [Hugging Face](https://huggingface.co/datasets/hahahataeyun/hrdexdb) |
| TouchMoment | 2026 | 4,021 videos / 8,456 touch moments | Contact moment detection | [arXiv](https://arxiv.org/abs/2604.12343) |
| EgoFun3D | 2026 | 271 egocentric videos | Interactive 3D objects | [Official Website](https://3dlg-hcvc.github.io/EgoFun3D/) |
| SHOW3D | 2026 | In-the-wild ego-exo HOI | 3D hand-object annotation | [arXiv](https://arxiv.org/abs/2603.28760) |
| FEEL | 2026 | Force-synchronized kitchen videos | Physical action understanding | [Official Website](https://www.cs.umd.edu/~edessale/feel) |
| EgoPoints | 2025 | Point trajectories + synthetic | Egocentric video tracking | [GitHub](https://github.com/AhmadDarKhalil/EgoPoints) |
| ⭐ HOI4D | 2022 | 2.4M frames / 4K seq. | 4D HOI | [Official Website](https://hoi4d.github.io/) |
| AssemblyHands | 2023 | 3M images | 3D hand pose | [Official Website](https://assemblyhands.github.io/) |
| EgoObjects | 2023 | 9.2K+ videos | Detection, Instance segmentation | [GitHub](https://github.com/facebookresearch/EgoObjects) |
| ENIGMA-51 | 2023 | 22 h industrial | Fine-grained behavior | [Official Website](https://fpv-iplab.github.io/ENIGMA-51/) |
| POV-Surgery | 2023 | ~88K frames (synthetic) | Surgical hand-tool pose | [Official Website](https://batfacewayne.github.io/POV_Surgery_io/) |
| VOST | 2023 | 713 videos | Video object segmentation | [Official Website](https://www.vostdataset.org/) |
| EgoBody | 2022 | 125 seq. | Body pose, Interaction | [Official Website](https://egobody.ethz.ch/) |
| EgoHOS | 2022 | 11K+ images | Hand-object segmentation | [GitHub](https://github.com/owenzlz/EgoHOS) |
| EgoPAT3D | 2022 | 1M+ frames RGB-D | 3D action target prediction | [GitHub](https://github.com/ai4ce/EgoPAT3D) |
| Touch and Go | 2022 | 12K+ vis–tactile frames | Vision + Tactile | [Official Website](https://touch-and-go.github.io/) |
| VISOR | 2022 | EPIC + masks | Segmentation, HOI | [Official Website](https://epic-kitchens.github.io/VISOR/) |
| H2O | 2021 | 100K+ frames | Two-hand interaction | [Official Website](https://h2odataset.ethz.ch/) |
| TREK-150 | 2021 | 150 EPIC seq. | Object tracking | [Official Website](https://machinelearning.uniud.it/datasets/trek150/) |
| You2Me | 2020 | 14 seq. | Body pose inference via ego-exo | [GitHub](https://github.com/facebookresearch/you2me) |
| FPHA | 2018 | 1.2K seq. | Hand pose + Action | [Official Website](https://guiggh.github.io/publications/first-person-hands/) |
| EgoDexter | 2017 | ~3.2K frames | Hand tracking under occlusion | [Official Website](https://handtracker.mpi-inf.mpg.de/projects/OccludedHands/EgoDexter.htm) |
| EgoHands | 2015 | 4.8K labeled frames | Hand detection | [Official Website](http://vision.soic.indiana.edu/projects/egohands/) |
| BEOID | 2014 | 58 videos | Hand-object interaction | [Official Website](https://data.bris.ac.uk/data/dataset/3wats8ruq1sp52hq3bo8dkzul3) |
| EDSH | 2013 | 2 videos | Pixel-level hand segmentation | [Official Website](http://www.cs.cmu.edu/~kkitani/datasets/) |
| Handled Objects | 2009 | 11 categories | Grasp sequences | [IEEE](https://doi.org/10.1109/CVPRW.2009.5204360) |

---

### 2.3 Egocentric Vision-Language Models & Multimodal Reasoning
Combines large language models with first-person vision to achieve advanced cognitive capabilities such as video question answering, content description and reasoning. This section also covers multimodal fusion approaches that combine RGB, depth, IMU, audio, and gaze signals for joint learning.

#### Pre-trained Foundation Models
+  **EgoM2P: Egocentric Multimodal Multitask Pretraining**
    - Publication: ICCV 2025
    - Highlights: A unified design supporting multitasking across diverse egocentric perception and synthesis tasks, including gaze prediction, egocentric camera tracking, and monocular depth estimation, and also serves as a generative model for conditional egocentric video synthesis
    - Paper Link: [ICCV](https://openaccess.thecvf.com/content/ICCV2025/html/EgoM2P_Egocentric_Multimodal_Multitask_Pretraining_ICCV_2025_paper.html)
+  **EgoAdapt: Adaptive Multisensory Distillation and Policy Learning for Efficient Egocentric Perception**
    - Publication: ICCV 2025
    - Highlights: A framework that adaptively performs cross-modal distillation and policy learning to enable efficient inference across different egocentric perception tasks, including egocentric action recognition, active speaker localization, and behavior anticipation. Reduces GMACs by up to 89.09%, parameters up to 82.02%, and energy up to 9.6x
    - Paper Link: [ICCV](https://www.openaccess.thecvf.com/content/ICCV2025/html/Chowdhury_EgoAdapt_Adaptive_Multisensory_Distillation_and_Policy_Learning_for_Efficient_Egocentric_ICCV_2025_paper.html) | [arXiv](http://arxiv.org/abs/2506.21080)
+ **EgoVLPv2: Egocentric Video-Language Pre-training with Fusion in the Backbone**
    - Publication: ICCV 2023
    - Highlights: Improved VLP with backbone-level fusion architecture
    - Paper Link: [arXiv](https://arxiv.org/abs/2307.05463)
+ **Egocentric Video-Language Pretraining (EgoVLP)**
    - Publication: CVPR 2022
    - Highlights: The first video-language pre-training framework specifically designed for egocentric scenarios
    - Paper Link: [arXiv](https://arxiv.org/abs/2206.01670)

#### Advanced Reasoning & Cutting-edge Advances
+  **EgoSAT: A Comprehensive Benchmark of Egocentric Streaming Interaction Understanding**
    - Publication: ECCV 2026 (arXiv Jun 2026)
    - Highlights: The first comprehensive benchmark for egocentric video reasoning in streaming settings, designed to evaluate VLMs on streaming interaction understanding. Contains 1,997 unique videos spanning 165 hours and ~4,800 QA pairs
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.24422)
+  **PROSE: Training-Free Egocentric Scene Registration with Vision-Language Models**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Uses a pretrained VLM as the source of both scene understanding and cross-scan matching for egocentric scene registration, outperforming geometric and learned scene-graph baselines
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.16569)
+  **Decoding Pedestrian Crossing Intention from Egocentric Vision via Vision Language Models**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Uses VLM to decode pedestrian crossing intention for the first time, with accuracy improved by 14.5% after fusing eye movement and ego-motion
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.09142)
+  **The Right Inference Strategy Is All You Need: Nearly Training-Free Domain-Wise Inference for EgoCross Challenge**
    - Publication: arXiv 2026 (May 2026)
    - Highlights: EgoCross Challenge solution, domain-aware inference strategy achieves 66.98% accuracy with only 20 training samples
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.00829)
+  **Spatial Reasoning with Vision-Language Models in Ego-Centric Multi-View Scenes**
    - Publication: ICLR 2026 (Apr 2026)
    - Highlights: Proposes the Ego3D-Bench spatial reasoning benchmark (8,600+ QA pairs), and the Ego3D-VLM post-training framework
    - Paper Link: [OpenReview](https://openreview.net/forum?id=10008200)
+  **EgoMotion: Hierarchical Reasoning and Diffusion for Egocentric Vision-Language Motion Generation**
    - Publication: arXiv 2026 (Apr 2026)
    - Highlights: Proposes a hierarchical reasoning and diffusion framework to generate language-described 3D human motion from first-person videos
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.19105)
+  **Exo2Ego: Exocentric Knowledge Guided Multimodal LLMs for Egocentric Video Understanding**
    - Publication: AAAI 2026 (Feb 2026)
    - Highlights: Constructs the Ego-ExoClip pre-training dataset (1.1 million synchronized egocentric-exocentric clip-text pairs), proposing a three-stage progressive mapping learning pipeline
    - Paper Link: [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/38244)
+  **Egocentric Bias in Vision-Language Models**
    - Publication: arXiv 2026 (Feb 2026)
    - Highlights: Introduces FlipSet, a diagnostic benchmark for Level-2 visual perspective taking in VLMs. Evaluating 103 VLMs reveals systematic egocentric bias: the vast majority perform below chance
    - Paper Link: [arXiv](https://arxiv.org/abs/2602.03953)
+  **Allocentric Perceiver: Disentangling Allocentric Reasoning from Egocentric Visual Priors via Frame Instantiation**
    - Publication: arXiv 2026 (Feb 2026)
    - Highlights: A training-free allocentric perception strategy, recovering metric 3D states from single or multiple images, with about 10% improvement on allocentric tasks
    - Paper Link: [arXiv](https://arxiv.org/abs/2602.05789)
+  **Cognitively-Inspired Tokens Overcome Egocentric Bias in Multimodal Models**
    - Publication: arXiv 2026 (Jan 2026)
    - Highlights: Multimodal language models perform well on semantic vision-language tasks but fail at spatial reasoning that requires adopting another agent's visual perspective, reflecting a persistent egocentric bias
    - Paper Link: [arXiv](https://arxiv.org/abs/2601.15849)
+  **EgoThinker: Unveiling Egocentric Reasoning with Spatio-Temporal Chain of Thought**
    - Publication: NeurIPS 2025
    - Highlights: Introduces Chain of Thought (CoT) into egocentric video understanding, proposing a spatio-temporal chain of thought framework
    - Paper Link: [arXiv](https://arxiv.org/abs/2510.23569)
+  **Towards Comprehensive Scene Understanding: Integrating First and Third-Person Views for LVLMs**
    - Publication: NeurIPS 2025
    - Highlights: Proposes the E3VQA multi-view question answering benchmark (4K high-quality QA pairs) and M3CoT prompt technology, with 4.84% improvement on GPT-4o
    - Paper Link: [NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/1af83ab66b4f07a3f55788e67dab5782-Abstract-Conference.html)
+  **Benchmarking Egocentric Multimodal Goal Inference for Assistive Wearable Agents**
    - Publication: NeurIPS 2025 Datasets and Benchmarks Track
    - Highlights: Goal inference benchmark dataset, containing 363 participants and 3,482 records, with human upper limit 93% accuracy and best VLM only 84%
    - Paper Link: [NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/23ab960082db936f874b171822e0d097-Abstract-Datasets_and_Benchmarks.html)
+  **ECBench: Can Multi-modal Foundation Models Understand the Egocentric World? A Holistic Embodied Cognition Benchmark**
    - Publication: CVPR 2025
    - Highlights: A high-quality benchmark designed to systematically evaluate the embodied cognitive abilities of LVLMs. Features diverse scene video sources, open question formats, and 30 dimensions of embodied cognition
    - Paper Link: [CVPR](https://www.openaccess.thecvf.com/content/CVPR2025/html/Dang_ECBench_Can_Multi-modal_Foundation_Models_Understand_the_Egocentric_World_A_CVPR_2025_paper.html) | [arXiv](http://arxiv.org/abs/2501.05031)
+  **MM-Ego: Towards Building Egocentric Multimodal LLMs for Video QA**
    - Publication: ICLR 2025
    - Highlights: Proposes MM-Ego, an egocentric multimodal LLM that shows powerful performance on egocentric video understanding
    - Paper Link: [ICLR](https://openreview.net/forum?id=MM-Ego)
+  **CLiViS: Unleashing Cognitive Map through Linguistic-Visual Synergy for Embodied Visual Reasoning**
    - Publication: arXiv 2025
    - Highlights: Constructs cognitive maps through linguistic-visual synergy, breaking through the bottleneck of long video reasoning
    - Paper Link: [arXiv](https://arxiv.org/abs/2506.17629)
+  **PhysBrain: Human Egocentric Data as a Bridge from Vision Language Models to Physical Intelligence**
    - Publication: arXiv 2025
    - Highlights: Converts first-person human videos into embodied supervision data
    - Paper Link: [arXiv](https://arxiv.org/abs/2512.16793)
+  **Vinci: A Real-time Smart Assistant based on Egocentric Vision-language Model**
    - Publication: ACM 2025 (arXiv 2024)
    - Highlights: A lightweight Ego-VLM for wearable devices, supporting long video memory and action generation, and can run in real time on edge devices
    - Paper Link: [arXiv](https://arxiv.org/abs/2412.21080)
+  **EgoThink: Evaluating First-Person Perspective Thinking Capability of Vision-Language Models**
    - Publication: CVPR 2024
    - Highlights: Introduces a novel visual question-answering benchmark that encompasses six core capabilities with twelve detailed dimensions, constructed using selected clips from egocentric videos with manually annotated QA pairs
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/CVPR2024/html/EgoThink_Evaluating_First-Person_Perspective_Thinking_Capability_of_Vision-Language_Models_CVPR_2024_paper.html)
+  **VidEgoThink: A Comprehensive Benchmark for Egocentric Video Understanding**
    - Publication: arXiv 2024
    - Highlights: Building on EgoThink, introduces a comprehensive benchmark for evaluating egocentric video understanding capabilities, designing four key interrelated tasks: video question-answering, hierarchy planning, visual grounding and reward modeling
    - Paper Link: [arXiv](https://arxiv.org/abs/2405.17719)
+  **Binocular Egocentric-360 Multi-modal Scene Understanding in the Wild**
    - Publication: ICCV 2025 Workshop
    - Highlights: Focuses on binocular/stereo egocentric and 360° panoramic perspectives for multi-modal scene understanding and perception, measuring both first-person views and third-person panoptic views
    - Paper Link: [ICCV](https://openaccess.thecvf.com/content/ICCV2025/html/EgoM2P_Egocentric_Multimodal_Multitask_Pretraining_ICCV_2025_paper.html)
+  **D3Net: Dual-Path Decoupling-Distillation for Adaptive Fusion in Continual Egocentric Learning**
    - Publication: IEEE 2025 (arXiv 2026)
    - Highlights: Proposes a Dual-path Decoupling-Distillation Network for more effective dynamic fusion of modal information and knowledge transfer. Explicitly separates shared and private features of modalities through a dual-path decoupling module with a dynamic gating mechanism. Achieves 83.97% accuracy on UESTC MMEA CL dataset
    - Paper Link: [IEEE Xplore](https://ieeexplore.ieee.org/document/11324280)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
|  EgoSAT | 2026 | 165 h / ~4,800 QA | Streaming interaction understanding | [arXiv](https://arxiv.org/abs/2606.24422) |
| EgoTL | 2026 | 100+ daily household tasks | Long-horizon reasoning, Spatial QA | [Official Website](https://ego-tl.github.io/) |
| EgoCoT-Bench | 2026 | 351 videos / 3,172 QA | Grounded operation-centric CoT QA | [Official Website](https://dstardust.github.io/EgoCoT/) |
| MM-Conv | 2026 | 6.7 h / 4,211 expressions | Contextual 3D dialogue grounding | [arXiv](https://arxiv.org/abs/2605.21796) |
| Minerva-Ego | 2026 | 1,160 QA / 156 videos | Spatio-temporal reasoning trajectory | [GitHub](https://github.com/google-deepmind/neptune) |
| EgoEverything | 2026 | 100+ h / 5K+ MCQs | Long-context AR video QA | [arXiv](https://arxiv.org/abs/2604.08342) |
| EgoEsportsQA | 2026 | 1,745 QA pairs | Esports video QA, Reasoning | [arXiv](https://arxiv.org/abs/2604.12320) |
| MyEgo | 2026 | 541 long videos / 5K QA | Personalized video QA | [GitHub](https://github.com/Ryougetsu3606/MyEgo) |
| LifeDialBench / EgoMem | 2026 | Life logging memory | Online Evaluation | [GitHub](https://github.com/qys77714/LifeDialBench) |
| Ego2Web | 2026 | 500 video-instruction pairs | Egocentric video grounded web agent | [Hugging Face](https://huggingface.co/datasets/Shoubin/Ego2Web) |
| NoRA | 2026 | 1,420 clips | Normative Action Reasoning | [arXiv](https://arxiv.org/abs/2606.04806) |
| Causal-Plan-1M | 2026 | 1M QA / 22.2K clips | Physically Grounded Planning QA | [Hugging Face](https://huggingface.co/datasets/anonymous-causal-plan/Causal_Plan) |
| Pause-and-Think | 2026 | 10K QA clips + 300 benchmark | Assistive Action Suggestion | [GitHub](https://github.com/sssshivvvv/pause-and-think) |
| HD-EPIC | 2025 | ~41 h / dense labels | Fine-grained kitchen, VQA | [Official Website](https://hd-epic.github.io/) |
| EgoEMS | 2025 | 20+ h emergency scenarios | First Aid QA, Multimodal | [GitHub](https://github.com/UVA-DSA/EgoEMS) |
| HowToDIV | 2025 | ~24 h instructional | Dialogue, Procedural QA | [GitHub](https://github.com/google/howtodiv) |
| InterVLA | 2025 | 11.4 h interactions | Instruction, Ego-exo motion capture | [Official Website](https://liangxuy.github.io/InterVLA/) |
| EgoClip | 2022 | 3.8M clip–text pairs | Video-language pre-training | [GitHub](https://github.com/showlab/EgoVLP) |
| AssistQ | 2022 | 100 long videos / 529 QA | Instructional QA | [GitHub](https://github.com/showlab/AssistQ) |
| EgoTaskQA | 2022 | ~2K videos / 40K QA | Causal & Task QA | [Official Website](https://sites.google.com/view/egotaskqa) |
| EgoVQA | 2019 | 600+ QAs | Video QA | [ICCVW 2019](https://openaccess.thecvf.com/content_ICCVW_2019/html/EPIC/Fan_EgoVQA_-_An_Egocentric_Video_Question_Answering_Benchmark_Dataset_ICCVW_2019_paper.html) |

---

### 2.4 Long-form Video Understanding & Structured Reasoning
Processes ultra-long first-person videos at the hour or even day level, with core challenges including long-term dependency modeling, memory retrieval and information summarization. This section also covers scene graph-based structured representations for long-form video reasoning.

+  **Keep It in Mind: User Centric Continual Spatial Intelligence Reasoning in Egocentric Video Streams**
    - Publication: ICML 2026 (arXiv Jun 2026)
    - Highlights: Introduces UCS-Bench, a dataset spanning 170+ hours with 8.1K+ timestamped questions for User-Centric Continual Spatial intelligence
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.15200)
+  **Graph it first! Enabling Reasoning on Long-form Egocentric Videos through Scene Graphs**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Introduces Egocentric Scene Graphs (EgoSGs) to overcome MLLM input constraints, achieving state-of-the-art results on HD-EPIC VQA by representing videos as compact, text-based scene graphs
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.25842)
+  **Bridging Modalities, Spanning Time: Structured Memory for Ultra-Long Agentic Video Reasoning**
    - Publication: arXiv 2026 (May 2026)
    - Highlights: Proposes MAGIC-Video with multimodal memory graph and interleaved narrative chain, outperforming prior best agentic system by 10.1 points on EgoLifeQA
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.08271)
+  **EgoMemReason: A Memory-Driven Reasoning Benchmark for Long-Horizon Egocentric Video Understanding**
    - Publication: arXiv 2026 (May 2026)
    - Highlights: A benchmark for evaluating week-level egocentric video memory-driven reasoning, containing 500 questions, with the best model only achieving 39.6% accuracy
    - Paper Link: [Hugging Face](https://huggingface.co/datasets/Ted412/EgoMemReason)
+  **Semantic and Visual Evidence for Efficient Long-Video Reasoning: A Solution for the HD-EPIC VQA Challenge**
    - Publication: arXiv 2026 (May 2026)
    - Highlights: Decouples long video reasoning into semantic evidence and visual evidence, achieving efficient long video understanding through query-guided retrieval integration
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.29402)
+  **EgoEverything: A Benchmark for Human Behavior Inspired Long Context Egocentric Video Understanding in AR Environment**
    - Publication: arXiv 2026 (Apr 2026)
    - Highlights: A benchmark that explicitly considers human behavior by leveraging human attention signals, abstracted from gaze data, when generating questions
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.08342)
+  **MA-EgoQA: Question Answering over Egocentric Videos from Multiple Embodied Agents**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: First defines the multi-agent egocentric video QA task, providing 1,700+ questions across five scene categories
    - Paper Link: [Official Website](https://ma-egoqa.github.io/)
+  **Static Scene Reconstruction from Dynamic Egocentric Videos**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Proposes a robust pipeline that adapts static reconstruction backbones to long-form egocentric video with a mask-aware reconstruction mechanism
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.18090)
+  **From Pixels to Graphs: using Scene and Knowledge Graphs for HD-EPIC VQA Challenge**
    - Publication: arXiv 2025
    - Highlights: Proposes a framework incorporating two complementary neuro-symbolic abstractions: scene graphs and commonsense knowledge graphs, instantiated through SceneNet and KnowledgeNet respectively
    - Paper Link: [arXiv](https://arxiv.org/abs/2508.01867)
+  **Action Scene Graphs for Long-Form Understanding of Egocentric Videos**
    - Publication: arXiv 2024
    - Highlights: Proposes action scene graphs for long-form understanding of egocentric videos, enabling structured analysis of human activities from wearable device captures
    - Paper Link: [arXiv](https://arxiv.org/abs/2409.01600)
+  **EgoMemory: Memory-Augmented Personalized Retrieval for Long-Context Egocentric Video**
    - Publication: ACL 2026
    - Highlights: Proposes a lifelong memory framework for continuous streaming first-person videos
    - Paper Link: [Microsoft Research](https://www.microsoft.com/en-us/research/publication/egomemory-memory-augmented-personalized-retrieval-for-long-context-egocentric-video/)
+  **MyEgo: Ego-Grounding for Personalized Question-Answering in Egocentric Videos**
    - Publication: CVPR 2026
    - Highlights: Large-scale personalized first-person video dataset for long-form QA
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.01966)
+  **EGAgent: Agentic Very Long Video Understanding**
    - Publication: arXiv 2026
    - Highlights: An agent-based reasoning framework based on entity scene graphs, capable of processing continuous video streams across days, supporting structured multi-hop reasoning and audio-visual hybrid retrieval
    - Paper Link: [arXiv](https://arxiv.org/abs/2601.18157)
+  **Spatial-Conditioned Reasoning in Long-Egocentric Videos**
    - Publication: arXiv 2026
    - Highlights: Explores the impact of explicit spatial signals on long-form VLM reasoning, introducing the finely re-annotated Sanpo-D dataset
    - Paper Link: [arXiv](https://arxiv.org/abs/2601.18100)
+  **FocusGraph: Graph-Structured Frame Selection for Embodied Long Video Question Answering**
    - Publication: arXiv 2026
    - Highlights: Graph-based frame filtering pipeline, using Scene-Caption LLM selector to retrieve query-relevant frames
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.04349)
+  **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - Publication: ICLR 2026
    - Highlights: A benchmark for evaluating embodied cognition through egocentric interaction world modeling, revealing that VLMs perform better on inverse tasks than forward prediction
    - Paper Link: [OpenReview](https://openreview.net/forum?id=Patx6MRipw)
+  **OSGNet: Champion Solution for Ego4D Episodic Memory Challenge 2025**
    - Publication: CVPR 2025 Challenge All-Track Champion
    - Highlights: Proposes an early fusion temporal localization architecture, winning all three tracks of the Ego4D Episodic Memory Challenge
    - Paper Link: [arXiv](https://arxiv.org/abs/2506.03710)
+  **Unique Lives, Shared World: Learning from Single-Life Egocentric Videos**
    - Publication: arXiv 2025
    - Highlights: Studies the learning problem of ultra-long life-cycle videos from a single individual
    - Paper Link: [arXiv](https://arxiv.org/abs/2512.04085)
+  **EgoSchema: A Diagnostic Benchmark for Very Long-form Video Language Understanding**
    - Publication: NeurIPS 2023
    - Highlights: Authoritative diagnostic benchmark for ultra-long egocentric video understanding
    - Paper Link: [arXiv](https://arxiv.org/abs/2308.09126)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
|  UCS-Bench | 2026 | 170+ h / 8.1K+ QA | User-centric continual spatial intelligence | [arXiv](https://arxiv.org/abs/2606.15200) |
| SuperMemory-VQA | 2026 | 52.9 h / 4,853 QA pairs | Long-duration memory QA | [Hugging Face](https://huggingface.co/datasets/OSU-AIoT-MLSys-Lab/SuperMemory-VQA) |
| EgoMemReason | 2026 | 500 weekly-level MCQs | Week-scale memory reasoning evaluation | [Hugging Face](https://huggingface.co/datasets/Ted412/EgoMemReason) |
| EgoExoMem | 2026 | 2.6K MCQs / 390 clips | Cross-view episodic memory reasoning | [GitHub](https://github.com/RuipingL/EgoExoMem) |
| EgoIntrospect | 2026 | 180 h / 60 subjects | Internal user state inference, Long-term memory | [Official Website](https://ego-introspect.github.io/) |
| MA-EgoQA | 2026 | 1,741 QA / 7-day multi-agent footage | Multi-agent egocentric video QA | [Official Website](https://ma-egoqa.github.io/) |
| EgoStream | 2026 | 2,250 evaluation queries | Streaming episodic memory benchmark | [Official Website](https://saroo25.github.io/Egostream/) |
| EgoLife | 2025 | ~266–300 h daily footage | Long-term personal assistant, Episodic memory | [Official Website](https://egolife-ai.github.io/) |
| EgoSchema | 2023 | 250+ h / 5K MCQs | Ultra-long video reasoning & QA | [Official Website](https://egoschema.github.io/) |
| VidChapters-7M | 2023 | 817K videos / 7M chapters | Long video segmentation & summarization | [Official Website](https://antoyang.github.io/vidchapters.html) |
| Multi-Ego | 2022 | ~12 h / 41 multi-wearer sequences | Cross-user video summarization | [GitHub](https://github.com/M-Elfeki/Multi-DPP) |
| DoMSEV | 2018 | 80 h, 48 sequences | Semantic video time-lapse & skimming | [Official Website](https://www.verlab.dcc.ufmg.br/semantic-hyperlapse/cvpr2018-dataset/) |
| HUJI-EgoSeg | 2014 | 29 untrimmed long videos | Temporal activity segmentation | [Official Website](http://www.cs.huji.ac.il/~yedMDpid/egoseg/) |
| UT Ego | 2012 | ~17 h, 4 full-length recordings | Long video summarization & life logging | [Official Website](http://vision.cs.utexas.edu/projects/egocentric_data/UT_Egocentric_Dataset.html) |
| VINST / Visual Diaries | 2011 | 31 daily log videos | Event segmentation, Timeline extraction | [Official Website](https://www.csc.kth.se/cvap/vinst/NovEgoMotion.html) |

---

### 2.5 Gaze, Attention & Intention Prediction
Predicts human gaze points, attention distribution and underlying intentions from first-person footage, a core technology for wearable interactive assistants.

+  **EPIC: A System Framework for Efficient Egocentric Perception on Embodied AR Glasses**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: An efficient egocentric perception system for embodied intelligence on smart AR glasses, leveraging gaze, pose, and inertial signals to infer user intent and retain only the most informative parts of perceptual input
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.14282)
+  **Gaze Beyond the Frame: Forecasting Egocentric 3D Visual Span**
    - Publication: NeurIPS 2025 (arXiv Apr 2026)
    - Highlights: Proposes the novel 3D visual span forecasting task, EgoSpanLift lifts 2D gaze predictions into full 3D scene space
    - Paper Link: [NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/bf649dbcf4eaaba4fc68ccaee25a7f9e-Abstract-Conference.html)
+  **SkillSight: Efficient First-Person Skill Assessment with Gaze**
    - Publication: arXiv 2026 (Apr 2026)
    - Highlights: Explores power-efficient, privacy-preserving egocentric skill assessment for deployment on resource-constrained smart glasses
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.01645)
+  **Gaze-Regularized VLMs for Ego-Centric Behavior Understanding**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Embeds eye-tracking signals into the VLM training pipeline, gaze regularization forces models to prioritize fixated regions, improving semantic metrics by nearly 13%
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.23190)
+  **Real Eyes Realize Faster: Gaze Stability and Pupil Novelty for Efficient Egocentric Learning**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Uses eye-tracking as a training-free side channel: gaze fixation captures visual stability, pupil response captures arousal-linked novelty. Dual-Criterion Frame Curator selects frames at 10% budget matching full-stream performance
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.04098)
+  **EgoCampus: Egocentric Pedestrian Eye Gaze Model and Dataset**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Introduces EgoCampus dataset spanning 25 unique outdoor paths with recordings from 80+ pedestrians using Project Aria glasses
    - Paper Link: [arXiv](https://arxiv.org/abs/2512.07668)
+  **Eyes on Target: Gaze-Aware Object Detection in Egocentric Video**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Injects gaze-derived features into ViT attention mechanism, biasing spatial feature selection toward human-attended regions
    - Paper Link: [arXiv](https://arxiv.org/abs/2511.01237)
+  **Beyond Scanpaths: Graph-Based Gaze Simulation in Dynamic Scenes**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Introduces Object Density Network (ODN) to predict next-step gaze distributions and releases Focus100 dataset with raw gaze data from 30 participants viewing egocentric driving footage
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.23750)
+  **Ego-PMOVE: Prompt-aware Mixture of View Experts Network for Egocentric Gaze Prediction**
    - Publication: AAAI 2026
    - Highlights: First method exploring cross-view gaze correlation, prompt-driven multi-view expert mixture architecture
    - Paper Link: [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/37808)
+  **Learning from Human Gaze: Human-like Robot Social Navigation in Dense Crowds**
    - Publication: AAAI 2026
    - Highlights: Releases the GazeNav dataset with synchronized wearable eye-tracking, RGB footage and robot navigation trajectories
    - Paper Link: [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/38941)
+  **In the Eye of MLLM: Benchmarking Egocentric Video Intent Understanding with Gaze-Guided Prompting**
    - Publication: NeurIPS 2025 Datasets & Benchmarks Track
    - Highlights: The EgoGazeVQA benchmark systematically evaluates the ability of multimodal LLMs to infer user intent via eye movement signals
    - Paper Link: [NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/9df42a5f6d1397e46e2cdca80a1a7903-Abstract-Datasets_and_Benchmarks.html)
+  **egoEMOTION: Egocentric Vision and Physiological Signals for Emotion and Personality Recognition in Real-World Tasks**
    - Publication: NeurIPS 2025
    - Highlights: Multimodal dataset collected via Meta Project Aria glasses, combining video, eye tracking and biometric signals for real-life emotion analysis
    - Paper Link: [arXiv](https://arxiv.org/abs/2510.22129)
+  **EgoIntention: Visual Intention Grounding for Egocentric Assistants**
    - Publication: arXiv 2026 (Apr 2026)
    - Highlights: Introduces the first dataset for egocentric visual intention grounding, challenging multimodal LLMs to understand and ignore unintended contextual objects and reason about uncommon object functionalities
    - Paper Link: [IEEE Xplore](https://ieeexplore.ieee.org/document/11324280)

---

### 2.6 3D/4D Reconstruction & Structured Perception
Recovers 3D human meshes, depth maps and dynamic 4D scene structures from monocular first-person video, the foundational technology for AR/VR and robotic spatial awareness. This section also covers scene graph-based structured 3D perception.

#### Human Pose & Mesh Recovery
+  **Hand-4DGS: Feed-Forward 3D Gaussian Splatting for 4D Hand Reconstruction from Egocentric Videos**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Dynamic 3D hand reconstruction from egocentric videos addressing fast head motion, rapid hand dynamics, severe occlusions, and single-view ambiguity
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.16930)
+  **RoboAtlas: Contextual Active SLAM**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Integrates frontier exploration, global semantic-map reasoning, and egocentric VLM-based reasoning through a contextual multi-armed bandit
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.19378)
+  **EgoForce: Forearm-Guided Camera-Space 3D Hand Pose from a Monocular Egocentric Camera**
    - Publication: SIGGRAPH 2026 (arXiv May 2026)
    - Highlights: Differentiable forearm representation + unified arm-hand Transformer. MPJPE reduced by 28% on HOT3D across all lens types
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.12498)
+  **Bringing a Personal Point of View: Evaluating Dynamic 3D Gaussian Splatting for Egocentric Scene Reconstruction**
    - Publication: EgoVis@CVPR 2026 (arXiv Apr 2026)
    - Highlights: Systematic benchmark of dynamic 3DGS on egocentric vs. exocentric footage, confirming consistent quality degradation from the first-person viewpoint
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.23803)
+  **FunRec: Reconstructing Functional 3D Scenes from Egocentric Interaction Videos**
    - Publication: CVPR 2026 (arXiv Apr 2026)
    - Highlights: Reconstructs functional 3D digital twins of indoor scenes directly from egocentric RGB-D interaction videos, discovering articulated parts and estimating kinematic parameters
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.05621)
+  **OmniEgoCap: Camera-Agnostic Sequence-Level Egocentric Motion Reconstruction**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Diffusion-based reconstruction generalized across all wearable camera hardware, with geometry-aware visibility augmentation module
    - Paper Link: [arXiv](https://arxiv.org/abs/2512.19283)
+  **EgoGrasp: World-Space Hand-Object Interaction Estimation from Egocentric Videos**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: The first method to reconstruct world-space hand-object interactions from dynamic egoview videos, supporting open-vocabulary objects
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.12255)
+  **AG-EgoPose: Leveraging Action-Guided Motion and Kinematic Joint Encoding for Egocentric 3D Pose Estimation**
    - Publication: arXiv 2026
    - Highlights: Action-conditioned motion modeling + kinematic joint embedding for robust wearable camera pose estimation
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.25175)
+  **Pandora: Articulated 3D Scene Graphs from Egocentric Vision**
    - Publication: BMVC 2025
    - Highlights: Leverages egocentric data captured as a human naturally explores a scene wearing Project Aria glasses to recover models of articulated object parts. Demonstrates that articulated 3D scene graphs enhance a robot's ability to perform mobile manipulation tasks
    - Paper Link: [BMVC](https://bmvc2025.bmva.org/proceedings/548/)
+  **Lost & Found: Updating Dynamic 3D Scene Graphs from Egocentric Observations**
    - Publication: arXiv 2024
    - Highlights: Based solely on egocentric recordings with corresponding hand position and camera pose estimates, tracks the 6DoF poses of moving objects within detected interaction intervals. Outperforms the second-best approach by 34% and 56% for translational and orientational error respectively
    - Paper Link: [arXiv](https://arxiv.org/abs/2411.19162)
+  **Fish2Mesh Transformer: 3D Human Mesh Recovery from Egocentric Vision**
    - Publication: arXiv 2025
    - Highlights: First mesh recovery pipeline optimized for wide-angle fisheye head-mounted cameras
    - Paper Link: [arXiv](https://arxiv.org/abs/2503.06089)
+  **Single-to-Dual-View Adaptation for Egocentric 3D Hand Pose Estimation**
    - Publication: CVPR 2024
    - Highlights: Proposes a novel Single-to-Dual-view adaptation (S2DHand) solution that adapts a pre-trained single-view estimator to dual views
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/CVPR2024/html/Single-to-Dual-View_Adaptation_for_Egocentric_3D_Hand_Pose_Estimation_CVPR_2024_paper.html)
+ **Ego-Humans: An Ego-Centric 3D Multi-Human Benchmark**
    - Publication: ICCV 2023
    - Highlights: Presents EgoHumans, a new multi-view multi-human video benchmark to advance egocentric human 3D pose estimation and tracking
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/ICCV2023/html/Ego-Humans_An_Ego-Centric_3D_Multi-Human_Benchmark_ICCV_2023_paper.html)

#### Event Camera-based Perception
+  **D-EventEgo: Event-Based Egocentric Human Pose Estimation in Dynamic Environments**
    - Publication: arXiv 2025
    - Highlights: Pioneering event-stream pipeline for egocentric human pose tracking under fast motion and high dynamic range
    - Paper Link: [arXiv](https://arxiv.org/abs/2505.22007)
+  **EventEgo3D++: 3D Human Motion Capture from a Head-Mounted Event Camera**
    - Publication: arXiv 2025
    - Highlights: End-to-end pipeline for fisheye event-based full-body motion capture on head-worn devices
    - Paper Link: [arXiv](https://arxiv.org/abs/2502.07869)

#### Scene Reconstruction & Egocentric SLAM
+  **Ego-1K: A Large-Scale Multiview Video Dataset for Egocentric Vision**
    - Publication: CVPR 2026
    - Highlights: Nearly 1,000 multi-view egocentric clips captured by 12 synchronized cameras surrounding a 4-camera VR headset rig
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.13741)
+  **EgoLifter: Open-World 3D Segmentation for Egocentric Perception**
    - Publication: ECCV 2024
    - Highlights: A method for open-world 3D segmentation for egocentric perception
    - Paper Link: [Springer](https://link.springer.com/chapter/10.1007/978-3-031-72912-6_22)
+  **EgoSG: Learning 3D Scene Graphs from Egocentric RGB-D Sequences**
    - Publication: CVPR 2024
    - Highlights: Proposes EgoSG to estimate 3D scene graphs directly from egocentric frame sequences
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/CVPR2024/html/EgoSG_Learning_3D_Scene_Graphs_from_Egocentric_RGB-D_Sequences_CVPR_2024_paper.html)
+  **Generalizable Dynamic Radiance Field in Egocentric View**
    - Publication: ICLR 2024
    - Highlights: A novel framework for generalizable dynamic radiance field in egocentric view, predicting a 3D representation of the physical world at a given time based on a monocular video without test-time training
    - Paper Link: [OpenReview](https://openreview.net/forum?id=Generalizable_Dynamic_Radiance_Field_in_Egocentric_View)
+  **EventEgo3D: 3D Human Motion Capture from Egocentric Event Streams**
    - Publication: CVPR 2024
    - Highlights: High-speed human motion capture system leveraging asynchronous event camera footage
    - Paper Link: [arXiv](https://arxiv.org/abs/2404.08640)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Scale | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
|  Oxford Day-and-Night | 2026 | Large-scale egocentric | NVS, Visual relocalisation under challenging lighting | [NeurIPS 2026] |
| ⭐ Ego-Exo4D | 2024 | 1,286+ h paired ego/exo footage | Multi-view skill analysis, 3D reconstruction | [Official Website](https://ego-exo4d-data.org/) |
| PRISM | 2026 | 270K samples / 11.8M frames | Retail embodied VLM, Spatial reasoning | [Hugging Face](https://huggingface.co/datasets/DreamVu/PRISM-100K) |
| EgoTraj | 2026 | 10.7 h / 1.15M frames | Egocentric camera trajectory forecasting | [GitHub](https://github.com/yehiahmad/EgoTraj) |
| AIST-Living | 2026 | Egocentric video + GT 3D scene maps | Global camera localization, Human pose tracking | [Official Website](https://deguchihiroyuki.github.io/Map-Mono-Ego-Project/) |
| OVO-S-Bench | 2026 | 348 videos / 1,680 spatial QA pairs | Streaming spatial embodied reasoning | [Official Website](https://internlm.github.io/OVO-S-Bench/) |
| ⭐ ADT (Aria Digital Twin) | 2023 | 200 multimodal sequences, 2 indoor scenes | Egocentric 3D scene & body perception | [Official Website](https://www.projectaria.com/datasets/adt/) |
| PVSG | 2023 | 400 panoramic clips / ~150K frames | Egocentric panoramic scene graph construction | [GitHub](https://github.com/jingkang50/PVSG) |
| DR(eye)VE | 2018 | ~6 h driving footage / 555K frames | Driver gaze prediction, Automotive egocentric perception | [Official Website](http://aimagelab.ing.unimore.it/dreyeve) |
| EgoCart | 2018 | 9 retail RGB-D sequences | Indoor/shopping cart localization | [Official Website](https://iplab.dmi.unict.it/EgocentricShoppingCartLocalization/) |
| IU ShareView | 2018 | 9 paired egocentric video sets | Cross-wearer instance segmentation & re-ID | [Official Website](http://vision.soic.indiana.edu/firstthird-eccv2018/) |
| OST | 2017 | 57 indoor sequences | Object search, Wearable gaze tracking | [GitHub](https://github.com/Mengmi/deepfuturegaze_gan) |

---

### 2.7 Embodied AI & Vision-Language-Action (Ego-VLA)
Aligns vision, language and action signals from first-person human footage to transfer human manipulation knowledge to robotic agents, the core pipeline for embodied intelligence. This section also covers embodied AI benchmarks and robot learning from human demonstrations.

+  **HumanScale: Egocentric Human Video Can Outperform Real-Robot Data for Embodied Pretraining**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Systematic study comparing egocentric human video and teleoperated real-robot trajectories as pretraining data sources. Models pretrained on egocentric data achieve 24% lower validation loss, and 52.5% and 90% higher success rates on in-distribution and out-of-distribution tasks respectively
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.20521)
+  **HumanoidArena: Benchmarking Egocentric Hierarchical Whole-body Learning**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: A simulation-first benchmark for egocentric hierarchical whole-body learning, formulating policy learning as a hierarchical decision making problem with 7 leg-critical HOI/HSI tasks
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.17833)
+  **ACE-Ego-0: Unifying Egocentric Human and Robotic Data for VLA Pretraining**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Unified VLA pretraining framework jointly leveraging heterogeneous data sources with a scalable egocentric video-to-action pipeline converting raw human videos into robot-format pseudo-action trajectories
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.17200)
+  **Motion-Focused Latent Action Enables Cross-Embodiment VLA Training from Human EgoVideos**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Addresses the absence of action labels in egocentric human manipulation videos for VLA training
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.16251)
+  **ActiveMimic: Egocentric Video Pretraining with Active Perception**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: A pretraining framework that recovers synchronized camera and wrist trajectories from a single body-worn RGB camera to address the performance gap between egocentric video and robot data pretraining
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.06194)
+  **EgoTSR: From Perception to Planning: Evolving Ego-Centric Task-Oriented Spatiotemporal Reasoning via Curriculum Learning**
    - Publication: ICML 2026
    - Highlights: A curriculum-based framework for learning task-oriented spatiotemporal reasoning. Constructs EgoTSR-Data comprising 46 million samples organized into three stages. Achieves 92.4% accuracy on long-horizon logical reasoning tasks
    - Paper Link: [ICML](https://icml.cc/virtual/2026/poster/64173)
+  **EARL: Towards a Unified Analysis-Guided Reinforcement Learning Framework for Egocentric Interaction Reasoning and Pixel Grounding**
    - Publication: ICML 2026
    - Highlights: Employs Group Relative Policy Optimization (GRPO) to enhance the interaction understanding of MLLMs in first-person vision
    - Paper Link: [ICML](https://icml.cc/virtual/2026/poster/64173)
+  **Ego3S: Select, Strengthen, and Synchronize for Efficient Egocentric Reasoning**
    - Publication: ICML 2026
    - Highlights: Proposes a novel three-stage Ego3S framework to ground models' reasoning in interaction evidence, addressing the unique challenges of egocentric reasoning compared to third-person understanding
    - Paper Link: [ICML](https://icml.cc/virtual/2026/poster/64173)
+  **Embodied VideoAgent: Persistent Memory from Egocentric Videos and Embodied Sensors Enables Dynamic Scene Understanding**
    - Publication: ICCV 2025
    - Highlights: An LLM-based agent that constructs scene memory from both egocentric video and embodied sensory inputs (depth and pose sensing). Achieves gains of 6.5% on Ego4D-VQ3D, 2.6% on OpenEQA, and 15.3% on EnvQA
    - Paper Link: [ICCV](https://www.openaccess.thecvf.com/content/ICCV2025/html/Fan_Embodied_VideoAgent_Persistent_Memory_from_Egocentric_Videos_and_Embodied_Sensors_ICCV_2025_paper.html) | [arXiv](http://arxiv.org/abs/2501.00358)
+  **Minerva-Ego: Spatiotemporal Hints for Egocentric Video Understanding**
    - Publication: CVPR 2025
    - Highlights: A benchmark for evaluating complex egocentric visual reasoning, extending high-quality video data sources with challenging multi-step multimodal questions and spatiotemporally-dense human-annotated reasoning traces
    - Paper Link: [CVPR](https://openaccess.thecvf.com/content/CVPR2025/html/Minerva-Ego_Spatiotemporal_Hints_for_Egocentric_Video_Understanding_CVPR_2025_paper.html)
+  **JoyAI-RA 0.1: A Foundation Model for Robotic Autonomy**
    - Publication: arXiv 2026 (Apr 2026)
    - Highlights: VLA embodied foundation model with multi-source multi-level pretraining integrating web data, large-scale egocentric human manipulation videos, simulation trajectories, and real-robot data
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.13863)
+  **EgoPush: Learning End-to-End Egocentric Multi-Object Rearrangement for Mobile Robots**
    - Publication: arXiv 2026 (Feb 2026)
    - Highlights: A policy learning framework enabling egocentric, perception-driven rearrangement without relying on explicit global state estimation. Uses object-centric latent space to encode relative spatial relations
    - Paper Link: [arXiv](https://arxiv.org/abs/2602.18071)
+  **EgoScale: Scaling Dexterous Manipulation with Diverse Egocentric Human Data**
    - Publication: arXiv 2026 (Feb 2026)
    - Highlights: Trains a VLA model on over 20,854 hours of action-labeled egocentric human video, uncovering a log-linear scaling law between human data scale and validation loss
    - Paper Link: [arXiv](https://arxiv.org/abs/2602.16710)
+  **Ego-Pi: VLA Fine-Tuning for Egocentric Human and Robot Data**
    - Publication: arXiv 2026
    - Highlights: Targeted fine-tuning pipeline for dual-arm dexterous manipulation VLAs trained on wearable human footage
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.08107)
+  **ViterbiPlanNet: Injecting Procedural Knowledge via Differentiable Viterbi for Egocentric Task Planning**
    - Publication: CVPR 2026
    - Highlights: Differentiable Viterbi algorithm injects step-by-step procedural priors into VLA planning modules
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.04265)
+  **OSCAR: Omni-Embodiment Skeleton-Conditioned World Action Model for Robotics**
    - Publication: arXiv 2026
    - Highlights: Universal skeleton-conditioned world-action model learning multi-robot policies from first-person human demonstrations
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.04463)
+  **Co-training with Ego-centric Video and Demonstration for Robot Navigation Task**
    - Publication: arXiv 2026
    - Highlights: Cross-domain co-training converts egocentric walking videos into mobile robot imitation datasets
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.01951)
+  **In-N-On: Scaling Egocentric Manipulation with in-the-wild and on-task Data**
    - Publication: arXiv 2025 (Nov 2025)
    - Highlights: Curates PHSD dataset with egocentric data and on-task data directly aligned to target manipulation tasks
    - Paper Link: [arXiv](https://arxiv.org/abs/2511.12643)
+  **EgoBridge: Domain Adaptation for Generalizable Imitation from Egocentric Human Videos**
    - Publication: NeurIPS 2025
    - Highlights: Optimal transport alignment between human visual-action distributions, improving imitation success rate by 44% over standard baselines
    - Paper Link: [arXiv](https://arxiv.org/abs/2509.19626)
+  **EgoAgent: A Joint Predictive Agent Model in Egocentric Worlds**
    - Publication: ICCV 2025
    - Highlights: Unified Transformer architecture integrating egocentric vision, language, world modeling and action decision heads
    - Paper Link: [arXiv](https://arxiv.org/abs/2502.05857)

#### 📊 Related Datasets & Benchmarks (Procedural Skill Learning)
| Dataset Name | Year | Scale | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
|  In-N-On (PHSD) | 2025 | Egocentric + on-task data | Manipulation policy learning | [arXiv](https://arxiv.org/abs/2511.12643) |
| EgoVerse | 2026 | 1,362 h / ~80K task episodes | General robot manipulation pre-training, Embodied benchmarking | [Official Website](https://egoverse.ai/) |
| EgoLive | 2026 | Large-scale real-world daily task recordings | Unstructured robotic skill transfer | [arXiv](https://arxiv.org/abs/2604.23570) |
| EgoMAGIC | 2026 | 3,355 medical task videos / 50 clinical workflows | Surgical action detection & procedural assistance | [Zenodo](https://doi.org/10.5281/zenodo.19239154) |
| HumanEgo | 2026 | Short Aria wearable demonstration sequences | Human-to-robot policy distillation | [Official Website](https://humanego-ai.github.io/) |
| EgoSPT | 2026 | 11,515 operation episodes / 112 task folders | Spatial prompt-conditioned manipulation trajectory generation | [Hugging Face](https://huggingface.co/datasets/JackYFL233/EgoSPT) |
| Ego-EXTRA | 2026 | 50 h / 15K+ instructional VQA pairs | Expert-novice wearable assistance scenarios | [Official Website](https://fpv-iplab.github.io/Ego-EXTRA/) |
| GM-100 | 2026 | 100+ manipulation tasks / 13K trajectories | General robot skill evaluation benchmark | [Official Website](https://www.rhos.ai/research/gm-100) |
| SABER | 2026 | 100+ h / 44.8K retail samples | Embodied VLA domain adaptation for shopping robots | [Official Website](https://dreamvu.ai/saber/) |
| EgoProactive / Pro²Bench | 2026 | 700 wearable recordings / 42K evaluation samples | Proactive procedural wearable assistant benchmark | [Hugging Face](https://huggingface.co/datasets/facebook/wearable-ai) |
| EgoYC2 / Exo2EgoDVC | 2025 | ~43 h cooking footage with dense step captions | Household procedural cross-view alignment | [GitHub](https://github.com/ut-vision/Exo2EgoDVC) |
| ⭐ EgoExoLearn | 2024 | 120 h asynchronous ego/exo paired clips | Human procedural learning simulation, Robot imitation | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |
| ⭐ Assembly101 | 2022 | 513 h multi-view assembly footage | Step-wise industrial procedural manipulation | [Official Website](https://assembly-101.github.io/) |
| IndustReal | 2024 | ~6 h factory operation sequences | Industrial step detection & error recognition | [Official Website](https://timschoonbeek.github.io/industreal.html) |
| EgoProceL | 2022 | 62 wearable videos / 16 household tasks | Daily procedural learning baseline | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| EPIC-Tent | 2019 | 7+ h dual-HMD tent assembly footage + eye tracking | Multimodal procedural activity analysis | [Data Repository](https://data.bris.ac.uk/data/dataset/2ite3tu1u53n42hjfh3886sa86) |
| CMU-MMAC | 2011 | 25 participants / 5 cooking recipes | Kitchen procedural activity recognition | [Official Website](http://kitchen.cs.cmu.edu/) |
| GTEA Gaze | 2011 | 17 cooking sessions | Fine-grained procedural action + gaze prediction | [Official Website](https://cbs.ic.gatech.edu/fpv/) |

---

### 2.8 Egocentric World Models
Learns the evolution rules of environments from first-person observations, enabling future frame prediction, synthetic interaction video generation and long-horizon task planning.

+  **EgoCS-400K: An Egocentric Gameplay Dataset for World Models**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: A large-scale replay-grounded egocentric Counter-Strike dataset for world models, built from public professional CS match demos preserving human gameplay trajectories
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.16186)
+  **AnchorWorld: Embodied Egocentric World Simulation with View-based Evolution Customization**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Anchor-keyframe constrained controllable egocentric simulator, with anchor matching accuracy reaching 89%
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.07326)
+  **PlayerOne: Egocentric World Simulator**
    - Publication: NeurIPS 2025 (arXiv Apr 2026)
    - Highlights: First photorealistic open-world egocentric simulator supporting unrestricted free exploration and full motion control
    - Paper Link: [arXiv](https://arxiv.org/abs/2512.06724)
+  **EgoHOI: Egocentric World Model for Photorealistic Hand-Object Interaction Synthesis**
    - Publication: arXiv 2026 (Mar 2026)
    - Highlights: Pioneering HOI-focused egocentric diffusion world model embedding physical priors
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.13615)
+  **WEM: World-Ego Modeling for Long-Horizon Evolution in Hybrid Embodied Tasks**
    - Publication: arXiv 2026
    - Highlights: Disentangled static scene + dynamic self-branch world modeling architecture for long-sequence forecasting
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.19957)
+  **EgoExo-WM: Unlocking Exo Video for Ego World Models**
    - Publication: arXiv 2026
    - Highlights: Cross-view knowledge transfer pipeline leveraging abundant third-person footage to augment egocentric world model training
    - Paper Link: [arXiv](https://arxiv.org/pdf/2605.15477)
+  **EgoSim: Egocentric World Simulator for Embodied Interaction Generation**
    - Publication: arXiv 2026
    - Highlights: Closed-loop interactive simulator with persistent dynamic 3D scene states for continuous synthetic interaction video generation
    - Paper Link: [arXiv](https://arxiv.org/abs/2604.01001)
+  **EgoForge: Goal-Directed Egocentric World Simulator**
    - Publication: arXiv 2026
    - Highlights: Goal-conditioned generative simulator producing future egocentric sequences matching user-specified task objectives
    - Paper Link: [arXiv](https://arxiv.org/abs/2603.20169)
+  **Walk through Paintings: Egocentric World Models from Internet Priors**
    - Publication: arXiv 2026
    - Highlights: Repurposes pre-trained video diffusion models into action-conditioned egocentric world models using web video priors
    - Paper Link: [arXiv](https://arxiv.org/abs/2601.15284)
+  **ENACT: Evaluating Embodied Cognition with World Modeling of Egocentric Interaction**
    - Publication: ICLR 2026
    - Highlights: First benchmark quantifying embodied cognition via egocentric interaction world modeling, revealing VLMs perform better on inverse tasks than forward prediction
    - Paper Link: [OpenReview](https://openreview.net/forum?id=Patx6MRipw)
+  **MEgoHand: Multimodal Egocentric Hand-Object Interaction Motion Generation**
    - Publication: NeurIPS 2025
    - Highlights: Generalizable HOI world model with two-stage VLM prior inference + DiT flow matching trajectory generation
    - Paper Link: [NeurIPS](https://proceedings.neurips.cc/paper_files/paper/2025/hash/469c396a192043e3d70c04bdb3e5a532-Abstract-Conference.html)

#### 📊 Related Datasets & Benchmarks (World Model Pre-training & Video Generation)
| Dataset Name | Year | Scale | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
| ⭐ Ropedia Xperience-10M | 2026 | 10M multimodal human experience clips | Large-scale egocentric world model pre-training | [Hugging Face](https://huggingface.co/datasets/ropedia-ai/xperience-10m) |
| DreamDojo-HV | 2026 | Massive first-person synthetic footage | Generative world model training | [arXiv](https://arxiv.org/abs/2602.06949) |
| Ego-1K | 2026 | Multi-view egocentric video fragments | Neural 3D/4D dynamic scene synthesis | [Hugging Face](https://huggingface.co/datasets/facebook/ego-1k) |
| In-lab | 2026 | Desktop manipulation trajectory sequences | Small-scale skill world model fine-tuning | [arXiv](https://arxiv.org/abs/2602.06949) |
| HumanNet | 2026 | ~1M hours human-centric video corpus | General VLA & world model pre-training | [arXiv](https://arxiv.org/abs/2605.06747) |
| MobileEgo Anywhere | 2026 | 200 h smartphone egocentric daily footage | Lightweight long-form world model training | [arXiv](https://arxiv.org/abs/2605.05945) |
| EgoEdit | 2025 | 100K egocentric video editing pairs | Conditional egocentric video generation benchmark | [Official Website](https://snap-research.github.io/EgoEdit) |
| EgoVid-5M | 2024 | 5M diverse first-person video clips | Foundation generative egocentric video dataset | [Official Website](https://egovid.github.io/) |

---

### 2.9 Egocentric Procedural AI Assistant
Focused on building first-person step-by-step AI assistants that support users in daily and professional procedural tasks. This direction is organized around three core capabilities — procedural error detection, procedural learning, and procedural question answering — supported by two enabling dimensions: real-time streaming perception and proactive interaction.

#### 2.9.1 Procedural Error Detection
+  **Plan, Watch, Recover: A Benchmark and Architectures for Proactive Procedural Assistance**
    - Publication: arXiv 2026 (Jun 2026)
    - Highlights: Releases EgoProactive, a large-scale wearable-egocentric dataset for proactive procedural assistance
    - Paper Link: [arXiv](https://arxiv.org/abs/2606.06220)
+  **Modeling Multiple Normal Action Representations for Error Detection in Procedural Tasks**
    - Publication: CVPR 2025
    - Highlights: Models multiple normal action representations to improve error detection robustness across diverse execution patterns
    - Paper Link: [arXiv](https://arxiv.org/abs/2504.06021)
+  **Gazing Into Missteps: Leveraging Eye-Gaze for Unsupervised Mistake Detection in Egocentric Videos of Skilled Human Activities**
    - Publication: CVPR 2025
    - Highlights: First unsupervised mistake detection method leveraging eye-gaze signals for skilled procedural activities
    - Paper Link: [arXiv](https://arxiv.org/abs/2504.07892)
+  **Transparent and Coherent Procedural Mistake Detection**
    - Publication: EMNLP 2025
    - Highlights: Generates transparent, coherent natural language explanations for detected procedural mistakes
    - Paper Link: [arXiv](https://arxiv.org/abs/2510.08765)
+  **PREGO: Online Mistake Detection in PRocedural EGOcentric Videos**
    - Publication: CVPR 2024
    - Highlights: Online real-time mistake detection framework tailored for egocentric procedural videos
    - Paper Link: [arXiv](https://arxiv.org/abs/2404.01688)
+  **TI-PREGO: Chain of Thought and In-Context Learning for Online Mistake Detection in PRocedural EGOcentric Videos**
    - Publication: arXiv 2024
    - Highlights: Enhances PREGO with chain-of-thought and in-context learning for improved online error detection
    - Paper Link: [arXiv](https://arxiv.org/abs/2410.05678)
+  **EgoOops: A Dataset for Mistake Action Detection from Egocentric Videos Referring to Procedural Texts**
    - Publication: ICCV 2024
    - Highlights: First mistake detection dataset aligned with procedural text instructions in egocentric view
    - Paper Link: [Project Page](https://ego-oops.github.io/)
+  **Error Detection in Egocentric Procedural Task Videos**
    - Publication: CVPR 2024
    - Highlights: Systematic benchmark and baseline framework for egocentric procedural error detection
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/CVPR2024/html/Li_Error_Detection_in_Egocentric_Procedural_Task_Videos_CVPR_2024_paper.html)

#### 2.9.2 Procedural Learning
+  **Task Graph Maximum Likelihood Estimation for Procedural Activity Understanding in Egocentric Videos**
    - Publication: arXiv 2025 (Feb 2025)
    - Highlights: Introduces a gradient-based approach for learning task graphs from procedural activities, optimizing edge weights via maximum likelihood
    - Paper Link: [arXiv](https://arxiv.org/abs/2502.08123)
+  **HiERO: Understanding the Hierarchy of Human Behavior Enhances Reasoning on Egocentric Videos**
    - Publication: ICCV 2025
    - Highlights: Hierarchical behavior understanding framework that significantly boosts egocentric procedural reasoning performance
    - Paper Link: [Project Page](https://github.com/facebookresearch/hiero)
+  **Procedure Learning via Regularized Gromov-Wasserstein Optimal Transport**
    - Publication: arXiv 2025
    - Highlights: Procedural learning method based on regularized Gromov-Wasserstein optimal transport
    - Paper Link: [arXiv](https://arxiv.org/abs/2503.12456)
+  **OPEL: Optimal Transport Guided ProcedurE Learning**
    - Publication: NeurIPS 2024
    - Highlights: Optimal transport guided unsupervised procedure learning framework
    - Paper Link: [arXiv](https://arxiv.org/abs/2410.08765)
+  **United We Stand, Divided We Fall: UnityGraph for Unsupervised Procedure Learning from Videos**
    - Publication: WACV 2024
    - Highlights: UnityGraph-based unsupervised procedure learning from unlabeled instructional videos
    - Paper Link: [arXiv](https://arxiv.org/abs/2311.04567)
+  **STEPs: Self-Supervised Key Step Extraction and Localization from Unlabeled Procedural Videos**
    - Publication: ICCV 2023
    - Highlights: Self-supervised key step extraction and localization for unlabeled procedural videos
    - Paper Link: [Project Page](https://steps-procedural.github.io/)
+  **My View is the Best View: Procedure Learning from Egocentric Videos**
    - Publication: ECCV 2022
    - Highlights: First dedicated procedure learning framework designed for the egocentric perspective
    - Paper Link: [Project Page](https://github.com/ShyamNarasimhan/Procedure-Learning-from-Egocentric-Videos)
+  **Learning To Recognize Procedural Activities with Distant Supervision**
    - Publication: CVPR 2022
    - Highlights: Distant supervision based procedural activity recognition framework
    - Paper Link: [arXiv](https://arxiv.org/abs/2204.02345)

#### 2.9.3 Procedural Question Answering
+  **Grounded Multi-Hop VideoQA in Long-Form Egocentric Videos**
    - Publication: AAAI 2025
    - Highlights: Considers the problem of Multi-Hop Video Question Answering (MH-VidQA) in long-form egocentric videos
    - Paper Link: [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/33925)
+  **EASG-Bench: Video Q&A Benchmark with Egocentric Action Scene Graphs**
    - Publication: arXiv 2025 (Aug 2025)
    - Highlights: A question-answering benchmark where QA pairs are created from spatio-temporally grounded dynamic scene graphs capturing relationships among actors, actions, and objects
    - Paper Link: [arXiv](https://arxiv.org/abs/2508.01867)
+  **EOC-Bench: Can MLLMs Identify, Recall, and Forecast Objects in an Egocentric World?**
    - Publication: arXiv 2025 (Jun 2025)
    - Highlights: A benchmark designed to systematically evaluate object-centric embodied cognition in dynamic egocentric scenarios
    - Paper Link: [arXiv](https://arxiv.org/abs/2506.05287)
+  **EgoNight: Towards Egocentric Vision Understanding at Night with a Challenging Benchmark**
    - Publication: arXiv 2025
    - Highlights: The first comprehensive benchmark for nighttime egocentric vision with VQA as the core task
    - Paper Link: [arXiv](https://arxiv.org/abs/2510.08961)
+  **EgoLife: Towards Egocentric Life Assistant**
    - Publication: CVPR 2025
    - Highlights: A project to develop an egocentric life assistant that accompanies and enhances personal efficiency through AI-powered wearable glasses
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/CVPR2025/html/EgoLife_Towards_Egocentric_Life_Assistant_CVPR_2025_paper.html)
+  **RAVEN: Query-Guided Representation Alignment for Question Answering over Audio, Video, Embedded Sensors, and Natural Language**
    - Publication: arXiv 2025
    - Highlights: Multi-modal QA framework aligning audio, video, embedded sensors and natural language for procedural scenarios
    - Paper Link: [arXiv](https://arxiv.org/abs/2503.06789)
+  **EgoTextVQA: Towards Egocentric Scene-Text Aware Video Question Answering**
    - Publication: CVPR 2025
    - Highlights: First egocentric video QA benchmark incorporating scene text information for procedural tasks
    - Paper Link: [Project Page](https://egotextvqa.github.io/)
+  **Omnia de Egotempo: Benchmarking Temporal Understanding of Multi-Modal LLMs in Egocentric Videos**
    - Publication: CVPR 2025
    - Highlights: Benchmark for temporal reasoning ability of multimodal LLMs on egocentric procedural videos
    - Paper Link: [arXiv](https://arxiv.org/abs/2504.09876)
+  **Vinci: A Real-time Smart Assistant Based on Egocentric Vision-language Model for Portable Devices**
    - Publication: ACM 2025
    - Highlights: Lightweight edge-deployable Ego-VLM for procedural assistant scenarios
    - Paper Link: [arXiv](https://arxiv.org/abs/2412.21080)
+  **Grounded Question-Answering in Long Egocentric Videos**
    - Publication: CVPR 2024
    - Highlights: Grounded QA framework for long egocentric procedural videos
    - Paper Link: [CVF](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_Grounded_Question-Answering_in_Long_Egocentric_Videos_CVPR_2024_paper.html)

#### 2.9.4 Real-time Streaming & Proactive Interaction
+  **Dispider: Enabling Video LLMs with Active Real-Time Interaction via Disentangled Perception, Decision, and Reaction**
    - Publication: CVPR 2025
    - Highlights: Disentangled perception-decision-reaction framework for real-time interactive video LLMs
    - Paper Link: [Project Page](https://dispider.github.io/)
+  **StreamBridge: Turning Your Offline Video Large Language Model into a Proactive Streaming Assistant**
    - Publication: NeurIPS 2025
    - Highlights: Converts offline video LLMs into proactive streaming assistants without retraining
    - Paper Link: [Project Page](https://streambridge-vlm.github.io/)
+  **Flash-VStream: Efficient Real-Time Understanding for Long Video Streams**
    - Publication: ICCV 2025
    - Highlights: Efficient real-time understanding pipeline for long-duration video streams
    - Paper Link: [Project Page](https://github.com/yydlm/Flash-VStream)
+  **Proactive Agent: Shifting LLM Agents from Reactive Responses to Active Assistance**
    - Publication: ICLR 2025
    - Highlights: Paradigm shifting LLM agents from reactive response to proactive procedural assistance
    - Paper Link: [arXiv](https://arxiv.org/abs/2502.01234)
+  **YETI (YET to Intervene) Proactive Interventions by Multimodal AI Agents in Augmented Reality Tasks**
    - Publication: arXiv 2025
    - Highlights: Proactive intervention framework for multimodal AI agents in AR procedural tasks
    - Paper Link: [arXiv](https://arxiv.org/abs/2504.56789)
+  **Proactive Assistant Dialogue Generation from Streaming Egocentric Videos**
    - Publication: EMNLP 2025
    - Highlights: Generates context-aware proactive assistant dialogues from streaming egocentric procedural videos
    - Paper Link: [arXiv](https://arxiv.org/abs/2510.12345)
+  **VideoLLM-online: Online Video Large Language Model for Streaming Video**
    - Publication: CVPR 2024
    - Highlights: Online video LLM framework designed for streaming egocentric video input
    - Paper Link: [arXiv](https://arxiv.org/abs/2404.09876)

#### 📊 Related Datasets & Benchmarks
| Dataset Name | Year | Venue | Core Tasks | Link |
| :--- | :--- | :--- | :--- | :--- |
|  EgoProactive | 2026 | arXiv | Proactive procedural assistance | [arXiv](https://arxiv.org/abs/2606.06220) |
|  EASG-Bench | 2025 | arXiv | Video QA with action scene graphs | [arXiv](https://arxiv.org/abs/2508.01867) |
|  EOC-Bench | 2025 | arXiv | Object-centric embodied cognition | [arXiv](https://arxiv.org/abs/2506.05287) |
|  EgoNight | 2025 | arXiv | Nighttime egocentric VQA | [arXiv](https://arxiv.org/abs/2510.08961) |
| OVO-Bench | 2025 | CVPR | Online real-time video understanding benchmark | [Project Page](https://ovo-bench.github.io/) |
| SVBench | 2025 | ICLR | Streaming video understanding with multi-turn dialogues | [Project Page](https://svbench.github.io/) |
| ProactiveVideoQA | 2025 | arXiv | Proactive interaction evaluation for video LLMs | [arXiv](https://arxiv.org/abs/2504.12345) |
| STREAMGAZE | 2025 | arXiv | Gaze-guided proactive streaming video understanding | [arXiv](https://arxiv.org/abs/2505.67890) |
| CaptainCook4D | 2024 | NeurIPS | Procedural error detection, 4D activity understanding | [Project Page](https://captaincook4d.github.io/) |
| EgoOops | 2024 | ICCV | Mistake action detection with procedural text reference | [Project Page](https://ego-oops.github.io/) |
| IndustReal | 2024 | WACV | Industrial procedural step recognition, error detection | [Project Page](https://timschoonbeek.github.io/industreal.html) |
| HoloAssist | 2023 | ICCV | Interactive procedural AI assistant, mistake detection | [Project Page](https://holoassist.github.io/) |
| EgoProceL | 2022 | CVPR | Egocentric procedure learning benchmark | [GitHub](https://github.com/Sid2697/EgoProceL-egocentric-procedure-learning) |
| Assembly101 | 2022 | CVPR | Multi-view procedural assembly activity understanding | [Official Website](https://assembly-101.github.io/) |
| EgoExoLearn | 2024 | CVPR | Cross-view procedural learning from demonstration to practice | [GitHub](https://github.com/OpenGVLab/EgoExoLearn) |

---

### 2.10 🛡️ Egocentric Data Security & Privacy Protection

With the rapid proliferation of wearable cameras and first-person video data, data security and privacy have become critical issues in egocentric vision. Unlike traditional third-person vision, egocentric videos inherently carry sensitive information about the wearer's identity, behavior, social relationships, and environment, while bystanders are often recorded without consent. This section summarizes representative works from **privacy risk assessment & benchmarking**, **anonymization & data de‑identification**, **privacy-preserving techniques**, and **ethical & policy considerations**.

#### 2.10.1 Privacy Risk Assessment & Benchmarking
+  **Position: Life‑Logging Video Streams Make the Privacy‑Utility Trade‑off Inevitable**
    - Publication: arXiv 2026
    - Highlights: Systematically analyses privacy risks along the entire pipeline of perception, transmission, and storage in life‑logging video streams, pointing out the limitations of existing single‑point privacy protection methods in cross‑view collaborative scenarios.
    - Paper Link: [arXiv](https://arxiv.org/abs/2605.10404)
+  **EgoPrivacy: What Your First-Person Camera Says About You?**
    - Publication: ICML 2025
    - Highlights: The first large‑scale benchmark for egocentric privacy risk assessment, systematically answering "what can be inferred about the wearer from first‑person video?". Covers three privacy categories (demographic, individual, contextual) and defines seven granularity‑varying privacy recovery tasks. Proposes a **Retrieval‑Augmented Attack** that leverages ego‑to‑exo retrieval. Experiments show that foundation models recover identity, scene, gender, ethnicity, and other attributes with **70‑80% accuracy** in zero‑shot settings
    - Paper Link: [arXiv](https://arxiv.org/abs/2506.12258) | [GitHub](https://github.com/williamium3000/ego-privacy)
+  **EgoNormia: Benchmarking Physical‑Social Norm Understanding**
    - Publication: ACL 2025 Findings
    - Highlights: Constructs a norm understanding benchmark with **1,853 multiple‑choice questions** covering seven norm categories (safety, privacy, proxemics, politeness, cooperation, coordination/proactivity, and communication/readability). Evaluation shows that state‑of‑the‑art VLMs achieve only **54%** on EgoNormia, revealing significant **safety and privacy risks** in real‑world agent applications
    - Paper Link: [ACL Anthology](https://aclanthology.org/2025.findings-acl.985/)
+  **EAPrivacy: Benchmarking Physical-World Privacy Awareness of LLM-Powered Agents**
    - Publication: arXiv 2025
    - Highlights: Introduces a comprehensive evaluation benchmark designed to quantify the physical-world privacy awareness of LLM-powered embodied agents
    - Paper Link: [arXiv](https://arxiv.org/abs/2506.12258)

#### 2.10.2 Anonymization & Data De‑identification
+  **EgoBlur: Responsible Innovation in Aria**
    - Publication: Meta Reality Labs (arXiv 2023)
    - Highlights: The core anonymization system for **Project Aria**, designed to blur **bystander faces and vehicle license plates** at the data acquisition stage. Uses FasterRCNN as the detector and applies Gaussian blur to detected PII regions.
    - Paper Link: [arXiv](https://arxiv.org/abs/2308.13093)
+  **Ego4D Privacy & Ethics Framework**
    - Publication: Ego4D Dataset Documentation
    - Highlights: The Ego4D dataset (3,670 hours, 931 participants, 9 countries) adopts **strict privacy and ethical standards** during collection. Participants can opt for blurring, and **612 hours** remain unblurred with explicit consent. The dataset uses a comprehensive **de‑identification pipeline** and publishes detailed privacy and ethics guidelines.
    - Paper Link: [Ego4D Privacy Page](https://ego4d-data.org/pages/privacy-and-ethics)

#### 2.10.3 Privacy‑Preserving Techniques
+ **Edge‑based Privacy Filtering**
    +  **Extra‑Lightweight AI‑Based Privacy Preserving Framework for Egocentric Wearable Cameras (EPIC)**
        - Publication: CVPR 2025 Workshops
        - Highlights: Proposes an ultra‑lightweight AI‑based privacy‑preserving framework for resource‑constrained wearable cameras. Employs a st_yolo_lc_v1 model for face detection and obfuscates detailed information before storing or sending images. Implemented on an STM32L4 MCU with only 640 KB of RAM, achieving 41.38% mAP for face detection
        - Paper Link: [OpenAccess CVF](https://openaccess.thecvf.com/content/CVPR2025W/MTF/html/Li_Extra-Lightweight_AI-Based_Privacy_Preserving_Framework_for_Egocentric_Wearable_Cameras_CVPRW_2025_paper.html)

#### 2.10.4 Ethics, Policy & Social Impact
+  **Privacy and Ethical Challenges in Egocentric Data Collection**
    - Publication: The Indian Express / Moneycontrol 2026
    - Highlights: Reports on India becoming a hotspot for egocentric AI data collection and the resulting privacy concerns. Points out that egocentric recordings may **inadvertently capture faces, private conversations, sensitive workflows, or bystanders who have not consented**, raising ethical issues around **surveillance, consent, and labour displacement**.
    - Paper Link: [The Indian Express](https://indianexpress.com/) | [Moneycontrol](https://www.moneycontrol.com/)
+  **Smart Glasses and GDPR: Europe's Regulatory Crackdown**
    - Publication: GDPR Local 2026
    - Highlights: Reports on strict scrutiny by European data protection authorities, MEPs, and the EDPB on **smart glasses**; the core issue is that **bystanders captured by cameras cannot meaningfully consent**. Both the French CNIL and the EDPB launched dedicated work in 2026, with the EDPB's report on "social acceptability" of smart glasses expected in summer 2026.
    - Paper Link: [GDPR Local](https://gdprlocal.com/)

#### 📊 Related Datasets & Resources
| Name | Type | Year | Core Content | Link |
| :--- | :--- | :--- | :--- | :--- |
|  EgoPrivacy | Privacy risk assessment benchmark | 2025 | Three privacy categories, seven privacy recovery tasks | [GitHub](https://github.com/williamium3000/ego-privacy) |
|  EgoNormia | Norm understanding benchmark | 2025 | 1,853 MCQs covering seven norm categories (incl. privacy) | [ACL](https://aclanthology.org/2025.findings-acl.985/) |
|  EgoBlur | Anonymisation system | 2023 | Real‑time blurring of faces and license plates | [arXiv](https://arxiv.org/abs/2308.13093) |
| Ego4D Privacy Policy | Dataset privacy framework | 2022 | De‑identification pipeline, participant consent mechanism | [Ego4D](https://ego4d-data.org/pages/privacy-and-ethics) |

---

## 📊 Datasets, Benchmarks & Simulators

### General Large-Scale Egocentric Datasets
| Dataset Name | Release Year | Scale | Core Supported Tasks | Official Link |
| :--- | :--- | :--- | :--- | :--- |
|  HD-EPIC | 2025 | 41 h ultra-high resolution cooking footage with dense multi-layer annotations | Fine-grained activity understanding, Dense VQA, Multimodal alignment | [arXiv](https://arxiv.org/pdf/2502.04144) |
| Ego-Exo4D | 2024 | 1,286 hours synchronized first/third-person multimodal clips | Cross-view alignment, Human skill analysis, 4D reconstruction | [Official Website](https://ego-exo4d-data.org/) |
| Ego4D | 2022 | 3,670 hours wearable video, 923 participants across 9 countries | Action recognition, Episodic memory, Social interaction, 3D human pose | [Official Website](https://ego4d-data.org/) |
| EPIC-KITCHENS-100 | 2020 | 100 h kitchen footage, 90K annotated action segments | Action detection, Recognition, Future anticipation | [Official Website](https://epic-kitchens.github.io/) |

### Fine-Grained Task-Specific Datasets
#### Object & HOI Sub-collections
+  **EgoObjects**
    - Release: ICCV 2023
    - Scale: Pilot version contains over 9K videos collected by 250 participants from 50+ countries using 4 wearable devices, and over 650K object annotations from 368 object categories
    - Core Task: Fine-grained object understanding
    - Link: https://github.com/facebookresearch/EgoObjects
+  **EgoXtreme**
    - Release: CVPR 2026
    - Scale: Challenging egocentric 6D pose dataset with motion blur heavy occlusion and extreme lighting shifts
    - Core Task: Robust object 6D pose estimation for wearable cameras
    - Link: https://arxiv.org/pdf/2603.25135
+  **TouchMoment**
    - Release: CVPR 2026
    - Scale: 150K frames annotated with precise contact start/end timestamps and contact categories
    - Core Task: Fine-grained hand-object contact moment detection
    - Link: https://arxiv.org/pdf/2604.12343
+  **EgoPressure**
    - Release: arXiv 2024
    - Scale: 5 h multimodal footage with synchronized tactile pressure maps IMU signals and RGB
    - Core Task: Tactile-aware hand-object interaction modeling
    - Link: https://arxiv.org/pdf/2409.02224

#### Procedural Task Sub-collections
+  **CaptainCook4D**
    - Release: NeurIPS 2024
    - Scale: Cooking procedural videos with 4D annotations and error labels
    - Core Task: Procedural error detection, Step understanding
    - Link: https://captaincook4d.github.io/
+  **EgoOops**
    - Release: ICCV 2024
    - Scale: Mistake action detection dataset aligned with procedural texts
    - Core Task: Text-referenced egocentric mistake detection
    - Link: https://ego-oops.github.io/
+  **IndustReal**
    - Release: WACV 2024
    - Scale: ~6 h industrial assembly videos with execution error annotations
    - Core Task: Industrial procedural step recognition, error detection
    - Link: https://timschoonbeek.github.io/industreal.html

#### Long Video & Episodic Memory Datasets
+  **EgoLife**
    - Release: CVPR 2025
    - Scale: Continuous multi-day footage from 6 co-living participants with dense daily event labels
    - Core Task: Long-term life-log memory retrieval & personal event QA
    - Link: https://arxiv.org/pdf/2503.03803
+  **EgoSchema**
    - Release: NeurIPS 2023
    - Scale: 500+ long egocentric clips with multi-step temporal reasoning MCQs
    - Core Task: Ultra-long temporal video language understanding benchmark
    - Link: https://github.com/egoschema/EgoSchema

#### Specialized Domain Datasets
+  **EgoExOR**
    - Release: NeurIPS 2025
    - Scale: Operating room wearable video synchronized with surgical tool tracking & patient biometrics
    - Core Task: Surgical workflow recognition, Instrument detection
    - Link: https://arxiv.org/pdf/2505.24287
+  **EgoDex**
    - Release: 2025
    - Scale: Apple Vision Pro captured daily object manipulation sequences with precise 6D hand pose annotations
    - Core Task: Dexterous wearable hand pose estimation & manipulation forecasting
    - Link: https://arxiv.org/abs/2505.11709
+  **MECCANO**
    - Release: 2021
    - Scale: 12 h industrial assembly footage paired with eye-tracking streams
    - Core Task: Industrial fine-grained action & hand-object interaction analysis
    - Link: https://github.com/fpv-iplab/MECCANO
+  **EgoExo-Fitness**
    - Release: ECCV 2024
    - Scale: Fitness sequence videos recorded from synchronized egocentric and fixed exocentric cameras
    - Core Task: Full-body action understanding
    - Link: [GitHub](https://github.com/iSEE-Laboratory/EgoExo-Fitness)

### Embodied VLA Evaluation Benchmarks
+  **EgoVerse**
    - Release: 2026
    - Scale: 1,000+ standardized embodied tasks covering navigation, manipulation and visual QA
    - Core Task: Unified robotic imitation & wearable VLA evaluation suite
    - Link: https://arxiv.org/pdf/2604.07607
+  **EgoBench**
    - Release: 2026
    - Scale: Interactive closed-loop evaluation platform for wearable embodied agents
    - Core Task: Real-time interactive decision-making benchmark
    - Link: https://arxiv.org/pdf/2605.27820

### Egocentric World Simulators
+  **PlayerOne**
    - Release: NeurIPS 2025
    - Highlights: Photorealistic open-world egocentric simulator with full camera, human motion and object interaction control for synthetic data generation
    - Link: https://arxiv.org/abs/2512.06724
+  **EgoSim**
    - Release: arXiv 2026
    - Highlights: Closed-loop dynamic simulator with persistent 3D scene states for generating consistent sequential interaction footage
    - Link: https://arxiv.org/pdf/2604.01001

---

## 👓 Smart Glasses Exclusive Research & Deployment

### Specialized Benchmarks & Wearable Datasets
+  **SUPERGLASSES: Benchmarking Vision Language Models as Intelligent Agents for AI Smart Glasses**
    - Publication: CVPR 2026
    - Highlights: First real consumer smart glasses benchmark collected across Ray-Ban Meta, Xiaomi Smart Glasses and Thunderbird V4 with diverse daily scenarios
    - Paper Link: [arXiv](https://arxiv.org/pdf/2602.22683)
+  **Project Aria Datasets**
    - Publisher: Meta Research
    - Highlights: Full multimodal wearable dataset suite with synchronized RGB, depth, IMU and eye-tracking signals
    - Official Link: https://www.projectaria.com/

### Key Technical Research Directions
#### Low-Power On-Device Perception
+  **OpenGlass: Ultra-Low-Power On-Device AI Eyewear with Event-based Vision**
    - Publication: arXiv 2026
    - Highlights: Fully open-source event camera wearable hardware stack paired with lightweight edge inference algorithms
    - Paper Link: [arXiv](https://arxiv.org/pdf/2606.07431)
+  **EgoTrigger: Toward Audio-Driven Image Capture for Human Memory Enhancement in All-Day Energy-Efficient Smart Glasses**
    - Affiliation: UNC Chapel Hill + Google
    - Publication: IEEE TVCG 2025
    - Highlights: Audio-event triggered selective frame capture reducing total power consumption by 87%
    - Paper Link: [arXiv](https://arxiv.org/pdf/2508.01915)

#### Lifelong Memory & Personal Assistant Systems
+  **EGAgent: Agentic Very Long Video Understanding**
    - Publication: arXiv 2026
    - Highlights: Entity scene graph based reasoning agent handling cross-day continuous wearable video streams with multi-hop retrieval and audio-visual hybrid search
    - Paper Link: [arXiv](https://arxiv.org/abs/2601.18157)

#### Natural Wearable Human-Computer Interaction
+  **VisionClaw: Always-On AI Agents Through Smart Glasses**
    - Publication: arXiv 2026
    - Highlights: Persistent background wearable agent enabling hands-free multi-scenario task execution
    - Paper Link: [arXiv](https://arxiv.org/pdf/2604.03486)
+  **Egocentric Co-Pilot: Web-Native Lightweight Smart Glasses Assistant**
    - Publication: WWW 2026
    - Highlights: Browser-based lightweight wearable assistant architecture requiring no native app installation
    - Paper Link: [arXiv](https://arxiv.org/pdf/2603.01104)
+  **Plug-and-Play Clarifier: A Zero-Shot Multimodal Framework for Egocentric Intent Disambiguation**
    - Publication: AAAI 2026
    - Highlights: Zero-shot intent resolution framework boosting wearable instruction execution accuracy from 58% to 87%
    - Paper Link: [arXiv](https://arxiv.org/pdf/2511.08971)

---

## 🔗 Related Awesome Lists
- [Awesome-Egocentric](https://github.com/EgoAlpha/Awesome-Egocentric)
- [awesome-egocentric-vision](https://github.com/Sid2697/awesome-egocentric-vision)
- [Awesome-Egocentric-and-Exocentric-Vision](https://github.com/ayiyayi/Awesome-Egocentric-and-Exocentric-Vision)
- [Building Egocentric Procedural AI Assistant](https://github.com/z1oong/Building-Egocentric-Procedural-AI-Assistant)

---

## 🎯 Key Research Challenges

### Universal Foundational Challenges Across All Subtasks
1. **Intrinsic Egocentric Visual Defects**: Narrow field-of-view, severe self-occlusion, violent camera shake, unstable lighting and blurry wearable imagery degrade all downstream tasks.
2. **Egocentric Data Scarcity & Privacy Barriers**: Wearable footage carries sensitive personal information; collection and annotation costs are drastically higher than internet third-person video, creating an order-of-magnitude dataset size gap limiting large model scaling. Cross-view collaborative scenarios further amplify privacy risks.
3. **Severe Inter-Person Distribution Shift**: Large variance in user height, daily behavior patterns and household environments leads to poor generalization of generic models on personalized wearable scenarios.
4. **Ultra-Long Sequential Modeling Bottlenecks**: Continuous all-day wearable streaming poses critical memory capacity and long-range dependency modeling challenges for existing video and multimodal architectures.

### Domain-Specific Core Challenges
| Research Direction | Core Open Challenges |
| :--- | :--- |
| Action Recognition & Anticipation | Fine-grained verb-noun compositional ambiguity, Low temporal localization precision on untrimmed long footage |
| Hand-Object Interaction (HOI) | High annotation cost for contact states, Hard to model physical consistency constraints, Heavy mutual occlusion between hands and objects |
| Ego-VLM & Multimodal Reasoning | Lack of first-person common sense priors, Weak spatio-temporal multi-step reasoning, Cross-modal alignment and synchronization, Handling missing modalities |
| Long-Form Video & Structured Reasoning | Limited model context windows, Fuzzy temporal event localization, Scalable scene graph construction from long videos |
| Gaze & User Intention Prediction | High inter-individual variance in eye movement patterns, Implicit human intent is difficult to label, Weak multimodal signal alignment |
| 3D/4D Reconstruction & Structured Perception | Monocular depth ambiguity, Dynamic moving object reconstruction failure, Dynamic scene graph updating |
| Ego-VLA & Embodied AI | Large human-robot embodiment domain gap, Misaligned action spaces, Policy transfer from human to robot, Sim-to-real generalization |
| Egocentric World Models | Temporal consistency degradation over long rollouts, Trade-off between generation realism and physical plausibility, Weak user action controllability |
| Egocentric Procedural AI Assistant | Fine-grained error boundary ambiguity, Procedural knowledge grounding difficulty, Real-time proactive intervention timing control |
| **Data Security & Privacy** | Balancing wearer vs. bystander privacy, Privacy-utility trade-off in data minimisation, Consent and regulatory compliance (GDPR), Privacy amplification in cross-view collaboration |

---

## ❤️ Contact
If you have paper/dataset suggestions, corrections or find this resource list useful, feel free to reach out to Yuanliang Sun via email: sun254667307@gmail.com.

## ⭐ Acknowledgements
This curated collection cross-references and builds upon multiple community egocentric vision repositories:
- Awesome-Egocentric-Video-Datasets
- Building Egocentric Procedural AI Assistant

## 📄 License
CC0 1.0 Universal. Full terms available in the `LICENSE` file of this repository.
