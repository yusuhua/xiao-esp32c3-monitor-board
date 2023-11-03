# xiao-esp32c3-monitor-board
这是一块空气监测报警器，基于[Seeed Studio的XIAO-ESP32C3](https://www.seeedstudio.com/Seeed-XIAO-ESP32C3-p-5431.html)，主要功能主要有：
- 温湿度监测与报警
- CO浓度监测与报警
- WIFI天气时钟等

其可支持的功能并不限于以上几个，更多、更好玩的功能等你来开发！！！

<p align="center">
  <img src="https://github.com/yusuhua/xiao-esp32c3-monitor-board/blob/main/image/monitor.jpg" alt="Monitor display photo"/>
</p>

## 引脚图
XIAO Esp32C3的引脚图如图所示：

<p align="center">
  <img src="https://github.com/yusuhua/xiao-esp32c3-monitor-board/blob/main/image/pinout.png" alt="Esp32C3 pinout photo"/>
</p>

注意：板子上的Esp32C3模块的Type-C口是朝下的，确定每个引脚的功能时请将上图旋转180度后查看。

具体引脚功能如下：
| 按键           | 引脚   |
| :--------------| :---- |
| OLED_SCK_PIN   | 7     |
| OLED_SDA_PIN   | 6     |
| DHT11_PIN      | 20    |
| MQ7_PIN        | 2     |
| SW1_SELECT_PIN | 9     |
| SW1_NEXT_PIN   | 10    |
| SW1_PREV_PIN   | 5     |
| SW1_UP_PIN     | 21    |
| SW1_DOWN_PIN   | 4     |
| SW2_PIN        | 8     |
| BUZZER_PIN     | 3     |

## 元器件说明
- R1~R3为0805的1K贴片电阻
- DHT11为普通的DHT11传感器，注意焊接时将引脚折弯
- 0.96 OLED最好使用白色款，如果不喜欢白色建议用蓝色
- RF1天线座为斜插式的，具体看上边的成品图
- LED1为3mm 1.8V~2.0V的发光二极管
- SW1为五向多功能开关
- SW2为四脚贴片式轻触开关
- U1为弯角1x4P的排母
- Q1为S8050时，BUZZER1为有源蜂鸣器；Q1为S8550时，BUZZER1为无源蜂鸣器
- LED1下方的挖槽为天线连接线的出入孔
- ESP32C3下侧的挖槽为锂电池引出孔
- RF2可以焊接IPEX 1代天线座子，然后使用双头IPEX 1代连接线连接ESP32C3；也可以不焊接，使用单头IPEX 1代连接线，无头的一侧直接焊在RF1天线座的中心引脚上
