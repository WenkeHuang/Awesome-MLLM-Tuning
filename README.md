<p align="center">
<img src="./assert/Framework.jpg" width="700" alt="MLLM-Tuning" />
</p>

# <p align="center">Awesome-MLLM-Tuning</p>

<p align="center"><em>Curated list of Multimodal Large Language Model (MLLM) Tuning resources, aligned with our work:</em><br><strong>Keeping Yourself is Important in Downstream Tuning Multimodal Large Language Model</strong></p>

<p align="center">
<a href="https://arxiv.org/abs/2503.04543"><img src="https://img.shields.io/badge/arXiv-2502.14881-b31b1b.svg" alt="arXiv Badge"></a>
<img src="https://badges.toozhao.com/badges/01JNMP5KB247X0F52D94216CT0/blue.svg" alt="Custom Badge" />
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
| 2024.12 | **Revisiting Weight Averaging for Model Merging** | arXiv'24 | [link](https://arxiv.org/abs/2412.12153) | [link](https://github.com/JH-GEECS/CART_public) |
| 2024.10 | **Parameter Competition Balancing for Model Merging** | NeurIPS'24 | [link](https://arxiv.org/abs/2410.02396) | [link](https://github.com/duguodong7/pcb-merging) |
| 2024.06 | **Twin-Merging: Dynamic Integration of Modular Expertise in Model Merging** | NeurIPS'24 | [link](https://arxiv.org/abs/2406.15479) | [link](https://github.com/LZY-the-boys/Twin-Merging) |
| 2024.05 | **TEMR-Merging: Tuning-Free High-Performance Model Merging** | NeurIPS'24 | [link](https://arxiv.org/abs/2405.17461) | [link](https://github.com/harveyhuang18/emr_merging) |
| 2024.02 | **Model Tailor: Mitigating Catastrophic Forgetting in Multi-modal Large Language Models** | ICML'24 | [link](https://arxiv.org/abs/2402.12048) | [link](https://github.com/didizhu-zju/Model-Tailor) |
| 2023.11 | **Language Models are Super Mario: Absorbing Abilities from Homologous Models as a Free Lunch** | ICML'24 | [link](https://arxiv.org/abs/2311.03099) | [link](https://github.com/yule-buaa/mergelm) |
| 2023.06 | **TIES-Merging: Resolving Interference When Merging Models** | NeurIPS'23 | [link](https://arxiv.org/abs/2306.01708) | [link](https://github.com/prateeky2806/ties-merging) |
| 2021.11 | **Merging Models with Fisher-Weighted Averaging** | NeurIPS'22 | [link](https://arxiv.org/abs/2111.09832) | [link](https://github.com/mmatena/model_merging) |


### Reparameterization Tuning

#### Structure Reparameterization Tuning

| Time    | Title                                                        | Venue | Paper | Code |
| ------- | ------------------------------------------------------------ | :---: | :---: | :--: |
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
| 2025.03 | **Lorasculpt: Sculpting lora for harmonizing general and specialized knowledge in multimodal large language models** | CVPR'25 | [link](https://arxiv.org/abs/2503.16843) | [link](https://github.com/LiangJian24/LoRASculpt) |
| 2024.10 | **Controlled low-rank adaptation with subspace regularization for continued training on large language models** | arXiv'24 | [link](https://arxiv.org/abs/2410.16801) | - |
| 2024.07 | **Learn to preserve and diversify: Parameter-efficient group with orthogonal regularization for domain generalization** | ECCV'24 | [link](https://arxiv.org/abs/2407.15085) | [link](https://github.com/JudgingH/PEGO) |
| 2024.06 | **Corda: Context-oriented decomposition adaptation of large language models for task-aware parameter-efficient fine-tuning** | NeurIPS'24 | [link](https://arxiv.org/abs/2406.05223) | [link](https://github.com/iboing/CorDA) |
| 2024.06 | **Milora: Harnessing minor singular components for parameter-efficient llm finetuning** | NAACL'25 | [link](https://arxiv.org/abs/2406.09044) | [link](https://github.com/sufenlp/MiLoRA) |
| 2024.04 | **Pissa: Principal singular values and singular vectors adaptation of large language models** | NeurIPS'24 | [link](https://arxiv.org/abs/2404.02948) | [link](https://github.com/GraphPKU/PiSSA) |
| 2024.03 | **Lora meets dropout under a unified framework** | ACL'24 | [link](https://arxiv.org/abs/2403.00812) | - |
| 2024.03 | **Bilora: A bi-level optimization framework for overfitting-resilient low-rank adaptation of large pre-trained models** | arXiv'24 | [link](https://arxiv.org/abs/2403.13037) | - |
| 2024.02 | **Melora: mini-ensemble low-rank adapters for parameterefficient fine-tuning** | ACL'24 | [link](https://arxiv.org/abs/2402.17263) | [link](https://github.com/ChasonShi/MELoRA) |
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
