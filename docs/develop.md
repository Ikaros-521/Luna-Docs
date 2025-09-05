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



