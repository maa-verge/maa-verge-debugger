# Maa Verge Debugger

专门调试 [Maa Verge](https://github.com/maa-verge/maa-verge) 中 [MaaFramework（MaaFW）](https://github.com/MaaXYZ/MaaFramework) 流程的独立桌面工具，由 [maa-verge](https://github.com/maa-verge) 组织维护。

当前处于规划阶段，尚无可用安装包或调试实现。开发范围与进度见[第一版计划 #1](https://github.com/maa-verge/maa-verge-debugger/issues/1)。

## 计划能力

- 查看 Pipeline 节点图、JSON、资源来源与 TS Custom/子能力调用关系。
- 编辑流程草稿与识别参数，检查登记、引用、覆盖顺序和运行端实际加载的配置。
- 使用本地图片测试 OCR、模板匹配，查看区域、坐标和识别结果。
- 显式连接模拟器，运行和停止受控流程，查看节点时间线与失败证据。
- 保存草稿、查看差异并导出修改与诊断资料。

Windows、macOS、Linux 为支持目标，兼容范围以实际验证结果为准。保留上下文的单步与断点作为后续能力，需先验证 SDK 支持边界。

## 与 Maa Verge、Automation 的关系

Debugger 独立安装、启动，Maa Verge 本体不新增界面入口。两端共同消费 [`maa-verge/maa-verge-automation`](https://github.com/maa-verge/maa-verge-automation) 的 JSON/JSONC、TS Custom、注册及契约，通过 Git submodule 固定共享提交。

第一版面向开发者，由 Debugger 启动 Maa Verge 的隔离调试宿主，复用 backend/worker 和设备控制边界；要求所选 checkout 已接入共享库并支持调试宿主协议。无需打开本体主界面，调试数据与业务数据库隔离。

正式流程保持构建内置，编辑生成独立调试草稿，显式校验后用于下一次调试；修改不会直接替换正在执行或正式安装的流程。TS Custom 变更通过构建或重启宿主生效。

## 参与

- [Debugger 第一版计划](https://github.com/maa-verge/maa-verge-debugger/issues/1)
- [Automation 共享库重构计划](https://github.com/maa-verge/maa-verge-automation/issues/1)
- [原生化与唤醒/公招试点](https://github.com/maa-verge/maa-verge-automation/issues/2)

功能建议、设计讨论与问题反馈请提交到 [Issues](https://github.com/maa-verge/maa-verge-debugger/issues)。

## 许可与致谢

本项目采用 **AGPL-3.0-only**，详见 [LICENSE](LICENSE)。MaaFramework 及其他第三方组件遵循各自许可，本项目为独立社区项目。
