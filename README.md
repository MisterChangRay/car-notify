# car-notify
汽车 挪车通知H5

这里是一个很简单的需求，停车时车上需要有联系方式方便别人叫你挪车。之前我搞了一张纸板写上电话号码直接放在在挡风玻璃前面（其实就是买汽车用品商家送的）。
但是有个问题是，那张纸经常会卡到前挡风玻璃最前面的缝隙里面， 导致电话号码被挡住，经常需要手动摆正。

偶然间我看到车前挡风玻璃上面的车辆年检标志。突然想到做一个H5,然后生成一个链接二维码贴上面，别人想联系我扫码就OK了啊。

说做就做，项目很简单。大家可以直接下载使用：


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


我在二维码后面贴上了NFC标签贴,所以也支持NFC贴一贴就拨打电话。现在应该不会联系不到我了吧，哈哈哈。
