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

对接使用视频教程：[https://www.bilibili.com/video/BV1Jy411q7sy](https://www.bilibili.com/video/BV1Jy411q7sy)  

训练模型视频教程：[https://www.bilibili.com/video/BV1rJ4m1u7sy/](https://www.bilibili.com/video/BV1rJ4m1u7sy/)  

#### DH_live

官方仓库：[https://github.com/kleinlee/DH_live](https://github.com/kleinlee/DH_live)  

对接时，虚拟身体选择“其他”，运行DH_live[整合包](https://pan.quark.cn/s/936dcae8aba0#/list/share/56a79e143a8b4877a98a61854e07b229-AI%20Vtuber/741f94606e414157b8d0a021d3a9ca77-%E8%99%9A%E6%8B%9F%E8%BA%AB%E4%BD%93/f7a1815edf4846ca874c53c4ed9afcbd-DH_live)（就是项目整合包内可以找到）的 麦克风驱动脚本即可。

#### live2d-TTS-LLM-GPT-SoVITS-Vtuber

视频教程：[【AI主播-虚拟身体篇】对接 刘悦佬Live2D项目 源码魔改，提供API 实现音频URL传入来驱动口型](https://www.bilibili.com/video/BV1fz421v7Yx)  

对接项目地址: [https://github.com/Ikaros-521/live2d-TTS-LLM-GPT-SoVITS-Vtuber](https://github.com/Ikaros-521/live2d-TTS-LLM-GPT-SoVITS-Vtuber)  

原始项目地址：[https://github.com/v3ucn/live2d-TTS-LLM-GPT-SoVITS-Vtuber](https://github.com/v3ucn/live2d-TTS-LLM-GPT-SoVITS-Vtuber)  
