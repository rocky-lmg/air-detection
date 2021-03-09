This project is developed using Tuya SDK, which enables you to quickly develop branded apps connecting and controlling smart scenarios of many devices.
For more information, please check Tuya Developer Website.  
一、方案标题  
    智能宠物喂食器
二、方案应用场景  
    地点：拥有爱宠的室内家庭、宠物医院、宠物饲养场所等 
    功能：随着人们生活水平的提高，饲养宠物的人越来越多，但由于平时工作、学习、生活繁忙等，饲养者因为其他事情忘记投喂，出现宠物无法及时喂食等问题，特别是在外出游玩期间，家中宠物的喂食问题更是困扰很多家庭。设计一款智能宠物喂食器，通过按键结合手机终端 APP 控制以及语音提示等方式给宠物进行定时、定量自动喂食，保证宠物能够按时进食，解决了饲养宠物家庭的后顾之忧。通过按键设置喂食时间、餐数、喂食量等信息，实现在无人的状况下自动喂食。用户也可以通过手机 APP 与 WiFi 模块连接，及时跟踪喂食投放情况，也可以远程控制喂食器工作，实现自动喂食及远程监控的目的。
    系统结构设计：
    智能宠物喂食器以STM32单片机作为控制核心，由 OLED 显示模块、用户设置按键模块、音频录放模块、WiFi模块、1302时钟电路、喂料直流电机控制模块组成。电源板和直流电机控制使用涂鸦智能提供三明治套件的H桥直流电机驱动板、直流供电电源板。
    （1）采用0.96 寸带字库OLED显示模块，OLED显示一些宠物喂食相关信息，作为主要人机交互界面，可以更加直观、科学的进行宠物喂食；
    （2）音频录放模块由语音芯片电路及音频输入、输出电路组成，用户可以预先为自己的爱宠录制一段或多段喂食提示语音，在宠物喂食时进行播放，提示自己的爱宠进食；
    （3）控制器通过读取 DS1302 所提供的时间作为用餐基准，用户能够通过按键模块对宠物喂食的餐数、各餐喂食时间、喂食量等信息以及录音的启动及停止等参数进行设置，使控制器能控制喂料电机定时、定
     餐、定量的执行喂食行为，并结合语音提示宠物进行进食；
    （4）WiFi模块使用涂鸦的WIFI通信模块，用于连接STM32和涂鸦IOT云平台。宠物当前的喂食状态信息能通过 WiFi 模块反馈给远程的用户，用户通过手机 APP 可实时监测喂食器工作状态，当用户工作上班或者外出忘      记设置宠物喂食信息的情况下，用户也可以通过 APP远程发送喂食设置信息，启动喂食器工作，不让自己的爱宠饿肚子。
    技术难点：
        智能宠物喂食器应定量出料的喂食器功能，其出料料斗必须具备精准控制出料量、不卡料的能力，否则就会出现宠物进食量不足或者进食过多的情况发生。
三、开发计划      
    3月25前完成.   
    1）2月28前准备物料  
    2）3月1-20日嵌入式开发、云开发  
    3）3月15日前整体调试。  
     
