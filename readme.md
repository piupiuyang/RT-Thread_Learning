# 

#作品名称：智能手表（原型机）

##作品简介

    基于国民技术的芯片-N32G457VEL7，RT-Thread实时操作系统，与LVGL8.3,开发的一款智能手表。可以通过WIFI模块ESP8266模块获取实时的时间，天气信息，通过MPU6050获取步数信息。

##硬件信息：

   1. 国民技术N32G45XVL-STB开发板

   2. AHT10温湿度传感器

   3. 加速度计MPU6050

##作品图片

<img title="" src="file:///C:/Users/piupiuY/AppData/Local/Temp/WeChat%20Files/c6895f19be9f5aec50b3db41492ba09.jpg" alt="c6895f19be9f5aec50b3db41492ba09.jpg" width="412">

##作品展示视频链接

    [RT- thread 夏令营 作品展示 基于 RT-thread 和LVGL8.3 的智能手表雏形_哔哩哔哩_bilibili](https://www.bilibili.com/video/BV1Ld4y1N7Tj?spm_id_from=333.337.search-card.all.click&vd_source=dcfacbf5268adf5c99b87c526fd7d375)

##RT-Thread使用情况

    ###线程：

                weather    每十分钟进行一次天气信息，实时时间的获取

                LVGL          负责屏幕的显示刷新

                agbtn        监测按键使用情况

####线程通信目前只应用了邮箱让weather线程向LVGL线程发送天气数据                                 

    ###软件包：

                    agile_button-latest    一款已经封装好按键各项功能的软件包

                    at_device_latest         用来进行ESP8266的初始化

                    cJSON-latest               用来解析通过get请求获得到的天气信息与实时时间

                    LVGL-v8.3.0                一个免费的开放源代码图形库

                    mpu6xxx-latest         用来接收mpu6050数据

                    webclient-latest           WebClient 软件包是 RT-Thread 自主研发的，基于 HTTP 协议的客户端的实现，它提供设备与 HTTP Server 的通讯的基本功能。

##硬件架构

![ca4b9a0831ec26b9086e70eb9f3d26f.jpg](C:\Users\piupiuY\AppData\Local\Temp\WeChat%20Files\ca4b9a0831ec26b9086e70eb9f3d26f.jpg)

##软件架构

![ebb5ad15b3aa775db0e3c991107668a.jpg](C:\Users\piupiuY\AppData\Local\Temp\WeChat%20Files\ebb5ad15b3aa775db0e3c991107668a.jpg)
