
各IC10プログラムの仕様とかメモ書き

# Pressure Controller v0.0.0
## Device ports

| port | alias      | description |
| ---- | ---------- | ----------- |
| d0   | Target     | A device to be turned on/off. If device is Logic Memory, it's Setting value using as NameHash. |
| d1   | Sensor     | A Sensor (Gas Sensor or etc.) in target room. |
| d2   | Dial       | A Dial (or Logic Memory, etc. setting device) to set threshold value (kPa). |
| d3   | CurrentDsp | (Optional) A display to show current pressure. |
| d4   | SettingDsp | (Optional) A display to show setting pressure. |
| d5   | Operation  |  |

Operation

| value | description |
| ----- | ----------- |
| 0     | pressure > setting -> ON, pressure < setting -> OFF |
| 1     | pressure > setting -> OFF, pressure < setting -> ON |
