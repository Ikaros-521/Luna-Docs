---
hide:
  - navigation
---

# ✨ Luna AI ✨

!!! tip "数据"

    <a href="//github.com/Ikaros-521/AI-Vtuber/stargazers">
        <img alt="GitHub stars" src="//img.shields.io/github/stars/Ikaros-521/AI-Vtuber?color=%09%2300BFFF&style=flat-square">
    </a>
    <a href="//github.com/Ikaros-521/AI-Vtuber/issues">
        <img alt="GitHub issues" src="//img.shields.io/github/issues/Ikaros-521/AI-Vtuber?color=Emerald%20green&style=flat-square">
    </a>
    <a href="//github.com/Ikaros-521/AI-Vtuber/network">
        <img alt="GitHub forks" src="//img.shields.io/github/forks/Ikaros-521/AI-Vtuber?color=%2300BFFF&style=flat-square">
    </a>
    <a href="/">
        <img src="//img.shields.io/github/license/Ikaros-521/AI-Vtuber.svg" alt="license">
    </a>
    <a href="//www.python.org">
        <img src="//img.shields.io/badge/python-3.10+-blue.svg" alt="python">
    </a>

!!! example inline end "广告"

    如需付费调试，请联系 `327209194`

    交流群 `587663288`

!!! quote "介绍"

    `Luna AI` 是一款结合了最先进技术的虚拟AI主播。它整合了很多高效的人工智能模型和平台，包括 `ChatterBot、GPT、Claude、langchain、chatglm、text-generation-webui、讯飞星火、智谱AI、谷歌Bard、文心一言、通义星尘、通义千问、千帆大模型、Gemini、Kimi Chat、QAnything、koboldcpp、FastGPT、Ollama、One-API、AnythingLLM、LLM_TPU`。通过 Luna AI, 我们既可以在本地运行本地模型，也可以通过云端服务使用开放式 AI 平台的功能。当然，为了让对话照进现实，Luna AI 还结合了多模态模型，包括 `Gemini` 的图像识别能力，获取电脑画面进行分析讲解。 

    `Luna AI` 的外观由 `Live2D、Vtube Studio、xuniren、UE5 结合 Audio2Face、EasyAIVtuber、数字人视频播放器（Easy-Wav2Lip、Sadtalker、GeneFace++、MuseTalk、本地视频）、metahuman-stream（ernerf、musetalk）` 技术打造，为用户提供了一个生动、互动的虚拟形象。这使得 `Luna AI` 能够在各大直播平台，如 `Bilibili、抖音、快手、微信视频号、拼多多、1688、斗鱼、YouTube、Twitch 和 TikTok`，进行实时互动直播。当然，它也可以在本地环境中与您进行个性化对话。

    为了使交流更加自然，`Luna AI` 使用了先进的自然语言处理技术和文本转语音技术，如 `Edge-TTS、VITS-Fast、elevenlabs、bark-gui、VALL-E-X、睿声AI、genshinvoice.top、tts.ai-lab.top、OpenVoice、GPT_SoVITS、clone-voice、Azure TTS、fish-speech、ChatTTS`。这些技术能够生成流畅的回答，而且 Luna AI 还可以通过 `so-vits-svc 和 DDSP-SVC` 实现声音的变化，以适应不同的场景和角色。

    此外，`Luna AI` 还能够通过特定指令与 `Stable Diffusion` 协作，展示画作。用户还可以自定义文案，让 Luna AI 循环播放，以满足不同场合的需求。

!!! warning "License"

    这个项目采用 GNU通用公共许可证（GPL） 进行许可。有关详细信息，请参阅 LICENSE 文件。  

    This project is licensed under the `GNU General Public License (GPL)`. Please see the `LICENSE` file for more details.  

!!! danger "注意"

    严禁将此项目用于一切违反《中华人民共和国宪法》，《中华人民共和国刑法》，《中华人民共和国治安管理处罚法》和《中华人民共和国民法典》之用途。  
    
    严禁用于任何政治相关用途。

!!! note "导航"

    <a href="//space.bilibili.com/3709626/channel/collectiondetail?sid=1422512" target="_blank">:fontawesome-solid-video: 视频教程合集</span></a>
    <span> | </span>
    <a href="/">:material-file-document: 在线文档</span></a>
    <span> | </span>
    <a href="//github.com/Ikaros-521/AI-Vtuber" target="_blank">:simple-github: GitHub</span></a>
    <span> | </span>
    <a href="//gitee.com/ikaros-521/AI-Vtuber" target="_blank">:simple-gitee: Gitee</span></a>

![mind-map](./static/images/luna-ai/xmind.png)

## :material-file-tree: 项目结构

!!! abstract "项目结构"

    - `config.json` 配置文件
    - `main.py` GUI主程序。会根据配置调用各平台程序
    - `utils` 文件夹，存储聊天、音频、通用类相关功能的封装实现
    - `data` 文件夹，存储数据文件、违禁词、文案等
    - `log` 文件夹，存储运行日志、字幕日志等
    - `out` 文件夹，存储TTS、SVC输出的音频文件，文案输出的音频文件
    - `Live2D` 文件夹，存储Live2D源码及模型
    - `song` 文件夹，存储点歌模式的歌曲
    - `docs` 文件夹，存储项目相关文档
    - `tests` 文件夹，存储单一功能点的测试程序
    - `cookie` 文件夹，存储部分功能需要用到的cookie数据

## :material-cloud-download: 下载项目

#### 首先你得装个 `git`（啥，没装？[百度:material-file-search:](https://bing.com/search?q=git)），当然也可以直接在页面切换分支后下载各版本 ZIP 压缩包   

```shell
# 主线（推荐）
git clone https://github.com/Ikaros-521/AI-Vtuber.git

# owner分支
git clone -b owner https://github.com/Ikaros-521/AI-Vtuber.git
```

