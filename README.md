修改配置版，只保留 http/https 下载功能，体积缩小一半。

2020-12-15 克隆自：https://github.com/myfreeer/aria2-build-msys2

【Windows下编译方法】
1、下载 init-msys2.bat 

2、下载 busybox 和 mingw 编译器，置于 init-msys2.bat  同目录。
https://frippery.org/files/busybox/busybox.exe
http://repo.msys2.org/distrib/msys2-x86_64-latest.tar.xz

3、运行 init-msys2.bat，将自动执行下载解压编译，编译后的文件在“.\msys64\home\%username%\aria2\aria2\src\aria2.exe”

【其他说明】
默认编译64位，修改 init-msys2.bat 中的 set MSYSTEM=MINGW64 为 set MSYSTEM=MINGW32，删除 “.\msys64\home\%username%\” 文件夹，再次执行 init-msys2.bat 则编译32位。
编译时间大概为30-60分钟。
