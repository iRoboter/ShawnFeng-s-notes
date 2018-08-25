VBS脚本也可以有退出码，这里展示如何使用和获取。

# 测试

1、创建待测试VBS脚本保存名为tested.vbs：

wscript.Quit  999

2、创建测试用的bat脚本test.bat：

cscript.exe   tested.vbs

echo %errorlevel% 

pause

3、将两个文件放在同一个目录下，执行test.bat即可看到控制台输出 999，这个数字就是来自VBS里的退出码999.

# 说明
* VBS不区分大小写
* wscript.Quit 代表本脚本文件执行完成退出code，不能改写任何拼写

# demo 源码
https://github.com/iRoboter/mynotes/tree/master/VBS%20exit%20code

# 参考
https://ss64.com/vb/quit.html