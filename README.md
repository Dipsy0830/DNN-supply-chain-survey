# 深度学习模型供应链的安全性研究综述
这个 Github 存储库总结了深度学习模型供应链相关的资源。 有关更多详细信息和分类标准，请参阅我们的综述论文。

预训练模型解决了训练数据和算力受限的问题，已在各领域被广泛使用，它也催生了模型开发和应用的新范式——深度学习模型供应链。

模型经过设计和训练，由发布者上传至预训练模型仓库，由二次开发者进行迁移和压缩，部署到边缘端设备，并提供给用户使用。模型供应链引入了新环节和多要素，带来数据泄露风险和计算安全问题。

我们调研了相关的研究工作，根据模型生命周期的阶段，对模型设计、二次开发、部署和使用阶段的攻击和防御进行梳理和总结。
# 模型设计阶段的攻击
## 下游任务相关的攻击

Weight Poisoning Attacks on Pretrained Models [\[pdf\]](https://aclanthology.org/2020.acl-main.249/)  [\[code\]](https://github.com/neulab/RIPPLe)
Backdoor Attacks on Pre-trained Models by Layerwise Weight Poisoning  [\[pdf\]](https://aclanthology.org/2021.emnlp-main.241/)


## 下游任务无关的攻击

Model-reuse attacks on deep learning systems [\[pdf\]](https://dl.acm.org/doi/abs/10.1145/3243734.3243757)


# 二次开发阶段的攻击
## 针对迁移的攻击

With great training comes great vulnerability: Practical attacks against transfer learning [\[pdf\]](https://www.usenix.org/conference/usenixsecurity18/presentation/wang-bolun)
