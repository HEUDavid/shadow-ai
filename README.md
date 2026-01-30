# Shadow AI

## 影子 AI, 一款无痕无感的 AI 工具，让你可以在「受控设备/受限环境」使用 AI, 极速且高效且稳定

## 应用依赖

<details>
  <summary>MacOS 依赖</summary>

```shell
1. 语音识别 STT 模型, 下载并解压
https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-zh-2025-06-30.tar.bz2

2. 驱动 BlackHole: Audio Loopback Driver, 安装默认的 blackhole-2ch 即可
https://github.com/ExistentialAudio/BlackHole?tab=readme-ov-file#option-1-download-installer

3. 打开「音频 MIDI 设置」-> 创建「多输出设备」，勾选内建输出 + BlackHole 2ch -> 右键将多输出设备设为系统默认输出
```

</details>

<details>
  <summary>Windows 依赖</summary>

```shell
1. 语音识别 STT 模型, 下载并解压
https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-zh-2025-06-30.tar.bz2
```

</details>

## 应用设置

```shell
1. 应用启动后, 会自动打开功能引导页
2. 设置中添加您的 AI 服务, 默认模型, 添加您自定义的提示词
3. 配置上一步中解压的 STT 模型路径, 例如: /Users/david/Downloads/models/sherpa-onnx-streaming-zipformer-zh-2025-06-30
```

## 功能介绍

```shell
1. 语音识别区: 系统会使用模型实时识别系统音频里的语音, 并在这里实时更新字幕
2. AI 回答区: 返回你配置的默认模型的回答, 当您选择多个模型时, 回答是最快返回内容的那一个
3. 按钮介绍: 
  3.1 截屏分析按钮, 点击会截取设备当前屏幕, 提交给 AI 获取回答
  3.2 语音分析按钮, 点击会提交当前语音转写文本「作为问题」, 提交给 AI 获取回答 注意: 会提交缓存的所有的语音转写文本
  3.3 语音文本重置按钮, 点击之后可以清理语音转写文本缓存
  3.4 程序退出按钮
```
