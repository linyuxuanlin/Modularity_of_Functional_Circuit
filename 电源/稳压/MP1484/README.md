# 基本参数

* Input: 4.75V ~ 18V
* Output: 0.925V ~ 20V
* Current: 3A
* Efficiency: Up to 95%



# 输出电压调整

Rx = 10.81 x ( Vout - 0.925 ) (kΩ)

For example, for a 3.3V output voltage, R1 is 26.1kΩ.

Recommended resistance Rx values lists: 

| Vout | Rx     |
| ---- | ------ |
| 1.8V | 9.53kΩ |
| 2.5V | 16.9kΩ |
| 3.3V | 26.1kΩ |
| 5V   | 44.2kΩ |
| 12V  | 121kΩ  |

# 肖特基二极管选型

| 型号    | 电压/额定电流 | 供应商                  |
| ------- | ------------- | ----------------------- |
| B130    | 30V, 1A       | Diodes, Inc.            |
| SK13    | 30V, 1A       | Diodes, Inc.            |
| MBRS130 | 30V, 1A       | International Rectifier |

# PCB 布局

1. Keep the path of switching current short and
   minimize the loop area formed by Input cap,
   high-side MOSFET and low-side MOSFET
2. Bypass ceramic capacitors are suggested
   to be put close to the Vin Pin
3. Ensure all feedback connections are short
   and direct. Place the feedback resistors
   and compensation components as close to
   the chip as possible
4. Rout SW away from sensitive analog areas
   such as FB
5. Connect IN, SW, and especially GND
   respectively to a large copper area to cool
   the chip to improve thermal performance
   and long-term reliability

布局参考预览图请见数据手册。

