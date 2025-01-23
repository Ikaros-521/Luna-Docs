## API

API接口地址根据配置文件中webui的ip端口地址决定，默认：`http://127.0.0.1:8081`  
API在线文档：[https://apifox.com/apidoc/shared-3b2abc65-37f3-4812-a604-ffc35c8ec3ec](https://apifox.com/apidoc/shared-3b2abc65-37f3-4812-a604-ffc35c8ec3ec)  

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
| message    | string  | 响应消息，描述请求的处理结果 |

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
| message    | string  | 响应消息，描述请求的处理结果 |

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
| message    | string  | 响应消息，描述请求的处理结果 |


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
| message    | string  | 响应消息，描述请求的处理结果 |
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
| message    | string  | 响应消息，描述请求的处理结果 |
| data   | object  | 数据内容，含传参外还有一个result键值，里面就有合成情况内容，和最后合成后文件存储路径，配合本地路径映射到URL路径，即可实现跨网段文件下载（json）。例如：{"result":{"code":200,"message":"合成成功","audio_path":"E:\\GitHub_pro\\AI-Vtuber\\out\\gpt_sovits_4.wav"},其他键值对忽略} |
