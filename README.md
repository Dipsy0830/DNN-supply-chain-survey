![img](imgs/vis.png)

# 深度学习模型供应链的安全性研究综述
这个 Github 存储库总结了深度学习模型供应链相关的资源。 有关更多详细信息和分类标准，请参阅我们的综述论文。

预训练模型解决了训练数据和算力受限的问题，已在各领域被广泛使用，它也催生了模型开发和应用的新范式——深度学习模型供应链。

模型经过设计和训练，由发布者上传至预训练模型仓库，由二次开发者进行迁移和压缩，部署到边缘端设备，并提供给用户使用。模型供应链引入了新环节和多要素，带来数据泄露风险和计算安全问题。

我们调研了相关的研究工作，根据模型生命周期的阶段，对模型设计、二次开发、部署和使用阶段的攻击和防御进行梳理和总结。
## 模型设计阶段的攻击
### 下游任务相关的攻击

Weight Poisoning Attacks on Pretrained Models [\[pdf\]](https://aclanthology.org/2020.acl-main.249/)  [\[code\]](https://github.com/neulab/RIPPLe)

Backdoor Attacks on Pre-trained Models by Layerwise Weight Poisoning  [\[pdf\]](https://aclanthology.org/2021.emnlp-main.241/)

Trojaning language models for fun and profit [\[pdf\]](https://ieeexplore.ieee.org/abstract/document/9581257/)  [\[code\]](https://github.com/alps-lab/trojan-lm)

Badprompt: Backdoor attacks on continuous prompts [\[pdf\]](https://proceedings.neurips.cc/paper_files/paper/2022/hash/f0722b58f02d7793acf7d328928f933a-Abstract-Conference.html)   [\[code\]](https://github.com/papersPapers/BadPrompt)

Badencoder: Backdoor attacks to pre-trained encoders in self-supervised learning  [\[pdf\]](https://ieeexplore.ieee.org/abstract/document/9833644/)   [\[code\]](https://github.com/jinyuan-jia/BadEncoder)

PoisonedEncoder: Poisoning the Unlabeled Pre-training Data in Contrastive Learning [\[pdf\]](https://www.usenix.org/conference/usenixsecurity22/presentation/liu-hongbin) 

CorruptEncoder: Data Poisoning based Backdoor Attacks to Contrastive Learning [\[pdf\]](https://arxiv.org/abs/2211.08229) 

### 下游任务无关的攻击

Model-reuse attacks on deep learning systems [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3243734.3243757)

Badpre: Task-agnostic backdoor attacks to pre-trained nlp foundation models [\[pdf\]](https://arxiv.org/abs/2110.02467)   [\[code\]](https://github.com/kangjie-chen/BadPre)

Red alarm for pre-trained models: Universal vulnerability to neuron-level backdoor attacks  [\[pdf\]](https://link.springer.com/article/10.1007/s11633-022-1377-5)   [\[code\]](https://github.com/thunlp/NeuBA)

Backdoor Pre-trained Models Can Transfer to All   [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3460120.3485370)

A Data-free Backdoor Injection Approach in Neural Networks  [\[pdf\]](https://www.usenix.org/system/files/sec23fall-prepub-573-lv.pdf)   [\[code\]](https://github.com/lvpeizhuo/Data-free_Backdoor)

NOTABLE: Transferable Backdoor Attacks Against Prompt-based NLP Models   [\[pdf\]](https://arxiv.org/abs/2305.17826)   [\[code\]](https://github.com/RU-System-Software-and-Security/Notable)

UOR: Universal Backdoor Attacks on Pre-trained Language Models  [\[pdf\]](https://arxiv.org/abs/2305.09574)

Training-free Lexical Backdoor Attacks on Language Models   [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3543507.3583348)   [\[code\]](https://github.com/Jinxhy/TFLexAttack)

Multi-target Backdoor Attacks for Code Pre-trained Models  [\[pdf\]](https://arxiv.org/abs/2306.08350)


## 二次开发阶段的攻击
### 针对迁移的攻击

With great training comes great vulnerability: Practical attacks against transfer learning [\[pdf\]](https://www.usenix.org/conference/usenixsecurity18/presentation/wang-bolun)

Latent backdoor attacks on deep neural networks  [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3319535.3354209)   [\[code\]](https://github.com/Huiying-Li/Latent-Backdoor)

Backdoor attacks against transfer learning with pre-trained deep learning models [\[pdf\]](https://ieeexplore.ieee.org/abstract/document/9112322/)

Incremental Learning, Incremental Backdoor Threats [\[pdf\]](https://ieeexplore.ieee.org/abstract/document/9872528/)

Pre-trained Adversarial Perturbations [\[pdf\]](https://proceedings.neurips.cc/paper_files/paper/2022/hash/084727e8abf90a8365b940036329cb6f-Abstract-Conference.html)

Ppt: Backdoor attacks on pre-trained models via poisoned prompt tuning [\[pdf\]](https://www.ijcai.org/proceedings/2022/0096.pdf)

Instructions as Backdoors: Backdoor Vulnerabilities of Instruction Tuning for Large Language Models [\[pdf\]](https://arxiv.org/abs/2305.14710)

Teacher model fingerprinting attacks against transfer learning [\[pdf\]](https://www.usenix.org/conference/usenixsecurity22/presentation/chen-yufei)

Manipulating Transfer Learning for Property Inference  [\[pdf\]](http://openaccess.thecvf.com/content/CVPR2023/html/Tian_Manipulating_Transfer_Learning_for_Property_Inference_CVPR_2023_paper.html)   [\[code\]](https://github.com/yulongt23/Transfer-Inference)

Information leakage in embedding models [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3372297.3417270)
 
Extracting training data from large language models [\[pdf\]](https://www.usenix.org/conference/usenixsecurity21/presentation/carlini-extracting)

EncoderMI: Membership inference against pre-trained encoders in contrastive learning [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3460120.3484749)

StolenEncoder: stealing pre-trained encoders in self-supervised learning [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3548606.3560586)

Can't Steal? Cont-Steal! Contrastive Stealing Attacks Against Image Encoders [\[pdf\]](https://openaccess.thecvf.com/content/CVPR2023/html/Sha_Cant_Steal_Cont-Steal_Contrastive_Stealing_Attacks_Against_Image_Encoders_CVPR_2023_paper.html)


### 针对压缩的攻击
Qu-anti-zation: Exploiting quantization artifacts for achieving adversarial outcomes  [\[pdf\]](https://proceedings.neurips.cc/paper_files/paper/2021/hash/4d8bd3f7351f4fee76ba17594f070ddd-Abstract.html)  [\[code\]](https://github.com/Secure-AI-Systems-Group/Qu-ANTI-zation)

Quantization backdoors to deep learning commercial frameworks  [\[pdf\]](https://ieeexplore.ieee.org/abstract/document/10113762/)   [\[code\]](https://github.com/quantization-backdoor)

Stealthy backdoors as compression artifacts  [\[pdf\]](https://ieeexplore.ieee.org/abstract/document/9737144/)   [\[code\]](https://github.com/yulongtzzz/Stealthy-Backdoors-as-Compression-Artifacts)

RIBAC: Towards R obust and I mperceptible B ackdoor A ttack against C ompact DNN  [\[pdf\]](https://link.springer.com/chapter/10.1007/978-3-031-19772-7_41)   [\[code\]](https://github.com/huyvnphan/ECCV2022-RIBAC)

Anti-distillation backdoor attacks: Backdoors can really survive in knowledge distillation  [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3474085.3475254)


## 部署阶段的攻击
Towards practical deployment-stage backdoor attack on deep neural networks  [\[pdf\]](http://openaccess.thecvf.com/content/CVPR2022/html/Qi_Towards_Practical_Deployment-Stage_Backdoor_Attack_on_Deep_Neural_Networks_CVPR_2022_paper.html)  [\[code\]](https://github.com/Unispac/Subnet-Replacement-Attack)

## 使用阶段的攻击
Analyzing information leakage of updates to natural language models  [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3372297.3417880) 

Dataset reconstruction attack against language models [\[pdf\]](https://ceur-ws.org/Vol-2942/paper1.pdf)

Analyzing Leakage of Personally Identifiable Information in Language Models [\[pdf\]](https://www.computer.org/csdl/proceedings-article/sp/2023/933600a346/1NrbXJj80H6)

The thieves on sesame street are polyglots-extracting multilingual models from monolingual APIs [\[pdf\]](https://aclanthology.org/2020.emnlp-main.501/)

Student Surpasses Teacher: Imitation Attack for Black-Box NLP APIs [\[pdf\]](https://aclanthology.org/2022.coling-1.251/)

On the feasibility of specialized ability stealing for large language code models [\[pdf\]](https://arxiv.org/abs/2303.03012)

## 供应链中的安全防护方法

### 设计阶段的防护
Detecting Backdoors in Pre-trained Encoders [\[pdf\]](https://openaccess.thecvf.com/content/CVPR2023/html/Feng_Detecting_Backdoors_in_Pre-Trained_Encoders_CVPR_2023_paper.html)    [\[code\]](https://github.com/GiantSeaweed/DECREE)

### 二次开发阶段的防护
How should pre-trained language models be fine-tuned towards adversarial robustness? [\[pdf\]](https://proceedings.neurips.cc/paper/2021/hash/22b1f2e0983160db6f7bb9f62f4dbb39-Abstract.html)     [\[code\]](https://github.com/dongxinshuai/RIFT-NeurIPS2021)


### 部署阶段的防护
Metamorphic testing of deep learning compilers [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3508035)

### 使用阶段的防护
TextFusion: Privacy-Preserving Pre-trained Model Inference via Token Fusion [\[pdf\]](https://aclanthology.org/2022.emnlp-main.572/)



