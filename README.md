# WearOSApps
 Wear OS Apps Collections 
 提取自Ticwatch（国际版ROM）以及部分China版ROM中
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
   ` adb pull /data/XXXXXXXX/***.apk .
