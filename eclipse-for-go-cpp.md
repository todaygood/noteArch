1. Eclipse中配置CDT 

安装MinGW

For windows, MinGW and Cygwin are the two main platform choices for acquiring the GNU toolchain. It is important to understand the difference between them. Cygwin produces executables that use the Cygwin POSIX runtime. Note that this runtime is GPL licensed. MinGW produces native Windows executables that do not require a separate runtime.

•For MinGW, it is recommended to use the MinGW installer, mingw-get, to manage your MinGW installation. Download and run the lateset mingw-get-inst package from the MinGW Downloads page. The CDT MinGW toolchain will find this install if it is located in the default C:\MinGW directory, the MinGW bin directory is placed in your path, or if the MinGW location is stored in the MINGW_HOME environment variable.

 
 


https://blog.csdn.net/weixin_32534653/article/details/114184567


gcc on windows 使用mingw , 安装包：http://mingw-w64.org/doku.php/download
不要使用TDM-GCC ，他带的gdb运行失败。


 运行可执行.exe程序

右键单击Release目录下面的.exe文件，选择“Run As”→“Local C/C++ Application”即可运行程序了。如需要debug程序，只需在Eclipse的Debug视图下面单击工具栏中的debug图标即可自动执行Debug目录下的.exe文件。


Binaries：存放所有编译后的二进制文件，这里主要是用于Debug, Release的二进制文件，而且Binaries目录只能在Eclipse中才能看到，从电脑磁盘上面是直接看不到的。

Debug：里面包含两个文件（.exe与.o）。这里.exe文件是可以直接执行的文件，因为在Debug目录里面，表明它只用于debug；而.o文件则是一个object文件，即目标文件，编译器产生的，对源代码的“直译”，未经过连接等操作的目标代码。（注意：代码编译后生成目标文件(即.o文件)，目标文件经过连接后才能变成.exe文件）。

Release：也包含两个文件（.exe与.o）。这里.exe文件是可以直接执行的文件，因为在Release目录里面，表明它只用于发布运行；.o文件则也是一个object文件，原理同Debug里面的.o文件。

https://blog.csdn.net/faihung/article/details/73496959?utm_medium=distribute.pc_relevant_bbs_down.none-task-blog-baidujs-2.nonecase&depth_1-utm_source=distribute.pc_relevant_bbs_down.none-task-blog-baidujs-2.nonecase



2. Eclipse中配置Go

https://blog.csdn.net/dgh_84/article/details/54973974

https://cookcode.blog.csdn.net/article/details/80144814?utm_medium=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.control


GoClipse使用文档  https://github.com/GoClipse/goclipse/blob/latest/documentation/UserGuide.md


Windows note: Using Cygwin GDB doesn't work very well, if at all. The recommended way to debug in Windows is to use the GDB of mingw-w64, or the one of TDM-GCC.


421125198111232719



 白沙洲地区当前存在土地、基础设施配套、产业发展、城市形象等多方面问题。土地方面，因存量土地打包问题突出，白沙洲地区整体规划打造的难度极大；从行政区划上看，大白沙洲片分属武昌区白沙洲街、洪山区张家湾街各自管辖，两区在城市发展理念和功能定位上存在较大差别，给区域整体打造和配套设施提升带来难度。人口及基础配套设施问题，一是现状住宅空置率高，低收入人口占比高；二是公共配套设施严重不足，居民诉求极为强烈；三是道路建设滞后，高峰拥堵严重；四是市政设施老旧，城市内涝严重。产业发展方面，坐拥长江主轴绝佳区位，却沦为产业功能、创新发展、土地价值的多重洼地。城市形象问题，一是公园及开放空间体系破碎，绿化覆盖率低；二是建筑空间形象，缺乏亮点空间。以上迫切需要解决的问题，对加快推进白沙洲地区规划建设提出了现实要求。
 
 
 http://zrzyhgh.wuhan.gov.cn/zwgk_18/fdzdgk/jytabl/sjjyta/202010/t20201030_1487209.shtml
 
 
 