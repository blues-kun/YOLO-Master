# MoT 路由研究实验

本 Fork 用于整理目标检测模型的路由可解释性、检测效用建模与动态专家计算实验。

## 当前工作

实验链路：

```text
目标级匹配审计 -> 检测效用矩阵 -> Utility Router -> Adaptive K
```

- 目标级匹配审计：分析不同目标场景与 Transformer 专家激活之间的关系。
- 检测效用矩阵：通过专家干预测量各专家对检测损失的实际贡献。
- Utility Router：以检测效用监督路由，并使用 KL 漂移保护处理跨序列失效。
- Adaptive K：按输入置信度动态选择专家数量，并记录真实专家调用次数。

## 代码与报告

- [实验分支](https://github.com/blues-kun/YOLO-Master/tree/rhino-2026/issue-54-medical-routing)
- [完整中文实验链路](https://github.com/blues-kun/YOLO-Master/blob/rhino-2026/issue-54-medical-routing/examples/mot_cross_domain_audit/utility_router_adaptive_k_zh.md)
- [可公开结果索引](https://github.com/blues-kun/YOLO-Master/tree/rhino-2026/issue-54-medical-routing/examples/mot_cross_domain_audit/results/utility_routing)

当前实现属于研究性验证，结论以仓库中保存的原始实验数据和复现实验为准。

代码许可见 [LICENSE](LICENSE)。
