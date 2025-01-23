### TTS

#### elevenlabs

[elevenlabs官网](//beta.elevenlabs.io)

[官方文档](//docs.elevenlabs.io/api-reference/quick-start/introduction)

不注册账号也可以使用，不过应该是有限制的（具体多少未知）。免费账号拥有每月1万字的额度。

#### genshinvoice.top

[在线体验官网](//genshinvoice.top)

[官方GitHub仓库](//github.com/Stardust-minus/vits)，内含api使用说明

官方视频讲解：[【在线合成&效果优化】基于VITS的米哈游全角色语音合成现已发布](//www.bilibili.com/video/BV1Sg4y1K7kg)

#### tts.ai-lab.top

在线体验官网: [https://tts.ai-hobbyist.org/](https://tts.ai-hobbyist.org/)

注册账号，登录，然后在在线合成页面，按下键盘`F12`打开开发者工具，在选择`Network`网络，随便合成一个音频，然后找到`vits`的一个请求，点进去，点击`负载`，找到`appid`和`token`，配置即可。  

#### VITS（vits-simple-api）

emotional-vits官方仓库：[emotional-vits](//github.com/innnky/emotional-vits)  

接入API：[vits-simple-api](//github.com/Artrajz/vits-simple-api)  

vits-simple-api整合包下载：[github.com/Artrajz/vits-simple-api/releases](//github.com/Artrajz/vits-simple-api/releases)  

个人提供的已训练好的模型：[github](//github.com/Ikaros-521/emotional-vits/releases) ,   [迅雷云盘](https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1?path=%2F%E5%88%86%E4%BA%AB%2FTTS%2FVITS%2F%E6%A8%A1%E5%9E%8B)  

视频教程：[【AI主播-TTS篇】新增 纯 VITS 接入，配合vits-simple-api，支持情感控制，语速调控](https://www.bilibili.com/video/BV1ku4y1R73r) , [【AI主播-TTS篇】新增 bert-vits2 的接入，配合vits-simple-api食用，强有力的中文TTS让你到达新高度~](https://www.bilibili.com/video/BV1Ph4y1A79w)   

如何白嫖huggingface上的`vits-simple-api`？ 只需要开启魔法，将`API地址`修改为项目提示的接口地址即可，例如：`https://artrajz-vits-simple-api.hf.space`  

vits-simple-api配置，修改 `config.py` ，参考配置如下，路径为追加的相对模型路径和配置文件路径（注意，新版本的变动，配置改到config.yml了，所以你需要直接改yml或者删除yml，修改py，然后重启）：

```python
# Fill in the model path here
MODEL_LIST = [
    # VITS
    [ABS_PATH + "/Model/ikaros/G_95500.pth", ABS_PATH + "/Model/ikaros/config.json"],
    # Bert-VITS2
    [ABS_PATH + "/bert_vits2/G_0.pth", ABS_PATH + "/bert_vits2/config.json"],
```

如果使用 `bert_vits2` ，需要注意 `vits-simple-api\bert_vits2\bert\chinese-roberta-wwm-ext-large` 路径下 `flax_model.msgpack` 等模型文件是否缺失，如果缺失，可以从隔壁 `bert_vits2` 整合包中拷贝进来 或者 从`huggingface`下载：[hfl/chinese-roberta-wwm-ext-large](//huggingface.co/hfl/chinese-roberta-wwm-ext-large/tree/main) 。另外模型需要存放在 `bert_vits2` 目录里面。  

相关模型备份：[夸克网盘](//pan.quark.cn/s/0ec7deae974a)  


另外如果运行闪退、报错  

```python
Traceback (most recent call last):
  File "E:\vits-simple-api\app.py", line 49, in <module>
    tts = merge_model(app.config["MODEL_LIST"])
  File "E:\vits-simple-api\utils\merge.py", line 117, in merge_model
    for id, name in enumerate(obj.get_speakers()):
  File "E:\vits-simple-api\utils\utils.py", line 29, in __getitem__
    return getattr(self, key)
TypeError: getattr(): attribute name must be string
```

需要修改 `utils\merge.py` 116行左右。

```python
for id, (key, name) in enumerate(obj.get_speakers().items()):
# for id, name in enumerate(obj.get_speakers()):
```

如果在使用`bert-vits2`时，报错：

```bash
error, ref_enc.convs.0.bias is not in the checkpoint
error, ref_enc.convs.0.weight_g is not in the checkpoint
......
```

解决方案参考：[issues/311](https://github.com/Ikaros-521/AI-Vtuber/issues/311)  

改 `bert_vits2/models.py` 中第`646`行 `if n_speakers > 1:` 修改为 `if n_speakers >= 1:`  

#### VITS-fast-fine-tuning

官方仓库：[VITS-fast-fine-tuning](//github.com/Plachtaa/VITS-fast-fine-tuning)  

官方推理包：[inference-webui-v1.1](//github.com/Plachtaa/VITS-fast-fine-tuning/releases/tag/webui-v1.1)  

个人提供的已训练好的模型：[点我跳转](//github.com/Ikaros-521/VITS-fast-fine-tuning/releases)  

视频教程：[【AI语音合成-数据集篇#00】模型使用简单讲解，手把手演示](//www.bilibili.com/video/BV1Lm4y1r7Pi) ，[【AI主播-功能篇】TTS语音合成 VITS-Fast怎么使用？为什么没有合成语音？VITS不行吗？模型兼容吗？](https://www.bilibili.com/video/BV1Tm4y1J71B)   

训练用整合包（原作者整合包备份）：[pan.quark.cn/s/da52e78983da](//pan.quark.cn/s/da52e78983da)  

整合包视频教程：[AI声音克隆又进化了，10分钟学会声音克隆！一键启动包发布！](//www.bilibili.com/video/BV1K94y1k7Bw)  

整合包视频教程2：[【VITS一键包】本地训练独属于你的AI嘴替？训练部署AI语音合成教程](//www.bilibili.com/video/BV1B841197Em)  

#### 睿声

官网：[https://www.reecho.ai/](https://www.reecho.ai/)  

在 [角色管理](https://dash.reecho.ai/voices) 页面，创建训练一个你想用使用的角色的声音模型，点击更多，顶部可以看到一串字符串，就是角色ID，配置到配置项中。  

申请API Key：[https://dash.reecho.ai/apiKey](https://dash.reecho.ai/apiKey)，配置到对应配置项中，保存即可。

#### VALL-E-X

官方仓库：[VALL-E-X](//github.com/Plachtaa/VALL-E-X)  

个人提供的已训练好的preset预设：[点我跳转](//github.com/Ikaros-521/VALL-E-X/releases/tag/preset)  

官方视频讲解：[仅需3秒音频实现声音克隆！我开源了微软的最新语音合成模型VALL-E X](//www.bilibili.com/video/av617666708)  

视频教程：[【AI主播-功能篇】接入 VALL-E-X（整合包附赠），进行TTS，3秒声音克隆，“好用”喵hhh](https://www.bilibili.com/video/BV1Zh4y1T7YU)  

整合包下载：[pan.quark.cn/s/b817e285ab41](//pan.quark.cn/s/b817e285ab41)  

#### OpenVoice

官方仓库：[OpenVoice](https://github.com/myshell-ai/OpenVoice)  

视频教程：[OpenVoice 整合包 | 一句话快速克隆？英文可调语气？效果实测【TTS】](https://www.bilibili.com/video/BV1kK4y167WJ)

整合包下载：[迅雷云盘](https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1?path=%2F%E5%88%86%E4%BA%AB%2FTTS%2FOpenVoice), 
[夸克网盘](https://pan.quark.cn/s/936dcae8aba0#/list/share/56a79e143a8b4877a98a61854e07b229-AI%20Vtuber/5c251d9c745643868c0b17b7b6a0ecb6-TTS/9d6e066f2ed14ae4aef3e74cda6cd078-OpenVoice)

启动webui后就可以对接了，适配gradio监听端口即可。  

#### GPT-SoVITS

官方仓库：[GPT-SoVITS](https://github.com/RVC-Boss/GPT-SoVITS)  

整合包下载：[https://pan.quark.cn/s/936dcae8aba0](https://pan.quark.cn/s/936dcae8aba0)，[https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1](https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1)     

视频教程：[BV1CJ4m1b7pR](https://www.bilibili.com/video/BV1CJ4m1b7pR)  

天降之物模型分享：[https://github.com/Ikaros-521/GPT-SoVITS/releases](https://github.com/Ikaros-521/GPT-SoVITS/releases)  

运行webui后，启动TTS推理，然后适配配置项即可，注意参考音频路径还有ws的端口即可，别的配置问题不大。  

#### clone-voice

官方仓库：[clone-voice](https://github.com/jianchang512/clone-voice)  

整合包下载：[https://pan.quark.cn/s/936dcae8aba0](https://pan.quark.cn/s/936dcae8aba0) ，[https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1](https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1)   

视频教程：[BV17z421d7T9](https://www.bilibili.com/video/BV17z421d7T9/)  

#### Azure TTS

视频教程：[【AI主播-TTS篇】接入 Azure TTS，微软官方商用语音合成，随便造（](https://www.bilibili.com/video/BV1aJ4m1h7eY)  

官网：[https://azure.microsoft.com/zh-cn/products/ai-services/text-to-speech/](https://azure.microsoft.com/zh-cn/products/ai-services/text-to-speech/)  

注册账号，领取一年免费试用额度，创建 语音转文本服务，获取 区域 和 密钥，配置后进行使用。  

#### fish-speech

官方仓库：[fish-speech](https://github.com/fishaudio/fish-speech)  

官方文档：[https://speech.fish.audio/inference/](https://speech.fish.audio/inference/)  

##### 在线web

官网：[https://fs.firefly.matce.cn/](https://fs.firefly.matce.cn/)  

进入官网，选好参数，F12打开开发者工具，抓包 网络，ws，点击 Generate 合成音频，查看 join请求，展开后可以看到 参考音频的绝对路径和其他配置，配置到webui保存 运行即可使用。  

![参考图](https://private-user-images.githubusercontent.com/40910637/329521947-c123e1e1-ac26-4275-a8be-4e8f6224d1d2.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTU0MTk3NTEsIm5iZiI6MTcxNTQxOTQ1MSwicGF0aCI6Ii80MDkxMDYzNy8zMjk1MjE5NDctYzEyM2UxZTEtYWMyNi00Mjc1LWE4YmUtNGU4ZjYyMjRkMWQyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA1MTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwNTExVDA5MjQxMVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTQwYmQ0ZGJjNmNiZmY5NzE2ZGQ1OWJmZGNlMDJkNjY2ZjA2MGZhM2E5ODVmMDRhZDlkODAzODJiZDM2NTc4ZWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.sMJEI5tYYLZnPv0bZWXeoeMWL9yYpFOvYJDjN157HMQ)  

##### api 1.1.0

B站找个对应版本的整合包，启动API的bat脚本。然后把配置都配上就行了。  
图文文档：[https://github.com/Ikaros-521/AI-Vtuber/pull/827](https://github.com/Ikaros-521/AI-Vtuber/pull/827)  

#### ChatTTS

官方仓库：[https://github.com/2noise/ChatTTS](https://github.com/2noise/ChatTTS)  

视频教程：[https://www.bilibili.com/video/BV17D421g7cx](https://www.bilibili.com/video/BV17D421g7cx)  

#### CosyVoice

官方仓库：[https://github.com/FunAudioLLM/CosyVoice](https://github.com/FunAudioLLM/CosyVoice)  

视频教程：[https://www.bilibili.com/video/BV1iw4m1a7zx/](https://www.bilibili.com/video/BV1iw4m1a7zx/)  

#### MultiTTS

图文文档：[https://github.com/Ikaros-521/AI-Vtuber/pull/1042](https://github.com/Ikaros-521/AI-Vtuber/pull/1042)  

视频教程：[https://www.bilibili.com/video/BV1DRSbYaEP3/](https://www.bilibili.com/video/BV1DRSbYaEP3/)  

