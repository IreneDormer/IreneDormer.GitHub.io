win10+hugo+github搭建博客纯操作（无图无错误解析）

一、安装hugo

1. https://github.com/gohugoio/hugo/releases中下载对应版本.zip
2. 解压，将其中的.exe文件重命名为hugo.exe 并保存至`D:\Hugo\bin` 文件夹中。
3. 使用 `D:\Hugo\bin>set PATH=%PATH%;D:\Hugo\bin` 或在系统属性-高级-环境变量-path变量中手动添加，把 hugo.exe 可执行文件添加到你的 PATH路径中。

完成检查：运行几个命令来验证可执行命令可以运行，然后构建一个示例网站作为起点。

1. 打开一个命令提示符窗口，输入 

   ```
   hugo help
   ```

    并按下 Enter 键。你看到的输出应该以下面的文字开始：

   ```
   A Fast and Flexible Static Site Generator built with love by spf13 and friends in Go. Complete documentation is available at http://gohugo.io
   ```

试创建网站：

1. 在命令提示符中，跳转当前目录到sites文件夹。

   ```
   C:\Program Files> cd D:\Hugo\Sites
   C:\Program Files> D:
   D:\Hugo\Sites>
   ```

2. 运行命令来生成一个新的网站。我使用 `example.com` 作为网站的名字。

   ```
   D:\Hugo\Sites> hugo new site example.com
   ```

你现在应该拥有一个叫做 D:\Hugo\Sites\example.com 的文件夹。进入这个文件夹，并列出文件夹中的内容。你应该得到类似下面的输出内容：

```
D:\Hugo\Sites>cd example.com
D:\Hugo\Sites\example.com>dir
 Directory of D:\hugo\sites\example.com
 ......
```

二、设置github

