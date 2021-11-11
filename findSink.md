非常简单的寻找sink的小工具,不限语言,基于关键字正则匹配
初衷:每次grep搜索关键字好麻烦,写成这种小工具代码审计的时候快捷方便多了
适用于:Mac/Linux
Windows需要单独安装grep
默认保存文件:sinkValue.txt,可自定义
Usage of ./findSink_mac:
  -ext string
    	特定后缀查询 ext=*为查询所有后缀 (default "*.java")
  -f string
    	-f sinkFile (default "sink.txt")
  -o string
    	输入你要保存的文件格式 (default "sinkValue.txt")
  -path string
    	必填项:输入你的项目工程路径
常规使用:
sink.txt中输入你的关键字payload,如java常用执行命令函数exec(,command(,outputstream(等
关键字默认不区分大小写,多个关键字存放在sink.txt中
1.png
使用:
2.png
运行程序,自动把sink,按照你-o设置的文件保存
3.png
