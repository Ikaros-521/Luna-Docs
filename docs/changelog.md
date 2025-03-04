## 📝更新日志
- 2025-02-27
    - 优化：dify支持流式响应；
    - 优化：dify流式响应 过滤DeepSeek思维链

- 2025-01-23
    - 修复：main中错误的包导入

- 2025-01-11
    - 新增：弹幕监听脚本支持视频号 弹幕接入

- 2025-01-07
    - 新增：小红书监听适配
    - 新增：dify支持工作流模式（自定义传参，获取文本返回）

- 2024-12-31
    - 新增：webui和main增加https ssl证书的demo例程；main新增tts合成接口；main新增本地路径挂载功能
- 2024-12-29
    - 优化：LLM流式响应 openai接口的数据时，有的服务端会返回none数据，进行特殊处理
    
- 2024-12-16
    - 新增：增加get_sys_info接口，可以获取系统当前待播放音频数、等待合成消息数量

- 2024-12-12
    - 修复：GSV删除ws配置导致的运行bug 

- 2024-11-26
    - 新增：对接MeloTTS API
    - 删除：GSV ws配置，旧版gradio废弃 

- 2024-11-14
    - 修复：异常报警 和 DDSP配置保存错乱bug
    - 修复：补充遗漏的火山引擎 显隐开关功能

- 2024-11-13
    - 修复：因为板块隐藏导致变量未定义的bug
- 2024-11-10
    - 修复：Text Gen WebUI 日志调用错误bug（未测试，脑测没问题） 
    - 修复：metahuman_stream情况下播放状态检查 阻塞了main运行的bug 

- 2024-11-3
    - 新增：洛曦 直播弹幕助手 新增类型 按键映射-文案，对此类型消息支持(播放时的转发没有实现，因为类型定义没有这么细化)
    
- 2024-10-31
    - 新增：淘宝直播的接入（配合 监听脚本使用） 

- 2024-10-31
    - 新增：文本转语音 新增 不启用类型，可以不进行TTS合成喵
    - 优化：修改默认multitts的语速为50 

- 2024-10-30
    - 新增：对接MultiTTS
- 2024-10-29
    - UI：修改webui默认选中样式（换个口味）
- 2024-10-26
    - 修复：快手弹幕监听失败的bug；
    - 新增：对接 让弹幕飞（多直播平台弹幕监听平台）
- 2024-10-26
    - 新增：洛曦 直播弹幕助手 新增类型 弹幕消息，用于转发直播中的弹幕消息
    - 修复：智谱AI因为对接智能体 导致的代码写漏了判断条件遗留的bug
    
- 2024-10-25
    - 新增：聊天页 新增 对话打断功能，支持自定义 打断词、打断时清除什么类型的数据等。
- 2024-10-24
    - 优化：消息&音频队列优先级新增 助播文本、音频的设置
- 2024-10-23
    - 新增：本地问答-文本 调用洛曦 直播弹幕助手接口（配置 弹幕回复 即可）
    - 新增：对接F5-TTS gradio API（20241023主线版本）

- 2024-10-22
    - 新增：通用配置-辅助软件板块 新增 “洛曦 直播弹幕助手”的对接，用于将系统相关消息转发到直播间弹幕区等

- 2024-10-18
    - 新增：按键映射板块新增 图片映射功能，可以通过关键词或者礼物触发，将本地图片添加到虚拟摄像头用于直播使用（默认随机路径）沿用SD做为虚拟摄像头服务托管，背景色#00ff00ff 纯绿色，像素1080P

- 2024-10-16
    - 优化：common通用请求增加proxy参数；webui所有同步http请求更换为异步请求

- 2024-10-10
    - 新增：对接智谱AI 智能体
    - 重大更新：对webui配置保存的代码实现进行了简化，只进行了简单测试，可能有bug，请谨慎使用
    - 待办：路径统一到pathlib库规范

- 2024-10-9
    - 优化：基础配置页面排版，对配置板块进行分类到抽屉，便于用户理解
    - 待办：尝试兼容新版gemini

- 2024-10-4
    - 新增：blip图像识别模型

- 2024-10-2
    - 修复：流式LLM时 如果结尾没有中文标点符号会丢句子的bug

- 2024-10-1
    - 新增：联网搜索新增触发关键词

- 2024-9-27
    - 新增：联网搜索功能（暂时支持 百度、谷歌），联网搜索内容执行点在llm前，所以其结果会组合到弹幕中一并提交给LLM

- 2024-9-12
    - 新增：对接CosyVoice 0819的API

- 2024-9-5
    - 修复：OpenAI接口 测试按钮执行的测试流程缺少最后的数据解析，导致出现实际不行却测试通过的问题
    - 优化：内部API请求及webui API请求在IP配置为0.0.0.0时自动替换为127.0.0.1，避免请求发送异常；
    - 优化：平台为抖音时，启动定时任务阻塞主线程，防止异常问题（如：Edge-TTS不正常）

- 2024-9-4
    - 新增：大语言模型 接入 火山引擎（豆包）
    
- 2024-9-1
    - 优化：GPT-SOVITS 模型加载兼容V2的API
    
- 2024-8-31
    - 新增：GPT-SOVITS-V2 0821整合包API对接
    
- 2024-8-30
    - 新增：main程序新增 待播放音频数量（在使用 音频播放器 或者 metahuman-stream等不通过AI Vtuber播放音频的对接项目时，使用此变量记录是是否还有音频没有播放完），开发者通过8082的callback回调传入，即可更新此变量

