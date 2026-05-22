---
title: 快速上手
description: 按步骤完成网关安装与接线，快速开始使用
---

# 快速上手


## 1. 准备线缆       

在开始前，请根据你的使用场景准备好对应线缆：
<img src={require("./img/interfaces.png").default} width="360" /> 

| 接口类型 | 用途 | 所需线缆 |
|----------|------|----------|
| WAN / LAN | 网络连接（路由器 / 设备通信） | RJ45 网线 |
| RS485 / DO / 12V_OUT | 逆变器 / 热泵通信与控制 | RS485 信号线 |
| P1 | 电表数据读取 | RJ12 信号线 |

<img src={require("./img/rj12_45.png").default} width="240" /> 
<img src={require("./img/rs485.png").default} width="240" /> 

:::warning 
- 不同接口线缆不可混用（RJ12 ≠ RJ45）  
- RS485 通信需特别注意 A/B 线序
:::

## 2. 安装设备

选择合适的位置安装设备，有助于后续稳定运行：
- 通风良好，避免密闭空间
- 远离热源（如暖气、阳光直射）
- 避开强电磁干扰（如配电箱、大功率电器）

**安装步骤：**

1. 确定螺钉安装位置：根据设备背面卡槽的位置，在安装面上标记对应的螺钉固定点。
2. 固定螺钉：在标记好的位置固定螺钉。
3. 对准与安装：将设备背面的卡槽完全对准已固定的螺钉。
4. 卡入固定：将设备向下滑动固定到位。

<img src={require("./img/size.png").default} width="480" /> 
<img src={require("./img/installation.png").default} width="480" /> 


## 3. 电气连接

### 3.1 连接网线

使用 RJ45 网线连接 EMH-2 **WAN口**与路由器 **LAN口**

<img src={require("./img/connection_router.png").default} width="240" /> 

### 3.2 连接信号线


**插入信号线端子**

将 8Px2 插线端子插入设备对应接口

<img src={require("./img/connection_8p.png").default} width="480" /> 


**连接充电桩（如有）**

使用 RJ45 网线将 EMH-2 的 LAN 口连接至充电桩
<img src={require("./img/connection_charger.png").default} width="480" /> 


**连接 P1 电表（如有）**

使用 RJ12 信号线连接 EMH-2 P1 接口与电表 P1 接口  

<img src={require("./img/connection_meter.png").default} width="240" /> 

**连接逆变器**

将 RS485 通信线接入 8Px2 端子：
- RS485 A 线连接到端子上的 A 端口
- RS485 B 线连接到端子上的 B 端口

:::warning
请确保 A/B 线序连接正确，且必须接在**同一组端子**（如 A1/B1），否则通信将无法建立。
:::

<img src={require("./img/connection_inverter.png").default} width="480" /> 


**连接热泵**

根据热泵 SG Ready 接口类型选择连接方式：

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
  <TabItem value="wire" label="1️⃣ 继电器控制" default>
    
    1. EMH-2 **+** 连接 EMH-2 **NO1**
    2. EMH-2 **COM1** 连接 外部继电器线圈 +
    3. EMH-2 **-** 连接 外部继电器线圈 -
    4. 继电器触点 连接 热泵

    <img src={require("./img/connection_heat_pump1.png").default} width="480" /> 

    > - 通过设备 DO（NO1/COM1）控制 +12V 是否送到继电器线圈，从而间接控制热泵  
    > - 适用于：功率较大或需要更稳定控制的场景

  </TabItem>
  <TabItem value="wireless" label="2️⃣ 直接连接">
    
    EMH-2的 DO 输出口 (NO1 / COM1) 直接连接热泵 DI 输入口

    <img src={require("./img/connection_heat_pump2.png").default} width="480" /> 

    > - 通过设备内部开关直接控制信号通断    
    > - 适用于：小电流控制场景  
    
  </TabItem>
</Tabs>


### 3.3 插入 4G SIM 卡

按照 SIM 卡槽旁的图示方向，将 SIM 卡芯片的金属接触面朝上，带有缺口的短边朝外，推入卡槽直至卡住。
<img src={require("./img/sim_card.png").default} width="240" /> 

### 3.4 连接电源

使用原装电源适配器，将其 DC 插头插入 EMH-2 设备上的 DC 电源口。
<img src={require("./img/power_on.png").default} width="360" /> 
