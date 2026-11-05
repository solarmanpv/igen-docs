---
title: 外观介绍
description: MR1-D5 系列电表的外观、接口定义、指示灯与按键说明
---

# 外观介绍

## MR1-D5-W、MR1-D5-WR 外观和接口定义

<div style={{display:'flex', gap:'40px', alignItems:'flex-start', flexWrap:'wrap', margin:'12px 0'}}>
  <img src={require('./img/mr1-appearance.png').default} width="155" alt="MR1-D5-W 外观" />
  <img src={require('./img/mr1-appearance-w.png').default} width="150" alt="MR1-D5-WR 外观" />
</div>

| 接口 | 名称 | 说明 |
| --- | --- | --- |
| ![零线接口](img/interface-mr1-terminal.png) | N | 零线接口，电表供电输入，零线接口 |
| ![火线接口](img/interface-mr1-terminal.png) | L | 火线接口，电表供电输入，火线接口 |
| ![CT 端口](img/interface-mr1-ct.png) | CT | CT 端口，CT 电流采集端口 |

## MR3-D5-W、MR3-D5-WR 外观和接口定义

<div style={{display:'flex', gap:'40px', alignItems:'flex-start', flexWrap:'wrap', margin:'12px 0'}}>
  <img src={require('./img/mr3-appearance.png').default} width="135" alt="MR3-D5-W 外观" />
  <img src={require('./img/mr3-appearance-w.png').default} width="170" alt="MR3-D5-WR 外观" />
</div>

| 接口 | 名称 | 说明 |
| --- | --- | --- |
| ![零线接口](img/interface-mr3-terminal.png) | N | 零线接口，电表供电输入，零线接口 |
| ![A相火线接口](img/interface-mr3-terminal.png) | L1 | A 相火线接口，电表供电输入，火线接口 |
| ![B相火线接口](img/interface-mr3-terminal.png) | L2 | B 相火线接口，电表供电输入，火线接口 |
| ![C相火线接口](img/interface-mr3-terminal.png) | L3 | C 相火线接口，电表供电输入，火线接口 |
| ![CT 端口](img/interface-mr3-ct.png) | CT | CT 端口，CT 电流采集端口 |

## MR1-D5-WR、MR3-D5-WR 指示灯说明

| 指示灯标识 | 指示灯含义 | 状态说明 |
| --- | --- | --- |
| ![电源指示灯](img/indicator-power.png) | 电源（红色） | 灯常亮：电源指示灯，电表供电正常。<br/>灯不亮：电表未供电或异常。 |
| ![网络指示灯](img/indicator-wifi.png) | 网络（WiFi）（绿色） | 灯常亮：设备连上云平台。<br/>1s 间隔闪烁：设备连上路由或获取到 IP。<br/>100ms 间隔快闪：设备升级状态。<br/>灯灭：设备未连接到路由或未获取 IP。 |
| ![LoRa 指示灯](img/indicator-rf.png) | LoRa（绿色） | 灯常亮：LoRa 连接成功。<br/>灯灭：LoRa 未连接。 |

## MR1-D5-W、MR3-D5-W 指示灯说明

| 指示灯标识 | 指示灯含义 | 状态说明 |
| --- | --- | --- |
| ![电源指示灯](img/indicator-power.png) | 电源（红色） | 灯常亮：电源指示灯，电表供电正常。<br/>灯不亮：电表未供电或异常。 |
| ![网络指示灯](img/indicator-wifi.png) | 网络（WiFi）（绿色） | 灯常亮：设备连上云平台。<br/>1s 间隔闪烁：设备连上路由或获取到 IP。<br/>100ms 间隔快闪：设备升级状态。<br/>灯灭：设备未连接到路由或未获取 IP。 |

## 按键说明

| 按键标识 | 按键含义 | 功能说明 |
| --- | --- | --- |
| ![RESET 按键](img/reset-button.png) | RESET | 长按 10 秒可恢复出厂设置。<br/>所有灯常亮 2s 恢复正常状态。 |
