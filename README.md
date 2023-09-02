![main](https://i.imgur.com/roX0N3C.png)

## 注意事项:
- 请确保您没有运行任何游戏内插件 (Blitz, Mobalytics, etc.).
- 英雄联盟客户端和游戏内（League & client）必须为中文。
- 请将游戏窗口设置为比例 16:9 的无边框模式, 并且游戏必须运行在主显示器上（请使用 1920x1080 的分辨率来获取最佳效果）。
- 如果程序发生崩溃，可以在 Github 上创建一个问题（issue） 来反馈错误（error）。

## 安装:
1. 请从 https://www.python.org/downloads/windows/ 下载并安装 Python 3.11.4 版本。
   - 注意：Windows 7 或更早版本上无法运行 Python 3.11.4。
2. 请从 https://github.com/jfd02/TFT-OCR-BOT/archive/refs/heads/main.zip 下载（Download）或者克隆（Clone）代码库（Repository）
3. 请从 https://github.com/UB-Mannheim/tesseract/wikiInstall 下载并安装 tesseract 5.3.1.20230401 版本。 
   - 请留意 tesseract 的安装路径。
   - 请在 settings.py 文件中设置 Tesseract tessdata 文件夹路径（可能已经是正确的）。
4. 请从 https://github.com/simonflueckiger/tesserocr-windows_build/releases 下载 tesserocr v2.6.0 版本到文件夹（cwd）。
   - tesserocr 的版本必须是 2.6.0，用来适配 tesseract 5.3.1。
   - 根据已安装的 Python 版本来选择 3.10 或 3.11 版本的安装文件。
   - 文件名只能是 tesserocr-2.6.0-cp311-cp311-win_amd64.whl 或其对应的 cp310 版本。
5. 运行 install.py 文件。
6. 请在 settings.py 文件中设置正确的英雄联盟客户端（league client）路径。
7. 关闭所有游戏内插件。
8. 运行 main.py 文件。

## 功能:
![main](https://i.imgur.com/1bXOmag.png)
- 读取棋盘信息（回合/等级/金币/商店/装备）
- 监测棋盘/备战席奕子信息（名称/等级）
- 选秀回合随机选择奕子/装备
- 野怪回合之后捡取掉落的法球
- 给奕子们穿戴正确的装备（散件/成装）
- 自定义阵容
- 自动接受对局

## 待实现:
- 关于纹章之书的功能
- 改进金币花费功能 
- 改进自动接受对局功能来使其有更多的失败措施
- 从网站上获取最强大（毒瘤）的阵容
- 选秀回合根据阵容智能选择奕子或装备
- 优化捡取法球功能（根据法球坐标来捡取）