- 2024-8-28
    - 新增：智谱AI新增glm4-flash，模型选择框支持自定义输入，用于支持其他模型
    
- 2024-8-20
    - 修复：谷歌翻译 代理没配置的情况下，变量未定义问题

- 2024-8-16
    - 优化：千帆大模型，AppBuilder输出内容过滤*和特殊[]，数据解析改至倒叙遍历返回
    
- 2024-8-14
    - 通义星尘兼容流式推理（脑测没问题）
    - 千帆大模型支持流式输出（AppBuilder脑测兼容，不兼容的话提个issue）
    
- 2024-8-13
    - 聊天页，语音唤醒新增模式选择：长期唤醒/单次唤醒，新的单次唤醒意味着每次触发都需要携带唤醒词
    - 聊天页 唤醒后，唤醒词将被替换为空

- 2024-8-11
    - 虚拟身体对接 live2d_TTS_LLM_GPT_SoVITS_Vtuber

- 2024-8-8
    - 通义千问支持流式输出，另外追加了 阿里云百炼支持的几个其他公司的大模型（百川、月之暗面、Yi）

- 2024-8-6
    - webui配置保存提示优化（提示当前平台、LLM、TTS等选项）
    - 聊天页 新增 直接语音对话 开关，如果启用了，将在首次运行时直接进行语音识别，而不需手动点击开始按键。针对有些系统按键无法触发的情况下，配合连续对话和唤醒词使用

- 2024-8-1
    - 协同 数字人视频播放器-v0.2.2 接入AniTalker
    
- 2024-7-31
    - 讯飞星火 模型命名改为官方新命名，新增4.0和pro-128k，使用请先更新库 [sparkdesk-api](https://github.com/Ikaros-521/sparkdesk-api)
    - 聊天页 聊天框提前到核心配置下，省得拉到底下才能对话
    - 修复音频播放间隔的随机数生成后 没有int化的bug
    - OpenAI接口支持流式输出（简单测试暂时没啥问题），默认OpenAI ChatGPT模式使用流式 提速
    - 弹幕日志相关记录封装函数，降低冗余
    - 优化openai流式返回的语句切分逻辑
    - 智谱AI，2.x+的库兼容流式推理

- 2024-7-30
    - 使用uv 进行环境安装

- 2024-7-28
    - 修复qwen漏改的log

- 2024-7-27
    - 聊天模式 STT识别为空 过滤不触发

- 2024-7-26
    - 使用poetry锁定依赖环境
    - 聊天页 新增 唤醒词和睡眠词，可以通过此功能唤醒ai对话，不需要时使用睡眠词停止回复，配合连续对话使用 
    - 部分第三方库版本升级，简单测试暂时没发现问题（待稳定性测试）

- 2024-7-24
    - audio.py中 pygame部分导入、实例化和调用统一改至播放器配置为pygame时生效，避免pygame异常情况下无法正常使用的问题
    - 删除文心一言，请统一使用 千帆大模型
    - 聊天页新增 SenseVoice，需要安装funasr，模型请自行下载（如魔塔社区、huggingface、我网盘备份等），ASR速度大大提升 

- 2024-7-23
    - 弃用flask，改用fastapi（测试了 聊天页发送、微信号对接，暂时没有发现问题。稳定性待测试）
    - 补充webui遗漏的API set_config接口，规范化api实现。api返回键值msg改为message

- 2024-7-21
    - 兼容gpt sovits官方整合包0706
    
- 2024-7-20
    - youtube监听增加重连机制，短时间内多次重连判断为无法连接，超过30s则无限重连 

- 2024-7-19
    - 【webui】gpt新增gpt-4o-mini模型
    - 修复 按键映射 礼物触发部分的bug，增加单个触发类型的异常捕获，单个触发出错不影响其他触发工作

- 2024-7-17
    - 接入Dify 聊天助手的API
    
- 2024-7-13
    - 修正 录音配置的描述

- 2024-7-8
    - 修复串口功能无法使用的bug（单例模式没有，串口的等待数据返回删了，会影响运行，只发送，不接收）
    - 修复了串口页的数据保存bug
    - 串口页的按钮仍有bug
    - 对接CosyVoice（使用刘悦佬0707的版本）

- 2024-7-7
    - 串口功能发布，在串口页完成配置和连接后，可以在通用配置-按键映射配置串口的映射关系（适用于弹幕现实游戏-串口控制功能）

- 2024-7-3
    - 修改faster-whisper默认模型为small
    - 本地问答板块 新增文本框用于json编辑，默认用于编辑 本地问答.json，方便修改内容，你也可以用作修改其他json文件。格式一定要对啊；
    - 修复睿声配置保存格式错误bug

- 2024-7-2
    - webui 通用配置的聊天类型 改名为 大语言模型
    - 通用函数增加异常捕获

- 2024-6-27
    - 修复睿声调用，音频后缀名改为mp3
    - 睿声AI 新增新版API的几个参数，可以支持V2.0的调用（没测过，不确定）

- 2024-6-26
    - 聊天页 补充参数CHANNELS RATE的设置 
    - 全局替换日志 logging为loguru 

- 2024-6-24
    - LLM返回内容，一律替换 \n换行符 \n字符串为空

- 2024-6-23
    - 智谱 2.x版本API调用补充top_p和temperature的参数
    - 补充遗漏的智谱模型，修复配置项描述错误

- 2024-6-22
    - 针对通义星尘 上下文长度配置项数据类型错误问题进行修复
    - metahuman-stream 支持wav2lip
    - 新增 抖音2 监听方案（以便适配非win平台）

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