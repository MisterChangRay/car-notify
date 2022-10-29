# car-notify
汽车 挪车通知H5

这里是一个很简单的需求，有时候停车别人叫你来挪车。于是我搞了一张纸弄在挡风玻璃前面。但是那张纸经常到挡风玻璃
的缝隙里面， 导致真正需要挪车的时候找不到电话。

今天我看到车上面，静电贴贴在车玻璃上的车辆年检标志。我想我生成一个二维码不就OK了？ 贴再挡风玻璃上，别人想联系我
扫码就OK了啊。

于是就产生了此项目，项目很简单。大家可以直接下载使用：


# 快速使用

### 1. 下载发布的项目部署到nginx上面

下载并部署项目，然后生成一个二维码指向部署目录：

二维码链接指向项目，参数格式为：`https://xxx.xx?tel=13558810XXX,18380380XXX`  

连接中的手机号即为通知的手机号,多个使用英文逗号隔开。

### 2. 生成二维码并通过静电贴贴在挡风玻璃上：

<img alt="二维码贴图" src="https://github.com/MisterChangRay/car-notify/blob/main/example0.png" width="800" height="400">

### 3. 别人扫码进入链接显示如下图：

<img alt="打开首屏" src="https://github.com/MisterChangRay/car-notify/blob/main/example1.jpg" width="400" height="790">
<img alt="点击拨号" src="https://github.com/MisterChangRay/car-notify/blob/main/example2.jpg" width="400" height="790">


由于我在二维码后面贴上了NFC,所以也支持NFC。现在就比较nice了。
