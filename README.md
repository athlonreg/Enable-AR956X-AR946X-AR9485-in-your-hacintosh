# How to install AR956x in Hacintosh
    
#问题描述：

	许多朋友在装上黑果后自己的 AR956x 无线网卡驱动不了，或者驱动之后速度非常慢，又或者经常掉驱动，这个问题就是驱动方法造成的；

这里我教给大家一种比较稳定的驱动方法。


#准备工作：
    
    首先下载这个项目我所提供的三个 kext 
    
![2017-09-10-01](http://ovefvi4g3.bkt.clouddn.com/2017-09-10-01-1.png)


#具体方法如下：
    
    将下载的三个 kext 拷贝到 /EFI/CLOVER/kexts/Other 

    接着进入到 /System/Library/Extensions 目录，删除IO80211开头的所有文件

![2017-09-10-02](http://ovefvi4g3.bkt.clouddn.com/2017-09-10-02-1.png)

![2017-09-10-03](http://ovefvi4g3.bkt.clouddn.com/2017-09-10-03-1.png)

    然后打开 Kext Utility 输入密码等待重建缓存、修复权限完成就可以了，重启之后就会发现网卡已经驱动了，而且很稳定，只是每
    
    次升级系统都要进 SLE 删掉那两个文件重建缓存、修复权限。
    
    下面是笔者的一个成功后的截图：
    
![2017-09-10-04](http://ovefvi4g3.bkt.clouddn.com/2017-09-10-04-1.png)

#完工

#如果你喜欢我的帖子，可以酌情打赏哦

![reward](http://ovefvi4g3.bkt.clouddn.com/reward-1.jpg)




