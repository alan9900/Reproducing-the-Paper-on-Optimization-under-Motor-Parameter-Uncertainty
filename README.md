# Reproducing-the-Paper-on-Optimization-under-Motor-Parameter-Uncertainty

本仓库用于复现论文中的电机参数不确定性建模与鲁棒优化工作。

## 文档

- [电机参数不确定性优化复现指南（Maxwell / IPMSM）](MOTOR_OPTIMIZATION_REPRODUCTION.md)：整理目标复现资料中的电机规格、12 个初始结构参数、7 个优化变量与范围、Maxwell 初始模型搭建步骤、OLHS 样本、代理模型结果、NSGA-II 参数、优化前后性能基准及尚待补齐的原始信息。
- [永磁同步电机设计参数不确定性优化工作流（参考方案）](WORKFLOW_REFERENCE.md)：整理 SolidWorks → ANSYS Workbench/Maxwell → DOE → Kriging 代理模型 → Monte Carlo/Six Sigma → 稳健优化 → 回代验证的参考流程，并保留示例参数、软件模块和操作检查点。

## 使用说明

- **目标论文复现指南优先用于确认目标论文的电机参数、变量、约束、算法和结果基准。**
- **工作流文档只作为方法参考，不要求全部照搬。** 可根据目标论文、实际工程文件、软件版本、许可证和计算资源调整流程。
- 不要将参考工作流中的 L1–L6、辐条式转子、材料示例、CCD、Kriging 或 NLPQLP 直接替换目标论文明确给出的设置。
- 文档已区分原始资料明确给出的内容与待确认细节。没有原始 Maxwell 工程或完整几何、材料、绕组和激励信息时，不能保证一比一重建论文模型。
