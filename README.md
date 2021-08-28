# WearOSApps
 Wear OS Apps Collections 
 提取自Ticwatch（国际版ROM）以及部分China版ROM中,除google系列APP外对其他组件无依赖
 理论上都支持Wear OS的手表
 ## APP 列表
 目前的APP
 ```
 .
|-- Communication
|   `-- qqlite_2.1.3.apk
|-- Entertainment
|   `-- netease_cloudmusic_2.9.10.apk
|-- LICENSE
|-- README.md
|-- Tools
|   |-- alipayGphone_10.3.1.1909061.apk
|   |-- gms_21.31.12.apk
|   |-- google_fitness_2.13.32-230.apk
|   `-- todoist_v8433.apk
`-- WatchFaces
    |-- ustwo.watchfaces.moods_1.17.0.apk
    |-- ustwo_watchfaces_basic_2.0.0.apk
    |-- ustwo_watchfaces_hero_1.17.0.apk
    |-- vlad1m1r_watchface_2.8.0.apk
    `-- wear-normal-release_v6.1.4-pre.apk
```
 
 ## App 安装方法
 1. 开启手表的调试功能。
    *Devrloper options->ADB debugging*
 2. 连接手表 WIFI OR 数据线 OR 蓝牙，确认连接OK

    `adb devices`
 3. 安装APP
    
    `adb install APP_NAME.apk

 ## App 提取方法
 1. 开启手表的调试功能。
    *Devrloper options->ADB debugging*
 2. 连接手表 WIFI OR 数据线 OR 蓝牙，确认连接OK

    `adb devices`
    
 3. 查看已经安装的App列表
 
    `adb shell pm list packages`
    
 4. 查看app的信息,包括版本路径
 
    `adb shell dumpsys package [PACKAGE_NAME]`
    `adb shell pm path package [PACKAGE_NAME]`
    
 5. 保存apk到本地
   ` adb pull /data/XXXXXXXX/***.apk .`
   

   
