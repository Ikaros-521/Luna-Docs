## :material-microphone: 语音功能

Luna AI 支持多种语音交互功能，包括文本转语音（TTS）和语音转换（Voice Conversion）。

### 文本转语音 (TTS)

支持的 TTS 引擎：

- Edge-TTS
- VITS-Fast
- elevenlabs
- bark-gui
- VALL-E-X
- 睿声AI
- OpenVoice
- GPT_SoVITS
- clone-voice
- Azure TTS
- fish-speech
- ChatTTS
- CosyVoice
- F5-TTS

### 语音转换

支持以下语音转换技术：

- so-vits-svc
- DDSP-SVC

这些技术能够实现声音的变化，以适应不同的场景和角色。

### 语音配置

在 `config.json` 中可以配置语音相关参数：

```json
{
    "tts": {
        "type": "edge-tts",
        "voice": "zh-CN-XiaoyiNeural",
        "rate": "+0%",
        "volume": "+0%"
    }
}
``` 