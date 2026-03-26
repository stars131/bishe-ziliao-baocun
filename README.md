# bishe-ziliao-baocun

本仓库用于保存 `cc-bishe` 毕业设计相关的重要材料，供服务器关机后长期留存与后续写作使用。

本地工作目录保存的是更完整的全量镜像；GitHub 远端优先保存：

- 可直接浏览的关键文档
- 代码快照
- 论文素材
- 环境快照
- 实验汇总
- 可恢复全量内容的 `bundle` 备份

## 目录说明

- `code/cc-bishe/`
  精简后的代码快照，保留核心源码、配置、实验脚本、威胁情报脚本、实验记录文档和 LaTeX 素材。
- `experiments/cc-bishe-experiments/`
  本地完整实验记录镜像。GitHub 远端默认保留实验汇总与 `bundle` 备份，而不是所有大文件逐个展开。
- `threat_intel/cc-bishe-threat-intel/`
  模拟威胁情报目录，包含不同版本的合成 IOC 库。
- `fusion_studies/`
  复用已有 checkpoint 做的融合策略扫参与分析结果。
- `thesis_materials/`
  可直接迁移到毕业论文模板中的 LaTeX 草稿与结果表格。
- `environment/`
  环境快照，包括 Python 版本、依赖列表、GPU 信息和服务器参数。

## 已保留的关键内容

- 毕设代码与新增实验流水线
- 全量实验结果汇总 `summary.csv` / `summary.md`
- 11 组主实验的完整训练与测试日志
- 结构化评估结果、混淆矩阵、训练曲线与 checkpoint
- 合成威胁情报生成脚本与不同版本情报库
- 融合策略扫参与对照结果
- `EXPERIMENTS.md` 论文实验记录底稿
- `thesis_materials/main.tex` 论文 LaTeX 草稿

## 有意未纳入 GitHub 的内容

以下内容体积过大或属于可再生中间产物，因此未纳入本仓库：

- 原始 CSV 数据与压缩数据集
- 数据缓存 `dataset_cache.pt`
- 运行时缓存、`__pycache__` 与 `.git` 元数据

说明：

- 每个实验目录中的 `processed/preprocessor.pkl` 已保留，便于后续直接衔接实验。
- `dataset_cache.pt` 未保留到 GitHub，原因是单文件体积约 5GB，超出常规 GitHub 仓库存储边界；后续如需继续实验，可基于原始数据重新生成缓存，或在新的服务器上从其他介质恢复该缓存。

## 配套代码仓

代码主仓库：

- `https://github.com/stars131/cc-bishe.git`

本资料仓主要承担“离线保存”和“论文素材留档”的作用。
