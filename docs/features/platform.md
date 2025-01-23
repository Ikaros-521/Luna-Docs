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

浏览器安装`油猴`插件，然后在前往 插件商店安装 直播弹幕监听 转发至本地WS服务端-[https://greasyfork.org/zh-CN/scripts/490966](https://greasyfork.org/zh-CN/scripts/490966) 插件，安装完成后，前往你想捕获的直播间，按F12打开开发者工具，看看console 控制台的输出，是否有监听到弹幕信息，有的话就没事了，没有的话可以刷新重试或者手动在console注入js运行。  

最后AI Vtuber选择`斗鱼`平台，然后运行就可以了，ws会传输弹幕信息。  

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
监听项目：[https://github.com/isaackogan/TikTokLive](https://github.com/isaackogan/TikTokLive)  

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

