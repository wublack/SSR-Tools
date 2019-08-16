<!--
 * @Author: Wu
 * @Date: 2019-08-16 14:19:27
 * @LastEditors: Wu
 * @LastEditTime: 2019-08-16 15:24:23
 * @Description: 
 -->
## 因为最近在玩绝地求生，但是要加速器，游戏98，以后加速器每月都得还贷一样每个月要30块，决定自己弄一个加速器，我的steam账号是erhuabushuo0820400，有兴趣一起玩的加我，我很菜，哈哈！
## 第一步
### 搭建ssr翻墙梯子 （我使用的是谷歌云的免费服务器debian 9）
我以前写[教程参考链接](https://note.youdao.com/ynoteshare1/index.html?id=fad0d10e7f7973a91b15bbb29bbdc9fd&type=note)

## 第二步
### 在搭好的梯子上安装[udpspeeder](https://github.com/wangyu-/UDPspeeder/blob/branch_libev/README.md)
== 以下代码能复制粘贴就不要装逼敲 ==

1、安装必要工具
```
yum install -y wget vim
```

2、下载udpspeeder
```
wget https://github.com/yobabyshark/onekeyopenvpn/raw/master/speederv2
```

授权
```
chmod +x speederv2
```

3、开启udpspeeder
```
nohup ./speederv2 -s -l0.0.0.0:9090 -r127.0.0.1:5656 -f2:4 --mode 0 --timeout 0 >speeder.log 2>&1 &
```
== 5656为你搭建ssr的端口号，记得修改 9090是udpspeeder转发端口 ==

4、打开9090防火墙端口

如何打开端口在搭建ssr教程里有，不赘述！

## 第三步
下载我提供的[ssr+sstap.zip](https://github.com/wublack/SSR-Tools/raw/master/ssr%2Bsstap.zip)文件，解压打开start.bat文件，修改成你服务器的IP，端口设置成ssr梯子端口，保存双击运行就好了，记得关掉杀毒软件。

## 第四步
1、添加ssr节点，服务器ip设置成：127.0.0.1
2、端口号设置成start.bat的设置的转发端口2090
3、设置代理端口：右键右下角小飞机 -> 选项设置 ->本地代理下的本地端口设置成1090 
4、加密混淆协议跟搭建ssr设置的一样
保存就好了

## 第五步
安装SSTAP 打开SSTAP
点击代理右边有个加号 -> 添加一个SOCKS5代理 -> 服务器IP设置成：127.0.0.1 -> 端口设置成1090 -> 附加路由设置成你ssr服务器IP -> 保存就ok了

## 最后
点击代理选择框右侧的闪电图标测试。1ms延迟！
!(image)(https://www.atrandys.com/wp-content/uploads/2018/09/sstappeizhi3.png)

