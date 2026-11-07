# MaaFW Debugger

面向 [MaaFramework（MaaFW）](https://github.com/MaaXYZ/MaaFramework) 的独立 Pipeline 编辑与调试工具，由 [maa-verge](https://github.com/maa-verge) 组织维护。

当前处于规划阶段，尚无可用安装包或调试实现。开发范围与进度见[项目计划](https://github.com/maa-verge/maafw-debugger/issues/1)。

## 计划能力

- 查看 Pipeline 节点图、JSON、资源引用与 Custom 调用关系。
- 编辑流程与识别参数，检查引用、覆盖顺序和运行端实际加载的配置。
- 使用本地图片调试 OCR、模板匹配和 Custom Recognition。
- 显式连接模拟器，执行受控流程，查看节点时间线、识别结果和失败证据。
- 保存草稿、比较修改与运行结果，导出可审阅的诊断资料。

Windows、macOS、Linux 为支持目标，兼容范围以未来实际验证结果为准。保留上下文的单步与断点需先验证 SDK 能力。

## 与 Maa Verge 的关系

本项目独立于 [Maa Verge](https://github.com/maa-verge/maa-verge)，面向 MaaFW 资源与项目，不要求安装 Maa Verge，也不依赖明日方舟账号。

需求起源于 [Maa Verge #35](https://github.com/maa-verge/maa-verge/issues/35)。Maa Verge 的注册表、TS 绑定和业务流程作为可选适配，不是通用 Pipeline 的前置条件。

## 参与

功能建议、设计讨论与问题反馈请提交到 [Issues](https://github.com/maa-verge/maafw-debugger/issues)。当前仓库用于建立项目定位和开发计划，具体技术栈与实现将分阶段确定。

## 许可与致谢

本项目采用 **AGPL-3.0-only**，详见 [LICENSE](LICENSE)。MaaFramework 及其他第三方组件遵循各自许可，本项目是独立社区工具。
