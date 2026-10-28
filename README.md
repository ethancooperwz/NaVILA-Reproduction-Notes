# NaVILA 复现笔记

本仓库记录 [NaVILA](https://github.com/AnjieCheng/NaVILA) 的中文复现进度，沿用 StreamVLN 复现笔记的六篇文档结构。

> 🚧 进行中：截至 2026-10-28，正在整理环境配置，尚未完成推理评测。部分文档仍为 StreamVLN 模板，已在文首标记，不代表 NaVILA 的配置或结果。

## 文档目录

1. [论文介绍](docs/01%20-%20论文介绍.md)：待改写为 NaVILA
2. [环境配置](docs/02%20-%20环境配置.md)：正在整理 Conda 与 Habitat-Sim 源码准备步骤
3. [数据集准备](docs/03%20-%20数据集准备.md)：待改写为 NaVILA
4. [模型推理与测评](docs/04%20-%20模型推理与测评.md)：待改写，尚未运行评测
5. [常见报错与解决](docs/05%20-%20常见报错与解决.md)：待整理 NaVILA 的实际问题
6. [实验结果与分析](docs/06%20-%20实验结果与分析.md)：尚无本地评测结果

## 当前进度与下次继续

- 本地已克隆 NaVILA 源码，版本为 `76b98f233dd0fff05dfcd69435eec6740febff9d`。
- 已记录 Python 3.10、PyTorch 2.3.0、CUDA 12.1 的环境准备草稿；安装是否成功尚未核验。
- 本地已有 `NaVILA/third_party/habitat-sim` 源码，当前版本标记为 `challenge-2021`，与草稿要求的 `v0.1.7` 尚需核对，子模块也有本地变更。
- 下次先核对 Habitat-Sim 的实际版本及编译状态，再继续 Habitat-Lab、NaVILA 依赖和环境自检。
- 数据集、checkpoint、推理与指标待核验和记录；模板中的 StreamVLN 命令与指标不能直接用于 NaVILA。

## 仓库结构

```text
.
├── README.md
├── docs/
│   ├── 01 - 论文介绍.md
│   ├── 02 - 环境配置.md
│   ├── 03 - 数据集准备.md
│   ├── 04 - 模型推理与测评.md
│   ├── 05 - 常见报错与解决.md
│   └── 06 - 实验结果与分析.md
└── images/                 # 截图和实验结果（可选）
```

本仓库保存复现笔记；本地上游源码、编译产物、数据集和模型权重不纳入版本管理。

## 参考资料

- [论文（arXiv 2412.04453）](https://arxiv.org/abs/2412.04453)
- [官方代码](https://github.com/AnjieCheng/NaVILA)
- [项目主页](https://navila-bot.github.io/)
- [复现项目索引](https://github.com/ethancooperwz/Awesome-VLN-Reproductions)
