# **AutoFlyB**
~~用于刷取飞行者联盟论坛的工具chinaflier~~
## 1.使用
基于Python开发，确保应当安装有高于Python 3.7的Python环境，涉及的库：

```language CMD
pip install selenium
```
为了使程序使用，需要手动下载与当前浏览器版本相同的driver，该程序使用的是Microsoft Edge的edgedriver
[](https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/?form=MA13LH)
在Edge设置中>关于 中找到相对应的版本号并将下载好的edgedriver.exe解压到运行目录

运行 main.py，首次运行请配置 config.ini
> url = 需要回复的链接，禁止使用他人
> text = 回复的内容
> cookie = 留空，首次运行程序后会自动补充

输入回复的次数和是否限流，请关闭与Microsoft Edge的一切有关进程
##  2.原理
通过控制浏览器进行输入并计时执行，通过首次登录获取用户Cookie方便后续登录，后续浏览器更新应当重新手动下载新的edgedriver，该程序遵循MIT开源协议，频繁使用可能导致论坛封禁IP。
