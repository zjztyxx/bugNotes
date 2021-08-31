# bugNotes


## Ubuntu使用

1. Error1  
*nautilus无法打开 终端可以正常显示文件*  
step1.清除安装路径下的三个文件夹  
step2.重启系统  
如果依旧不行，参考以下过程  
链接：https://askubuntu.com/questions/1087345/nautilus-symbol-lookup-error-usr-lib-x86-64-linux-gnu-tracker-2-0-libtracker/  
![](qt_1.png)  
)1 `wget https://sqlite.org/2018/sqlite-autoconf-3250200.tar.gz`  
)2 `tar -xvf sqlite-autoconf-35250200.tar.gz`    
)3 `cd sqlite-autoconf-3250200`  
)4 `./configure`  
)5 `make`  
)6 `sudo make install`  


## Qt开发过程  

 Error1  
*exec database not open*
检查是否已经创建了表 
___
Error2  
*ubuntu18.0.4 qt无法生成可执行文件*  
pro文件中加入如下几行代码  
`TEMPLATE = app`  
`QMAKE_LFLAGS = -no - pie`  
___  
  Error3  
*use of undeclared of ***报错  
函数所在的类，类所继承的父类，要在头文件中标注好  



