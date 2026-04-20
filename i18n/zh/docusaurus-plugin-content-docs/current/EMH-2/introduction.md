---
title: 产品概述
description: todo
---

# 产品概述

## 1. 型号说明

本文主要涉及产品具体型号：EMH-2-RG、EMH-2-R

**产品具体型号说明**

<img src={require("./img/model.png").default} width="240" /> 

| 序号 | 含义     | 取值                                    |
| ---- | -------- | --------------------------------------- |
| ⑴    | 产品标识 | EMH：家庭能源管理中心                   |
| ⑵    | 产品代际 | 2：第2代产品                            |
| ⑶    | 通信方式 | R：支持LoRa通信<br / >G：支持4G通信 |
 
## 2. 应用场景

EMH-2是一款专为家庭能源管理场景设计的智能设备，旨在通过实时监控、分析和优化家庭能源消耗，帮助用户有效降低能源成本、节省电费，并提升家庭能源使用的智能化水平。该设备支持多种接口，能够无缝接入逆变器、电池、充电桩、SG Ready热泵、P1电表等多种设备，实现光伏发电、储能、充电和用电设备的集中控制与优化管理。
 
**适用场景**

适用欧洲户用能源管理，解决户用场景下能源管理和经济用能的问题

## 3. 产品优势

**核心价值**
- 降本：合理使用光伏、储能和电网电力，最优经济用能
- 增收：可结合电费进行合理的电能规划，实现峰谷套利
- 增效：支持本地或远程监控、管理家庭能源系统，提升运维效率
- 体验：可视化UI界面，能量数据可以直观展示、查看
 
**产品特性**
- 支持接入逆变器、电池、充电桩、热泵等多种新能源设备
- 支持光、储、充、用设备的接入与场景联动
- 支持4G、WiFi、以太网等多种通信方式上传数据至云平台，方便用户进行远程监控和管理
- 内嵌本地化管理界面，用户可以本地查看发电、储能、用电情况
- 支持多种能源策略，帮助用户优化用电模式，降低电费支出，提升能源使用效率
- 符合EN18031物联网网络安全标准

## 4. 产品结构

EMH-2尺寸（单位：mm，尺寸精度 ±2%）

<img src={require("./img/size.png").default} width="480" /> 

## 5. 外观介绍

<img src={require("./img/appearance.png").default} width="480" /> 

### 外观与接口

| 序号 | 接口                | 说明                                                                                                          |
| ---- | ------------------- | ------------------------------------------------------------------------------------------------------------- |
| 1    | WAN 接口            | RJ45 网口（带指示灯）。                                                                                       |
| 2    | LAN 接口            | RJ45 网口（带指示灯）。                                                                                       |
| 3    | 3 位拨码接口        | 对应 3 路 RS485 接口的 120Ω 端接电阻配置：<br />- 拨至 ON：启用 120Ω 端接电阻<br />- 默认状态：关闭（不启用） |
| 4    | 8Px2 插线端子接口   | 详细引脚功能如下表（*8Px2 插线端子引脚定义*）。                                                               |
| 5    | DC 电源输入接口     | 外接输入电源：DC 5V/2A。                                                                                      |
| 6    | RJ12 母座（P1）接口 | 用于连接 P1 电表。                                                                                            |
| 7    | 复位键（RESET）     | 用于设备重启或恢复出厂设置。                                                                                  |
| 8    | Micro SIM 卡槽      | 安装时芯片金属面朝上，缺口朝外；仅 4G 版本支持本接口。                                                        |



**8Px2 插线端子引脚定义**

<table><thead>
  <tr>
    <th>编号</th>
    <th>定义名称</th>
    <th>功能定义</th>
    <th>功能说明</th>
  </tr></thead>