!!! 整合包

    Windows整合包下载（不会装环境就用整合包捏）：
    - [github :octicons-link-16:](//github.com/Ikaros-521/AI-Vtuber/releases)
    - [迅雷云盘 :octicons-link-16:](https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1)
    - [夸克网盘 :octicons-link-16:](https://pan.quark.cn/s/936dcae8aba0)

## :material-run-fast: 运行环境

#### 操作系统

- Windows 10 及以上
- MacOS
- Linux

Windows部署建议直接使用整合包！  

MacOS部署问题讨论：[https://github.com/Ikaros-521/AI-Vtuber/issues/423](https://github.com/Ikaros-521/AI-Vtuber/issues/423)  
Linux部署问题讨论：[https://github.com/Ikaros-521/AI-Vtuber/issues/520](https://github.com/Ikaros-521/AI-Vtuber/issues/520)  

#### Python 版本 `3.10.11`

依赖的库在 `requirements.txt` 中，请自行安装。 
 
!!! danger "注意"
    
    安装目录请勿在 `中文路径、带有空格的路径、带有特殊字符的路径` ，可能会导致程序无法运行或运行异常

依赖版本参考 `requirements_common.txt`

安装命令参考：  

```shell
pip install -r requirements.txt
```

直接安装会版本冲突，需要注释冲突部分，手动安装，部分库向下兼容，版本参考`requirements_comment.txt`：[issue#868](https://github.com/Ikaros-521/AI-Vtuber/issues/868)  

自行安装依赖100%出现依赖冲突问题，参考仓库issue：[https://github.com/Ikaros-521/AI-Vtuber/issues/655](https://github.com/Ikaros-521/AI-Vtuber/issues/655)  

!!! note

    部署视频教程 [哔哩哔哩 :octicons-link-16:](//www.bilibili.com/video/BV1fV4y1C77r)  

## :material-file-edit: 配置

#### WebUI 程序运行后会自动加载配置文件，可以通过 WebUI 程序进行配置修改（清空配置项可以看到配置项的说明），也可以手动修改配置运行。

配置都在 `config.json`（此处只列举了大部分，因为实在是太多了，懒了）

??? note "config.json"

    ```json
    {
        // 你的直播间号,兼容全平台，都是直播间页面的链接中最后的数字和字母。例如:123
        "room_display_id": "你的直播间号",
        // 选用的聊天类型：chatterbot/chatgpt/claude/chat_with_file/chatglm/sparkdesk/reread/none 其中reread就是复读机模式,none是不启用
        "chat_type": "none",
        // 弹幕语言筛选，none就是全部语言，en英文，jp日文，zh中文
        "need_lang": "none",
        // 请求chatgpt/claude时，携带的字符串头部，用于给每个对话追加固定限制
        "before_prompt": "请简要回复:",
        // 请求chatgpt/claude时，携带的字符串尾部
        "after_prompt": "",
        // 弹幕日志类型，用于记录弹幕触发时记录的内容，默认只记录回答，降低当用户使用弹幕日志显示在直播间时，因为用户的不良弹幕造成直播间被封禁问题
        "comment_log_type": "回答",
        "filter": {
            // 弹幕过滤，必须携带的触发前缀字符串（任一）
            "before_must_str": [],
            // 弹幕过滤，必须携带的触发后缀字符串（任一）
            "after_must_str": [
                ".",
                "。",
                "?",
                "？"
            ],
            // 本地违禁词数据路径（你如果不需要，可以清空文件内容）
            "badwords_path": "data/badwords.txt",
            // 最长阅读的英文单词数（空格分隔）
            "max_len": 30,
            // 最长阅读的字符数，双重过滤，避免溢出
            "max_char_len": 50
        },
        // 答谢相关配置
        "thanks": {
            // 是否启用入场欢迎
            "entrance_enable": true,
            // 是否启用礼物答谢
            "gift_enable": true,
            // 入场欢迎文案
            "entrance_copy": "欢迎 {username}",
            // 礼物答谢文案
            "gift_copy": "感谢 {username} 送的 {gift_name}",
            // 最低礼物答谢金额
            "lowest_price": 1.0
        },
        // Live2D皮
        "live2d": {
            // 是否启用
            "enable": true,
            // web服务监听端口
            "port": 12345
        },
        "openai": {
            "api": "https://api.openai.com/v1",
            "api_key": [
                "你的api key"
            ]
        },
        // claude相关配置
        "claude": {
            // claude相关配置
            // 参考：https://github.com/bincooo/claude-api#readme
            "slack_user_token": "",
            "bot_user_id": ""
        },
        // chatglm相关配置
        "chatglm": {
            "api_ip_port": "http://127.0.0.1:8000",
            "max_length": 2048,
            "top_p": 0.7,
            "temperature": 0.95
        },
        // 讯飞星火相关配置
        "sparkdesk": {
            // 两种类型 web api
            "type": "web",
            // web类型下 抓包中的cookie，详情见拓展教程
            "cookie": "",
            // web类型下 抓包中的fd
            "fd": "",
            // web类型下 抓包中的GtToken
            "GtToken": "",
            // api类型下 申请api后平台中的appid
            "app_id": "",
            // api类型下 申请api后平台中的appsecret
            "api_secret": "",
            // api类型下 申请api后平台中的appkey
            "api_key": ""
        },
        "chat_with_file": {
            // 本地向量数据库模式
            "chat_mode": "claude",
            // 本地文件地址
            "data_path": "data/伊卡洛斯百度百科.zip",
            // 切分数据块的标志
            "separator": "\n",
            // 向量数据库数据分块
            "chunk_size": 100,
            // 每个分块之间的重叠字数。字数越多，块与块之间的上下文联系更强，但不能超过chunk_size的大小。同时chunk_size和chunk_overlap越接近，构造向量数据库的耗时越长
            "chunk_overlap": 50,
            "chain_type": "stuff",
            // 适用于openai模式，显示消耗的token数目
            "show_token_cost": false,
            "question_prompt": "请根据以上content信息进行归纳总结，并结合question的内容给出一个符合content和question语气、语调、背景的回答。不要出现'概括''综上''感谢'等字样，向朋友    直接    互相交流即可。如果发现不能content的信息与question不相符，抛弃content的提示，直接回答question即可。任何情况下都要简要地回答!",
            // 最大查询数据库次数。限制次数有助于节省token
            "local_max_query": 3,
            // 默认本地向量数据库模型
            "local_vector_embedding_model": "sebastian-hofstaetter/distilbert-dot-tas_b-b256-msmarco"
        },
        // 语音合成类型选择 edge-tts/vits_fast/elevenlabs
        "audio_synthesis_type": "edge-tts",
        // vits_fast相关配置
        "vits_fast": {
            // 配置文件的路径
            "vits_fast_config_path": "E:\\GitHub_pro\\VITS-fast-fine-tuning\\inference\\finetune_speaker.json",
            // 推理服务运行的链接（需要完整的URL）
            "vits_fast_api_ip_port": "http://127.0.0.1:7860",
            // 选择的说话人，配置文件中的speaker中的其中一个
            "character": "ikaros"
        },
        // so-vits-svc相关配置
        "so_vits_svc": {
            // 启用功能 true启用 false关闭
            "enable": false,
            // 模型配置文件路径
            "config_path": "D:\\so-vits-svc\\configs\\ikaros_v1.json",
            // 服务运行的ip端口（注意，请运行flask_api_full_song.py）
            "api_ip_port": "http://127.0.0.1:1145",
            // 说话人，源自配置文件
            "spk": "ikaros",
            // 音调
            "tran": 1.0,
            // 输出音频格式
            "wav_format": "wav"
        },
        // edge-tts相关配置
        "edge-tts": {
            // edge-tts选定的说话人(cmd执行：edge-tts -l 可以查看所有支持的说话人)
            "voice": "zh-CN-XiaoyiNeural"
            // 语速增益 默认是 +0%，可以增减，注意 + - %符合别搞没了，不然会影响语音合成
            "rate": "+0%",
            // 音量增益 默认是 +0%，可以增减，注意 + - %符合别搞没了，不然会影响语音合成
            "volume": "+0%",
            // 语速
            "speed": 1
        },
        // elevenlabs相关配置
        "elevenlabs": {
            // elevenlabs密钥，可以不填，默认也有一定额度的免费使用权限，具体多少不知道
            "api_key": "",
            // 选择的说话人名
            "voice": "Domi",
            // 选择的模型
            "model": "eleven_monolingual_v1"
        },
        // genshinvoice.top相关配置
        "genshinvoice_top": {
            // 说话人
            "speaker": "神里绫华",
            // 输出音频格式 不建议修改
            "format": "wav",
            // 可用于控制整体语速。默认为1.2
            "length": "1.25",
            // 控制感情变化程度，默认为0.2
            "noise": "0.2",
            // 控制音节发音长度变化程度，默认为0.9
            "noisew": "0.9"
        },
        // chatterbot相关配置
        "chatterbot": {
            // 机器人名
            "name": "bot",
            // bot数据库路径
            "db_path": "db.sqlite3"
        },
        // chatgpt相关配置
        "chatgpt": {
            "model": "gpt-3.5-turbo",
            // 控制生成文本的随机性。较高的温度值会使生成的文本更随机和多样化，而较低的温度值会使生成的文本更加确定和一致。
            "temperature": 0.9,
            "max_tokens": 2048,
            "top_p": 1,
            "presence_penalty": 0,
            "frequency_penalty": 0,
            "preset": "请扮演一个AI虚拟主播。不要回答任何敏感问题！不要强调你是主播，只需要回答问题！"
        },
        // text-generation-webui相关配置
        "text_generation_webui": {
            // 服务监听的IP和端口
            "api_ip_port": "http://127.0.0.1:5000",
            "max_new_tokens": 250,
            // 有 'chat', 'chat-instruct', 'instruct'
            "mode": "chat",
            // 角色
            "character": "Example",
            // 聊天指导模板
            "instruction_template": "Vicuna-v1.1",
            // 你的名字
            "your_name": "你"
        },
        // 是否启用本地问答库匹配机制，优先级最高，如果匹配则直接合成问答库内的内容/返回本地音频，如果不匹配则按照正常流程继续。
        "local_qa": {
            // 文本匹配模式
            "text": {
                // 是否启用
                "enable": true,
                // 文本问答库文件路径，数据为一问一答形式（换行分隔）
                "file_path": "data/本地问答库.txt"
            },
            // 音频匹配模式
            "audio": {
                // 是否启用
                "enable": true,
                // 文本问答库音频文件路径，匹配的关键词就是音频文件名，为模糊最优匹配
                "file_path": "out/本地问答音频/"
            }
        },
        // 点歌模式设置
        "choose_song": {
            // 是否启用 true启用 false关闭
            "enable": true,
            // 点歌触发命令（完全匹配才行）
            "start_cmd": "点歌 ",
            // 停止点歌命令（完全匹配才行）
            "stop_cmd": "取消点歌",
            // 歌曲音频路径（默认为本项目的song文件夹）
            "song_path": "song",
            // 匹配失败返回的音频文案 注意 {content} 这个是用于替换用户发送的歌名的，请务必不要乱删！影响使用！
            "match_fail_copy": "抱歉，我还没学会唱{content}"
        },
        // stable diffusion相关配置
        "sd": {
            // 是否启用
            "enable": false,
            // 触发的关键词（弹幕头部触发）
            "trigger": "画画：",
            // 服务运行的IP地址
            "ip": "127.0.0.1",
            // 服务运行的端口
            "port": 7860,
            // 负面文本提示，用于指定与生成图像相矛盾或相反的内容
            "negative_prompt": "ufsw, longbody, lowres, bad anatomy, bad hands, missing fingers, pubic hair,extra digit, fewer digits, cropped, worst quality,   low quality",
            // 随机种子，用于控制生成过程的随机性。可以设置一个整数值，以获得可重复的结果。
            "seed": -1,
            // 样式列表，用于指定生成图像的风格。可以包含多个风格，例如 ["anime", "portrait"]。
            "styles": [],
            // 提示词相关性，无分类器指导信息影响尺度(Classifier Free Guidance Scale) -图像应在多大程度上服从提示词-较低的值会产生更有创意的结果。
            "cfg_scale": 7,
            // 生成图像的步数，用于控制生成的精确程度。
            "steps": 30,
            // 是否启用高分辨率生成。默认为 False。
            "enable_hr": false,
            // 高分辨率缩放因子，用于指定生成图像的高分辨率缩放级别。
            "hr_scale": 2,
            // 高分辨率生成的第二次传递步数。
            "hr_second_pass_steps": 20,
            // 生成图像的水平尺寸。
            "hr_resize_x": 512,
            // 生成图像的垂直尺寸。
            "hr_resize_y": 512,
            // 去噪强度，用于控制生成图像中的噪点。
            "denoising_strength": 0.4
        },
        // 文案相关配置（待更新）
        "copywriting": {
            // 文案文件存储路径，不建议更改。
            "file_path": "data/copywriting/",
            // 文案文件存储路径2，不建议更改。
            "file_path2": "data/copywriting2/",
            // 文案音频文件存储路径，不建议更改。
            "audio_path": "out/copywriting/",
            // 文案音频文件存储路径2，不建议更改。
            "audio_path2": "out/copywriting2/",
            // 播放音频文件列表
            "play_list": [
                "测试文案2.wav",
                "测试文案3.wav",
                "吐槽.wav"
            ],
            // 播放音频文件列表2
            "play_list": [
                "test.wav"
            ],
            // 文案音频播放之间的间隔时间。就是前一个文案播放完成后，到后一个文案开始播放之间的间隔时间。
            "audio_interval": 5,
            // 文案音频切换到弹幕音频的切换间隔时间（反之一样）。就是在播放文案时，有弹幕触发并合成完毕，此时会暂停文案播放，然后等待这个间隔时间后，再播放弹幕回复音频。
            "switching_interval": 5,
            // 文案随机播放，就是不根据播放音频文件列表的顺序播放，而是随机打乱顺序进行播放。
            "random_play": true
        },
        "header": {
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.42"
        },
        // 聊天模式相关配置
        "talk": {
            // 你的名称
            "username": "主人",
            // 使用的语音识别类型 baidu / google
            "type": "google",
            // 录音触发按键（长按此按键进行录音）
            "trigger_key": "1",
            // 音量阈值，指的是触发录音的起始音量值，请根据自己的麦克风进行微调到最佳
            "volume_threshold": 800,
            // 沉默阈值，指的是触发停止路径的最低音量值，请根据自己的麦克风进行微调到最佳
            "silence_threshold": 15,
            // 百度语音识别 申请：https://console.bce.baidu.com/ai/#/ai/speech/overview/index
            "baidu": {
                // 百度云 语音识别应用的 AppID
                "app_id": "",
                // 百度云 语音识别应用的 API Key
                "api_key": "",
                // 百度云 语音识别应用的 Secret Key
                "secret_key": ""
            },
            // 谷歌语音识别
            "google": {
                // 录音后识别转换成的目标语言（就是你说的语言）
                "tgt_lang": "zh-CN"
            }
        },
        // 字幕相关配置
        "captions": {
            // 是否启用字幕记录
            "enable": true,
            // 字幕输出路径
            "file_path": "log/字幕.txt"
        }
    }
    ```

## :material-chat: ChatGPT 代理

- 例如 [API2D :octicons-link-16:](//api2d.com/wiki/doc)  

```json
"openai": {
    // 代理地址，需要和官方接口一致的才行。例如：api2d
    "api": "https://oa.api2d.net/v1",
    // 代理站提供的密钥
    "api_key": [
        "fkxxxxxxxxxxx"
    ]
}
```

- one-api

官方仓库：[one-api](//github.com/songquanpeng/one-api)  

!!! note "或者纯代理的镜像站"

    - 合作伙伴 [智来星球 :octicons-link-16:](//m.zlxqai.com) 提供

        - [129.226.219.212:9000 :octicons-link-16:](//129.226.219.212:9000)
        - [43.134.230.167:9000 :octicons-link-16:](//43.134.230.167:9000)

    - 源自互联网

        - [openai-pag.wangzhishi.net :octicons-link-16:](//openai-pag.wangzhishi.net)

    - 如何配置呢？  

        GUI中openai api地址配置为：`http://openai-pag.wangzhishi.net/v1`

        ![image](./static/images/luna-ai/253742483-ce47dd53-118e-488a-94d6-0d837db23e6c.png)


??? note "`chat_with_file` 模式说明"

    一. 模式简介


    用户上传的“人物设定”文件（如PDF、TXT等格式），允许用户自定义并配置角色的背景信息和设定。

    1.用户提出查询时，系统首先在本地文档库中执行相似性搜索，以寻找与查询最相关的文档。

    2.接着，系统将这些相关文档连同用户的查询一起作为输入，提交给语言模型。该模型据此生成答案。

    3.如果系统在本地文档库中未能找到与用户查询相关的文档，或者语言模型无法基于当前输入生成有意义的答案，系统可能无法回应用户的查询。


    二. 模式配置

    为了使用`chat_with_file`功能，您需要将`chat_type`设置为`chat_with_file`。在启用此功能之前，请确保您已经配置好了如`openai`、`claude`等模型的访问`token`。
    `chat_with_file`支持以下几种模式，您可以通过设置`chat_mode`来选择相应的模式：

    - **`claude`**：选择`claude`作为聊天模型。请确保您已经完成了相关配置。

    - **`local_vector_embedding_model`**：使用本地向量数据库模式。在此模式下，系统会利用本地向量数据库来存储和检索数据。

    - **`openai_vector_search`**：仅利用向量数据库进行查询，而不调用GPT模型，这样可以节省`token`，并且能够进行快速的本地数据搜索。目前，此模式采用`OpenAIEmbedding`进行数据的向量化处理，因此需要您提前配置好OpenAI的相关设置。

    - **`openai_gpt`**：在向量数据库中检索到相关信息后，将其作为输入传递给GPT模型进行更深层次的处理。

    我们推荐使用`claude`模式，因为它可以免费使用，并且不会消耗`openai`的`token`。

    后续会支持更多免费模型，如 `文心一言、讯飞星火` 等。

    !!! note "注意"

        1. 所有模型都应该采用 `HuggingFace` 模型，暂未适配其他模型

        2. 本地模型存储目录是 `data/text2vec_models` ，将自己的模型存储到该位置，在 `config.json` 配置中填写该模型的 `文件夹名字` 即可

        3. 如果需要其他模型，可以从 `HuggingFace` 中下载下来，存放到对应位置即可

        4. 也可以直接输入 `HuggingFace` 的模型名字，如 [GanymedeNil/text2vec-large-chinese :octicons-link-16:](//huggingface.co/GanymedeNil/text2vec-large-chinese) ，项目会自动从远程仓库下载。

            1. 请确保能够连接上 `HuggingFace` (可能需要科学上网)

            2. 远程仓库下载的模型，一般存储在系统cache中。win端一般是 `C:\Users\用户\.cache\torch\sentence_transformers` 。也可以将其移动到项目模型存储目录下使用

        5. `openai_vector_search` 和 `openai_gpt` 读取本地数据的内容默认以换行为分隔符，所以可能导致大标题数据丢失问题，需要注意你的数据内容在编辑时不要将核心的内容放在标题部分单独一行，导致丢失 核心数据，尽量将标题和正文写在一行，在真的需要分割的部分进行换行。  


## :fontawesome-solid-user: 使用

!!! note

    运行webui，`python webui.py`，配置平台配置、直播间号等，具体参考视频教程。  

    实战教程：[【AI主播-实战篇】AI前台/客服/看板娘，现实中对话AI，提供聊天/知识问答服务，实际全配置演示，手把手带你应用](https://www.bilibili.com/video/BV1sm411Z79H)  

### 各版本都需要做的前期准备操作。

#### Chatterbot

??? note "`Chatterbot` 相关安装&使用"

    ##### 运行环境

    - `Python 3.6+`

    ##### 安装依赖
    在命令行中安装所需的Python库，您可以使用以下命令：

    ```bash
    pip install spacy ChatterBot
    ```

    如果遇到ChatterBot安装错误，您可以尝试安装更新版本的ChatterBot。首先，访问ChatterBot的更新版本仓库：

    [ChatterBot_update :octicons-link-16:](https://github.com/RaSan147/ChatterBot_update)

    从该GitHub仓库下载更新版本的ChatterBot后，您可以在下载的文件夹内运行以下命令来安装：

    ```bash
    python setup.py install
    ```

    如果您在安装过程中遇到速度慢的问题，可以考虑单独安装依赖项。例如，如果您需要安装SQLAlchemy，可以使用以下命令：

    ```bash
    pip install SQLAlchemy==1.3.24
    ```

    ##### 如何训练自己的AI？

    - 打开 `data/db.txt` ，写入你想要训练的内容，格式如下

    ```
    问
    答
    问
    答
    ```

    - 将文件重命名为 `data/db.txt`
    - 在命令行中运行以下命令启动程序：

    ```bash
    python train.py
    ```

    - 训练完的模型名叫 `db.sqlite3` ，直接双击 `main.py` 即可使用

    ##### 常见问题
    1. 提示缺少 `en-core-web-sm` ，打开终端输入

    ```bash
    python -m spacy download en_core_web_sm
    ```

    2. 报错：no module named ‘spacy’解决办法

    ```bash
    pip install spacy
    ```
    

#### 哔哩哔哩

注意：如果使用方案2，需要手动克隆官方项目仓库的 [blivedm](https://github.com/xfgryujk/blivedm) 到`site-packages`  


#### 抖音

先安装第三方弹幕捕获软件，参考 [补充-抖音](#dy)

#### 抖音版 旧版

!!! danger "不稳定"


运行前请重新生成一下protobuf文件，因为机器系统不一样同时protobuf版本也不一样所以不能拿来直接用～  

```shell
protoc -I . --python_out=. dy.proto
```

!!! note

    依赖 [golang :octicons-link-16:](//go.dev/dl/) 环境，还没有的话，手动补一补 [protobuf :octicons-link-16:](//github.com/protocolbuffers/protobuf/releases)


#### 快手

##### 方案1：

请在安装完依赖后，安装火狐浏览器内核。参考命令：`playwright install firefox`

如果你是整合包，项目路径打开cmd，然后使用 `Miniconda3\python.exe Miniconda3\Scripts\playwright.exe install firefox` 进行安装。

使用新版本时需要注意，请使用小号登录，然后在每次用完之后，把 `cookie` 文件夹下的 `123.json` 文件删掉！！！用过一次后 cookie 就异常了，所以需要删了重新登录！！！  

##### 方案2：

配合油猴脚本：[https://greasyfork.org/zh-CN/scripts/490966](https://greasyfork.org/zh-CN/scripts/490966)，在浏览器直播间页面监听DOM变动，WS返回数据。  

浏览器安装[油猴插件](https://www.tampermonkey.net/)后，再安装上面的脚本，打开需要监听的直播间后，就会自动监听弹幕，连接WS服务，然后把AI Vtuber运行起来，进行对接。  

##### 方案0：  

运行前请重新生成一下 protobuf 文件，因为机器系统不一样同时 protobuf 版本也不一样所以不能拿来直接用～  

```shell
protoc -I . --python_out=. ks.proto
```

!!! note

    依赖 [golang :octicons-link-16:](//go.dev/dl/) 环境，还没有的话，手动补一补 [protobuf :octicons-link-16:](//github.com/protocolbuffers/protobuf/releases)


#### 微信视频号


!!! note

    安装监听程序（不保证安全性，自行斟酌） [wxlivespy](https://github.com/fire4nt/wxlivespy/releases)，设置监听地址为`http://127.0.0.1:8082/wxlive`，开播！开始监听，扫描登录直播的微信号。webui修改平台为`微信视频号`，运行即可。  


#### 拼多多

配合油猴脚本：[https://greasyfork.org/zh-CN/scripts/490966](https://greasyfork.org/zh-CN/scripts/490966)，在浏览器直播间页面监听DOM变动，WS返回数据。  

浏览器安装[油猴插件](https://www.tampermonkey.net/)后，再安装上面的脚本，打开需要监听的直播间后，就会自动监听弹幕，连接WS服务，然后把AI Vtuber运行起来，进行对接。  

#### 斗鱼


打开您的浏览器，找到您需要监听的直播间，然后按F12打开开发者工具，点击Console（控制台），复制 `douyu_ws_client.js` 脚本中的内容，粘贴到控制台，回车运行，启动监听服务

??? note "douyu_ws_client.js"

    ```javascript
    let socket = null;

    function connectWebSocket() {
    // 创建 WebSocket 连接，适配服务端
    socket = new WebSocket("ws://127.0.0.1:5000");

    // 当连接建立时触发
    socket.addEventListener("open", event => {
        console.log("ws连接打开");

        // 向服务器发送一条消息
        // socket.send("ws连接成功");
    });

    // 当收到消息时触发
    socket.addEventListener("message", event => {
        console.log("收到服务器数据:", event.data);
    });

    // 当连接关闭时触发
    socket.addEventListener("close", event => {
        console.log("WS连接关闭");

        // 重连
        setTimeout(() => {
        connectWebSocket();
        }, 1000); // 延迟 1 秒后重连
    });
    }

    // 初始连接
    connectWebSocket();


    // 选择需要观察变化的节点
    const targetNode = document.querySelector('.Barrage-list');

    // 创建观察器实例
    const observer = new MutationObserver(mutations => {
    mutations.forEach(mutation => {
        // 这里处理新增的DOM元素
        if (mutation.type === 'childList') {
        mutation.addedNodes.forEach(node => {
            // 判断是否是新增的弹幕消息
            if (node.classList.contains('Barrage-listItem')) {
            // 新增的动态DOM元素处理
            // console.log('Added node:', node);

            const spans = node.getElementsByTagName('span');

            let username = "";
            let content = "";

            for (let span of spans) {
                //console.log(span);
                if (span.classList.contains('Barrage-nickName')) {
                const targetSpan = span;
                // 获取用户名
                let tmp = targetSpan.textContent.trim().slice(0, -1);
                if (tmp != "") username = targetSpan.textContent.trim().slice(0, -1);
                } else if (span.classList.contains('Barrage-content')) {
                const targetSpan = span;
                // 获取弹幕内容
                content = targetSpan.textContent.trim();
                }
            }

            console.log(username + ":" + content);

            // 获取到弹幕数据
            if (username != "" && content != "") {
                const data = {
                type: "comment",
                username: username,
                content: content
                };
                console.log(data);
                socket.send(JSON.stringify(data));
            }
            }
        })
        }
    });
    });

    // 配置观察选项
    const config = {
    childList: true,
    subtree: true
    };

    // 开始观察
    observer.observe(targetNode, config);
    ```



## :material-image: 效果图

!!! note "WebUI 界面"

    ![动画](./static/images/luna-ai/261792128-6ba4ba49-aa1b-43b0-989f-58a851dfd054.gif)


!!! note "SD 接入"

    ![image](./static/images/luna-ai/248568910-a3e4b3b7-96d1-41b1-b45e-f2725acee27c.png)

## :material-frequently-asked-questions: 常见问题

??? note "部署过程问题"

    - CondaSSLError: OpenSSL appears to be unavailable on this machine

    本地已经有 `Anaconda` 环境，在执行 半自动包的`1.创建虚拟环境.bat`时，出现报错 `CondaSSLError: OpenSSL appears to be unavailable on this machine`

    ![image](./static/images/luna-ai/247523399-8f6af198-a362-40ad-9c33-5f9576cdcfa8.png)

    解决方案：参考 [blog.csdn.net/mynameisyaxuan/article/details/128323026](//blog.csdn.net/mynameisyaxuan/article/details/128323026)  

    - ModuleNotFoundError: No module named 'xxx' 大同小异

    都是依赖库缺失问题，可以打开`requirements_bilibili.txt`/`requirements_dy.txt`/`requirements_ks.txt`内查看需要安装的依赖（可能还是遗漏...）  

    视情况更换镜像源，国内推荐清华源，如果清华源没有缺失的库，可以走pypi的源，安装命令如：
    
    `pip install PyQt5 -i https://pypi.tuna.tsinghua.edu.cn/simple`  

    注意：请在虚拟环境中安装！！！（如果你是根据半自动整合包做的话，先激活虚拟环境`conda activate ai_vtb`，然后进行安装）  

    ```shell
    https://pypi.org/simple
    https://pypi.python.org/simple/
    https://pypi.tuna.tsinghua.edu.cn/simple
    ```

    - ModuleNotFoundError: No module named 'PyQt5'

    半自动包 运行 `GUI运行.bat` 时，出现

    ```shell
    Traceback (most recent call last):
      File "F:\github_pro\AI-Vtuber\main.py", line 10, in <module>
        from PyQt5.QtWidgets import QApplication, QMainWindow, QMessageBox, QLabel, QComboBox, QLineEdit, QTextEdit, QDialog
    ModuleNotFoundError: No module named 'PyQt5'
    ```

    解决方案：手动补装 `PyQt5` ，需要注意，得在 `ai_vtb` 的虚拟环境中安装

    可以发现最左侧有这个括号，表示你激活了 `ai_vtb` 的虚拟环境中，然后你在运行 后面的pip安装 `(ai_vtb) F:\github_pro\AI-Vtuber>pip install PyQt5`

    ![image](./static/images/luna-ai/247523915-ee3ad055-b562-4f12-8797-d6aff44331be.png)

    - ModuleNotFoundError: No module named 'langid'

    半自动包 运行 `GUI运行.bat` 时，出现

    ```shell
    Traceback (most recent call last):
      File "F:\github_pro\AI-Vtuber\main.py", line 20, in <module>
        from utils.common import Common
      File "F:\github_pro\AI-Vtuber\utils\common.py", line 8, in <module>
        import langid
    ModuleNotFoundError: No module named 'langid'
    ```

    解决方案：手动补装 `langid` ，需要注意，得在 `ai_vtb` 的虚拟环境中安装， `pip install langid`

    ![image](./static/images/luna-ai/247598426-3047406b-a25c-4e53-9248-a21684dbaea4.png)

    如果遇到上图安装失败的问题 ， 走官方源下载 `pip install langid -i https://pypi.python.org/simple/`

    ![image](./static/images/luna-ai/247524637-0f08c00f-f7ac-41dd-a6a4-7f7539efa843.png)

    - ModuleNotFoundError: No module named 'profanity'

    半自动包 运行 `GUI运行.bat` 时，出现  

    ```shell
    Traceback (most recent call last):
      File "F:\github_pro\AI-Vtuber\main.py", line 20, in <module>
        from utils.common import Common
      File "F:\github_pro\AI-Vtuber\utils\common.py", line 10, in <module>
        from profanity import profanity
    ModuleNotFoundError: No module named 'profanity'
    ```

    解决方案：手动补装 `profanity` ，需要注意，得在 `ai_vtb` 的虚拟环境中安装， `pip install profanity`

    ![image](./static/images/luna-ai/247524836-3501aaca-9a08-45e3-b7bd-6aa60f9ea4b9.png)

    - ModuleNotFoundError: No module named 'ahocorasick'

    半自动包 运行`3.GUI运行.bat`时，出现  

    ```shell
    Traceback (most recent call last):
      File "F:\github_pro\AI-Vtuber\main.py", line 20, in <module>
        from utils.common import Common
      File "F:\github_pro\AI-Vtuber\utils\common.py", line 11, in <module>
        import ahocorasick
    ModuleNotFoundError: No module named 'ahocorasick'
    ```

    解决方案：手动补装 `pyahocorasick` ，需要注意，得在 `ai_vtb` 的虚拟环境中安装， `pip install pyahocorasick`

    ![image](./static/images/luna-ai/247523915-ee3ad055-b562-4f12-8797-d6aff44331be.png)

??? note "使用过程问题"

    - 启动 webui 时报错:  No module named 'g4f'

    未安装 g4f，手动安装一下

    ```shell
    pip install g4f
    ```

    诸如此类依赖的报错需要在启动的时候注意，全部解决掉，否则即便 webui 正常打开了， web 服务依然是启动失败的，运行某些功能的时候会报错: HTTPConnectionPool(host='127.0.0.1', port=8082)

    - openai 接口报错:《empty message》

    可能是API KEY过期了/额度没了，请检查API KEY是否可用。  

    在线测试参考：  

    [ChatGPT-Html](//ikaros521.eu.org/chatgpt-html)  

    [ChatGPT-Next-Web](//chat-gpt-next-web-ikaros-521.vercel.app)  

    - ERROR: Cannot install -r requirements_bilibili.txt (line 23), aiohttp and langchain==0.0.142 because these package versions have conflicting dependencies.

    依赖冲突问题。可以删除 `requirements_bilibili.txt` 中的 `langchain==0.0.142` 和 `bilibili-api-python==9.1.0` ，然后进行重新安装。安装完成后，手动安装这2个库（按顺序安装）。  

    ```shell
    Miniconda3\python.exe -m pip install bilibili-api-python==9.1.0
    Miniconda3\python.exe -m pip install langchain==0.0.142
    ```

    - ERROR: Conmunicate.`__init__`() got an unexpected keyword argument 'text'

    问题根因：Edge-TTS版本过低

    解决方案：升级到指定版本 `pip install edge-tts==6.1.6`


    - File ".\flask_api_full_song.py", line 38, in wav2wav  out_audio, out_sr = svc_model.infer(spk, tran, raw_path) ValueError: too many values to unpack (expected 2)
    注意！！！如果你是 `4.1` 版本的整合包，很可能就有这个bug，需要修改 `flask_api_full_song.py` 的38行左右：  
    改  

    ```shell
    out_audio, out_sr = svc_model.infer(spk, tran, raw_path)
    ```

    为

    ```shell
    out_audio, out_sr, n_frames = svc_model.infer(spk, tran, raw_path)
    ```

    - RuntimeWarning: Couldn't find ffmpeg or avconv - defaulting to ffmpeg, but may not work warn("Couldn't find ffmpeg or avconv - defaulting to ffmpeg, but may not work", RuntimeWarning)

    问题：pydub依赖ffmpeg，但环境不存在ffmpeg  

    解决方案：安装ffmpeg并配置环境变量  

    ffmpeg安装教程：[ffmpeg安装教程](//blog.csdn.net/HYEHYEHYE/article/details/122000352)  

    ffmpeg官方下载：[ffmpeg.org/download.html](//ffmpeg.org/download.html)  

    ffmpeg本仓库内下载：[releases](//github.com/Ikaros-521/AI-Vtuber/releases/tag/v0.13.0)  

    简述就是下载，解压，配置 ffmpeg 的 bin 到系统环境变量path中，完事。  

    - qt.qpa.plugin: Could not find the Qt platform plugin "windows" in "" This application failed to start because no Qt platform plugin could be initialized.    Reinstalling the application may fix this problem.

    问题：无法找到Qt。

    解决方案：如果你是整合包，那请检查是否在 `中文路径` 下！！！如果是自行安装的，可以尝试重装pyqt5。

    - 保存配置后没有自动重启，报错 [Errno 2] No such file or directory

    现象：  

    ```shell
    2023-08-03 17:27:24,700 - D:\GitHub_pro\AI-Vtuber-20230 729\main.py[line:1386] - INFO: 配置数据已成功写入文件！程序将在3秒后重启~
    D:\GitHub_pro\AI-Vtuber-20230: can't open file 'D:\\GitHub_pro\\AI-Vtuber-20230 729\\729\\Miniconda3\\python.exe': [Errno 2] No such file or directory
    ```

    问题：没有自动重启程序，并报错

    解决方案：请将项目放在 `非中文，无空格` 的路径下。  

    `D:\\GitHub_pro\\AI-Vtuber-20230 729` ——> `D:\\GitHub_pro\\AI-Vtuber-20230729`

    - 更新后报错 ImportError: cannot import name 'sync' from 'bilibili_api'

    完整报错：

    ```shell
    File "D:\GitHub_pro\AI-Vtuber-20230815\bilibili.py", line 9, in <module>
        from bilibili_api import live, sync
    ImportError: cannot import name 'sync' from 'bilibili_api' (D:\GitHub_pro\AI-Vtuber-20230815\Miniconda3\lib\site-packages\bilibili_api\__init__.py)
    ```

    问题根因：`bilibili_api`没有`sync`模块，其实是更新后，`bilibili_api`不对了，需要重新安装对应依赖。  

    解决方案：

    1.删除 `bilibili-api-python` 和 `bilibili-api` ，参考命令（整合包）： `Miniconda3\python.exe -m pip uninstall bilibili-api-python bilibili-api`，然后在提示出入（y/n）部分输入 `y` ，然后回车，共2次。  

    ```shell
    Proceed (Y/n)? y
      Successfully uninstalled bilibili-api-python-15.5.3
    Proceed (Y/n)? y
      Successfully uninstalled bilibili-api-4.1.0
    ```  

    2.重新安装，可以手动安装 `Miniconda3\python.exe -m pip install bilibili-api-python bilibili-api` ，也可以直接执行`2-2.安装依赖.bat`完成安装。 

    - 使用ChatGPT API，报错：error_message='You exceeded your current quota, please check your plan and billing details.'

    可能是API KEY过期了/额度没了，请检查API KEY是否可用。  

    ![image](./static/images/luna-ai/266388062-46821c28-0a16-4b86-a395-358a6c8b5b89.png)

    在线测试参考：  
    [ChatGPT-Html](//ikaros521.eu.org/chatgpt-html/)  
    [ChatGPT-Next-Web](//chat-gpt-next-web-ikaros-521.vercel.app/)  

    - Miniconda3\Scripts\playwright.exe install Fatal error in launcher: Unable to create process using  '"D:\GitHub_pro\AI-Vtuber-20230729\Miniconda3\python.exe"  "D:\ai3\AI-Vtuber-20230825\Miniconda3\Scripts\playwright.exe" install': ???????????

    playwright安装浏览器内核失败。   

    解决方案：重新安装playwright，需要注意，前提是激活了本地环境  

    ```shell
    pip uninstall playwright
    pip install playwright
    playwright install
    ```

    - ModuleNotFoundError: No module named 'blivedm.models.web'; 'blivedm.models' is not a package

    解决方案：[AI-Vtuber/issues/381#issuecomment-1774128497](//github.com/Ikaros-521/AI-Vtuber/issues/381#issuecomment-1774128497)

## API

API接口地址根据配置文件中webui的ip端口地址决定，默认：`http://127.0.0.1:8081`  

### 配置config

#### 概述

- **请求地址:** `/set_config`
- **请求类型:** POST
- **描述:** 修改配置文件。

#### 请求参数

| 参数名     | 类型    | 是否必需 | 描述         |
|--------    |--------|----------|--------------|
| config_path | string | 是       | 配置文件路径，例如：config.json |
| data       | object  | 是       | 配置文件内容（json），例如：{"platform": "bilibili"} |

#### 响应

| 参数名  | 类型    | 描述         |
|--------|-------- |--------------|
| code   | int     | 状态码，200为成功，小于0为错误代码，大于0为部分成功代码 |
| msg    | string  | 响应消息，描述请求的处理结果 |

### 系统命令

#### 概述

- **请求地址:** `/sys_cmd`
- **请求类型:** POST
- **描述:** 控制系统运行相关命令。

#### 请求参数

| 参数名     | 类型    | 是否必需 | 描述         |
|--------    |--------|----------|--------------|
| type | string | 是       | 命令类型（run/stop/restart/factory）。例如：run |
| data | object  | 是       | 数据文件内容（json），根据命令不同，数据内容也相应改变，具体参考源码中的实例。例如：{"config_path": "config.json"} |

#### 响应

| 参数名  | 类型    | 描述         |
|--------|-------- |--------------|
| code   | int     | 状态码，200为成功，小于0为错误代码，大于0为部分成功代码 |
| msg    | string  | 响应消息，描述请求的处理结果 |

### 发送数据

#### 概述

- **请求地址:** `/send`
- **请求类型:** POST
- **描述:** 发送平台弹幕、礼物、入场、复读等数据进行功能调用。

#### 请求参数

| 参数名     | 类型    | 是否必需 | 描述         |
|--------    |--------|----------|--------------|
| type | string | 是       | 数据类型（comment/gift/entrance/reread）。例如：comment |
| data | object  | 是       | 数据文件内容（json），根据命令不同，数据内容也相应改变，具体参考源码中的实例。例如：{"platform":"哔哩哔哩","username":"用户名","content":"弹幕内容"} |


#### 响应

| 参数名  | 类型    | 描述         |
|--------|-------- |--------------|
| code   | int     | 状态码，200为成功，小于0为错误代码，大于0为部分成功代码 |
| msg    | string  | 响应消息，描述请求的处理结果 |


### 调用内部LLM接口

#### 概述

- **请求地址:** `/llm`
- **请求类型:** POST
- **描述:** 通过AI Vtuber内容配置的各个LLM的配置内容，选择指定LLM进行提问并获取回答。

#### 请求参数

| 参数名     | 类型    | 是否必需 | 描述         |
|--------    |--------|----------|--------------|
| type | string | 是       | LLM类型（具体是啥，参考webui源码内部的定义，或者参考配置文件中的key）。例如：chatgpt |
| username | string  | 是  | 用户名，内部设计预留的，随便传一个就行 |
| content | string  | 是   | 提问内容(prompt) |


#### 响应

| 参数名  | 类型    | 描述         |
|--------|-------- |--------------|
| code   | int     | 状态码，200为成功，小于0为错误代码，大于0为部分成功代码 |
| msg    | string  | 响应消息，描述请求的处理结果 |
| data   | object  | 数据内容（json）。例如：{"content":"这就是问题的回答"} |

### 调用内部TTS接口

#### 概述

- **请求地址:** `/tts`
- **请求类型:** POST
- **描述:** 通过AI Vtuber内容配置的各个TTS的配置内容，选择指定TTS进行音频合成。

#### 请求参数

| 参数名     | 类型    | 是否必需 | 描述         |
|--------    |--------|----------|--------------|
| type | string     | 是   | 消息类型（具体是啥，参考webui源码内部的定义，会影响项目内部工作机制，建议使用 reread）。推荐：reread |
| tts_type | string | 是   | TTS类型（具体是啥，参考webui源码内部的定义，或者参考配置文件中的key）。例如：gpt_sovits 或 bert_vits2 |
| data   | object   | 是   | tts配置内容（json）。例如：{"type":"api","ws_ip_port":"ws://localhost:9872/queue/join","api_ip_port":"http://127.0.0.1:9880","ref_audio_path":"F:\\GPT-SoVITS\\raws\\ikaros\\21.wav","prompt_text":"マスター、どうりょくろか、いいえ、なんでもありません","prompt_language":"日文","language":"自动识别","cut":"凑四句一切","gpt_model_path":"F:\\GPT-SoVITS\\GPT_weights\\ikaros-e15.ckpt","sovits_model_path":"F:\\GPT-SoVITS\\SoVITS_weights\\ikaros_e8_s280.pth","webtts":{"api_ip_port":"http://127.0.0.1:8080","spk":"sanyueqi","lang":"zh","speed":"1.0","emotion":"正常"}} |
| username | string | 是   | 用户名，内部设计预留的，随便传一个就行 |
| content | string  | 是   | 提问内容(prompt) |

#### 响应

| 参数名  | 类型    | 描述         |
|--------|-------- |--------------|
| code   | int     | 状态码，200为成功，小于0为错误代码，大于0为部分成功代码 |
| msg    | string  | 响应消息，描述请求的处理结果 |
| data   | object  | 数据内容，含传参外还有一个result键值，里面就有合成情况内容，和最后合成后文件存储路径，配合本地路径映射到URL路径，即可实现跨网段文件下载（json）。例如：{"result":{"code":200,"msg":"合成成功","audio_path":"E:\\GitHub_pro\\AI-Vtuber\\out\\gpt_sovits_4.wav"},其他键值对忽略} |

## :material-more: 应用实例

### PK、连麦玩法如何配置？

参考配置：[https://github.com/Ikaros-521/AI-Vtuber/issues/579](https://github.com/Ikaros-521/AI-Vtuber/issues/579)  


## :material-more: 补充

#### 补充板块提供了对项目接入的第三方技术或应用的详细说明。如果您需要与第三方应用进行对接，您可以查阅此板块的内容，并访问第三方官方网站以了解其使用方法。  

### 平台

#### b站直播监听

方案1 [bilibili-api :octicons-link-16:](//github.com/Nemo2011/bilibili-api)  

需要进行扫描登录或者配置 cookie 等信息，才能稳定监听弹幕。注意！！！请使用小号登录，有封号风险！！！  

方案2 [blivedm :octicons-link-16:](//github.com/xfgryujk/blivedm)  

注意：如果使用方案2，需要手动克隆官方项目仓库的`blivedm`到`site-packages`  

- cookie模式下，不配置cookie，获取不到完整用户名。自行选择配置。
- 开放平台模式下，请前往 开放平台: https://open-live.bilibili.com/ 注册成为开发者，“直播创作者服务中心” 创建项目，获取 项目ID 、 access_key_id 、 access_key_secred 

#### <span id="dy">抖音弹幕获取</span>

`dy.py` 稳定 [dy-barrage-grab :octicons-link-16:](//gitee.com/haodong108/dy-barrage-grab)

请到此仓库的 releases 下载官方软件包，并仔细阅读官方的使用说明，运行后能在cmd看到弹幕消息的话，即为成功。  

`dy_old.py` 不稳定 [douyin-live :octicons-link-16:](//github.com/YunzhiYike/douyin-live)   

#### 快手弹幕获取

##### 快手方案1

`ks.py` 新版本 [kuaishou_websocket :octicons-link-16:](//github.com/Superheroff/kuaishou_websocket)

使用新版本时需要注意，请使用小号登录，然后在每次用完之后，把 `cookie` 文件夹下的 `123.json` 文件删掉！！！用过一次后cookie就异常了，所以需要删了重新登录！！！

另外如果你是自行安装环境，请在安装完依赖后，安装火狐浏览器内核。参考命令： `playwright install firefox`

如果你是整合包，项目路径打开cmd，然后使用 `Miniconda3\python.exe Miniconda3\Scripts\playwright.exe install firefox` 进行安装。

`ks_old.py` 旧版本 [kuaishou-live :octicons-link-16:](//github.com/YunzhiYike/kuaishou-live)  

##### 快手方案2

视频教程：[https://www.bilibili.com/video/BV1HA4m1N7sF](https://www.bilibili.com/video/BV1HA4m1N7sF)  

配合油猴脚本：[https://greasyfork.org/zh-CN/scripts/490966](https://greasyfork.org/zh-CN/scripts/490966)，在浏览器直播间页面监听DOM变动，WS返回数据。  

浏览器安装[油猴插件](https://www.tampermonkey.net/)后，再安装上面的脚本，打开需要监听的直播间后，就会自动监听弹幕，连接WS服务，然后把AI Vtuber运行起来，进行对接。  

#### 微信视频号监听

监听程序（不保证安全性，自行斟酌）：[wxlivespy](https://github.com/fire4nt/wxlivespy/releases)  

设置监听地址为`http://127.0.0.1:8082/wxlive`，开播！开始监听，扫描登录直播的微信号。webui修改平台为`微信视频号`，运行即可。  

如果希望看到运行日志，可以自己下载项目部署运行。  

#### 拼多多方案

视频教程：[https://www.bilibili.com/video/BV1YE421T7Tm/](https://www.bilibili.com/video/BV1YE421T7Tm/)  

配合油猴脚本：[https://greasyfork.org/zh-CN/scripts/490966](https://greasyfork.org/zh-CN/scripts/490966)，在浏览器直播间页面监听DOM变动，WS返回数据。  

浏览器安装[油猴插件](https://www.tampermonkey.net/)后，再安装上面的脚本，打开需要监听的直播间后，就会自动监听弹幕，连接WS服务，然后把AI Vtuber运行起来，进行对接。 

#### 斗鱼直播监听

借鉴 [Live-Barrage :octicons-link-16:](//github.com/XiaoXinYo/Live-Barrage)  

#### YouTube直播监听

依赖库：[pytchat](//github.com/taizan-hokuto/pytchat/tree/master)  

修改平台后，配置直播间号即可，如`https://www.youtube.com/watch?v=P5wlxQgYhMY`的直播间号就是`P5wlxQgYhMY`  

#### twitch直播监听

接口源自官方接口: [irc.chat.twitch.tv](//irc.chat.twitch.tv)  

使用时需要配置token、用户名、http代理等  

其中token获取方式，通过访问[https://twitchapps.com/tmi/](//twitchapps.com/tmi/)，登录twitch账号授权后即可获取返回的token:`oauth:xxxxx`  

！！！注意：如果你的token和你监听的直播间是同一个账号，那会自动过滤你自己发送的弹幕！！！  

#### TikTok

视频教程：[BV1GU421o7Wq](https://www.bilibili.com/video/BV1GU421o7Wq)  

#### 聊天模式 

##### 百度

新用户+实名认证后有半年的免费额度可以使用。  

申请地址：[console.bce.baidu.com/ai/#/ai/speech/overview/index :octicons-link-16:](//console.bce.baidu.com/ai/#/ai/speech/overview/index)

??? note "详细教程"

    ![image](./static/images/luna-ai/253623086-a91e9dcb-c894-4844-885c-89b8f9f78e6e.png)

    ![image](./static/images/luna-ai/253623108-355e4d12-d854-4249-a736-03c2c93017db.png)

    ![image](./static/images/luna-ai/253623124-3028e135-0791-4638-b56f-028b8397f35f.png)

    ![image](./static/images/luna-ai/253623143-7731d5a0-72f5-4a07-bf98-4f6e34f8ef32.png)

    ![image](./static/images/luna-ai/253623159-6c2fca12-5c6b-478e-a1d3-d3dead79f192.png)

##### faster_whisper

安装[pytorch :octicons-link-16:](https://pytorch.org/)，自行适配版本，参考安装命令：`pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121`  

录音完后，识别会自动下载模型，模型默认存放在`models`文件夹，可以自行手动下载补充。  

如果在使用时出现下载过模型但第一次运行仍要连接huggingface的情况，可以指定模型路径为本地model.bin的路径，参考：`./models/models--Systran--faster-whisper-large-v3/snapshots/edaa852ec7e145841d8ffdb056a99866b5f0a478` ，则这个相对路径下有对应的`model.bin`文件，你的临时文件名不一样，自己找一下。  

### LLM

#### ChatGPT

官网 [chat.openai.com/chat :octicons-link-16:](//chat.openai.com/chat)  

openai 后台 [platform.openai.com :octicons-link-16:](//platform.openai.com/)  

新建 API KEY [platform.openai.com/account/api-keys :octicons-link-16:](//platform.openai.com/account/api-keys) 

查看账号额度 [platform.openai.com/account/usage :octicons-link-16:](//platform.openai.com/account/usage)  

官方 API 文档 [platform.openai.com/docs/api-reference :octicons-link-16:](//platform.openai.com/docs/api-reference)  

常见报错：[点击前往issue仓库查找，直接搜索报错内容，一次不要复制太多报错，不然搜不到，复制关键的报错点就行，比如最后一行](https://github.com/Ikaros-521/AI-Vtuber/issues)  

#### Claude

实现参考 [claude-in-slack-api :octicons-link-16:](//github.com/yokonsan/claude-in-slack-api)  

API申请方法（内含各个参数的获取方式） [claude-api :octicons-link-16:](//github.com/bincooo/claude-api)  

slack 官网 [slack.com/intl/zh-cn :octicons-link-16:](//slack.com/intl/zh-cn/)  

添加 claude 到 slack [www.anthropic.com/claude-in-slack :octicons-link-16:](//www.anthropic.com/claude-in-slack)  

!!! note "视频教程"

    [完美替代 chatGPT！保姆级 Claude 注册教程及使用上的优点和缺点 :octicons-link-16:](//www.bilibili.com/video/BV1PP41127mQ)  

    [解决现阶段 slack 新建工作区 Claude 不回复 :octicons-link-16:](//www.bilibili.com/video/BV17k4y1H7aa)  


以下文档转自：[claude-api :octicons-link-16:](//github.com/bincooo/claude-api)  
##### 授权以及获取user-token

网页([登录](https://app.slack.com))后, 进入api配置页面([点我跳转](https://api.slack.com/))。

〉》点击 【Create an app】

​	〉》主页看见Your Apps并弹出窗口【Create an app】  〉》  点击【From scratch】

​	〉》填写app名称以及选择工作空间（例：name: Bot, workspace: chat）	 〉》  点击【Create App】

​	〉》点击左侧边栏上的【OAuth & Permissions】	 〉》  下拉至【Scopes】卡片，在 【User Token Scopes】 项下添加权限，如下：

​							channels:history,  channels:read,  channels:write,  groups:history,  groups:read,  groups:write, 

​							chat:write,  im:history,  im:write,  mpim:history,  mpim:write

​	〉》回到顶部【OAuth Tokens for Your Workspace】栏，点击【Install to Workspace】，然后确认授权即可


至此，获得拥有一定权限的user-token

<img src="https://github.com/bincooo/claude-api/blob/main/static/%E6%88%AA%E5%B1%8F2023-04-18%2009.10.56.png?raw=true" alt="截屏2023-04-18 09.10.56" style="zoom:50%;" />



<img src="https://github.com/bincooo/claude-api/blob/main/static/%E6%88%AA%E5%B1%8F2023-04-18%2009.14.41.png?raw=true" alt="截屏2023-04-18 09.14.41" style="zoom:50%;" />



##### 获取 claude appid

<img src="https://github.com/bincooo/claude-api/blob/main/static/%E6%88%AA%E5%B1%8F2023-04-18%2008.49.20.png?raw=true" alt="截屏2023-04-18 08.49.20" style="zoom:50%;" />

#### Claude2

[Claude2-PyAPI :octicons-link-16:](//github.com/wwwzhouhui/Claude2-PyAPI)

claude2 官网 [claude.ai :octicons-link-16:](//claude.ai)

!!! note "Cookie 获取方式"
    
    F12 抓包 XHR ，然后请求头获取 cookie`

#### ChatGLM

官方仓库：[ChatGLM-6B](//github.com/THUDM/ChatGLM-6B)

整合包：[【ChatGLM】本地版ChatGPT？6G显存可用！ChatGLM-6B 清华开源模型一键包发布 可更新](//www.bilibili.com/video/BV1E24y1u7Go)  

视频教程：[【AI主播-功能篇】ChatGLM如何接入？上下文记忆~ 不需魔法，本地跑，省钱了喵~](https://www.bilibili.com/video/BV1NN411a7zG)  

运行 `api.py` ，然后配置相关信息接入本项目。

!!! note "参考"

    ```python
    if __name__ == '__main__':
        tokenizer = AutoTokenizer.from_pretrained("THUDM\chatglm-6b-int4", trust_remote_code=True)
        model = AutoModel.from_pretrained("THUDM\chatglm-6b-int4", trust_remote_code=True).half().cuda()
        model.eval()
        uvicorn.run(app, host='0.0.0.0', port=8000, workers=1)
    ```

##### ChatGLM3

官方仓库：[ChatGLM3](//github.com/THUDM/ChatGLM3)  

整合包：[https://pan.quark.cn/s/c2ded75100ac](https://pan.quark.cn/s/c2ded75100ac)  

视频教程：[【AI主播-功能篇】接入ChatGLM3，含整合包，看看有没有提升（](https://www.bilibili.com/video/BV1M94y137h4)  

运行 `1.运行api.bat` ，然后配置相关信息接入本项目（聊天类型：`ChatGPT/闻达`，API地址：`http://localhost:8000/v1`，模型：`chatglm3-6b`）。  

!!! openai_api.py "参考"

    ```python
    if __name__ == "__main__":
        tokenizer = AutoTokenizer.from_pretrained("THUDM\\chatglm3-6b-int4", trust_remote_code=True)
        model = AutoModel.from_pretrained("THUDM\\chatglm3-6b-int4", trust_remote_code=True).cuda()
        # 多显卡支持，使用下面两行代替上面一行，将num_gpus改为你实际的显卡数量
        # from utils import load_model_on_gpus
        # model = load_model_on_gpus("THUDM\\chatglm3-6b-int4", num_gpus=2)
    ```

#### 智谱AI

官方：[open.bigmodel.cn](//open.bigmodel.cn/)  

api key申请地址：[open.bigmodel.cn/usercenter/apikeys](//open.bigmodel.cn/usercenter/apikeys)  

注意，需要在"设置"->"账号设置"中完成实名认证后，才能使用API。新账号默认赠送了18元的免费额度。  

#### langchain-ChatGLM

官方仓库：[langchain-ChatGLM](//github.com/chatchat-space/langchain-ChatGLM)  

个人提供的整合包：[pan.quark.cn/s/8d8904fd4b30](//pan.quark.cn/s/8d8904fd4b30)  

chatglm-6b-int4模型下载(其实这个官方就行，有会员的话网盘快点)：[pan.quark.cn/s/a483e0c3e5fa](//pan.quark.cn/s/a483e0c3e5fa)  

官方模型仓库：[huggingface.co/THUDM](//huggingface.co/THUDM)  

配置相关信息，编辑 `configs` 文件夹下的 `model_config.py` ，模型路径需要是绝对路径，win的用户路径参考：`E:\\langchain-ChatGLM\\THUDM\\chatglm-6b-int4`  

修改部分参考：  

```python
embedding_model_dict = {
    "ernie-tiny": "nghuyong/ernie-3.0-nano-zh",
    "ernie-base": "nghuyong/ernie-3.0-base-zh",
    "text2vec-base": "shibing624/text2vec-base-chinese",
    # 下一行是改的地方
    "text2vec": "E:\\langchain-ChatGLM\\GanymedeNil\\text2vec-large-chinese",
    "text2vec-base-multilingual": "shibing624/text2vec-base-multilingual",
    "text2vec-base-chinese-sentence": "shibing624/text2vec-base-chinese-sentence",
    "text2vec-base-chinese-paraphrase": "shibing624/text2vec-base-chinese-paraphrase",
    "m3e-small": "moka-ai/m3e-small",
    "m3e-base": "moka-ai/m3e-base",
}


llm_model_dict = {
    "chatglm-6b-int4-qe": {
        "name": "chatglm-6b-int4-qe",
        "pretrained_model_name": "THUDM/chatglm-6b-int4-qe",
        "local_model_path": None,
        "provides": "ChatGLMLLMChain"
    },
    "chatglm-6b-int4": {
        "name": "chatglm-6b-int4",
        "pretrained_model_name": "THUDM/chatglm-6b-int4",
        # 下一行是改的地方
        "local_model_path": "E:\\langchain-ChatGLM\\THUDM\\chatglm-6b-int4",
        "provides": "ChatGLMLLMChain"
    },


# LLM 名称 改成你要用的模型name，没有的话会自动下载
LLM_MODEL = "chatglm-6b-int4"
```

运行 `api.py` ，然后接入本项目。  

#### chat_with_file

参考：[LangChainSummarize](//github.com/Ikaros-521/LangChainSummarize)

构建本地向量数据库时，如果本地电脑的配置太低，可以使用 [faiss_text2vec.ipynb](//drive.google.com/file/d/1rbt2Yv7_pC1cmuODwmR2-1_cxFBFOfn8/view?usp=sharing) 云端解析向量数据库，拷贝回本地后再使用即可

视频教程：[https://www.bilibili.com/video/BV1tM4y1v7i5](https://www.bilibili.com/video/BV1tM4y1v7i5)

- author: [HildaM/text2vec_colab](//github.com/HildaM/text2vec_colab)

#### text-generation-webui

官方仓库：[text-generation-webui](//github.com/oobabooga/text-generation-webui)

懒人包：b站：coyude [AI对话 懒人包v1发布 图形化启动界面(oobabooga/text-generation-webui)可用chatglm/rwkv/vicuna](//www.bilibili.com/video/BV1tP411d7wo)

API调用demo：[api-examples](//github.com/oobabooga/text-generation-webui/tree/main/api-examples)

视频教程：[https://www.bilibili.com/video/BV1U14y1d7rz](https://www.bilibili.com/video/BV1U14y1d7rz)

#### 讯飞星火

- web&API
    官网：[xinghuo.xfyun.cn](//xinghuo.xfyun.cn/)

    api库（HildaM开发）：[sparkdesk-api](//github.com/HildaM/sparkdesk-api)

    web配置获取方法：[sparkdesk-api/tree/main/docs](//github.com/HildaM/sparkdesk-api/tree/main/docs)

    api申请：提交工单申请，工单提交页 [console.xfyun.cn/services/cbm](//console.xfyun.cn/services/cbm)

    视频教程：[https://www.bilibili.com/video/BV1au4y127wW](https://www.bilibili.com/video/BV1au4y127wW)

- 应用API
    助手API：前往[https://xinghuo.xfyun.cn/botcenter/createbot](https://xinghuo.xfyun.cn/botcenter/createbot) 创建助手, 获取“助手ID”，然后协同讯飞星火大模型的其他密钥配置使用即可。  

    视频教程：[https://www.bilibili.com/video/BV1Zq421A73F](https://www.bilibili.com/video/BV1Zq421A73F)

#### 闻达

官方仓库：[github.com/wenda-LLM/wenda](//github.com/wenda-LLM/wenda)

整合包下载：[pan.quark.cn/s/c4cb08de666e](//pan.quark.cn/s/c4cb08de666e) 提取码：4b4R

视频教程：[https://www.bilibili.com/video/BV1ru4y1B7js](https://www.bilibili.com/video/BV1ru4y1B7js)

接入说明：

启动 `RWKV-Runner` ，配置配配好，模型搞搞好，然后启动。  

如果遇到midi2audio等库缺失的报错，你可以选中整合包的python环境下的python.exe，进行库补装，参考命令 `python.exe -m pip midi2audio mido lm_dataformat GPUtil sse_starlette
`  

![image](./static/images/luna-ai/258466304-2c3167ae-13ad-4f68-911b-d4262210e81d.png)

![闻达-接入说明](./static/images/luna-ai/258465928-228da499-9de6-45a3-8bb3-5cc684569c00.png)

#### ChatterBot

官方仓库：[https://github.com/gunthercox/ChatterBot](https://github.com/gunthercox/ChatterBot)  

视频教程：[https://www.bilibili.com/video/BV1fh411L72s](https://www.bilibili.com/video/BV1fh411L72s)  

ChatterBot 是一个开源的 Python 聊天机器人框架，使用机器学习算法（尤其是自然语言处理、文本语义分析等）来实现基于规则和语境的自动聊天系统。它可以让开发者通过简单的配置和训练，构建出各种类型的聊天机器人，包括问答机器人、任务型机器人、闲聊机器人等。

ChatterBot 的核心思想是：基于历史对话数据，使用机器学习和自然语言处理技术来分析和预测用户输入，然后生成响应。基于这种方法，聊天机器人的反应会更加智能、灵活、接近人类对话的方式。此外，ChatterBot 支持多种存储方式，如 JSON、SQLAlchemy、MongoDB 等，以及多种接口调用方式，如 RESTful API、WebSocket 等，方便开发者在不同场景中进行集成。

总的来说，ChatterBot 是一个非常强大、灵活、易用的聊天机器人框架，帮助开发者快速搭建出个性化、定制化的聊天机器人，从而提升用户体验和服务质量。  

#### Bard

官方：[bard.google.com](//bard.google.com)

token获取方式：  

访问 `bard.google.com`，登录账号  

键盘F12 打开开发者工具  

应用程序 → Cookie → 复制 Cookie 中 __Secure-1PSID 对应的值。  

ps：cookie有效期较短  

#### 文心一言

官网：[yiyan.baidu.com](//yiyan.baidu.com)  

视频教程：[https://www.bilibili.com/video/BV1kw411v7z6](https://www.bilibili.com/video/BV1kw411v7z6)  

- api

    百度智能云千帆大模型平台：[https://cloud.baidu.com/product/wenxinworkshop](https://cloud.baidu.com/product/wenxinworkshop)  

    API文档：[https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11)  

    [在线服务](https://console.bce.baidu.com/qianfan/ais/console/onlineService)，购买`ERNIE-Bot大模型公有云在线调用服务`，[应用接入](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) 创建应用，获取`API Key`和`Secret Key`，配置即可。

- web

    服务端：[yiyan-api](//github.com/zhuweiyou/yiyan-api)  

    下载yiyan-api源码，根据官方教程部署搭建运行即可。简述过程就是安装Node.js >= 18，然后再源码项目文件夹内运行`npm install`，最后运行`npm start`即可。  

    cookie 获取方式：

    访问 `yiyan.baidu.com`，登录账号  

    键盘F12 打开开发者工具  

    找到`源代码`或者`Sources`页，右键`debugger`左侧行号, 选择 `never pause here` 或者叫做 `永不在此处暂停`, 然后再刷新页面  

    此时就可以跳过`debugger`和重定向，然后找到`网络`或者`Network`。  

    再随便发送一个提问，随便找个XHR请求中，查看请求头内的`cookie`对应的一长串的值，复制粘贴回GUI中保存即可。  

#### 通义星尘

官网：[xingchen.aliyun.com](https://xingchen.aliyun.com/)  

视频教程：[https://www.bilibili.com/video/BV1iu4y1379B](https://www.bilibili.com/video/BV1iu4y1379B)  

进入官网，注册账号，登录，打开`接口管理`页面，点击`API-KEY管理`，`创建密钥`，复制密钥，配置对应配置项。  

角色ID如何获取？ 首页点击`创建角色`，自己创建去！创建完成后，进入角色聊天页，角色头像边上有个`信息`，点进去可以看见`ID`，复制配置即可。

当然，还没完，现在官方还在内测，所以你创建了密钥还不能用，需要联系官方开通调用权限。联系方式见 [使用文档-服务支持](https://xingchen.aliyun.com/xingchen/document/service_support)  

#### 千帆大模型

##### 第三方库

- 千帆大模型

    视频教程：[https://www.bilibili.com/video/BV1EC4y1Q7ob](https://www.bilibili.com/video/BV1EC4y1Q7ob)  

    接入库，我对原库做了修改：[WenxinWorkshop-Python-SDK](https://github.com/Ikaros-521/WenxinWorkshop-Python-SDK)  

    百度智能云千帆大模型平台：[https://cloud.baidu.com/product/wenxinworkshop](https://cloud.baidu.com/product/wenxinworkshop)  

    官方API文档：[https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11](https://cloud.baidu.com/doc/WENXINWORKSHOP/s/jlil56u11)  

    [在线服务](https://console.bce.baidu.com/qianfan/ais/console/onlineService)，购买`ERNIE-Bot大模型公有云在线调用服务`等服务，[应用接入](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) 创建应用，获取`API Key`和`Secret Key`，配置即可。  

- AppBuilder

    视频教程：[旧版API教程](https://www.bilibili.com/video/BV1b1421D7fz)  

    百度智能云 AppBuilder 应用中心：[https://console.bce.baidu.com/ai_apaas/appCenter](https://console.bce.baidu.com/ai_apaas/appCenter)，创建一个你的专属应用 —— 知识问答应用（RAG框架），创建好后，获取应用ID：[https://console.bce.baidu.com/ai_apaas/personalSpace](https://console.bce.baidu.com/ai_apaas/personalSpace)。获取密钥token：[https://console.bce.baidu.com/ai_apaas/secretKey](https://console.bce.baidu.com/ai_apaas/secretKey)  

    图文文档：[https://github.com/Ikaros-521/AI-Vtuber/pull/830](https://github.com/Ikaros-521/AI-Vtuber/pull/830)  

##### 官方库（有版本冲突，暂不启用）

接入库：[bce-qianfan-sdk](https://github.com/baidubce/bce-qianfan-sdk)  

使用文档：[bce-qianfan-sdk#readme](https://github.com/baidubce/bce-qianfan-sdk#readme)  

在使用千帆 SDK 之前，用户需要 [百度智能云控制台 - 安全认证](https://console.bce.baidu.com/iam/#/iam/accesslist) 页面获取 Access Key 与 Secret Key，并在 [千帆控制台](https://console.bce.baidu.com/qianfan/ais/console/applicationConsole/application) 中创建应用，选择需要启用的服务，具体流程参见平台 [说明文档](https://cloud.baidu.com/doc/Reference/s/9jwvz2egb)。在获得了 Access Key 与 Secret Key 后，配置好即可开始使用。  

#### Gemini

官方平台：[makersuite.google.com/app](https://makersuite.google.com/app)  

前往 [makersuite.google.com/app/apikey](https://makersuite.google.com/app/apikey) 创建一个API KEY，配置到项目中即可使用啦~（记得开魔法配置代理！）  

视频教程：[https://www.bilibili.com/video/BV1op4y1f7gr](https://www.bilibili.com/video/BV1op4y1f7gr)  

#### Kimi Chat

视频教程：[https://www.bilibili.com/video/BV1Vm411S7zL](https://www.bilibili.com/video/BV1Vm411S7zL)  

Kimi官网：[https://kimi.moonshot.cn/](https://kimi.moonshot.cn/)  

API申请：[https://platform.moonshot.cn/console/api-keys](https://platform.moonshot.cn/console/api-keys)  

使用：  
1. 大语言模型选择：ChatGPT
2. 配置
    API地址：https://api.moonshot.cn/v1  
    API密钥：上面申请的密钥  
    模型：moonshot-v1-8k  

#### QAnything

视频教程：[https://www.bilibili.com/video/BV1p2421F7QE](https://www.bilibili.com/video/BV1p2421F7QE)  

官方仓库：[https://github.com/netease-youdao/QAnything](https://github.com/netease-youdao/QAnything)  

##### 在线

在线官网：[https://ai.youdao.com/saas/qanything/#/home](https://ai.youdao.com/saas/qanything/#/home)  

登录官方平台，完成实名认证获得免费额度，创建应用，获取应用ID和密钥：[https://ai.youdao.com/console/#/app-overview](https://ai.youdao.com/console/#/app-overview)  

##### 本地

部署：Windows部署配合CUDA驱动、WSL2、docker，完成。主要坑点在docker加载cuda相关库上。根据官方仓库的run.sh脚本运行即可，具体报错参考issue。  
  
参考教程：  
[【2023最新版】Win11: WSL（Ubuntu22.04）使用docker远程容器教程（Windows的Docker Desktop下载安装、迁移到非系统盘、配置国内镜像源、设置 WSL2）](https://blog.csdn.net/m0_63834988/article/details/131816239)  
[Windows安装网易开源QAnything打造智能客服系统](https://www.bilibili.com/read/cv31412472/)  

#### 通义千问

官网：[qianwen.aliyun.com](//qianwen.aliyun.com/)   

##### API类型

视频教程：[https://www.bilibili.com/video/BV1dx4y1S7Ei](https://www.bilibili.com/video/BV1dx4y1S7Ei)  

API文档：[https://help.aliyun.com/zh/dashscope/developer-reference/quick-start](https://help.aliyun.com/zh/dashscope/developer-reference/quick-start)  
申请API KEY 文档（文档教程详细，我就不再赘述了）：[https://help.aliyun.com/zh/dashscope/developer-reference/activate-dashscope-and-create-an-api-key](https://help.aliyun.com/zh/dashscope/developer-reference/activate-dashscope-and-create-an-api-key)  


##### web类型

视频教程：[https://www.bilibili.com/video/BV1nc411Z7Db](https://www.bilibili.com/video/BV1nc411Z7Db)  

依赖库：[revTongYi](https://github.com/leeeduke/revTongYi)  

cookie 获取方式：  
1. 安装 [Chrome](//chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm)、[Edge](//microsoftedge.microsoft.com/addons/detail/cookie-editor-plus/nbmajjcfigmlcnikhnfhhicidleefhpp) 或 [Firefox](//addons.mozilla.org/en-US/firefox/addon/cookie-editor/) 上的`Cookies Editor`插件
2. 前往 [https://tongyi.aliyun.com/chat](//tongyi.aliyun.com/chat) 并登录
3. 打开此插件，点击 Export -> Export as JSON，将复制的Cookies内容保存到文件`cookie`文件夹下的`tongyi.json`  

ps:cookie有效期估计在6小时左右。  

#### FastGPT

##### 在线

官方：[https://doc.fastgpt.in/](https://doc.fastgpt.in/)  

![image](./static/images/luna-ai/fastgpt-1.png)  

![image](./static/images/luna-ai/fastgpt-2.png)  

#### koboldcpp

视频教程：[https://www.bilibili.com/video/BV1Ci421o7kt](https://www.bilibili.com/video/BV1Ci421o7kt)  

官方仓库：[https://github.com/LostRuins/koboldcpp](https://github.com/LostRuins/koboldcpp)  

exe程序下载(也可以去整合包网盘中下载)：[https://github.com/LostRuins/koboldcpp/releases](https://github.com/LostRuins/koboldcpp/releases)

#### AnythingLLM

视频教程：[https://www.bilibili.com/video/BV13x421k7Yf](https://www.bilibili.com/video/BV13x421k7Yf)  

官网：[https://useanything.com/](https://useanything.com/)  

下载安装，然后根据官方提示选择对接的LLM、向量数据库等，创建工作区（有知识库检索需求的请在工作区添加文档本导入到需要的工作区内）。  

左下角设置图标进去，到API KEYS创建密钥，复制密钥，配置到项目中，保存配置，读取工作区列表，然后选择你要使用的工作区，保存运行使用即可。  

#### GPT4Free

官方仓库：[https://github.com/xtekky/gpt4free](https://github.com/xtekky/gpt4free)  

免费白嫖GPT使用，不过得找个好的供应商，不然不稳定。有哪些代理商可以去官方仓库看文档。  

#### LLM-TPU

官方仓库：[https://github.com/sophgo/LLM-TPU](https://github.com/sophgo/LLM-TPU)  

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


### 变声

#### DDSP-SVC

官方仓库：[DDSP-SVC](//github.com/yxlllc/DDSP-SVC)  

个人提供的已训练好的模型：[点我跳转](//github.com/Ikaros-521/DDSP-SVC/releases)  

羽毛佬视频教程：[【AI翻唱/变声/整合包】有张N卡就能跑！媲美So-VITS却不吃配置，全新的DDSP-SVC 3.0训练/推理教程](//www.bilibili.com/video/BV1rs4y1Q7BQ)  

视频教程：[【AI主播-功能篇】新增 DDSP-SVC 接入。变声选项再加一，多种选择总有一个是适合你的（](https://www.bilibili.com/video/BV1s8411m7rX/)  

修改 `flask_api.py` 最后几行中的模型路径，其他配置自行调整，另外需要注意！ `enable_spk_id_cover` 改为 `False` ，即可接入。  

```python
# config和模型得同一目录。 这是我自己训练的DDSP模型，新鲜出炉
checkpoint_path = "exp/combsub-test/model_68000.pt"
# 是否使用预训练的基于声码器的增强器增强输出，但对硬件要求更高。
use_vocoder_based_enhancer = True
# 结合增强器使用，0为正常音域范围（最高G5)内的高音频质量，大于0则可以防止超高音破音
enhancer_adaptive_key = 0
# f0提取器，有parselmouth, dio, harvest, crepe
select_pitch_extractor = 'crepe'
# f0范围限制(Hz)
limit_f0_min = 50
limit_f0_max = 1100
# 音量响应阈值(dB)
threhold = -60
# 默认说话人。
spk_id = 1
# 是否优先使用默认说话人覆盖vst传入的参数，改为False，不要覆盖！！！
enable_spk_id_cover = False
```

#### so-vits-svc

官方仓库：[so-vits-svc](//github.com/svc-develop-team/so-vits-svc)  

个人提供的已训练好的模型：[点我跳转](//github.com/Ikaros-521/so-vits-svc/releases)  

视频教程：[【AI歌姬】so-vits-svc 简单使用讲解 + 伊卡洛斯 模型开源](//www.bilibili.com/video/BV1k24y1F7Us) ， [【AI主播-功能篇】如何接入so-vits-svc？用什么版本？4.1版为什么会报错？运行哪个程序？在哪下载？](https://www.bilibili.com/video/BV1dh4y1j7hM/)  

修改 `flask_api_full_song.py` 最后几行中的模型路径，运行，配置相关信息即可接入。  

```python
if __name__ == '__main__':
    model_name = "logs/44k/ikaros_G_54600.pth" # 你的模型地址
    config_name = "configs/ikaros_v1.json"  # 你的config地址
    svc_model = infer_tool.Svc(model_name, config_name)
    app.run(port=1145, host="0.0.0.0", debug=False, threaded=False)
```  

注意！！！如果你是 `4.1` 版本的整合包，还需要修改 `flask_api_full_song.py` 的38行左右：  
改  

```python
out_audio, out_sr = svc_model.infer(spk, tran, raw_path)
```

为

```python
out_audio, out_sr, n_frames = svc_model.infer(spk, tran, raw_path)
```

### 虚拟身体

#### Live2D

源自：[CyberWaifu](//github.com/jieran233/CyberWaifu)

官方免费模型下载：[releases/tag/live2d](//github.com/Ikaros-521/AI-Vtuber/releases/tag/live2d)  

官网：[www.live2d.com/zh-CHS](//www.live2d.com/zh-CHS)  

第三方软件 `Vtube Studio` ，配置教程：[【AI主播】虚拟人部分方案#1 基于Vtube Studio的口型驱动](https://www.bilibili.com/video/BV1vs4y1k71M)  

配合VB虚拟声卡时，如果想要让扬声器也可以听到输出的音频，可以通过 侦听 来实现，配置方法如下：

![image](./static/images/luna-ai/255964173-b2c0d632-c6ad-4044-892e-e809dfea8f21.png)

#### NVIDIA Omniverse Audio2Face

NVIDIA Omniverse下载：[www.nvidia.com/en-us/omniverse/download/](//www.nvidia.com/en-us/omniverse/download/)  

Character Creator 4下载：[www.reallusion.com/character-creator/download.html](//www.reallusion.com/character-creator/download.html)  

Epic下载：[store.epicgames.com/zh-CN/](//store.epicgames.com/zh-CN/)  

参考教程：  

[【AI主播】Audio2Face + UE5，轻松实现 数字人 口型同步，主打一个简单，就是配置要求高了点](//www.bilibili.com/video/BV1k94y147oG)  

[【Omniverse教程】【Audio2Face】1-仅需一个音频来源即可生成表情丰富的面部动画，也支持实时录音](//www.bilibili.com/video/BV1TS4y187P9)  

[玩转Omniverse | Reallusion Character Creator：生成角色](//www.bilibili.com/video/BV1wB4y1W7g4)  

[玩转Omniverse | Reallusion Character Creator：将角色 USD 文件导入NVIDIA Omniverse](//www.bilibili.com/video/BV1uG411x7we)  

[零代码让UE Metahuman说话的方法（使用omniverse audio2face串流至UE）](//www.bilibili.com/video/BV1FV411375V)   

[P6-UE5角色资产导入与说明!](//www.bilibili.com/video/BV1A24y1S77m)  

#### xuniren

xuniren官方仓库：[https://github.com/waityousea/xuniren](//github.com/waityousea/xuniren)  

项目对接推荐使用我的改版：[https://github.com/Ikaros-521/xuniren](//github.com/Ikaros-521/xuniren)  

半整合包（需要自行补充环境）：[https://pan.quark.cn/s/03db11314ca1](//pan.quark.cn/s/03db11314ca1), 需要注意的是这个项目环境十分难搭建，而且很多都需要自行编译，所以我编译的版本不一定适用于你的系统，那么你就需要自己重新编译安装了，那就是一件非常痛苦的事情，注意我的说明自行闭坑吧。  

使用：整合包用户启动我提供的`http_api运行.bat`脚本，普通用户自行启动`http_api.py`即可，看到服务正常监听即可。那么此时我们的AI Vtuber也需要配置对应的`虚拟身体`配置，然后运行即可。  

视频教程：[BV1uB4y1d7o6](//www.bilibili.com/video/BV1uB4y1d7o6/)  

#### EasyAIVtuber

EasyAIVtuber官方仓库：[https://github.com/Ksuriuri/EasyAIVtuber](https://github.com/Ksuriuri/EasyAIVtuber)  

参考官方文档完成部署后启动，虚拟身体选择“EasyAIVtuber”，保存运行即可对接使用。  

#### 数字人视频播放器

视频教程：[【AI主播-虚拟身体篇】对接 Easy-Wav2Lip（数字人视频播放器） 实现真人数字人驱动](https://www.bilibili.com/video/BV1iW421P7si)，[https://www.bilibili.com/video/BV1pi421R7N5](https://www.bilibili.com/video/BV1pi421R7N5)  

数字人视频播放器 官方仓库：[https://github.com/Ikaros-521/digital_human_video_player](https://github.com/Ikaros-521/digital_human_video_player)  

参考官方文档完成部署后启动，虚拟身体选择“数字人视频播放器”，保存运行即可对接使用。  

#### metahuman-stream

metahuman-stream 官方仓库：[https://github.com/lipku/metahuman-stream](https://github.com/lipku/metahuman-stream)  
官方部署教程：[https://www.bilibili.com/video/BV1kr421G7ho](https://www.bilibili.com/video/BV1kr421G7ho)  

使用概览：[https://github.com/Ikaros-521/AI-Vtuber/pull/881](https://github.com/Ikaros-521/AI-Vtuber/pull/881)  

视频教程：[https://www.bilibili.com/video/BV1Jy411q7sy](https://www.bilibili.com/video/BV1Jy411q7sy)  

### 图像识别

#### gemini

【AI主播-图像识别篇】新增 摄像头截图功能，可以进行现实互动，未来会继续互动方式：[https://www.bilibili.com/video/BV132421P7WT](https://www.bilibili.com/video/BV132421P7WT)  

【AI主播-图像识别篇】对接 Gemini-Pro-Vision，实时画面识别讲解，可用于游戏讲解等应用场景：[https://www.bilibili.com/video/BV1F6421F767](https://www.bilibili.com/video/BV1F6421F767)  

### 翻译

#### 百度翻译

官方文档：[https://api.fanyi.baidu.com/doc/21](https://api.fanyi.baidu.com/doc/21)  

根据文档提示，注册开发者并完整认证后，申请“通用文本翻译”服务，然后在[http://api.fanyi.baidu.com/manage/developer](http://api.fanyi.baidu.com/manage/developer)，获取`APP ID`和`密钥`，配置上即可使用。

### 其他

#### Stable Diffusion

官方仓库：[stable-diffusion-webui](//github.com/AUTOMATIC1111/stable-diffusion-webui)  

整合包：[【AI绘画】Stable Diffusion整合包v4.2发布！全新加速 解压即用 防爆显存 三分钟入门AI绘画 ☆可更新 ☆训练 ☆汉化](//www.bilibili.com/video/BV1iM4y1y7oA)

启动API模式，填写相关配置即可接入。  

视频教程：[BV1tV411u79T](//www.bilibili.com/video/BV1tV411u79T/)  

#### web字幕打印机

项目地址：[captions_printer](//github.com/Ikaros-521/captions_printer)  

具体使用参考项目文档即可。  

视频教程：[BV13h4y1e7z8](//www.bilibili.com/video/BV13h4y1e7z8/)  

#### 按键映射

pyautogui官方文档：[传送门，官方对按键名的定义](//pyautogui.readthedocs.io/en/latest/keyboard.html#keyboard-keys)  

#### audio player（音频播放器）

项目地址：[audio_player](//github.com/Ikaros-521/audio_player)  

具体使用参考项目文档即可。  


## 🀅开发&项目相关

### 简易流程图

![image](./static/images/luna-ai/simple_flowchart.png)

![image](./static/images/luna-ai/chart.jpg)

??? 详情展开

    ### UI设计

    #### NiceGUI

    webui使用的NiceGUI框架搭建，官方文档：[https://nicegui.io/documentation](//nicegui.io/documentation)  

    #### PyQt5

    打开QT设计师~o( =∩ω∩= )m `pyqt5-tools designer`  

    生成UI代码 `pyuic5 -o UI_main.py ui\main.ui`  

    对UI做改动时，加入新的配置，一般需要修改 init_config 和 save 部分，新配置的读取和写入部分。  

    ### 源码开发

    #### 新增LLM

    1.`utils/gpt_model` 下新建 新llm的py文件，内部封装类，实现通用函数 `get_resp(prompt)` ，传入提问，返回回答。

    2.`utils/gpt_model` 下新增下模型相关的配置内容，照葫芦画瓢 `gpt.py`

    3.根据相关传参，给 `config.json` 添加对应的配置。

    4.`utils`下，修改 `my_handle.py` ， `__init__` 初始化中相关配置读取，加载模型等。

    5.`utils`下，修改 `my_handle.py` ， `comment_handle` 中新增对应LLM选中时，所做的逻辑处理。

    6.打开QT设计师，修改 `ui\main.ui` 。为新的LLM设计位置和相应控件，可以参考其他LLM的设计。

    7.修改 `main.py` ，实现LLM的UI显示部分以及数据读取和配置保存。另外需要注意新增的LLM会影响到其他配置项的内容，以及显隐关系。需要修改的部分如下：

    - init_config()
    - init_ui()
    - oncomboBox_chat_type_IndexChanged()


    ### 打包懒人包

    1、直接在懒人包中安装miniconda  

    2、激活base虚拟环境（使用写好的激活脚本）  

    3、安装依赖  

    `pip install -r requirements_bilibili.txt -i https://pypi.tuna.tsinghua.edu.cn/simple`  

    `pip install -r requirements_dy.txt -i https://pypi.tuna.tsinghua.edu.cn/simple`  

    `pip install -r requirements_ks.txt -i https://pypi.tuna.tsinghua.edu.cn/simple`  

    `pip install -r requirements_douyu.txt -i https://pypi.tuna.tsinghua.edu.cn/simple`  

    4、安装chatterbot（可选）

    `pip install spacy SQLAlchemy==1.3.24 -i https://pypi.tuna.tsinghua.edu.cn/simple`  

    前提是你在当前目录下有clone chatterbot的项目（自行调整路径关系）  

    `python setup.py install`  

    ### MD目录自动生成

    [doctoc](//github.com/thlorenz/doctoc) ,在本地git存储库中生成降价文件的目录。链接通过命令行标志兼容github或其他网站生成的锚。

    #### 安装

    node.js环境  

    进入包含本地git项目的目录，键入: `npm install -g doctoc`  

    #### 使用

    在 `README.md` 中，找个生成目录位置，写入如下代码，确认生成位置：

    ```
    <!-- START doctoc -->
    <!-- END doctoc -->
    ```

    cmd输入命令即可：`doctoc /path/to/file`  

    例如：`doctoc README.md`  

    ### 文档生成

    基于编写 `mkdocs-material`，官方文档：[mkdocs-material](//squidfunk.github.io/mkdocs-material/getting-started/)  
    
    安装 `pip install mkdocs-material`  

    构建静态网站 `mkdocs build`  

    文档本地实时预览 `mkdocs serve`  

    ### 文档生成(简易旧版)

    依赖 [node.js](//nodejs.org) 环境。  

    #### 安装docsify-cli工具

    cmd运行 `npm i docsify-cli -g`  

    #### 初始化项目

    项目根目录cmd运行 `docsify init .`  

    #### 启动服务

    项目根目录cmd运行 `docsify serve .`  

### 测试
- [x] GUI运行配置完后，运行，监听无人直播间半天，时间到后发送命令尝试触发应用（复读机），正常监听并合成音频。
- [x] 监听1秒2弹幕的直播间，复读机配合vits-fast做语音合成，持续工作30分钟，正常监听并合成音频。

## 🖹待办事项

### 短期计划
- [x] chatglm拥有记忆功能
- [x] 抖音关注事件可以触发关注感谢话术
- [x] 本地问答文本库支持动态变量功能
- [x] 兼容bert vits2
- [x] LLM输出后，后置的过滤（双重过滤）
- [x] bark-gui的接入
- [x] 快手平台的重新兼容
- [x] 用户入场、投食感谢（自定义 文案）
- [x] 弹幕跳过机制（时间段内丢弃）
- [x] 点歌后的弹幕触发问题（如：只取最新的几个）—— 使用弹幕丢弃机制
- [x] 弹幕丢失bug修复（很可能是线程sleep造成的）& b站弹幕库版本更新
- [x] 文案页支持动态加载文案
- [x] 支持关闭聊天（LLM等）
- [x] langchain-chatglm的接入
- [x] chat_with_file在匹配不到结果时继续使用LLM进行回答——通过prompt实现
- [ ] 文案字幕显示
- [ ] 礼物答谢combo情况下的重复答谢问题
- [ ] RVC的接入
- [ ] live2d的嘴型、动作匹配
- [ ] 接入更多的2/3D模型软件（Unity、UE5等）
- [ ] 屏蔽词升级。如：可以根据屏蔽词库转拼音的二重屏蔽；接入第三方屏蔽词API等
- [x] 本机语音直接交流模式（本地版本whisper，其他方式）
- [ ] 本地的用户拉黑机制
- [ ] 礼物互动机制（跳舞，唱歌）
- [ ] wav2lip方案尝试（带货方面）
- [ ] 直播中可以由弹幕进行动态换装 
- [ ] TTS合成时，语句切分算法有待优化
- [ ] 文案拒绝打断机制
- [ ] Edge-TTS在合成音频时会出现合成成功但是系统找不到文件的bug
- [ ] 支持礼物或者其他形式的键盘映射
- [x] webui开发
- [x] 闲时任务功能（适用于自言自语）
- [x] 输出音频自定义输出设备


### 长期计划
- [ ] 懒人包优化
- [ ] 接入更多的LLM（new bing等）
- [ ] 接入更多的TTS方案
- [ ] 独立TTS功能
- [ ] 独立文案合成功能
- [ ] 压力测试
- [ ] 其他直播平台的适配（拼多多等）

## 📝更新日志

??? note "更新日志"
    - 2024-6-21
        - ChatTTS gradio新增 0621版的兼容 
        - 针对无桌面情况，将pyautogui移到运行处导入

    - 2024-6-18
        - chattts api调用改get为post请求

    - 2024-6-17
        - 新增 串口页面，为后期串口功能开发开路（暂未开放）

    - 2024-6-16
        - LLM新增 LLM_TPU 的gradio对接 
        - 补充webui的配置提示；
        - 新增串口类（为后期串口控制功能做准备）

    - 2024-6-15
        - 优化metahuman-stream对接部分源码（运行逻辑部分待调整）
        - 过滤板块新增 指定前后缀触发LLM功能，可以限制部分弹幕触发LLM，部分弹幕只进行其他功能的执行

    - 2024-6-14
        - bert_vits2 新增 刘悦-中文特化API 的对接；

    - 2024-6-14
        - 增加mentahuman和musetalk([metahuman-stream](https://github.com/lipku/metahuman-stream))实时交互数字人接入ai-vtuber的能力，可以直播带货，也可以做数字分身
        - 重新整理虚拟身体板块 排序
        
    - 2024-6-12
        - 音频mixer初始化增加异常捕获，针对声卡异常情况下给予提示，以不影响播放逻辑运行

    - 2024-6-7
        - cv2移到函数内导入；
        - 补充遗漏依赖版本；
        - 默认配置删除容易违禁的接口

    - 2024-6-4
        - 删除无用文档
        - 更新脚本默认执行备份脚本
        - 补充遗漏依赖和指定版本号
        - 针对webui运行程序功能不兼容问题进行修复（linux运行请使用root用户）

    - 2024-6-1
        - 修复ChatTTS无法使用的bug
        
    - 2024-5-29
        - 更新睿声tts接口

    - 2024-5-26
        - 违禁词新增到7w行（一定程度上会拖慢处理速度）
        - webui 音频播放 新增 音频信息回传 开关。在用户不需要回传信息的情况下，可以提升响应速度。
        - 新增ChatTTS的对接
        - 优化TTS页 通用合成时，会重载config配置

    - 2024-5-23
        - faster_whisper新增语言设定
        - 修复录音解析失败无法重复录音bug
        - 新增音频信息回调开关（因为这个音频信息回调是提供给闲时任务计时重置用的，但因为通过http实现，所以会有较大延迟，而这个延迟会阻塞音频播放。之后也会考虑把这个回调改成asyn）
        - 音频信息回调函数改为异步请求

    - 2024-5-22
        - 更新千帆新的模型配置(限时白嫖)
        - 删减部分live2d模型

    - 2024-5-20
        - 对webui部分配置项增加了鼠标悬停提示，方便用户理解配置功能。（工作量较大，慢慢推进
        - LLM新增自定义LLM板块，可以自定义API地址、请求类型、请求头、请求体、代理地址、数据解析等。通过此功能，理论上可以接入绝大多数的llm接口，不过没上下文。

    - 2024-5-19
        - 修复变量使用错误问题
        - 删除定时任务的用户名转换函数调用（定时任务没有用户名
        - 定时任务用户名传入 定时任务字符
        - 音频合成部分的用户名转换增加None判断
        - 优化消息遗忘保留的webui设计
        - 过滤 新增 限定时间段内的数据去重功能（针对数据有 弹幕、入场、礼物），时间段内的重复弹幕等会被丢弃
        - 答谢、念弹幕、本地问答，新增周期性触发机制，可以通过此配置缓存一段时间的数据，在周期到后触发n次

    - 2024-5-18
        - 补充本地问答-文本&助播的 [1|2]语法支持
        - 闲时任务的间隔支持到0-0，但是这么使用会丢数据也会日志爆炸
        - 音频播放间隔改为区间随机
        - 闲时任务新增2种触发类型，可以根据待合成消息、待播放音频队列设置限制触发
        - 普通音频播放支持设置 间隔时间重复次数区间，可以实现随机延时间隔的功能

    - 2024-5-17
        - fish-speech v1.1.0的参考音频参数传参错误问题修复
        - 优化github issue模板等
        - 语音聊天的数据 新增talk类型，用于区分语言和弹幕数据（待测）

    - 2024-5-16
        - 对接fish-speech-V1.1.0本地整合包API 
        - 修复fish-speech 在线调用功能
        - fish-speech在线api支持参考音频过期后自动更新功能，以便长期使用
        - 千帆AppBuilder更新新接口的对接

    - 2024-5-15
        - 数字人视频播放器 支持local类型，直接播放本地视频，支持 MuseTalk 对接

    - 2024-5-14
        - 更新gpt-4o模型的选项

    - 2024-5-13
        - 优化报错提示
        - 智谱AI 兼容zhipuai 1.x 2.x库版本
        - 图像识别板块 新增智谱AI glm-4v

    - 2024-5-12
        - 答谢、积分板块 礼物答谢 新增变量gift_num，unit_price，total_price，cur_time
        - 按键映射板块 文案通用也支持礼物答谢相关的变量
        - fish speech支持填入说话人 随机获取参考音频信息
        - 优化webui anythingLLM获取工作区的逻辑，直接获取webui配置进行获取，并优化了提示
        - 优化按键录音逻辑，不支持多次按录音键

    - 2024-5-11
        - webui多行配置 空配置情况下 有迭代出错问题，已修复
        - 修复gpt-sovits 0322的自动识别语言bug；杂项更新

    - 2024-5-10
        - b站监听的数据，针对用户头像数据 可能不存在问题，追加了None判断处理
        - fish speech支持在线web调用
        - 按键映射新增本地音频的映射配置（不过后端没实现）
        - 更新文档至：[Ikaros-521/Luna-Docs](https://github.com/Ikaros-521/Luna-Docs)
        - 按键映射 新增 本地音频的映射，同样可以通过关键词或礼物触发

    - 2024-5-8
        - 优先级补充 入场欢迎 优先级

    - 2024-5-7
        - 新增 弹幕黑名单，过滤指定用户名 的用户弹幕

    - 2024-5-5
        - 优化js直播监听脚本，新增监听1688直播间弹幕，使用同拼多多一致 

    - 2024-4-30
        - 内置的live2d功能移动到main中统一控制，不在需要重启生效

    - 2024-4-29
        - 闲时任务优化，新增待播放音频阈值和计时缩减值，main新增callback接口接收音频播放状态
        - 优化gradio_tts解析能力 
        - 【重要更新】修改voice_tmp_path_queue 由Queue改为List，待稳定性测试，为后期音频播放优先级打下基础
        - 修复部分功能中含随机抽文案功能，在文案为空时会异常的bug
        - 修复webui 多行输入框的字符串切分bug
        
    - 2024-4-28
        - webui中多行配置的输入框，改为仅换行符用作分隔符，删除空格切分
        
    - 2024-4-27
        - 闲时任务 本地音频 支持[1|2]单行随机抽取语法
        - 默认数据 本地问答库 删除过多的问答数据

    - 2024-4-26
        - 优化能自定义的下拉选择框在自定义输入后，重启webui可以追加自定义选项的功能

    - 2024-4-25
        - 优化openai 测试的报错日志

    - 2024-4-19
        - LLM新增gpt4free，具体哪些供应商好用得自行测试
        
    - 2024-4-17
        - 修改openai tts的官方api地址
        
    - 2024-4-16
        - webui 页面配置新增 配置模板
        - 删减违禁词
    
    - 2024-4-15
        - 兼容CyberWon的webtts-v1.4 v2

    - 2024-4-14
        - 支持拼多多 弹幕监听，实现逻辑同快手2一样，采用油猴前端监听
        - webui 新增 本地路径指定URL路径访问 功能，即添加映射后，可以通过http下载合成的音频

    - 2024-4-13 
        - 消息队列优先级数据类型不对导致的bug修复 
        - 修复队列判空函数的判断错误bug 
        - 优化faster_whisper模型加载逻辑，大幅提升处理速度 
        
    - 2024-4-12
        - 【大改】新增待合成音频消息队列结构大改，queue改list，支持消息优先级自定义&消息最大保留数，待稳定性测试
        - 闲时任务新增刷新计时类型自选
        - 聊天页 直接复读-插队首 全播放器适配 并 修复类型未携带的bug
        - 修改默认消息队列保留数为50

    - 2024-4-10
        - gpt-sovits新增gradio0322版本接口对接，但是！gradio版本需要更新，会库冲突！约等于没法使用
        
    - 2024-4-9
        - 答谢板块 修复 文案清空时 获取文案失败的bug，空时直接跳过功能
        - 更新启动脚本

    - 2024-4-7
        - webui API地址输入框新增url校验
        - common新增部分校验函数，用于未来的校验功能实现
        - 删减部分违禁词

    - 2024-4-6
        - gpt-sovits新增对刘悦佬0322整合包版本的兼容
        - 本地问答库 文本模式补充json文件数据加载异常报错

    - 2024-3-30
        - 部分函数区分操作系统执行
        - 新增部分测试程序

    - 2024-3-30
        - 切换openai测试功能为openai库（之前死活不行，今天一试噶噶顺，醉了
    
    - 2024-3-29
        - webui新增API，TTS合成、LLM推理。拆出独立的API接口，那么用户即可通过本项目做为中转站实现多项目接口统一管理，集成到自己的项目中使用 

    - 2024-3-28
        - 通义千问API调用时，预设不能为空，空时默认一个通用预设
        
    - 2024-3-27
        - 修复 联动程序无法禁用的bug 
        - 新增 油猴脚本，直播弹幕监听 转发至本地WS服务端，可以去greasyfork安装使用
        - 新增 快手2 方案，配合[油猴脚本](https://greasyfork.org/zh-CN/scripts/490966)使用，暂时仅支持弹幕信息 
        - pygame音频加载播放增加异常捕获，给予用户一定报错问题的原因猜测 

    - 2024-3-26
        - 助播 触发类型转换为中文，追加了几个类型，更方便用户理解
        - 新增CSS主题，蓝天白云
        - 新增 联动程序板块，支持在运行webui的时候协同运行其他程序，省得点来点去，但需要注意，别配错了，另外一起启动的情况下，日志会混在一起，别大惊小怪
        - 违禁词删减部分内容

    - 2024-3-25
        - 对接 AnythingLLM
        - vits新增gpt-sovits的兼容（vits-simple-api）
        - tts vits板块新增检索说话人按钮，点击后会调用api的获取说话人接口来更新说话人ID下拉框，不同类型下更新对应的数据

    - 2024-3-24
        - 定时任务 修改定时时间为最小最大时间段内随机，并且新增了按钮来增删任务组
        - 定时任务、闲时任务、动态文案，支持新语法[1|2|3]，括号中随机一个结果做拼接
        - 闲时任务加了time动态变量
        - 闲时任务 时间改成最大最小值内随机，新增了文案模式，纯进行闲时的文案内容复读。闲时任务 文案模式 相较于 文案页的文案，没有打断弹幕的功能（想要打断弹幕可以配合audio player v2使用）这个功能可以在没有弹幕的情况下，播放一些你希望说的一些文本内容，然后会通过tts合成，目前只有一个输入框，要么顺序，要么整体随机，功能还比较简单，请构思好逻辑后再配置使用。

    - 2024-3-22
        - 修复tts_ai_lab_top，增加新的选项 语言 
        - 图像识别 新增摄像头截图功能，核心功能类似窗口截图，配合CV2实现摄像头识别和截图
        - 补充遗漏的 闲时任务、图像识别的遗忘配置
        - 修复自定义命令默认配置API过期问题

    - 2024-3-21
        - 字幕写入文件的日志不显示
        - 音频处理函数会对文本内容的\n进行去除 
        
    - 2024-3-20
        - 补充webui聊天记录回调内容，优化代码实现
        - 复读处理新增type传参，动态文案数据附带type（配合最新版[audio_player_v2](https://github.com/Ikaros-521/audio_player)，可以自定义音频数据优先级排队！）
        - 音频随机变速合并入 音频播放板块
        
    - 2024-3-19 
        - webui chatgpt的llm模型下拉框支持搜索、自定义添加模型名（配合ollama这种，方便自定义模型名）
        - 录音按键支持删除和输入，方便找到对应按键
        - 修复gpt-SoVITS模型路径无法保存的bug
        - 聊天页 新增聊天记录，默认显示最新100条的聊天记录，在前端直接可以看到交互数据，不过前端容易被阻塞导致数据不显示或者卡死的情况（5s超时），都在正常情况下，不必慌张
        
    - 2024-3-18
        - 数字人视频播放器新增Sadtalker、GeneFace++
        - 按键映射 新增 组增减功能，新增单句触发单次按钮，针对表情控制时不希望一句话有多个关键词，表情乱变的情况发生
        - webui chatgpt的llm模型下拉框支持搜索、自定义添加模型名（配合ollama这种，方便自定义模型名）

    - 2024-3-17
        - 图像识别 新增循环定时截图触发功能，方便实现游戏解说、画面讲解等功能，自主触发，丰富直播内容
        - 新增 自定义命令板块，实现API调用解析获取数据，能动性很高，所以也会有点安全风险

    - 2024-3-15
        - 新增 图像识别 板块，使用多模态模型（Gemini）的能力实现，暂时仅支持n秒后截图识别内容，未来会继续拓展

    - 2024-3-14
        - TTS中的vits、bert-vits2、gpt-sovits的float类型的相关参数支持范围语法, 如 `0.8-0.9`
        - chatgpt配置项 大标题补充说明兼容的项目和模型
        - gpt-sovits新增模型配置项，支持动态加载模型

    - 2024-3-13
        - 对接fish-speech
        - 更新blivedm库，恢复兼容

    - 2024-3-9
        - username大一统 将会迎来巨大的危机，请各位更新的幸运儿留意
        - claude配置页 合并2个板块

    - 2024-3-8
        - 支持讯飞星火v3.5 和 助手API

    - 2024-3-6
        - 新增 虚拟身体 数字人视频播放器

    - 2024-3-4
        - 修复本地问答下 用户名变成助播的bug
    
    - 2024-3-3
        - 优化数据分析 页面运转 数据库不存在的异常提示
        - 修改qwen-alice为qwen，适配qwen官方库openai_api接口
        - 修复 文本转语音页面 通用的测试音频合成 gpt-sovits无法合成测试音频的bug
    
    - 2024-3-2
        - 通义千问 补充大模型常用配置项 和 联网搜索功能
        
    - 2024-3-1
        - 新增 通义千问官方API的调用；恢复 web类型下 通义千问 白嫖调用

    - 2024-2-29
        - 对接EasyAIVtuber
        - main程序在聊天模式下 主线程运行完没有等待子线程运行导致的edge-tts运行问题修复

    - 2024-2-28
        - 删除PyQT相关源码
        - 智谱AI新增 应用 功能的对接
        - 动态文案 前端新增文案组添加删除功能，新增LLM类型，可以指定动态文案选用的LLM
        
    - 2024-2-27
        - 补充动态文案和闲时任务默认数据
        
    - 2024-2-26
        - 对接 koboldcpp

    - 2024-2-25
        - 对接 Azure TTS

    - 2024-2-24
        - 合并各平台到单程序，减低冗余
        - 聊天页 新增 播放中不录音的配置，方便在本地做AI客服等场景应用时避免循环录音错误问题
        - 新增配置项 弹幕模板，可以在发送给LLM前对弹幕内容进行包装，如携带用户名等

    - 2024-2-23
        - 接入 在线版qanything
        - audio修改成员变量到类变量（后期应用使用

    - 2024-2-19
        - 对接 QAnything

    - 2024-2-17
        - 对接Kimi Chat（复用ChatGPT类型，具体使用参考上方文档）

    - 2024-2-14
        - 按键映射功能改为按键/文案映射，其中新增了按键触发、文案触发控制，可以实现关键词或礼物触发对应文案（比如：用户打赏了一个 辣条，那么在 文案触发类型 包含了 礼物 的情况下，会在对应文案中随机一个文案合成音频进行播放，此外这个文案也支持动态变量）

    - 2024-2-13
        - 修改so-vits-svc和ddsp-svc音频输出路径为绝对路径

    - 2024-2-11
        - 文档新增一个vercel的备份
        - 助播模式新增语音合成配置，可以自定义文本匹配后用的语音合成类型，从而区分助播和主播的声音
        - 文案页-文案音频合成新增语音合成类型选择，可以自定义TTS进行合成，不需要保存就可以切换

    - 2024-2-9
        - 接入clone-voice

    - 2024-2-7
        - 平台新增 TikTok 的接入，目前支持数据类型：弹幕、礼物、入场。

    - 2024-2-4
        - 新增 数据分析 页面，统计分析最热弹幕词云、积分榜单、礼物榜单
        - webui右下角新增返回顶部按钮
        - webui优化文档和关于
        - 抖音平台融合聊天模式
        - 抖音平台 在没有启动监听程序的情况下 优化提示日志，并不结束程序，用户可以通过webui重启

    - 2024-2-3
        - gpt-sovits对接CyberWon的WebTTS版的API
        
    - 2024-2-2
        - 智谱新增glm3-turbo和glm4的接入
        - gpt-sovits新增官方api对接，更加方便高效
    
    - 2024-2-1
        - webui 文案页 文案音频合成新增合成后音频在页面试听和删除的功能
        - 本地问答库-json新增积分的回答内容

    - 2024-1-31
        - webui实现板块显影功能
        - Live2D移到虚拟身体，新增模型名配置，可以自动检索模型名，进行模型加载
        
    - 2024-1-29
        - 优化翻译前原文字幕的保存实现
        - 页面配置新增 板块显影配置（实际显影功能还未实现，待推进，后续可能做成显示+功能开关）

    - 2024-1-27
        - 优化文案播放逻辑，文案播放过程中进行播放列表索引值记录，在被打断时，会从被打断的播放列表恢复播放（待大数据测试
        - 优化日志输出
        - 平台：哔哩哔哩2 融合聊天模式，可以变监听直播间，边监听按键触发语音聊天（待大规模测试

    - 2024-1-26
        - 优化webui排版
        - 补充原文字幕的配置项
        - 新增谷歌翻译，接入通用翻译和SD翻译

    - 2024-1-25
        - 聊天类型新增 alice（群友定制）
        - 延长聊天页 按键监听时长为0.5s，降低误触概率

    - 2024-1-23
        - 文案页 新增 文案文本加载相关的功能，合成功能开发中
        - 过滤新增表情弹幕过滤，就是[]包裹的内容
        - 优化日志输出
        - SD板块新增翻译功能，源自翻译页配置，暂时仅有百度翻译。
        
    - 2024-1-22
        - 按键映射 新增 礼物映射按键，可玩性增加

    - 2024-1-21
        - 聊天页 新增 复读音频插队，配合audio_player_v2可以使用
        
    - 2024-1-18
        - 修复GPT-SoVITS参考语言配置项的bug
        - 违禁词过滤新增违禁开关、违禁丢弃、违禁替换等功能
        - 修复动态文案无法使用的bug

    - 2024-1-17
        - 新增对接OpenVoice时gradio的配置参考
        - 更新思维导图
        - 聊天模式新增 按键监听开关
        - TTS新增GPT_SoVITS的接入

    - 2024-1-16
        - 新增音频播放器选项 audio_player_v2，对接新版播放器功能，具体参考对应项目更新日志
        - 删减违禁词

    - 2024-1-12
        - 兼容新版的langchain_chatchat
        - 本地问答新增配置项 最大用户名长度，用于自定义限制
        
    - 2024-1-11
        - chatgpt配置新增测试按钮，可以测试当前配置是否正确
        - 删减违禁词

    - 2024-1-10
        - SD追加虚拟摄像头创建的日志输出，方便用户使用

    - 2024-1-8
        - SD新增保存图片到本地相关功能，优化其UI布局
        
    - 2024-1-8
        - 聊天模式 新增 faster_whisper的接入，即可不使用魔法，不用花钱，本地进行语音转文本；聊天页 增加部分新配置方便自定义 
        - 删除torch相关的库，请手动安装 
        - 助播内容不再触发念用户名功能（脑测没bug） 
        - 修复SD加载LLM异常的bug 

    - 2024-1-7
        - 修复积分页UI错误问题
        - 修改默认配置，关闭所有异常报警
        - 异常报警计数改到函数内部计数，提高逻辑性

    - 2024-1-6
        - 闲时任务日志输出优化
        - text-gen新增官方api的对接并新增传参top_p、top_k、温度、seed

    - 2024-1-4
        - 完成 答谢板块 随机文案的开关功能
        - 聊天页新增调教功能，用于在直播中动态调教LLM而不进行TTS合成
        - 页面配置 新增 自动运行 功能。启用后，启动webui后会直接根据当前配置运行。
        - 异常报警新增 开始报警错误数、自动重启错误数的配置项，优化报警逻辑。其中自动重启配合“自动运行”使用，以便在部分功能出错时，可以重启自修复。

    - 2024-1-3
        - SD配置项补充其他LLM
        - 新增答谢板块的随机开关（后端未实现）
        - 删减违禁词

    - 2024-1-2
        - 新增最大用户名长度，在主要应用的版本实现此功能，防止有的用户名过长，影响观感
        - 新增普通音频播放时间间隔配置项（如果你感觉音频和音频之间太快或太慢，可以自行调节间隔时间）

    - 2023-12-31
        - 点歌模式新增相似度配置项，优化文件搜索函数，不被拓展名干扰
        - webui新增webui配置（IP、端口、标题）

    - 2023-12-30
        - 助播模式 音频匹配新增 匹配算法选项，提供可用性
        - 优化整理了部分代码
        - 助播模式 新增类型自定义选择，可以选择那些数据会触发助播，增加可用性
        - 修复红血球佬的在线tts调用失败问题（ssl禁用）

    - 2023-12-29
        - 针对文案内容被弹幕打断后顺序会错乱问题进行了修改，改为打断后恢复会重载整个数据列表，仍有大量的问题，暂时凑合
        
    - 2023-12-28
        - 优化chatgpt的测试程序
        - webui实现异常报警功能
        - 修复闲时任务随机列表无法关闭的bug
        - text-gen新增类型配置，默认为coyude
        - 修改LLM函数统一为get_resp
        - 删减违禁词

    - 2023-12-27
        - 优化chatgpt返回内容
        - 异常报警新增llm，平台，svc的后端实现
        - 补充异常报警语音

    - 2023-12-26
        - 修复b站2 开放平台 appid数据类型错误问题
        - 修改日志INFO等级颜色为白色，自定义请修改logger.py
        - webui尝试实现api接口，还在功能尝试中，请勿调用
        - 异常报警 新增 平台异常、TTS异常的后端实现

    - 2023-12-25
        - 给log增加颜色，看日志舒服了
        - 新增 助播模式（需要注意的是此功能的本地问答-文本 情况下语音区分暂未实现） 
        - 优化音频播放逻辑，之前哪些直接插队的本地音频将会老实排队，等前面文本先合成 
        - 新增配置检测函数，用于防止用户瞎配置导致无法使用（暂时只开了个头，后续推进功能实现）

    - 2023-12-24
        - 新增bert-vits2 v2.3 hiyori UI的API对接
        - 优化tts部分代码实现（有点小改动，可能有bug，待测） 

    - 2023-12-23
        - 更新多个gpt3.5的模型 
        - 过滤新增 弹幕过滤前后缀，用于直播间直接聊天而不触发LLM；
        - 删减违禁词 

    - 2023-12-21
        - TTS新增gradio模式，用于直接配置传参等信息，来适应绝大多数的有gradio接口的tts项目
        - 接入 微信视频号（暂时只有弹幕和入场数据）

    - 2023-12-18
        - 新增 谷歌 Gemini 的接入
        - 新增docker（但暂时并不适用）

    - 2023-12-17
        - 新增 极地极光、曲奇饼干 UI配色
        - 修复api 聊天模式相关bug
        - 新增按键UI设置
        - 补充“关于”说明
    
    - 2023-12-16
        - 新增API程序，第三方可以通过api控制程序运行、配置修改、直播数据发送等，后续系统全部功能皆可通过api进行操作
    
    - 2023-12-15
        - 新增 千帆大模型的接入；
        - 对llm相关源码加载和逻辑处理做了大优化，可能有bug，待测试
    
    - 2023-12-13
        - 接入 千帆大模型（有版本冲突，暂不启用）
        - elevenlabs升级到0.2.8，可以继续正常使用。一定要注意pydantic的版本，不能高于2.0

    - 2023-12-12
        - 通用配置-音频播放 新增 文本切分启用开关，关闭可以语句一次性合成（TTS吃得消的情况下）

    - 2023-12-9
        - 补充遗漏依赖
        - 依赖文件统一为一个
        - 优化通义千问报错日志
        - 增加了恢复出厂的功能，但隐藏了按钮
        - 新增 动态配置功能，暂时仅针对抖音，可以根据在线人数动态切换配置内容实现改话术、配音等功能（大改动！可能有很大的bug）
        - 聊天模式 新增自定义声卡输入，可以用于实现直播连麦互动效果

    - 2023-12-8
        - 删减违禁词
        - 接入 通义星尘（固定角色）
        - 答谢模块 文案部分改为多行文案随机获取

    - 2023-12-3
        - 优化线程启动实现，功能没启用不启动线程
        - 恢复聊天模式 翻译配置热加载，优化代码实现
        - text_generation_webui支持上下文记忆

    - 2023-12-1
        - 智谱AI 新增chatglm_turbo
        - 恢复tts.ai-lab.top的兼容，新使用方法参考文档说明
        - 优化tts、webui代码

    - 2023-11-29
        - 文案页 支持增删文案组
        - talk 后移线程到麦克风监听后，规避麦克风监听异常的bug
        - 优化tts异常日志
        
    - 2023-11-28
        - 聊天模式 补充动态文案、定时任务、闲时任务的触发功能 

    - 2023-11-27
        - 聊天模式 支持动态修改语音识别相关配置，从而实现多语言识别；config类删除单例（待测试）
        
    - 2023-11-26
        - 升级备份脚本，补充遗漏的out文件夹，改备份为强制覆盖
        - 优化talk部分源码
        - tts请求新增请求超时，默认60s
        - 接入langchain_chatchat
        - chatgpt兼容0.x.x和1.x.x版本
        - 接入文心一言官方API

    - 2023-11-22
        - 修复webui 智谱AI部分配置无法保存的bug
        - 点歌模式命令改为多命令形式

    - 2023-11-21
        - 新增备份配置和数据脚本，懒人包脚本位于Scripts文件夹内

    - 2023-11-20
        - 补充遗漏的依赖
        - 修复talk遗漏的全局变量

    - 2023-11-19
        - chatgpt增加请求超时时间，默认30s
        - 修复按键映射描述错误问题
        - 平台程序新增flask，创建http接口，修改webui的聊天页文本框为http请求对接的形式，修复了聊天页发送内容实例化2次My_handle类造成双重音频的问题

    - 2023-11-18
        - 优化webui配置项描述
        - 按键映射改为实际使用情况下的配置情况
        - webui补充遗漏的内置Live2D启动功能
        - 修复webui 聊天页 直接复读无法使用的bug

    - 2023-11-17
        - unity对接新增密码
        - 着手开发异常报警功能
        - 修复webui 过滤配置 文字描述错误问题
        - 修复webui 睿声AI配置项描述错误问题

    - 2023-11-16
        - 更新logo
        - 修复pyqt b站配置项错误问题
        - webui 文档页直接内嵌在线文档，方便用户直接查看
        - webui补充遗漏的 点歌模式 配置
        - 紧急关闭webui公网访问
        - 修复 webui 聊天页 直接复读 bug

    - 2023-11-15
        - 修复百度翻译配置读取错误问题
        - 接入 睿声AI（新的在线TTS）
        - webui 页面配置 新增 账号管理配置，可以自定义是否启用登录功能、修改账号密码

    - 2023-11-14
        - 禁用文案的自动播放
        - gpt新增gpt-4-1106-preview
        - 哔哩哔哩方案2新增开放平台对接，使用官方API进行监听，应该是最稳定方案了
        - 音频合成后的路径统一为绝对路径，稳妥点
        - 不在对PyQt进行兼容！！！
        - 新增翻译功能，暂时接入百度翻译API，可以配置弹幕或回复内容翻译
        
    - 2023-11-13
        - 新增 unity第三方项目对接，将LLM等响应数据传给HTTP中转站（可以用于对接其他项目使用）
        - 恢复genshinvoice的API调用
        - 移动unity对接的启用方式到 虚拟身体 配置项
        - 修复vits不能切换类型的bug
        - 默认不启用webui的登录功能

    - 2023-11-12
        - 修复webui闲时任务日志bug
        - webui重启前先停止程序
        - 文案机制增加自动播放功能，至此，webui开发已完全覆盖pyqt，开始推进废弃pyqt计划

    - 2023-11-11
        - twitch增加重连机制和多次失败停止运行机制
        - gpt默认token提升到4096
        - webui使用linux兼容路径语法
        - bilibili2 cookie问题bug修复
        - 优化闲时任务日志输出内容

    - 2023-11-10
        - 补充GUI遗漏的OpenAI TTS配置
        - 补充遗漏的依赖
        - webui新增 页面配置页，暂时支持设置UI主题
        - 优化webui提示框
        - TTS新增tts.ai-lab.top的接入（webui已适配）

    - 2023-11-09
        - 对闲时任务的闲时时间强制转型为int
        - 新增OpenAI TTS接入
        - 删减违禁词

    - 2023-11-07
        - 新增纯特殊字符和空格组成的文本的合成过滤，避免tts合成错误音频
        - 文案页 文案合成 vits传参补充遗漏的sdp_radio
        - 删减违禁词
        - 优化chatgpt特殊情况下token一直超长问题,2次都超长，直接清空上下文
        - 增加伊卡洛斯本地问答数据
        - 新增闲时任务功能
        - 闲时任务-本地音频 传递的内容改为文件名，而非完整路径
        - 修复文案页-tts用vits时，无法合成文案音频的bug

    - 2023-11-06
        - 修复audio_player模式下，取消点歌失效的bug
        - 通义千问不再适用

    - 2023-11-03
        - 修改点歌模式发送路径为绝对路径

    - 2023-11-02
        - audio_player类到单独文件中，补充audio_player接口的调用函数
        
    - 2023-11-01
        - 讯飞星火新增版本配置项，用于选择具体API调用版本
        - 删减违禁词
        - 新增audio_player的对接，内测阶段，bug较多，不建议使用

    - 2023-10-31
        - 升级星火库到1.5.0
        - 修订违禁词
        - 按键映射新增配置项 类型，可支持弹幕或回复触发
        - 按键映射 回复类型下，其触发规则改为 回复内容包含关键词即触发

    - 2023-10-29
        - 删除部分Live2D模型

    - 2023-10-28
        - 优化webui文本错误部分及UI排版

    - 2023-10-27
        - 支持智谱新模型32k
        - webui补充虚拟身体配置项
        - 删减部分违禁词

    - 2023-10-26
        - 新增虚拟身体配置页面
        - 修改webui图标和标题，拉出关键传参
        - webui新增开关灯功能
        
    - 2023-10-25
        - webui删除遗漏的登录页按钮

    - 2023-10-24
        - 修复b站监听方案2的用户名获取失败bug
        - webui增加登录页；美化UI
        - 补充遗漏的webui登录配置
        - webui新增登录页使能，咱本地使用不需要登录！

    - 2023-10-22
        - 修复斗鱼监听失败bug
        - b站登录新增2种登录方式
        - 新增哔哩哔哩监听方案2（后期实测稳定性）

    - 2023-10-21
        - 接入 twitch
        
    - 2023-10-20
        - 修复本地问答音频库触发后，会合成多余内容的bug
        - 提高httpx日志等级
        - 接入 YouTube
        - 修复webui，语音合成配置不生效bug

    - 2023-10-18
        - webui新增部分聊天页配置功能
        - 修改watchfiles日志等级
        - webui增加聊天输入框及发送按钮
        - 修复webui运行都是b站的问题
        - 优化webui的UI样式

    - 2023-10-17
        - webui补充积分页配置功能（修复部分bug）
        
    - 2023-10-15
        - 智谱AI新增无用内容删除，让回复更加正常点，不用把相关描述也输出
        - 提供多按键映射的配置实例；修复多按键映射bug
        - GUI增加按键映射配置板块；修改相似度配置项为字符串类型
        - webui新增文案页部分配置功能

    - 2023-10-14
        - webui补全通用配置页；修复配置上的部分bug

    - 2023-10-13
        - 修复平台配置bug
        - 新增音频随机变速、Live2D、定时任务的配置项

    - 2023-10-12
        - 补充遗漏的nicegui依赖
        - 修改按键映射的函数调用为按下释放，配置结构调整为单个按键多行配置的形式

    - 2023-10-11
        - 新增虚拟身体部分 对接xuniren项目

    - 2023-10-10
        - 补充遗漏的pyautogui库
        - 按键映射增加日志输出
        - webui新增答谢、按键映射板块的配置功能

    - 2023-10-09
        - 新增按键映射配置，执行晚于其他3个模式（GUI未适配）
        - 按键映射功能，新增配置项-起始命令（GUI未适配）
        - 修复文案音频合成bug补充genshinvoice的兼容（不确保没新bug）

    - 2023-10-07
        - 智谱AI新增CharacterGLM模型

    - 2023-10-06
        - webui开发进行中...进度预估30%

    - 2023-10-01
        - 音频部分相关的优化（音频输出路径自定义等）

    - 2023-09-26
        - 修复通义千问必须配置文件的bug

    - 2023-09-23
        - 新增积分页的GUI实现，并且优化了UI部分动态加载数据的源码
        - 新增 通义千问 的接入
        - GUI的下拉选择框支持编辑，可以填入关键词进行直接的搜索

    - 2023-09-22
        - 新增积分页，积分页暂时只完成了签到板块的显示功能
        - 完成积分机制目前所有后端功能

    - 2023-09-21
        - 弹幕处理新增全标点符号的弹幕过滤 
        - 追加几个本地问答，让ai有所b数；更新投资人信息 
        - 更新违禁词库

    - 2023-09-20
        - 智谱回复部分如果存在多\情况，则会删除重复的\仅保留一个

    - 2023-09-19
        - 新增游戏demo例程
        - 修改默认配置关闭积分机制

    - 2023-09-18
        - 积分机制 新增礼物和入场积分记录的实现，GUI未适配；默认配置修改。
        - 积分机制 新增查询功能，用户可以查询积分情况，GUI未适配；

    - 2023-09-17
        - 后移web字幕打印机调用的位置，让其可以对其音频合成部分

    - 2023-09-16
        - 录音页 新增录音按键` 数字1左边按键
        
    - 2023-09-16
        - 新增积分表，暂时只做了b站的签到部分功能，GUI未适配

    - 2023-09-14
        - 更新requirements_common.txt，解决aiohttp等版本冲突问题 —— vantang

    - 2023-09-13
        - GUI缩短配置项长度，给右侧预留10%的空间，方便鼠标在此处停留使用滚轮功能。
        - 更新切分算法，没有最长字符的强制切分，读句子会丝滑，但是千万要断句啊，怕你电脑吃不消

    - 2023-09-12
        - vits-fast新增配置项 语言，可以固定合成语言或自动识别
        - 新增文心一言web版API接入

    - 2023-09-11
        - 删除聊天页ctrl+c或z的程序退出功能
    
    - 2023-09-10
        - 新增 念弹幕功能，可以对直播间弹幕进行复读，更有针对性，试用助理场景（另外发现b站的用户名被加密了）
        - 修复GUI内置文档超链接过期问题

    - 2023-09-09
        - 文档独立到单独仓库，在线访问。
        - 聊天页 文本输入框支持回车按键触发发送。

    - 2023-09-08
        - VITS下，兼容bert-vits2

    - 2023-09-05
        - 修复后置回复没法关闭 念用户名 的bug
        - 删除部分无关紧要的违禁词
        - 本地问答文本库 新增动态变量{username}，用于替换用户名

    - 2023-09-03
        - 新增 谷歌bard的接入，支持上下文记忆。
        - b站板块可以选择不登录（部分用户不登录也可以正常使用）
    
    - 2023-09-02
        - 补充、删减部分违禁词
        - 补充遗漏的zhipuai库
        - 入场和礼物感谢部分删除用户名中存在的特殊符号
        - 抖音关注事件可以触发关注感谢话术
        - 基本实现动态文案功能，待后续使用体验中完善
        - 更新b站监听库到16.0.0版本，新增b站登录板块，获取cookie等信息解决弹幕监听丢失问题（强烈建议使用小号登录，有风险）
        - 修复GUI b站部分配置项描述错误

    - 2023-09-01
        - 新增 智谱AI的接入，支持上下文记忆。
        - 修复智谱AI返回内容有\n时，也会进行语音合成的bug
        - 删除部分违禁词
        - 念用户名时，删除用户名中存在的特殊符号
        - 顶部菜单栏新增Q群跳转，改名 帮助  

    - 2023-06-13
        - 兼容本地版ChatGLM API接口  

    - 2023-06-16
        - 增加Edge-TTS的语速、音量调节参数。  

    - 2023-06-17
        - 增加GUI版。
        - 增加GUI运行的bat文件，需要配合本地虚拟环境运行。请到releases下载。
        - 对config.json的结构做了调整，增加了弹幕前后缀过滤配置。
        - 增加langchain_pdf_local的配置内容，待和主线整合后合并。

    - 2023-06-18
        - 修复部分GUI的bug
        - 整合到主线
        - 新增本地live2d模型加载

    - 2023-06-20
        - 补充了整合包的打包方式
        - 音频合成更改多线程为队列结构，解决高并发的崩溃问题
        - langchain_pdf_local 增加 [GanymedeNil/text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese) 模型，该模型在中文解析上很好
        - 增加弹幕触发,回复部分日志记录时，每20字符自动换行的机制
        - 修改edge-tts合成音频的文件名范围
        - 更换抖音方案为`dy-barrage-grab`  
        - GUI新增 弹幕日志类型、修改langchain_pdf_local的模型下拉选择

    - 2023-06-21
        - 修复语音合成内容错误的bug

    - 2023-06-23
        - 针对整合包问题进行了优化和处理，新增了Scripts文件夹用于存储制作整合包时需要用的相关脚本。  
        - 新增本地回答库，启用后优先匹配库内问答，无匹配结果则按正常流程运行
        - 新增stable diffusion的接入。（UI还未适配，初步实现功能，搭配虚拟摄像头食用）

    - 2023-06-24
        - 新增stable diffusion的接入。（UI还未适配，初步实现功能，搭配虚拟摄像头食用）
        - bug修复：vits配置项依赖问题
        - 补充遗漏的ui文件
        - GUI补充缺失的vits的speed
        - GUI增加SD的配置
        - GUI修改Edge-TTS的说话人配置为下拉菜单，数据文件在data下，可以自行编辑修改

    - 2023-06-25
        - 修复保存配置时，edge-tts配置报错错误导致程序无法正常工作的bug

    - 2023-06-28
        - 将langchain_pdf和langchain_pdf_local两个模式统一为chat_with_file模式

    - 2023-06-29
        - 合并dev和main，并同步兼容GUI。
        - 修复GPT_MODEL初始化claude时的空配置bug
        - bilibili-api-python需要升级至15.5.1，更加稳定
        - GUI改langchain为chat_with_file
        - 正式合入主线

    - 2023-07-01
        - 修改chat_mode的gpt为chatgpt，适配调整。
        - MD增加目录
        - 追加对text-generation-webui的兼容。
        - 修复chat_with_file，openai相关模式下的无法使用的bug。
        - 补充缺失的faiss-cpu依赖。
        - 后置create_faiss_index_from_zip的加载。
        - 语音合成逻辑升级，会先对中文长文本进行切分，然后多线程队列合成，从而可以通过多次合成的方式处理长回复。
        - 修改默认音频合成长度为80 & 200。
        - GUI部分固定配置项改为下拉框形式，简化配置难度。
        - GUI chat_with_file部分对chatgpt/claude的配置依赖，改选中直接呼出3个配置box。
        - 修复音频分割部分对短音频丢失问题的恶性bug。

    - 2023-07-02
        - chat_with_file模式支持加载本地模型，无需链接huggingface仓库
        - 延长audio合成部分，合成队列的循环延时，一定程度上降低对Edge-TTS的压力。
        - 给audio合成中 vits没有启动时的数据解析追加try异常捕获。
        - 修复 回复文本切分时，对空字符串的过滤遗漏，并对.的过滤进行删除，默认中文环境的过滤
        - 音频合成部分基本上都进行了异常捕获。
        - 新增功能 点歌模式 触发优先级高于LLM和弹幕过滤机制，可以通过 自定义点歌和取消点歌命令 播放本机已有音频。

    - 2023-07-03
        - 新增so-vits-svc的接入，可以对edge-tts/vits-fast合成后的音频进行变声后在输出。
        - 优化链接过滤的实现，提升准确性。

    - 2023-07-04
        - 优化说明文档，以更利于用户通过文档解决相关问题、获得帮助。
        - 微调了语音合成前的文本切分算法，会控制在10-30字，结合合成时间大概可能也许可以达到不错的连续性。

    - 2023-07-05
        - 点歌模式 支持子文件夹的音频文件搜索，不用拘泥于一级目录了。
        - 修复source_data因为路径已存在而没有定义的bug。
        - 音频合成输出日志，方便用户了解音频合成情况。
        - 修复点歌完成后，还进行LLM对话的bug。
        - 修复chat_with_file openai_gpt模式，数据切分丢失数据的恶性bug。

    - 2023-07-08
        - 新增 文案模式，基本完成功能。可以自定义文案、合成音频、配置相关信息、循环暂停播放文案。
        - 修复 文案模式 合成音频失败的bug
        - 修复 文案模式 没有运行就可以进行合成、播放、暂停操作的bug
        - 优化 文案模式 音频播放部分的实现逻辑。新增加载文案不存在就创建的机制。追加了文案页的各个配置和相关说明。
        - 修复 audio子线程sleep阻塞主线程弹幕监听的问题。
        - 修复 文案音频暂停后 会被弹幕重新激活的bug。
        - 优化 文案模式 GUI相关交互

    - 2023-07-09
        - 新增 聊天模式-谷歌。可以本地直接与LLM进行语音聊天。（依赖魔法）
        - 新增 SD模型下 LLM对提示词优化的功能。GUI同步适配。

    - 2023-07-10
        - GUI可以检索Live2D路径下的模型进行动态修改配置。（需要注意，修改后浏览器缓存问题，请用无痕浏览器打开）
        - 追加 Live2D官网所有的免费模型
        - 新增 答谢功能（入场欢迎、礼物答谢），暂时只支持B站，GUI同步进行配置。

    - 2023-07-11
        - 优化文本切分算法

    - 2023-07-12
        - 增加项目的思维导图
        - 增加项目的简易流程图

    - 2023-07-13
        - 聊天页新增聊天框，在运行后可以直接使用聊天框进行聊天
        - 修改audio、sd、claude中所有的time.sleep为异步睡眠

    - 2023-07-14
        - 新增TTS模式 genshinvoice_top,调用第三方接口完成语音合成

    - 2023-07-15
        - 修改 聊天模式-谷歌 为 聊天模式，新增语音识别 百度接口。
        - 追加线程进程退出处理（部分有效）
        - 聊天模式 按键触发兼容英文大小写字母。
        - 聊天模式 支持循环录音功能，新增停止触发按键。

    - 2023-07-16
        - 优化cluade协程处理方式
        - chat_with_file的openai_gpt同样使用提示词模板来自定义回答方式
        - 新增字幕日志，只会输出即将播放的音频文本，用于直播时的字幕显示。
        - 音频合成的消息队列改成阻塞队列

    - 2023-07-17
        - 抖音版增加入场欢迎和礼物答谢（礼物答谢的金额需要手动维护价格表）
        - 新增 同拼音的违禁拼音过滤机制
        - GUI适配字幕日志的配置

    - 2023-07-18
        - 新增抖音礼物价格数据，礼物价值下限将生效（数据不全，可以自行补充）
        - 优化抖音日志信息，只输出info信息，不在输出debug日志，更加清爽。
        - 接入DDSP-SVC，简单测试了下，效果好像不太对。优化了变声部分的代码

    - 2023-07-19
        - GUI适配DDSP-SVC；补充说明文档
        - 优化audio中vits接口的设计&优化代码减少冗余
        - 新增本地问答音频库，机制类似点歌，通过编辑音频文件名做为触发匹配关键词，优先级第二高，匹配命中后直接会进行匹配音频的播放。
        - 新增自定义上下限音频随机变速，对普通音频播放和文案音频播放可以进行随机变速配置。(GUI未适配)

    - 2023-07-20
        - 增加ffmpeg缺失的解决方案
        - 文案模式增加了一组文案配置，也就是说有2块文案，会进行左右切换的播放，都播放完毕后会进行新的一轮播放。
        - 新增LLM后的第二重过滤（违禁词、链接、拼音）
        - 违禁拼音配置内容需要是中文，需要注意，已更正
        - 新增 念用户名的功能，例：回复xxx。你好
        - 新增用户名过滤（违禁词、链接、拼音）
        - 修复本地问答音频匹配，传入音频后缀导致的匹配错误bug
        - 新增本地问答库匹配 最低相似度配置，用于微调需要的关键词匹配度，已自定义触发灵敏度。
        - 音频随机变速 GUI适配

    - 2023-07-21
        - 修复edge-tts + so-vits-svc协同下，相对路径无法变声的bug
        - 针对部分用户绝对路径音频加载仍有系统找不到指定文件的情况，恢复相对路径，只在变声条件下转绝对路径
        - 音频变速部分改默认变速变调为默认变速不变调且函数兼容变速变调

    - 2023-07-22
        - 修复音频播放部分，音频变速调用缺失缩进导致变速必定执行的bug

    - 2023-07-23
        - 修复音频播放部分，音频变速语速低于1时变速合成的音频不正常的bug
        - 改变弹幕处理逻辑，先由process_data预处理函数进行指定时间内的数据丢弃后，再进行数据处理，可以有效降低高并发造成的一系列问题
        - dy_old改为接入第三方大佬提供的免费不可商用ws监听
        - 本地问答库支持自定义变量的形式来开发动态语句
        - 本地问答库-文本 修改完全匹配为相似度匹配，暂时和音频匹配共用一个相似度值
        - 文本切分算法，可以通过max_limit_len来对强制切分做自定义，对显卡性能高的用户而言，可以通过增大限制来提高语句流畅度。

    - 2023-07-24
        - 文案模式，文案格式修改，可以无限拓展文案路径数量来达到多类型文案切换的效果，GUI带适配动态加载。

    - 2023-07-25
        - 新增 不启用 聊天类型，修改none为不启用，reread为复读机。关闭聊天（LLM等）,既可以应用于直播助理等场景，只负责欢迎和感谢。
        - 接入科大讯飞 星火

    - 2023-07-26
        - 补充遗漏的星火依赖
        - 修复text-Gen max_new_tokens保存失败bug
        - 文案页，音频文件格式支持大写的MP3和WAV
        - 文案页 支持配置连续播放音频条件（超时切换&数量上限）
        - 文案页 文案切换播放逻辑变更，某一文案列表播放放完会重载列表内容，不再等待其他列表均播放完毕后才能重载

    - 2023-07-27
        - ChatGLM支持上下文，默认启动（GUI未适配）
        - 抖音版增加 定时播报任务功能，用户可以自定义是否启用，循环时间和定时任务文案（变量可自行修改源码追加功能）

    - 2023-07-29
        - 修复elevenlabs配置同新版不匹配导致无法使用的bug
        - 新增bark-gui的接入
        - 修复ChatGLM上下文记忆bug，并新增GUI相关配置，可以启用和设置最大记忆字符长度
        - 数据丢弃机制补全GUI配置

    - 2023-07-30
        - 修复点歌搜索失败bug
        - 修改默认的切分算法的最大长度为40字

    - 2023-07-31
        - 入场&礼物处理追加用户名违禁词过滤
        - 回复用户名支持选择变声开关&自定义前回复、后回复的文案，且支持多文案随机抽取(GUI未匹配)

    - 2023-08-01
        - 本地问答库升级，支持选择2种匹配算法。旧版本 一问一答，新版本 自定义json（更具灵活性）。文本和音频的相似度也分离了。
        - 回复用户名板块 GUI适配，顺便优化了GUI部分对多行文本处理的源码实现

    - 2023-08-02
        - 定时任务GUI支持动态加载
        - b站接入定时任务

    - 2023-08-03
        - 定时任务 报时任务补充分钟的播报
        - 修复定时任务同时存在多个变量时，无法正常运行的bug

    - 2023-08-04
        - 更换快手监听方案，新方案是playwright的形式，建议使用小号，每次用完需要删除cookie下的json文件，因为第二次就异常了，没法正常捕获。暂时只支持弹幕回复。
        - 快手 追加礼物Id和连击数日志，礼物价格和礼物名有待后期维护礼物表；补充默认cookie文件夹
        - 快手 补充定时任务（暂只支持 报时任务）
        - 闻达接入。ChatGPT改为ChatGPT/闻达，配合闻达启动器可以融入openai接口使用。

    - 2023-08-05
        - 聊天页 支持直接合成复读内容，适用于直播中有人值守时直接进行交流。
        - 点歌模式支持新功能-随机点歌，命令在配置文件/GUI中可以自定义
        - GUI新增 自定义板块显隐，用户可以根据自己喜好配置显示的box板块，让配置页面不再臃肿
        - 文案页，文案配置改为动态加载，即可以支持无限制的多套文案。
        - 修复文案和聊天同时使用时，音频播放会一次性播放2个的bug；b站重复调用的部分也做了删除。
        - 文案页 新增文案编号配置项和增删按钮，用于对文案配置进行动态的增删操作。

    - 2023-08-07
        - VITS全面改为VITS-Fast，新增VITS（原版，配合vits-simple-api使用），此更新变动较大，可能存在隐患，需要注意
        - 优化audio部分代码，tts部分源码全部拆到`utils\audio_handle\my_tts.py`中
        - 修复VITS配置保存后错乱的bug

    - 2023-08-08
        - 修复违禁拼音在拼音部分包含违禁拼音的情况下也被过滤的bug

    - 2023-08-09
        - 修复本地违禁词库不配置时无法正常工作的bug
        - 修复so-vits-svc+ddsp套娃变声失败的bug
        - 修复音频变声bug
        - 新增langchain_chatglm的接入

    - 2023-08-10
        - vits修改语言配置为下拉框，改默认为自动，修复bug

    - 2023-08-11
        - 过滤板块 新增遗忘保留数的配置项，从默认的1个数改为可以根据自定义配置保留，在定时触发后依次响应。

    - 2023-08-12
        - 新增 斗鱼平台的接入（初步接入，仅有弹幕数据的监听）
        - 修改commit为comment（大改动，单词拼错了，现在才发现，难绷）
        - 新增弹幕、入场、礼物的数据库日志记录(GUI未适配)

    - 2023-08-14
        - 新增Claude2的接入

    - 2023-08-15
        - 弹幕、入场、礼物的数据库日志记录GUI适配

    - 2023-08-16
        - 增加基于docsify的文档
        - 美化logo
        - 简单的初步美化下GUI

    - 2023-08-18
        - 后置部分GPT_MODEL配置，规避一次性全加载问题
        - 修复 LLM部分GUI板块显隐bug
        - 讯飞星火库需要升级才能恢复兼容（已更新依赖）
        - 修复部分GUI显示bug
        - 恢复Claude2的兼容

    - 2023-08-19
        - 新增 音频播放板块，暂时只提供音频播放的开关。
        - GUI优化按钮无边框问题；关于新增 在线文档 跳转入口

    - 2023-08-20
        - 新增 动态文案 版本GUI部分的实现（功能还未实现）

    - 2023-08-23
        - 近期发现有第三方直接套娃售卖项目，可怜的娃呀，收手吧。另外，套娃的，不分钱给我，我觉得这不合适吧（

    - 2023-08-24
        - audio合成 音频合成部分新增合成内容的日志，方便后期合成音频时的bug定位

    - 2023-08-27
        - 新增web字幕打印机的接入

    - 2023-08-29
        - TTS新增VALL-E-X的接入

## ⭐️Star 经历

[![image](//api.star-history.com/svg?repos=Ikaros-521/AI-Vtuber&type=Date)](https://star-history.com/#Ikaros-521/AI-Vtuber&Date)

## 🤝贡献

### 🎉鸣谢

感谢以下开发者对该项目做出的贡献：

<a href="//github.com/Ikaros-521/AI-Vtuber/graphs/contributors">
  <img src="//contrib.rocks/image?repo=Ikaros-521/AI-Vtuber" />
</a>

### 💸投资方

![image](./static/images/luna-ai/invest.png)

### 合作伙伴

青椒云：[qingjiaocloud.com](https://account.qingjiaocloud.com/signin?inviteCode=4Q92ROBQ)  ———— AIGC 高性能云桌面  

睿声AI：[reecho.ai](https://www.reecho.ai/)  ———— 瞬时创建 超级拟真的 人工智能克隆语音  

AIHubMix: [aihubmix.com](https://aihubmix.com/register?aff=1BMI)  ———— OpenAI,Google,通义千问等大语言模型API代理站  

### 🙌赞助

![image](./static/images/luna-ai/alipay.png){ width="200" }
![image](./static/images/luna-ai/wechatpay.png){ width="200" }

## 黑名单

| 用户信息 | 名人名言 |
|--------|------|
| QQ：750359376 | 笑死，连点开源精神都没有 |

