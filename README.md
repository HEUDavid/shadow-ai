<div align="center">

<h1>Shadow AI: Designed for Restricted Environments</h1>
  <p>
    <a href="https://github.com/HEUDavid/shadow-ai/releases" target="_blank">
        <img src="https://img.shields.io/github/v/release/HEUDavid/shadow-ai?color=c351e3&style=flat-square"
             alt="Releases"></a>
    <a href="https://github.com/HEUDavid/shadow-ai/releases/latest" target="_blank">
        <img src="https://img.shields.io/badge/Support-Windows, macOS-0969da?style=flat-square"
             alt="Support OS"></a>
  </p>

[中文](README_ZH.md) | **English**

</div>

## Features

Shadow AI is an AI assistant designed specifically for restricted environments. It provides a stealthy operation mode
without windows or traces, and enables cross-device AI Q&A interaction and control via the local area network (LAN).

Essentially, it is an automated collaboration layer of "screen/audio capture + AI inference + low-friction delivery",
helping users to immersively use AI assistants across applications on controlled devices or in restricted environments.

- **Stealth Operation**: Supports silent background operation on target devices with no frontend window.
- **Cross-Platform Control**: Supports remote takeover and control via LAN using devices like smartphones or tablets.
- **Major AI Services: Supports "Qwen, OpenAI, Claude, Gemini, Antigravity, Kimi" - FAST and STABLE.**
- **Standard Interface**: Supports other AI services that follow the OpenAI API standard.
- **Concurrency & Routing**: Supports multiple accounts and concurrent requests.
- **Multi-Language Support**: Speech recognition supports Chinese, English, and bilingual Chinese–English (more
  languages are being added). Choose the appropriate STT model based on your use case.

## Interface

![Welcome](assets/welcome.webp "Welcome")

| <img alt="Image Analysis Example" height="700px" src="assets/vlm-question.webp" title="Image Question"/> | <img alt="AI Answer Example" height="700px" src="assets/vlm-answer.jpg" title="AI Answer"/> |
|----------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------|

<details><summary><strong>AI Settings</strong></summary>

**Multi-Channel Support** Supports AI tools like "Qwen, OpenAI, Claude, Gemini, Antigravity, Kimi" as backend large
language models (LLMs).

![Login Authentication](assets/auth.webp "Login Authentication")

**Test Models** Click to add a model to custom AI, then test whether the model is working properly.

![Test AI](assets/test-ai.webp "Test AI")

**Switch Models** You can specify different models for visual (screenshot analysis) and audio (voice Q&A). Selecting
multiple models enables concurrent queries, displaying the fastest response.

![Configure AI](assets/default-model.webp "Configure Default AI Service")

**Prompts** Set system prompts tailored to your custom application scenarios.

![Set Prompts](assets/prompts.webp "Set Prompts")

</details>

## Feedback & Community

This project is under iterative development. If you have any **bug reports, feature requests, or usage questions**,
please feel free to join our group and provide feedback.

<details><summary><strong>Telegram</strong></summary>

> - [Join our Telegram](https://t.me/shadow_ai_group) and DM me

</details>

## FAQ

<details><summary><strong>Windows</strong></summary>

1. The program is installation-free; just extract it and use it.
2. How to enable speech recognition analysis? (Optional)
    * Download and extract the STT model, then configure the speech recognition model path in Settings.
    * STT Model URLs:
        * [Zipformer Chinese](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-zh-2025-06-30.tar.bz2)
        * [Zipformer English](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-en-2023-06-26.tar.bz2)
        * [Zipformer Bilingual Chinese-English](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-bilingual-zh-en-2023-02-20.tar.bz2)
        * [Paraformer Bilingual Chinese-English](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-paraformer-bilingual-zh-en.tar.bz2)
    * How to verify?
        * Play an audio clip. The speech recognition panel should transcribe subtitles in real time.
        * Note: Speech recognition analyzes the `system audio output (speaker playback)`, not the
          `microphone input (recording)`.

</details>

<details><summary><strong>macOS</strong></summary>

1. How to enable screenshot analysis?
    * Permission Check: Settings → Privacy & Security → Screen Recording: Allow this application.
    * **⚠️ Grant permissions, then restart the software.**
      ![Screenshot Permission](assets/screenshot-permission.png "Screenshot Permission")
2. How to enable speech recognition analysis? (Optional)
    1. macOS Audio Configuration
        1. Install [BlackHole](https://github.com/ExistentialAudio/BlackHole).
        2. Open "Audio MIDI Setup".
        3. Create a "Multi-Output Device" and check "Built-in Output" + "BlackHole 2ch".
        4. Set the Multi-Output Device as the default system output.
    2. STT Model Configuration
        * Download and extract the STT model, then configure the speech recognition model path in Settings.
        * STT Model URLs:
            * [Zipformer Chinese](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-zh-2025-06-30.tar.bz2)
            * [Zipformer English](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-en-2023-06-26.tar.bz2)
            * [Zipformer Bilingual Chinese-English](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-zipformer-bilingual-zh-en-2023-02-20.tar.bz2)
            * [Paraformer Bilingual Chinese-English](https://github.com/k2-fsa/sherpa-onnx/releases/download/asr-models/sherpa-onnx-streaming-paraformer-bilingual-zh-en.tar.bz2)
    3. How to verify?
        * Play an audio clip. The speech recognition panel should transcribe subtitles in real time.
        * Note: Speech recognition analyzes the `system audio output (speaker playback)`, not the
          `microphone input (recording)`.

</details>

## Disclaimer

This project is intended for technical communication and learning purposes only. Please use this software in strict
compliance with local laws and regulations, institutional rules, and platform agreements. The user bears full
responsibility for any legal violations, disciplinary actions, and legal disputes arising from the misuse of this
project. The developers assume no direct or indirect responsibility.
