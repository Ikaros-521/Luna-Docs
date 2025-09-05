## 下载项目

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
    - [百度网盘 :octicons-link-16:](https://pan.baidu.com/s/1kHNwVOmWPISar2XLnzLpLQ?pwd=atb7)
    - [夸克网盘 :octicons-link-16:](https://pan.quark.cn/s/936dcae8aba0)
    - [迅雷云盘 :octicons-link-16:](https://pan.xunlei.com/s/VNitDF0Y3l-qwTpE0A5Rh4DaA1)
    

## 运行环境

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

使用uv安装 解决冲突。直接安装会版本冲突，需要注释冲突部分，手动安装，部分库向下兼容，版本参考`requirements_comment.txt`：[issue#868](https://github.com/Ikaros-521/AI-Vtuber/issues/868)  

依赖冲突问题参考仓库issue：[https://github.com/Ikaros-521/AI-Vtuber/issues/655](https://github.com/Ikaros-521/AI-Vtuber/issues/655)  

（听劝的已经下载整合包了）  

安装命令参考：  

##### pip

```shell
pip install requests
pip install -r requirements.txt
```

##### uv (解决冲突问题)

```
pip install uv requests

uv venv  # Create a virtual environment at `.venv`.

# On macOS and Linux.
source .venv/bin/activate

# On Windows.
.venv\Scripts\activate
```

然后使用以下命令安装依赖：

```
uv pip install -r requirements.txt --override overrides.txt

# 或使用

uv pip install -r pyproject.toml --override overrides.txt
```

!!! note

    部署视频教程 [哔哩哔哩 :octicons-link-16:](//www.bilibili.com/video/BV1fV4y1C77r)  

