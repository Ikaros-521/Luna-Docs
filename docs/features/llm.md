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

##### 智能体

图文教程：[https://github.com/Ikaros-521/AI-Vtuber/pull/1015](https://github.com/Ikaros-521/AI-Vtuber/pull/1015)  
智能体创建：[https://chatglm.cn/main/toolsCenter?lang=zh](https://chatglm.cn/main/toolsCenter?lang=zh)  
密钥获取：[https://chatglm.cn/developersPanel/apiSet](https://chatglm.cn/developersPanel/apiSet)  
智能体 ID，浏览器打开智能体对话页后，可通过URL地址栏查看。例如：`https://chatglm.cn/main/gdetail/6706907a6c06eb2f71087d47?lang=zh`,那么ID为`6706907a6c06eb2f71087d47`  

模型选择“智能体”，配置密钥等，保存重新运行即可。  

#### langchain-ChatGLM

官方仓库：[langchain-ChatGLM](https://github.com/chatchat-space/langchain-ChatGLM)  

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

#### langchain-chatchat

官方仓库：[https://github.com/chatchat-space/Langchain-Chatchat](https://github.com/chatchat-space/Langchain-Chatchat)  
视频教程：[https://www.bilibili.com/video/BV1c94y1n7Ga/](https://www.bilibili.com/video/BV1c94y1n7Ga/)  

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

#### 文心一言（已弃用，更换千帆大模型）

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

#### 阿里云百炼（通义千问、百川、月之暗面、零一万物、MiniMax）

官网：[qianwen.aliyun.com](//qianwen.aliyun.com/)   

阿里云百炼平台：[bailian.console.aliyun.com](https://bailian.console.aliyun.com/)  

开通模型服务，申请API密钥，配置密钥到webui，选中模型，保存配置运行即可。

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

#### Dify

官方仓库: [https://github.com/langgenius/dify](https://github.com/langgenius/dify)  

图文教程：[https://github.com/Ikaros-521/AI-Vtuber/pull/924](https://github.com/Ikaros-521/AI-Vtuber/pull/924)  


