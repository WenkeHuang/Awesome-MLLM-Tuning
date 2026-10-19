<p align="center">
<img src="./assert/Framework.jpg" width="700" alt="MLLM-Tuning" />
</p>

# <p align="center">Awesome-MLLM-Tuning</p>

<p align="center"><em>Curated list of Multimodal Large Language Model (MLLM) Tuning resources, aligned with our work:</em><br><strong>Keeping Yourself is Important in Downstream Tuning Multimodal Large Language Model</strong></p>

<p align="center">
<a href="https://arxiv.org/abs/2503.04543"><img src="https://img.shields.io/badge/arXiv-2502.14881-b31b1b.svg" alt="arXiv Badge"></a>
<a href="https://creativecommons.org/licenses/by-nc/4.0/"><img src="https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg" alt="License Badge"></a>
<a href="https://github.com/WenkeHuang/Awesome-MLLM-Tuning"><img src="https://img.shields.io/github/stars/WenkeHuang/Awesome-MLLM-Tuning?style=social" alt="GitHub stars"></a>
</p>

## 🙌 Abstract

Multi-modal Large Language Models (MLLMs) integrate visual and linguistic reasoning to address complex tasks such as image captioning and visual question answering. While MLLMs demonstrate remarkable versatility, MLLMs appears limited performance on special application. But tuning MLLMs for downstream tasks encounters two key challenges: Task-Expert Specialization, where distribution shifts between pre-training and target datasets constrain target performance, and Open-World Stabilization, where catastrophic forgetting erases the model general knowledge. In this work, we systematically review recent advancements in MLLM tuning methodologies, classifying them into three paradigms: (I) Selective Tuning, (II) Additive Tuning, and (III) Reparameterization Tuning. Furthermore, we benchmark these tuning strategies across popular MLLM architectures and diverse downstream tasks to establish standardized evaluation analysis and systematic tuning principles. Finally, we highlight several open challenges in this domain and propose future research directions.

## 📖 Paper

### Selective Tuning

#### Iterative Selective Tuning

| Time    | Title                                                        | Venue | Paper | Code |
| ------- | ------------------------------------------------------------ | :---: | :---: | :--: |
| 2026.06 | **Harmonious Parameter Adaptation in Continual Visual Instruction Tuning for Safety-Aligned MLLMs** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Wang_Harmonious_Parameter_Adaptation_in_Continual_Visual_Instruction_Tuning_for_Safety-Aligned_CVPR_2026_paper.html) | [link](https://github.com/Minato-Zackie/HPA) |
| 2025.10 | **TR-PTS: Task-Relevant Parameter and Token Selection for Efficient Tuning** | ICCV'25 | [link](https://openaccess.thecvf.com/content/ICCV2025/html/Luo_TR-PTS_Task-Relevant_Parameter_and_Token_Selection_for_Efficient_Tuning_ICCV_2025_paper.html) | [link](https://github.com/synbol/TR-PTS) |
| 2025.10 | **SAFER: Sharpness Aware layer-selective Finetuning for Enhanced Robustness in vision transformers** | ICCV'25 | [link](https://openaccess.thecvf.com/content/ICCV2025/html/Gopal_SAFER_Sharpness_Aware_layer-selective_Finetuning_for_Enhanced_Robustness_in_vision_ICCV_2025_paper.html) | - |
| 2025.06 | **Skip Tuning: Pre-trained Vision-Language Models are Effective and Efficient Adapters Themselves** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Wu_Skip_Tuning_Pre-trained_Vision-Language_Models_are_Effective_and_Efficient_Adapters_CVPR_2025_paper.html) | [link](https://github.com/Koorye/SkipTuning) |
| 2025.06 | **Adaptive Parameter Selection for Tuning Vision-Language Models** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Zhang_Adaptive_Parameter_Selection_for_Tuning_Vision-Language_Models_CVPR_2025_paper.html) | - |
| 2024.10 | **AlphaEdit: Null-Space Constrained Knowledge Editing for Language Models** | ICLR'24 | [link](https://arxiv.org/abs/2410.02355) | [link](https://github.com/jianghoucheng/alphaedit) |
| 2023.12 | **Sparse is Enough in Fine-tuning Pre-trained Large Language Models** | ICML'24 | [link](https://arxiv.org/abs/2312.11875) | [link](https://github.com/song-wx/sift) |
| 2023.12 | **Gradient-based Parameter Selection for Efficient Fine-Tuning** | CVPR'24 | [link](https://arxiv.org/abs/2312.10136) | [link](https://arxiv.org/abs/2312.10136) |
| 2023.11 | **Unified Low-Resource Sequence Labeling by Sample-Aware Dynamic Sparse Finetuning** | EMNLP'23 | [link](https://arxiv.org/abs/2311.03748) | [link](https://github.com/psunlpgroup/fish-dip) |
| 2023.08 | **Overcoming Generic Knowledge Loss with Selective Parameter Update** | CVPR'24 | [link](https://arxiv.org/abs/2308.12462) | [link](https://github.com/wx-zhang/spu) |
| 2023.06 | **LoSparse: Structured Compression of Large Language Models based on Low-Rank and Sparse Approximation** | ICML'23 | [link](https://arxiv.org/abs/2306.11222) | [link](https://github.com/yxli2123/LoSparse) |
| 2022.10 | **ROSE: Robust Selective Fine-tuning for Pre-trained Language Models** | IJCAI'22 | [link](https://arxiv.org/abs/2210.09658) | [link](https://github.com/jiangllan/rose) |
| 2022.05 | **Parameter-Efficient Sparsity for Large Language Models Fine-Tuning** | IJCAI'22 | [link](https://arxiv.org/abs/2205.11005) | [link](https://github.com/alibaba/AliceMind) |
| 2021.10 | **Composable Sparse Fine-Tuning for Cross-Lingual Transfer** | ACL'22 | [link](https://arxiv.org/abs/2110.07560) | [link](https://github.com/cambridgeltl/composable-sft) |
| 2021.09 | **Raise a Child in Large Language Model: Towards Effective and Generalizable Fine-tuning** | EMNLP'21 | [link](https://arxiv.org/abs/2109.05687) | [link](https://github.com/alibaba/AliceMind) |
| 2015.06 | **Learning both Weights and Connections for Efficient Neural Networks** | NeurIPS'15 | [link](https://arxiv.org/abs/1506.02626) | - |