<tbody>
  <tr>
    <td>1</td>
    <td>B1</td>
    <td rowspan="2">RS485通道1</td>
    <td>RS485通道1数据B</td>
  </tr>
  <tr>
    <td>2</td>
    <td>A1</td>
    <td>RS485通道1数据A</td>
  </tr>
  <tr>
    <td>3</td>
    <td>B2</td>
    <td rowspan="2">RS485通道2</td>
    <td>RS485通道2数据B</td>
  </tr>
  <tr>
    <td>4</td>
    <td>A2</td>
    <td>RS485通道2数据A</td>
  </tr>
  <tr>
    <td>5</td>
    <td>B3</td>
    <td rowspan="2">RS485通道3</td>
    <td>RS485通道3数据B</td>
  </tr>
  <tr>
    <td>6</td>
    <td>A3</td>
    <td>RS485通道3数据A</td>
  </tr>
  <tr>
    <td>7</td>
    <td>DI1+</td>
    <td rowspan="2">DI 通道1</td>
    <td>DI 通道1 正电平信号</td>
  </tr>
  <tr>
    <td>8</td>
    <td>DI1-</td>
    <td>DI 通道1 参考地</td>
  </tr>
  <tr>
    <td>9</td>
    <td>DI2+</td>
    <td rowspan="2">DI 通道2</td>
    <td>DI 通道2 正电平信号</td>
  </tr>
  <tr>
    <td>10</td>
    <td>DI2-</td>
    <td>DI 通道2 参考地</td>
  </tr>
  <tr>
    <td>11</td>
    <td>+</td>
    <td rowspan="2">12V隔离电源输出</td>
    <td>DC 12V@100mA隔离电源输出</td>
  </tr>
  <tr>
    <td>12</td>
    <td>-</td>
    <td>隔离电源参考地</td>
  </tr>
  <tr>
    <td>13</td>
    <td>NO1</td>
    <td rowspan="2">DO 通道1</td>
    <td>DO 通道1常开端</td>
  </tr>
  <tr>
    <td>14</td>
    <td>COM1</td>
    <td>DO 通道1公共端</td>
  </tr>
  <tr>
    <td>15</td>
    <td>NO2</td>
    <td rowspan="2">DO 通道2</td>
    <td>DO 通道2常开端</td>
  </tr>
  <tr>
    <td>16</td>
    <td>COM2</td>
    <td>DO 通道2公共端</td>
  </tr>
</tbody></table>


### 指示灯说明

<table><tbody>
  <tr>
    <th colspan="2">指示灯</th>
    <th colspan="3">运行状态</th>
  </tr>
  <tr>
    <td>图标</td>
    <td>定义</td>
    <td>常亮</td>
    <td>闪烁</td>
    <td>熄灭</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/power.png").default} width="25" style={{verticalAlign: "middle"}}/> </td>
    <td>电源指示灯/系统运行状态指示灯</td>
    <td>1. 上电后6个灯亮30s，后熄灭，表示上电成功<br />2. 常亮代表程序系统异常</td>
    <td>系统程序正常运行</td>
    <td>上电失败/程序异常</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/cloud.png").default} width="40" style={{verticalAlign: "middle"}}/> </td>
    <td>服务器连接状态指示灯</td>
    <td>连接服务器成功</td>
    <td>正在连接服务器</td>
    <td>连接服务器失败</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/net.png").default} width="30" style={{verticalAlign: "middle"}}/> </td>
    <td>路由器/基站连接状态指示灯</td>
    <td>连接成功</td>
    <td>连接中</td>
    <td>4G功能关闭/连接失败</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/lora.png").default} width="30" style={{verticalAlign: "middle"}}/> </td>
    <td>LoRa指示灯</td>
    <td>采集器与LoRa子设备连接状态指示灯/兼容蓝牙连接指示灯,常亮连接正常</td>
    <td>LoRa/蓝牙正常通信中</td>
    <td>连接失败</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/com.png").default} width="80" style={{verticalAlign: "middle"}}/> </td>
    <td>串口指示灯</td>
    <td>RS485设备连接正常</td>
    <td>无</td>
    <td>连接失败</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/p1.png").default} width="25" style={{verticalAlign: "middle"}}/> </td>
    <td>P1指示灯</td>
    <td>连接正常</td>
    <td>无</td>
    <td>连接失败</td>
  </tr>
</tbody>
</table>

> **固件升级**：升级过程中 COM 指示灯与 P1 指示灯同时闪烁；升级完成后系统自动重启。
  

### 按键说明

<table>
<tbody>
  <tr>
    <th rowspan="2">按键</th>
    <td>Reset</td>
    <td>短按 RESET 按键（持续时间 &lt; 10s）：指示灯全亮后松开按键，设备执行**重启**</td>
  </tr>
  <tr>
    <td>Reload</td>
    <td>长按 RESET 按键（持续时间 ≥ 10s）：指示灯全亮后持续至熄灭，松开按键执行**恢复出厂设置**</td>
  </tr>

</tbody>
</table>

## 6. 配件说明

**电源适配器**

配备欧规电源作为市电输入电源，采用 DC 2.5 接口（线长 1m）为 EMH-2 提供供电。

<img src={require("./img/power_cable.png").default} width="240" /> 



| 输入特性 | 最小   | 额定值        | 最大   |
| -------- | ------ | ------------- | ------ |
| 输入电压 | 90Vac | 100Vac~240Vac | 264Vac |
| 输入频率 | 47Hz   | 60Hz/50Hz     | 63Hz   |

 
<table><thead>
  <tr>
    <th colspan="2">额定负载</th>
    <th rowspan="2">输出电压</th>
  </tr>
  <tr>
    <th>最小值</th>
    <th>最大值</th>
  </tr></thead>
<tbody>
  <tr>
    <td>0.1A</td>
    <td>2A</td>
    <td>+5V±5%</td>
  </tr>
</tbody>
</table>

**P1电表线**

配备 1.5m 普通 RJ12 连接线。

<img src={require("./img/p1_cable.png").default} width="360" /> 
