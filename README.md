# car-notify
汽车 挪车h5

这里是一个很简单的需求，有时候停车别人叫你来挪车。于是我搞了一张纸弄在挡风玻璃前面。但是那张纸经常到挡风玻璃
的缝隙里面， 导致真正需要挪车的时候找不到电话。

今天我看到车上面，静电贴贴在车玻璃上的车辆年检标志。我想我生成一个二维码不就OK了？ 贴再挡风玻璃上，别人想联系我
扫码就OK了啊。

于是就产生了此项目，项目很简单。大家可以直接下载使用：


# 快速使用

使用这个是很简单的，下载发布的项目部署到nginx上面，然后生成一个二维码指向部署目录：
二维码链接格式为：`https://xxx.xx/car/index?tel=13558810XXX,18380380XXX`  这个格式生成后贴再挡风玻璃即可。

别人扫码进入链接显示如下图：
![打开首屏](https://github.com/MisterChangRay/car-notify/blob/main/example1.jpg)
![点击拨号](https://github.com/MisterChangRay/car-notify/blob/main/example2.jpg)
