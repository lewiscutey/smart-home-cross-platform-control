# 基于多模态交互的智能家居跨端控制系统设计

- 项目名称：基于多模态交互的智能家居跨端控制系统设计
- 导师信息：吕新，lvxin5@xiaomi.com
- 难度：中高（需综合多模态交互算法、嵌入式开发、跨端通信等技术）
- 分类：人机交互与智能设备、嵌入式系统与物联网、AI应用开发

题目要求：
- 功能需求：
1. 多模态输入：支持手势（打响指）、动作（摇头/点头）、语音（VUI）控制设备，如灯光开关、媒体播放等。
2. 跨端控制：通过手环/手表/手机应用操控模拟硬件（如STM32、ESP32），需实现蓝牙/Wi-Fi/MQTT通信协议。
3. 健康提醒：基于手环传感器监测用户行为（如久坐、洗手），触发震动/弹窗提醒。
4. 硬件模拟：通过STM32模拟智能家居设备响应控制指令。
- 性能需求：
手势识别准确率≥90%；语音指令响应时间≤500ms。
- 应用场景：
家庭环境中的智能灯光、媒体控制；办公室久坐提醒等。

特征：
1. 多模态融合：需设计交互方式优先级（如语音优先于手势）。
2. 低延迟：通过优化算法和通信协议降低控制延迟。
3. 用户习惯适配：支持自定义手势和语音指令。

预期目标：
1. 完成可穿戴设备端（手环/手表）控制软件及STM32硬件模拟程序。
2. 提交设计文档（含交互流程图、硬件连接图）、源代码、演示视频。
3. 实现至少3种交互方式（如语音+手势+动作）。

参考资料：
1. 跨端快应用官方文档
- [概述](https://doc.quickapp.cn/)
- [概述 | Xiaomi Vela JS 应用开发文档](https://iot.mi.com/vela/quickapp/zh/guide/)
2. 智能家居多模态交互系统设计文档
- [2025年智能家居的多模态交互系统设计.pdf-原创力文档](https://max.book118.com/html/2025/0119/6042241135011031.shtm)
- [智能家居的多模态交互系统设计-20250103070349.pdf-原创力文档](https://max.book118.com/html/2025/0103/8071061017007015.shtm)
3. 基于STM32的智能家居控制系统
- [2025年基于plc的智能家居控制系统开题报告.pdf-原创力文档](https://max.book118.com/html/2025/0117/7105102131010024.shtm)
3. AI多模态实时交互技术解析
- [2025年：AI多模态实时交互技术引领智能化革命新潮流_互动_用户_应用](https://www.sohu.com/a/846829762_121798711)

备注：
1. 技术栈建议：
  - 交互算法：采用OpenCV（手势识别）、TensorFlow Lite（语音指令轻量化部署）。
  - 硬件通信：使用ESP32或STM32的蓝牙/BLE模块实现跨端控制。
  - 用户界面：基于快应用开发跨平台应用，适配手环、手表、手机等多终端。
2. 扩展方向：
  - 增加情感识别（通过语音语调或表情分析优化交互体验）。
  - 集成AI生成内容（如语音助手自动生成提醒文案）。

3. 评分重点：
  - 交互方式的创新性（如“打拳”动作设计需定义明确触发逻辑）。
  - 系统稳定性（硬件响应成功率≥95%）。

参考架构图：

![whiteboard_exported_image](https://github.com/user-attachments/assets/264df156-841b-4096-afdb-03547e8e60eb)
