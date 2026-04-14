<div align="center">

<h1>Shadow AI: 专为受限环境设计的 AI 辅助工具</h1>
  <p>
    <a href="https://github.com/HEUDavid/shadow-ai/releases" target="_blank">
        <img src="https://img.shields.io/github/v/release/HEUDavid/shadow-ai?color=c351e3&style=flat-square"
             alt="Releases"></a>
    <a href="https://github.com/HEUDavid/shadow-ai/releases/latest" target="_blank">
        <img src="https://img.shields.io/badge/Support-Windows, macOS-0969da?style=flat-square"
             alt="Support OS"></a>
  </p>

**中文** | [English](README.md)

</div>

## 特点

Shadow AI 是一款专为受限环境设计的 AI 辅助工具。提供无窗口、无痕迹的隐蔽运行方式，并通过局域网实现跨设备的 AI
问答交互与控制。

本质是一个「屏幕/音频采集 + AI 推理 + 低摩擦投送」的自动化协作层，帮助用户在受控设备/受限环境下沉浸式跨应用地使用 AI 助手。

- **隐蔽运行**：支持目标设备后台静默运行，无前端窗口
- **跨端操作**：通过局域网，支持手机或平板等设备远程接管控制
- **大厂 AI 服务：支持「千问、OpenAI、Claude、Gemini、Antigravity、Kimi」登录，极速稳定**
- **标准接口**：支持其他 OpenAI API 规范的 AI 服务
- **并发与路由**：支持多账号与并发
- **多语言支持**：语音识别支持中文、英文、中英双语（其他语言正在支持中），可根据语言场景选择 STT 模型

## 界面

![欢迎使用](assets/welcome.webp "欢迎使用")

| <img alt="图片分析示例" height="700px" src="assets/vlm-question.webp" title="图片提问"/> | <img alt="AI 回答示例" height="700px" src="assets/vlm-answer.jpg" title="AI 回答"/> |
|--------------------------------------------------------------------------------|-------------------------------------------------------------------------------|

<details><summary><strong>AI 设置</strong></summary>

**多渠道支持** 支持「千问、OpenAI、Claude、Gemini、Antigravity、Kimi」等 AI 工具作为后端大模型

![登录认证](assets/auth.webp "登录认证")

**测试模型** 点击添加模型到自定义 AI，然后测试模型是否正常工作

![测试AI](assets/test-ai.webp "测试AI")

**切换模型** 可以为视觉（截图分析）、音频（语音问答）指定不同的模型，多选则并发提问，然后显示最快的回答

![配置AI](assets/default-model.webp "配置默认AI服务")

**提示词** 结合自定义应用场景，设置系统提示词

![设置提示词](assets/prompts.webp "设置提示词")

</details>

## 反馈交流

本项目在迭代开发中，如果您有**BUG 反馈、功能需求、任何使用问题**，欢迎加入群组进行反馈。

<details><summary><strong>Telegram</strong></summary>

> - [加入 Telegram](https://t.me/shadow_ai_group)

</details>

## 常见问题

<details><summary><strong>Windows</strong></summary>

1. 程序免安装，解压即可使用。
2. 如何启用语音识别分析？（可选功能）
    * 下载 STT 模型并解压，然后在设置中配置语音识别模型路径
    * STT 模型下载地址：
        * [Zipformer (仅中文场景，准确率挺好)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-zh-2025-06-30.tar.bz2)
        * [Zipformer (仅英文场景，准确率非常好)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-en-2023-06-26.tar.bz2)
        * [Zipformer (中英双语版本比单语言版本准确率要差一些)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-bilingual-zh-en-2023-02-20.tar.bz2)
        * [Paraformer (中英双语)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-paraformer-bilingual-zh-en.tar.bz2)
    * 如何验证？
        * 播放一段音频，语音识别区应实时转写字幕
        * 注意：语音识别分析的是`系统音频输出（外放）`，不监听`麦克风输入（录音）`

</details>

<details><summary><strong>macOS</strong></summary>

1. 如何启用截图分析？
    * 权限检查：设置 → 安全性与隐私 → 屏幕录制：允许本程序
    * **⚠️ 授予权限后，需要重启软件**
      ![截图权限](assets/screenshot-permission.png "截图权限")
2. 如何启用语音识别分析？（可选功能）
    1. macOS 音频配置
        1. 安装 [BlackHole](https://github.com/ExistentialAudio/BlackHole)
        2. 打开「音频 MIDI 设置」
        3. 创建「多输出设备」，勾选内建输出 + BlackHole 2ch
        4. 将多输出设备设为系统默认输出
    2. STT 模型配置
        * 下载 STT 模型并解压，然后在设置中配置语音识别模型路径
        * STT 模型下载地址：
            * [Zipformer (仅中文场景，准确率挺好)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-zh-2025-06-30.tar.bz2)
            * [Zipformer (仅英文场景，准确率非常好)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-en-2023-06-26.tar.bz2)
            * [Zipformer (中英双语版本比单语言版本准确率要差一些)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-bilingual-zh-en-2023-02-20.tar.bz2)
            * [Paraformer (中英双语)](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-paraformer-bilingual-zh-en.tar.bz2)
    3. 如何验证？
        * 播放一段音频，语音识别区应实时转写字幕
        * 注意：语音识别分析的是`系统音频输出（外放）`，不监听`麦克风输入（录音）`

</details>

## 免责声明

本项目仅供技术交流与学习使用。请在严格遵守当地法律法规、机构规章及平台协议的前提下使用本软件。因滥用本项目产生的违规违法行为、纪律处分及法律纠纷，由使用者本人承担全部责任，开发者不承担任何直接或间接责任。