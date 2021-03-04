# petfeed-redme
    This project is developed using Tuya SDK, which enables you to quickly develop branded apps connecting and controlling smart scenarios of many devices.For more information, please check Tuya Developer Website.<br>
宠物自动喂食器<br>
==
工作过程<br>
-------
        >>利用单片机、Wi-Fi通信板等设计一个宠物自动喂食器。<br>
        通过利用单片机(AT89S52)对各个模块进行控制，通过键盘设<br>
        定喂食时间，LCD(12864)显示定时时间。当达到这个时间时，<br>
        发光二极管发光，蜂鸣器发出声响，吸引宠物过来进食并自动<br>
        投放食物。此外，该喂食器还配有日历和温度传感器，方便记录宠物的生长周期。<br>
总体设计方案构思<br>
---------
        >>设计一个宠物自动喂食器，目标实现自动控制、正常显示时间、温<br>
        度测试和闹钟提示的功能，所以要细分到各个模块去实现。首先要准<br>
        备一个主控系统控制整个电路正常工作，可以利用单片机担任这个任<br>
        务，还要准备显示时间的模块电路，闹钟设置可以通过按键随意更改<br>
        ，电机控制门阀自动投放食物。电源电路给整个电路供电，喂食过程<br>
        中伴随照明灯的点亮。<br>
        >>因此，可以确定本系统的整体设计结构，包括：单片机系统、显示<br>
        电路、时钟电路、电源电路、电机控阀门、按键电路、温度测试、照明灯和闹钟提示。<br>
系统组成模块设计<br>
--------------
#单片机的设计<br>
        >>若使用AT89S52，其片内ROM是Flash ROM 能在3V的超低压下正常工作，<br>
        而且和MCS-51系列单片机也是兼容的，此芯片内部有8KB ROM的存储空间，<br>
        也有89C51的功能和在线编程可擦除技术，进行电路调试时，由于需要随时<br>
        对程序进行修改和新增一些程序的功能，因此选择AT89S52作为主控系统。<br>
#时钟显示电路的设计<br>
        >>若采用LCD液晶显示器显示，LCD液晶显示不但耗能少，而且能过够显示年<br>
        、月、日和星期等汉字，在显示方面更加灵活，当需要改变显示时，只要改<br>
        变软件设计就可以，不需要改变硬件电路的设计，而且电路的功能也容易扩展。<br>
        
