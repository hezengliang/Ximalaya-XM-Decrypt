<h1 align="center">喜马拉雅xm文件解密工具</h1>
<h4 align="center">Ximalaya-XM-Decrypt</h4>

### 说明

由于喜马拉雅官方客户端下载的音频文件为加密格式，无法在普通播放器中播放，所以我写了这个小工具来解密喜马拉雅下载的音频文件。本工具参考@aynakeya的[博文](https://www.aynakeya.com/2023/03/15/ctf/xi-ma-la-ya-xm-wen-jian-jie-mi-ni-xiang-fen-xi/)，并加入了批量解密的功能。我还写了一个程序[Ximalaya-Downloader](https://github.com/Diaoxiaozhang/Ximalaya-Downloader)，用于直接爬取未加密的喜马拉雅音频文件。本工具作为Ximalaya-Downloader的补充，当每日下载vip音频达到上限时，可以使用客户端下载加密的xm文件并使用本工具解密。

在使用该软件时，请确保xm_encryptor.wasm文件与主程序文件处在同一目录下，最好是一个单独的文件夹。


### 使用方法
python 3.8 环境实测可以使用。  
1. 创建 python 虚拟环境
```bash
python -m venv env_xmdec
source env_xmdec/bin/activate
```
2. 安装必要的库
```bash
pip install -r requirements.txt
```
4. 运行程序
```bash
python main.py
```
