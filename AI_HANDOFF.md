# AI Handoff

本仓库保存的是 `cc-bishe` 毕设项目的长期留档材料。

如果你是下一次接手该项目的 AI，请先按以下顺序阅读：

1. `code/cc-bishe/NEXT_AI_HANDOFF.md`
2. `code/cc-bishe/EXPERIMENTS.md`
3. `experiments/cc-bishe-experiments/summary.md`
4. `thesis_materials/main.tex`

## 最重要的信息

- 代码主仓当前最佳纯 DL 方案：`exp05_ablation_concat_no_attention`
- 最佳少数类优化方案：`exp04_weighted_sampler_ce`
- 最强 threat intel 融合结果：`exp10_concat_synthintel_soft_voting`
- 全部实验都保留了：
  - checkpoint
  - 日志
  - 配置
  - 指标摘要
  - 训练曲线
  - 混淆矩阵
  - `processed/preprocessor.pkl`

## 如果要继续实验

优先检查：

- 原项目本地路径是否仍存在：`/root/bishe/cc-bishe`
- 实验目录是否仍存在：`/root/autodl-tmp/cc-bishe-experiments`
- 数据缓存是否仍存在：`/root/autodl-tmp/cc-bishe-cache/full_v1/dataset_cache.pt`

## 资料仓定位

这个仓库的作用不是替代原始数据盘，而是作为：

- 代码与实验记录备份
- 论文素材备份
- 未来继续实验时的上下文恢复入口

最完整的操作说明仍在：

- `code/cc-bishe/NEXT_AI_HANDOFF.md`