#### Posterior Selective Tuning

| Time    | Title                                                        | Venue | Paper | Code |
| ------- | ------------------------------------------------------------ | :---: | :---: | :--: |
| 2026.06 | **Label-Free Cross-Task LoRA Merging with Null-Space Compression** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Lee_Label-Free_Cross-Task_LoRA_Merging_with_Null-Space_Compression_CVPR_2026_paper.html) | [link](https://github.com/wonyoung01/nsc_merging) |
| 2026.06 | **DuetMerging: Synergizing Dynamic and Static Strategies for Mitigating Task Interference in Model Merging** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Li_DuetMerging_Synergizing_Dynamic_and_Static_Strategies_for_Mitigating_Task_Interference_CVPR_2026_paper.html) | - |
| 2026.06 | **DC-Merge: Improving Model Merging with Directional Consistency** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_DC-Merge_Improving_Model_Merging_with_Directional_Consistency_CVPR_2026_paper.html) | [link](https://github.com/Tobeginwith/DC-Merge) |
| 2026.06 | **ACE-Merging: Data-Free Model Merging with Adaptive Covariance Estimation** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Xu_ACE-Merging_Data-Free_Model_Merging_with_Adaptive_Covariance_Estimation_CVPR_2026_paper.html) | [link](https://github.com/unravel-xu/ACE-Merging/tree/main) |
| 2025.06 | **Task Singular Vectors: Reducing Task Interference in Model Merging** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Gargiulo_Task_Singular_Vectors_Reducing_Task_Interference_in_Model_Merging_CVPR_2025_paper.html) | [link](https://github.com/AntoAndGar/task_singular_vectors) |
| 2025.06 | **IterIS: Iterative Inference-Solving Alignment for LoRA Merging** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Chen_IterIS_Iterative_Inference-Solving_Alignment_for_LoRA_Merging_CVPR_2025_paper.html) | - |
| 2025.06 | **AdaMMS: Model Merging for Heterogeneous Multimodal Large Language Models with Unsupervised Coefficient Optimization** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Du_AdaMMS_Model_Merging_for_Heterogeneous_Multimodal_Large_Language_Models_with_CVPR_2025_paper.html) | [link](https://github.com/THUNLP-MT/AdaMMS) |
| 2024.12 | **Revisiting Weight Averaging for Model Merging** | arXiv'24 | [link](https://arxiv.org/abs/2412.12153) | [link](https://github.com/JH-GEECS/CART_public) |
| 2024.10 | **Parameter Competition Balancing for Model Merging** | NeurIPS'24 | [link](https://arxiv.org/abs/2410.02396) | [link](https://github.com/duguodong7/pcb-merging) |
| 2024.06 | **Twin-Merging: Dynamic Integration of Modular Expertise in Model Merging** | NeurIPS'24 | [link](https://arxiv.org/abs/2406.15479) | [link](https://github.com/LZY-the-boys/Twin-Merging) |
| 2024.05 | **TEMR-Merging: Tuning-Free High-Performance Model Merging** | NeurIPS'24 | [link](https://arxiv.org/abs/2405.17461) | [link](https://github.com/harveyhuang18/emr_merging) |
| 2024.02 | **Model Tailor: Mitigating Catastrophic Forgetting in Multi-modal Large Language Models** | ICML'24 | [link](https://arxiv.org/abs/2402.12048) | [link](https://github.com/didizhu-zju/Model-Tailor) |
| 2023.11 | **Language Models are Super Mario: Absorbing Abilities from Homologous Models as a Free Lunch** | ICML'24 | [link](https://arxiv.org/abs/2311.03099) | [link](https://github.com/yule-buaa/mergelm) |
| 2023.06 | **TIES-Merging: Resolving Interference When Merging Models** | NeurIPS'23 | [link](https://arxiv.org/abs/2306.01708) | [link](https://github.com/prateeky2806/ties-merging) |
| 2021.11 | **Merging Models with Fisher-Weighted Averaging** | NeurIPS'22 | [link](https://arxiv.org/abs/2111.09832) | [link](https://github.com/mmatena/model_merging) |

### Additive Tuning



#### Adapter Tuning
| Time    | Title                                                        | Venue |                  Paper                   |                             Code                             |
| ------- | ------------------------------------------------------------ | :---: | :--------------------------------------: | :----------------------------------------------------------: |
| 2026.06 | **PACT: Phase-Like Transition Constraints in Adapter-Based Continual Learning of Vision-Language Models** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Wang_PACT_Phase-Like_Transition_Constraints_in_Adapter-Based_Continual_Learning_of_Vision-Language_CVPR_2026_paper.html) | - |
| 2026.06 | **CoVFT: Context-aware Visual Fine-tuning for Multimodal Large Language Models** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Zhou_CoVFT_Context-aware_Visual_Fine-tuning_for_Multimodal_Large_Language_Models_CVPR_2026_paper.html) | [link](https://github.com/weeknan/CoVFT) |
| 2026.06 | **Beyond Graph Model: Reliable VLM Fine-Tuning via Random Graph Adapter** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Jiang_Beyond_Graph_Model_Reliable_VLM_Fine-Tuning_via_Random_Graph_Adapter_CVPR_2026_paper.html) | - |
| 2025.06 | **Minimal Interaction Seperated Tuning: A New Paradigm for Visual Adaptation** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Tang_Minimal_Interaction_Seperated_Tuning_A_New_Paradigm_for_Visual_Adaptation_CVPR_2025_paper.html) | - |
| 2025.06 | **Faster Parameter-Efficient Tuning with Token Redundancy Reduction** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Kim_Faster_Parameter-Efficient_Tuning_with_Token_Redundancy_Reduction_CVPR_2025_paper.html) | - |
| 2025.06 | **5%>100%: Breaking Performance Shackles of Full Fine-Tuning on Visual Recognition Tasks** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Yin_5100_Breaking_Performance_Shackles_of_Full_Fine-Tuning_on_Visual_Recognition_CVPR_2025_paper.html) | [link](https://github.com/Leiyi-Hu/mona) |
| 2024.04 | **Conditional Prototype Rectification Prompt Learning** | TCSVT'25  | [link](https://arxiv.org/abs/2404.09872) | [link](https://github.com/chenhaoxing/CPR) |
| 2023.11 | **Meta-Adapter: An Online Few-shot Learner for Vision-Language Model** | NeurIPS'23  | [link](https://arxiv.org/abs/2311.03774) | [link](https://github.com/ArsenalCheng/Meta-Adapter) |
| 2023.09 | **GraphAdapter: Tuning Vision-Language Models With Dual Knowledge Graph** | NeurIPS'23  | [link](https://arxiv.org/abs/2309.13625) | [link](https://github.com/lixinustc/GraphAdapter) |
| 2023.04 | **Not All Features Matter: Enhancing Few-shot CLIP with Adaptive Prior Refinement** | ICCV'23  | [link](https://arxiv.org/abs/2304.01195) | [link](https://github.com/yangyangyang127/APE) |
| 2023.03 | **Revisiting Multimodal Representation in Contrastive Learning: From Patch and Token Embeddings to Finite Discrete Tokens** | CVPR'23  | [link](https://arxiv.org/abs/2303.14865) | [link](https://github.com/yuxiaochen1103/FDT) |
| 2023.02 | **Side Adapter Network for Open-Vocabulary Semantic Segmentation** | CVPR'23  | [link](https://arxiv.org/abs/2302.12242) | [link](https://github.com/MendelXu/SAN) |
| 2022.11 | **Task Residual for Tuning Vision-Language Models** | CVPR'23  | [link](https://arxiv.org/abs/2211.10277) | [link](https://github.com/geekyutao/TaskRes) |
| 2022.06 | **LST: Ladder Side-Tuning for Parameter and Memory Efficient Transfer Learning** | NeurIPS'22 | [link](https://arxiv.org/abs/2206.06522) | [link](https://github.com/ucinlp/autoprompt) |
| 2021.11 | **Tip-Adapter: Training-free CLIP-Adapter for Better Vision-Language Modeling** |  ECCV'22 | [link](https://arxiv.org/abs/2111.03930) | [link](https://github.com/gaopengcuhk/Tip-Adapter) |
| 2021.10 | **CLIP-Adapter: Better Vision-Language Models with Feature Adapters** | IJCV'23  | [link](https://arxiv.org/abs/2110.04544) | [link](https://github.com/gaopengcuhk/CLIP-Adapter) |
| 2019.02 | **Parameter-Efficient Transfer Learning for NLP** | ICML'19  | [link](https://arxiv.org/abs/1902.00751) | [link](https://github.com/cs-mshah/Adapter-Bert) |


#### Prompt Tuning
| Time    | Title                                                        | Venue |                  Paper                   |                             Code                             |
| ------- | ------------------------------------------------------------ | :---: | :--------------------------------------: | :----------------------------------------------------------: |
| 2026.06 | **SoC: Semantic Orthogonal Calibration for Test-Time Prompt Tuning** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Fillioux_SoC_Semantic_Orthogonal_Calibration_for_Test-Time_Prompt_Tuning_CVPR_2026_paper.html) | - |
| 2026.06 | **Improving Calibration in Test-Time Prompt Tuning for Vision-Language Models via Data-Free Flatness-Aware Prompt Pretraining** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Jang_Improving_Calibration_in_Test-Time_Prompt_Tuning_for_Vision-Language_Models_via_CVPR_2026_paper.html) | [link](https://github.com/YonseiML/fpp) |
| 2026.06 | **CAPT: Confusion-Aware Prompt Tuning for Reducing Vision-Language Misalignment** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Shao_CAPT_Confusion-Aware_Prompt_Tuning_for_Reducing_Vision-Language_Misalignment_CVPR_2026_paper.html) | [link](https://github.com/greatest-gourmet/CAPT) |
| 2025.10 | **Hierarchical Cross-modal Prompt Learning for Vision-Language Models** | ICCV'25 | [link](https://openaccess.thecvf.com/content/ICCV2025/html/Zheng_Hierarchical_Cross-modal_Prompt_Learning_for_Vision-Language_Models_ICCV_2025_paper.html) | [link](https://github.com/zzeoZheng/HiCroPL) |
| 2025.06 | **O-TPT: Orthogonality Constraints for Calibrating Test-time Prompt Tuning in Vision-Language Models** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Sharifdeen_O-TPT_Orthogonality_Constraints_for_Calibrating_Test-time_Prompt_Tuning_in_Vision-Language_CVPR_2025_paper.html) | [link](https://github.com/ashshaksharifdeen/O-TPT) |
| 2025.06 | **NLPrompt: Noise-Label Prompt Learning for Vision-Language Models** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Pan_NLPrompt_Noise-Label_Prompt_Learning_for_Vision-Language_Models_CVPR_2025_paper.html) | [link](https://github.com/qunovo/NLPrompt) |
| 2025.06 | **DPC: Dual-Prompt Collaboration for Tuning Vision-Language Models** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Li_DPC_Dual-Prompt_Collaboration_for_Tuning_Vision-Language_Models_CVPR_2025_paper.html) | [link](https://github.com/JREion/DPC) |
| 2024.03 | **PromptKD: Unsupervised Prompt Distillation for Vision-Language Models** |  CVPR'24  | [link](https://arxiv.org/abs/2403.02781) | [link](https://github.com/zhengli97/PromptKD) |
| 2024.03 | **Domain-agnostic mutual prompting for unsupervised domain adaptation** |  CVPR'24  | [link](https://arxiv.org/abs/2403.02899) | [link](https://github.com/TL-UESTC/DAMP) |
| 2024.01 | **Learning to prompt with text only supervision for vision-language models** |  AAAI'25  | [link](https://arxiv.org/abs/2401.02418) | [link](https://github.com/muzairkhattak/ProText) |
| 2023.11 | **ArGue: Attribute-guided prompt tuning for vision-language models** |  CVPR'24  | [link](https://arxiv.org/abs/2311.16494) | [link](https://github.com/xytian1008/ArGue) |
| 2023.09 | **Dept: Decoupled prompt tuning** |  CVPR'24  | [link](https://arxiv.org/abs/2309.07439) | [link](https://github.com/Koorye/DePT) |
| 2023.09 | **Distribution-aware prompt tuning for vision-language models** |  ICCV'23  | [link](https://arxiv.org/abs/2309.03406) | [link](https://github.com/mlvlab/DAPT) |
| 2023.08 | **Knowledge-aware prompt tuning for generalizable vision-language models** |  ICCV'23  | [link](https://arxiv.org/abs/2308.11186) | - |
| 2023.07 | **Self-regulating prompts: Foundational model adaptation without forgetting** |  ICCV'23  | [link](https://arxiv.org/abs/2307.06948) | [link](https://github.com/muzairkhattak/PromptSRC) |
| 2023.03 | **Visual-language prompt tuning with knowledge-guided context optimization** |  CVPR'23  | [link](https://arxiv.org/abs/2303.13283) | [link](https://github.com/htyao89/KgCoOp) |
| 2022.10 | **MaPLe: Multi-modal prompt learning** |  CVPR'23  | [link](https://arxiv.org/abs/2210.03117) | [link](https://github.com/muzairkhattak/multimodal-prompt-learning) |
| 2022.10 | **Prompt learning with optimal transport for vision-language models** |  ICLR'23  | [link](https://arxiv.org/abs/2210.01253) | [link](https://github.com/CHENGY12/PLOT) |
| 2022.06 | **Dualcoop: Fast adaptation to multi-label recognition with limited annotations** |  NeurIPS'22  | [link](https://arxiv.org/abs/2206.09541) | [link](https://github.com/sunxm2357/DualCoOp) |
| 2022.05 | **Prompt-aligned Gradient for Prompt Tuning** |  ICCV'23  | [link](https://arxiv.org/abs/2205.14865) | [link](https://github.com/BeierZhu/Prompt-align) |
| 2022.03 | **Visual prompt tuning** |  ECCV'22  | [link](https://arxiv.org/abs/2203.12119) | [link](https://github.com/KMnP/vpt) |
| 2022.03 | **Conditional prompt learning for vision-language models** |  CVPR'22  | [link](https://arxiv.org/abs/2203.05557) | [link](https://github.com/KaiyangZhou/CoOp) |
| 2021.09 | **Learning to prompt for vision-language models** |  IJCV'22  | [link](https://arxiv.org/abs/2109.01134) | [link](https://github.com/KaiyangZhou/CoOp) |
| 2021.01 | **Prefix-Tuning: Optimizing Continuous Prompts for Generation** | ACL'21  | [link](https://arxiv.org/abs/2101.00190) | [link](http://github.com/XiangLi1999/PrefixTuning) |
| 2020.10 | **AUTOPROMPT: Eliciting Knowledge from Language Models with Automatically Generated Prompts** | EMNLP'20  | [link](https://arxiv.org/abs/2010.15980) | [link](https://github.com/ucinlp/autoprompt) |
| 2019.11 | **How Can We Know What Language Models Know?** | TACL'20  | [link](https://arxiv.org/abs/1911.12543) | [link](https://github.com/jzbjyb/LPAQA) |



### Reparameterization Tuning

#### Structure Reparameterization Tuning

| Time    | Title                                                        | Venue | Paper | Code |
| ------- | ------------------------------------------------------------ | :---: | :---: | :--: |
| 2026.06 | **Sparse Spectral LoRA: Routed Experts for Medical VLMs** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Nejatimanzari_Sparse_Spectral_LoRA_Routed_Experts_for_Medical_VLMs_CVPR_2026_paper.html) | - |
| 2026.06 | **S2FT: Parameter-Efficient Fine-Tuning in Sparse Spectrum Domain** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_S2FT_Parameter-Efficient_Fine-Tuning_in_Sparse_Spectrum_Domain_CVPR_2026_paper.html) | - |
| 2026.06 | **Parameter-Efficient Adaptation for MLLMs via Implicit Modality Decomposition** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Zhang_Parameter-Efficient_Adaptation_for_MLLMs_via_Implicit_Modality_Decomposition_CVPR_2026_paper.html) | [link](https://github.com/mmffzzz/IMoD) |
| 2025.10 | **SMoLoRA: Exploring and Defying Dual Catastrophic Forgetting in Continual Visual Instruction Tuning** | ICCV'25 | [link](https://openaccess.thecvf.com/content/ICCV2025/html/Wang_SMoLoRA_Exploring_and_Defying_Dual_Catastrophic_Forgetting_in_Continual_Visual_ICCV_2025_paper.html) | [link](https://github.com/Minato-Zackie/SMoLoRA) |
| 2025.10 | **From Holistic to Localized: Local Enhanced Adapters for Efficient Visual Instruction Fine-Tuning** | ICCV'25 | [link](https://openaccess.thecvf.com/content/ICCV2025/html/Jiao_From_Holistic_to_Localized_Local_Enhanced_Adapters_for_Efficient_Visual_ICCV_2025_paper.html) | [link](https://github.com/pengkun-jiao/FHTC) |
| 2025.04 | **RandLoRA: Full rank parameter-efficient fine-tuning of large models** | ICLR'25 | [link](https://proceedings.iclr.cc/paper_files/paper/2025/hash/382b95a6580cfb0b5ca33c74b4e0e770-Abstract-Conference.html) | [link](https://github.com/PaulAlbert31/RandLoRA) |
| 2025.02 | **REMEDY: Recipe merging dynamics in large vision-language models** | ICLR'25 | [link](https://openreview.net/forum?id=iX7eHHE5Tx) | - |
| 2024.12 | **Lora.rar: Learning to merge loras via hypernetworks for subject-style conditioned image generation** | ICCV'25 | [link](https://arxiv.org/abs/2412.05148) | [link](https://github.com/donaldssh/LoRA.rar) |
| 2024.08 | **Teamlora: Boosting low-rank adaptation with expert collaboration and competition** | arXiv'24 | [link](https://arxiv.org/abs/2408.09856) | [link](https://github.com/Lin-Tianwei/TeamLoRA) |
| 2024.06 | **Twinmerging: Dynamic integration of modular expertise in model merging** | NeurIPS'24 | [link](https://arxiv.org/abs/2406.15479) | [link](https://github.com/LZY-the-boys/Twin-Merging) |
| 2024.06 | **Mixture-of-subspaces in low-rank adaptation** | EMNLP'24 | [link](https://arxiv.org/abs/2406.11909) | [link](https://github.com/wutaiqiang/MoSLoRA) |
| 2024.06 | **Sharelora: Parameter efficient and robust large language model fine-tuning via shared low-rank adaptation** | arXiv'24 | [link](https://arxiv.org/abs/2406.10785) | [link](https://github.com/Rain9876/ShareLoRA) |
| 2024.05 | **Parameter-Efficient Fine-Tuning with Discrete Fourier Transform** | ICML'24 | [link](https://arxiv.org/abs/2405.03003) | [link](https://github.com/Chaos96/fourierft) |
| 2024.03 | **Mtlora: Low-rank adaptation approach for efficient multi-task learning** | CVPR'24 | [link](https://arxiv.org/abs/2403.20320) | [link](https://github.com/scale-lab/MTLoRA) |
| 2024.02 | **Multimodal instruction tuning with conditional mixture of lora** | ACL'24 | [link](https://arxiv.org/abs/2402.15896) | [link](https://github.com/PLUM-Lab/MixLoRA) |
| 2023.12 | **Loramoe: Alleviating world knowledge forgetting in large language models via moe-style plugin** | ACL'24 | [link](https://arxiv.org/abs/2312.09979) | [link](https://github.com/Ablustrund/LoRAMoE) |
| 2023.10 | **Vera: Vectorbased random matrix adaptation** | ICLR'24 | [link](https://arxiv.org/abs/2310.11454) | [link](https://huggingface.co/docs/peft/main/en/package_reference/vera) |
| 2023.07 | **Lorahub: Efficient cross-task generalization via dynamic lora composition** | COLM'24 | [link](https://arxiv.org/abs/2307.13269) | [link](https://github.com/sail-sg/lorahub) |


#### Calibration Reparameterization Tuning

| Time    | Title                                                        | Venue | Paper | Code |
| ------- | ------------------------------------------------------------ | :---: | :---: | :--: |
| 2026.07 | **JANUS-LORA: A Balanced Low-Rank Adaptation for Continual Learning** | ICML'26 | [link](https://proceedings.mlr.press/v306/chen26fz.html) | - |
| 2026.07 | **Balanced LoRA: Removing Parameter Invariance to Accelerate Convergence** | ICML'26 | [link](https://proceedings.mlr.press/v306/castin26a.html) | [link](https://github.com/vcastin/balora) |
| 2026.06 | **FairLLaVA: Fairness-Aware Parameter-Efficient Fine-Tuning for Large Vision-Language Assistants** | CVPR'26 | [link](https://openaccess.thecvf.com/content/CVPR2026/html/Bhosale_FairLLaVA_Fairness-Aware_Parameter-Efficient_Fine-Tuning_for_Large_Vision-Language_Assistants_CVPR_2026_paper.html) | [link](https://github.com/bhosalems/FairLLaVA) |
| 2025.07 | **LoRA-One: One-Step Full Gradient Could Suffice for Fine-Tuning Large Language Models, Provably and Efficiently** | ICML'25 | [link](https://proceedings.mlr.press/v267/zhang25ax.html) | [link](https://github.com/YuanheZ/LoRA-One) |
| 2025.06 | **BiLoRA: Almost-Orthogonal Parameter Spaces for Continual Learning** | CVPR'25 | [link](https://openaccess.thecvf.com/content/CVPR2025/html/Zhu_BiLoRA_Almost-Orthogonal_Parameter_Spaces_for_Continual_Learning_CVPR_2025_paper.html) | - |
| 2025.04 | **LoRA-Pro: Are Low-Rank Adapters Properly Optimized?** | ICLR'25 | [link](https://proceedings.iclr.cc/paper_files/paper/2025/hash/ea184f920a0f0f8d8030aa1bd7ac9fd4-Abstract-Conference.html) | [link](https://github.com/mrflogs/LoRA-Pro) |
| 2025.04 | **LoRA Done RITE: Robust Invariant Transformation Equilibration for LoRA Optimization** | ICLR'25 | [link](https://proceedings.iclr.cc/paper_files/paper/2025/hash/bcbc0f660d2dde42f9d1d0ecb14a6f9a-Abstract-Conference.html) | - |
| 2025.04 | **Decoupling Angles and Strength in Low-rank Adaptation** | ICLR'25 | [link](https://proceedings.iclr.cc/paper_files/paper/2025/hash/3379ce104189b72d5f7baaa03ae81329-Abstract-Conference.html) | [link](https://github.com/ExplainableML/DeLoRA) |
| 2025.03 | **Lorasculpt: Sculpting lora for harmonizing general and specialized knowledge in multimodal large language models** | CVPR'25 | [link](https://arxiv.org/abs/2503.16843) | [link](https://github.com/LiangJian24/LoRASculpt) |
| 2024.10 | **Controlled low-rank adaptation with subspace regularization for continued training on large language models** | arXiv'24 | [link](https://arxiv.org/abs/2410.16801) | - |
| 2024.07 | **Learn to preserve and diversify: Parameter-efficient group with orthogonal regularization for domain generalization** | ECCV'24 | [link](https://arxiv.org/abs/2407.15085) | [link](https://github.com/JudgingH/PEGO) |
| 2024.06 | **Corda: Context-oriented decomposition adaptation of large language models for task-aware parameter-efficient fine-tuning** | NeurIPS'24 | [link](https://arxiv.org/abs/2406.05223) | [link](https://github.com/iboing/CorDA) |
| 2024.06 | **Milora: Harnessing minor singular components for parameter-efficient llm finetuning** | NAACL'25 | [link](https://arxiv.org/abs/2406.09044) | [link](https://github.com/sufenlp/MiLoRA) |
| 2024.04 | **Pissa: Principal singular values and singular vectors adaptation of large language models** | NeurIPS'24 | [link](https://arxiv.org/abs/2404.02948) | [link](https://github.com/GraphPKU/PiSSA) |
| 2024.03 | **Lora meets dropout under a unified framework** | ACL'24 | [link](https://arxiv.org/abs/2403.00812) | - |
| 2024.03 | **Bilora: A bi-level optimization framework for overfitting-resilient low-rank adaptation of large pre-trained models** | arXiv'24 | [link](https://arxiv.org/abs/2403.13037) | - |
| 2024.02 | **Melora: mini-ensemble low-rank adapters for parameter-efficient fine-tuning** | ACL'24 | [link](https://arxiv.org/abs/2402.17263) | [link](https://github.com/ChasonShi/MELoRA) |
| 2024.02 | **Prolora: Partial rotation empowers more parameter-efficient lora** | ACL'24 | [link](https://arxiv.org/abs/2402.16902) | [link](https://github.com/Forence1999/PRoLoRA) |
| 2024.02 | **Lora+: Efficient low rank adaptation of large models** | ICML'24 | [link](https://arxiv.org/abs/2402.12354) | [link](https://github.com/nikhil-ghosh-berkeley/loraplus) |
| 2024.02 | **Dora: Weight-decomposed low-rank adaptation** | ICML'24 | [link](https://arxiv.org/abs/2402.09353) | [link](https://github.com/NVlabs/DoRA) |
| 2024.02 | **Flora: Low-rank adapters are secretly gradient compressors** | ICML'24 | [link](https://arxiv.org/abs/2402.03293) | [link](https://github.com/BorealisAI/flora-opt) |
| 2023.08 | **Bayesian low-rank adaptation for large language models** | ICLR'24 | [link](https://arxiv.org/abs/2308.13111) | [link](https://github.com/MaximeRobeyns/bayesian_lora) |



## 👋 Contact

This repository is currently maintained by [Wenke Huang](https://wenkehuang.github.io/) 👨‍💻.  
If you have any questions, concerns, or suggestions regarding the contents of this repository or the resources shared here, feel free to reach out! I'm more than happy to assist you with any inquiries or help you navigate through the materials.  
Please don't hesitate to send an email to me at [wenkehuang@whu.edu.cn](mailto:wenkehuang@whu.edu.cn) 📧 or [Wechat](assert/wechat.jpg) 🤗.

## 🥳 Citation

If you find this repository helpful for your research, we would greatly appreciate it if you could cite our papers. ✨

```bibtex
@misc{MLLMTuning_arXiv25,
      title={Keeping Yourself is Important in Downstream Tuning Multimodal Large Language Model}, 
      author={Wenke Huang, Jian Liang, Xianda Guo, Yiyang Fang, Guancheng Wan, Xuankun Rong, Chi Wen, Zekun Shi,  Qingyun Li, Didi Zhu, Yanbiao Ma, Ke Liang, Bin Yang, He Li, Jiawei Shao, Mang Ye, Bo Du},
      year={2025},
      eprint={2503.04543},
      archivePrefix={arXiv},
      primaryClass={cs.CR}
}

@inproceedings{LiangLoRASculpt_CVPR2025,
    author    = {Liang, Jian and Huang, Wenke and Wan, Guancheng and Yang, Qu and Ye, Mang},
    title     = {LoRASculpt: Sculpting LoRA for Harmonizing General and Specialized Knowledge in Multimodal Large Language Models},
    booktitle = {CVPR},
    year      = {2025},
}

@inproceedings{FangSEPM_ICML2025,
  title     = {Catch Your Emotion: Sharpening Emotion Perception in Multimodal Large Language Models},
  author    = {Fang, Yiyang and Liang, Jian and Huang, Wenke and Li, He and Su, Kehua and Ye, Mang},
  booktitle = {ICML},
  year      = {2025},
}

@misc{ye2025surveysafetylargevisionlanguage,
      title={A Survey of Safety on Large Vision-Language Models: Attacks, Defenses and Evaluations}, 
      author={Mang Ye and Xuankun Rong and Wenke Huang and Bo Du and Nenghai Yu and Dacheng Tao},
      year={2025},
      eprint={2502.14881},
      archivePrefix={arXiv},
      primaryClass={cs.CR}
}
```




## 🔍 Relevant Projects
[1] LoRASculpt: Sculpting LoRA for Harmonizing General and Specialized Knowledge in Multimodal Large Language Models - CVPR 2025 [[Link](https://arxiv.org/abs/2503.16843)][[Code](https://github.com/LiangJian24/LoRASculpt)]

[2] Catch Your Emotion: Sharpening Emotion Perception in Multimodal Large Language Models - ICML 2025 [[Link](https://openreview.net/forum?id=IYOksPHJKT)][[Code](https://github.com/fuyyyyy/SEPM)]

[3] A Survey of Safety on Large Vision-Language Models: Attacks, Defenses and Evaluations - arXiv 2025 [[Link](https://arxiv.org/abs/2502.14881)][[Code](https://github.com/XuankunRong/Awesome-LVLM-Safety)]




**You Only Live Once.**

**I hope that all players have fun.**
