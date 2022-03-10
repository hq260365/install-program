# n1-install-program
Install to emmc script for phicomm n1, which will help you to copy openwrt system to emmc.  
Execute `n1-install` in terminal to run this program!
注意：
一键安装到emmc脚本已迁移至openwrt package，解决需要自选依赖的问题。使用方法如下，悉知！！

用法：

0、如果使用官方或其他源码，可能会缺少parted这个包，执行下面的命令从Lean的仓库中checkout
      svn co https://github.com/coolsnowwolf/packages/tree/master/utils/parted package/parted
1、git clone https://github.com/tuanqing/install-program package/install-program
2、执行 make menuconfig ，选中Utilities下的install-program

Utilities  --->  
   <*> install-program
3、编译完成之后使用本源码制作镜像写入U盘启动，之后执行 n1-install 即可安装到emmc
