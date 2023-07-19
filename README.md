![img]('https://github.com/Dipsy0830/DNN-supply-chain-survey/blob/main/imgs/vis.png')


# 深度学习模型供应链的安全性研究综述
这个 Github 存储库总结了深度学习模型供应链相关的资源。 有关更多详细信息和分类标准，请参阅我们的综述论文。

预训练模型解决了训练数据和算力受限的问题，已在各领域被广泛使用，它也催生了模型开发和应用的新范式——深度学习模型供应链。

模型经过设计和训练，由发布者上传至预训练模型仓库，由二次开发者进行迁移和压缩，部署到边缘端设备，并提供给用户使用。模型供应链引入了新环节和多要素，带来数据泄露风险和计算安全问题。

我们调研了相关的研究工作，根据模型生命周期的阶段，对模型设计、二次开发、部署和使用阶段的攻击和防御进行梳理和总结。
## 模型设计阶段的攻击
### 下游任务相关的攻击

Weight Poisoning Attacks on Pretrained Models [\[pdf\]](https://aclanthology.org/2020.acl-main.249/)  [\[code\]](https://github.com/neulab/RIPPLe)

Backdoor Attacks on Pre-trained Models by Layerwise Weight Poisoning  [\[pdf\]](https://aclanthology.org/2021.emnlp-main.241/)


### 下游任务无关的攻击

Model-reuse attacks on deep learning systems [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3243734.3243757)


## 二次开发阶段的攻击
### 针对迁移的攻击

With great training comes great vulnerability: Practical attacks against transfer learning [\[pdf\]](https://www.usenix.org/conference/usenixsecurity18/presentation/wang-bolun)


### 针对压缩的攻击
Qu-anti-zation: Exploiting quantization artifacts for achieving adversarial outcomes  [\[pdf\]](https://proceedings.neurips.cc/paper_files/paper/2021/hash/4d8bd3f7351f4fee76ba17594f070ddd-Abstract.html)  [\[code\]](https://github.com/Secure-AI-Systems-Group/Qu-ANTI-zation)


## 部署阶段的攻击
Towards practical deployment-stage backdoor attack on deep neural networks  [\[pdf\]](http://openaccess.thecvf.com/content/CVPR2022/html/Qi_Towards_Practical_Deployment-Stage_Backdoor_Attack_on_Deep_Neural_Networks_CVPR_2022_paper.html)  [\[code\]](https://github.com/Unispac/Subnet-Replacement-Attack)

## 使用阶段的攻击
Analyzing information leakage of updates to natural language models  [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3372297.3417880) 

## 供应链中的安全防护方法

### 设计阶段的防护
Detecting Backdoors in Pre-trained Encoders [\[pdf\]](https://openaccess.thecvf.com/content/CVPR2023/html/Feng_Detecting_Backdoors_in_Pre-Trained_Encoders_CVPR_2023_paper.html)    [\[code\]](https://github.com/GiantSeaweed/DECREE)

### 二次开发阶段的防护
How should pre-trained language models be fine-tuned towards adversarial robustness? [\[pdf\]](https://proceedings.neurips.cc/paper/2021/hash/22b1f2e0983160db6f7bb9f62f4dbb39-Abstract.html)     [\[code\]](https://github.com/dongxinshuai/RIFT-NeurIPS2021)


### 部署阶段的防护
Metamorphic testing of deep learning compilers [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3508035)

### 使用阶段的防护
TextFusion: Privacy-Preserving Pre-trained Model Inference via Token Fusion [\[pdf\]](https://aclanthology.org/2022.emnlp-main.572/)



