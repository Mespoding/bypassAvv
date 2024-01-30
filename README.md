## BypassAV

**仅用于技术交流，请勿用于非法用途。**

该插件没有什么技术含量，本质上利用的ps2exe.ps1脚本编译为exe，只是不想在命令行里操作，将其写为cna脚本，方便直接快速生成免杀的可执行文件。且只有50KB，目前仅支持exe文件格式。

*注：建议在powershell 4.0版本以上机器运行，可向下兼容powershell 2.0。*

(师傅们别传VT了，没姿势了。呜呜呜~)

## 更新日志2023/2/27

- 使用一定的加密方式进行静态免杀
- 随机命名key值

## 更新日志2022/7/27

- 生成的```c:\windows\temp\payload_tmp.ps1```作为临时文件
- debug 参数，生成cs文件，可自行编译
- 随机命名可执行文件

## 更新日志2022/3/30

- 自定义输出地址
- 提供ico图标bypass


修改了部分代码，再重新写份使用说明。

在导入cna脚本之前，只需要修改当前路径$path所在的真实路径即可。


![image-20220324174004915](images/image-20220324174004915.png)

首先选择Cobalt Strike生成后门文件，为bin格式。

![image-20210711183204262](images/image-20210711183204262.png)

选择刚才生成的bin文件、ico图标，以及powershell的版本，点击即可生成exe可执行文件

![image-20220421152337126](images/Snipaste_2023-02-28_09-10-40.jpg)

使用powershell 4.0上线server 2012

![image-20210711183628292](images/image-20210711183628292.png)

使用powershell 2.0上线server 2008

![image-20210711183645879](images/image-20210711183645879.png)

如果在webshell触发该可执行文件，需要start命令

![image-20210713120053228](images/image-20210713120053228.png)


## 参考文章

https://www.jianshu.com/p/fb078a99e0d8

https://www.jianshu.com/p/f158a9d6bdcf
