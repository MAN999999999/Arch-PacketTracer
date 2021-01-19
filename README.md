# 基于Arch Linux的Cisco,PacketTracer软件;
## 纪念一学期的大学生活;
一转眼一个学期完蛋了,想着下个学期好好干PT软件;  
***不料***,他妈的连课都没有了;

### GNU/Linux下软件运行状态;
[![pt.png](https://i.postimg.cc/tJfvr1Gk/pt.png)](https://postimg.cc/JHNQ0znH)

#### Arch Linux 直接安装方法;
```
已经打好了包,复制下面命令安装: {
pacman -Syy wget 
wget 'https://github.com/MAN999999999/Arch-PacketTracer/releases/download/V7.3.1/packettracer-7.3.1-3-x86_64.pkg.tar.zst'
pacman -U *.zst
}
```

#### Arch Linux 手动构建打包安装方法;
```
自行构建,需要耐心,和一些小小的折腾 {
0X00 安装依赖;
pacman -Syy base-devel fakeroot git
0X01 克隆PKGBUILD文件准备构建;
git clone https://github.com/MAN999999999/Arch-PacketTracer.git
0X02 进入目录,
makepkg -si    #安装速度取决于网络速度,最好使用代理;
###--------如何加快构建速度------#
首先下载好PacketTracer_731_amd64.deb
并且放置在packettracer目录中;
修改PKGBUILD第18行,替换为
'local://PacketTracer_731_amd64.deb'
然后在 makepkg -si
}
```

##### Debian系/Ubuntu 安装方法;
```
非常的简单,直接复制下面的命令: {
apt-get update && apt-get install wget
wget 'http://archive.org/download/packet-tracer-731-amd-64/PacketTracer_731_amd64.deb'
dpkg -i *deb
如果报错了,执行命令
apt-get install -f
}
```

# 最后来张***本人***
###### 老师的
# ***靓照*** 
西安某大学计算机网络专业***女神老师***;
[![1504564308.jpg](https://i.postimg.cc/66Hk23gy/1504564308.jpg)](https://postimg.cc/grZS1YYW)
