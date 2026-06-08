---
title: Quick Start
description: Follow step-by-step instructions to install and wire the gateway and get started quickly.
---

# Quick Start

## 1. Prepare Cables

Before getting started, prepare the required cables according to your application scenario:

<img src={require("./img/interfaces.png").default} width="480" />

| Interface Type | Purpose | Required Cable |
|----------------|---------|----------------|
| WAN / LAN | Network connection (router / device communication) | RJ45 Ethernet cable |
| RS485 / DO / 12V_OUT | Inverter / heat pump communication and control | RS485 signal cable |
| P1 | Smart meter data reading | RJ12 signal cable |

<img src={require("./img/rj12_45.png").default} width="240" />
<img src={require("./img/rs485.png").default} width="240" />

:::warning
- Do not mix different cable types (RJ12 ≠ RJ45)  
- Pay special attention to correct A/B wiring for RS485 communication
:::

## 2. Device Installation

Choose an appropriate installation location to ensure stable operation:

- Well-ventilated area, avoid enclosed spaces  
- Keep away from heat sources (e.g., radiators, direct sunlight)  
- Avoid strong electromagnetic interference (e.g., distribution boxes, high-power electrical equipment)  

**Installation Steps:**

1. Determine mounting positions: Mark screw positions on the installation surface according to the mounting slots on the back of the device.  
2. Fix the screws: Secure screws at the marked positions.  
3. Align the device: Align the rear mounting slots with the installed screws.  
4. Secure the device: Slide the device downward to lock it into place.  

<img src={require("./img/size.png").default} width="480" />
<img src={require("./img/installation.png").default} width="480" />

## 3. Electrical Connections

### 3.1 Connect the Ethernet Cable

Connect the EMH-2 **WAN port** to the router **LAN port** using an RJ45 Ethernet cable.

<img src={require("./img/connection_router.png").default} width="240" />

### 3.2 Signal Wiring

**Insert Terminal Block**

Insert the 8P×2 terminal connector into the corresponding device interface.

<img src={require("./img/connection_8p.png").default} width="480" />

**Connect EV Charger (if applicable)**

Use an RJ45 cable to connect the EMH-2 LAN port to the EV charger.

<img src={require("./img/connection_charger.png").default} width="480" />

**Connect P1 Smart Meter (if applicable)**

Use an RJ12 cable to connect the EMH-2 P1 port to the meter P1 interface.

<img src={require("./img/connection_meter.png").default} width="240" />

**Connect Inverter**

Connect RS485 communication wires to the 8P×2 terminal:

- RS485 A wire → terminal A port  
- RS485 B wire → terminal B port  

:::warning
Ensure correct A/B wiring and connect to the **same terminal group** (e.g., A1/B1). Otherwise, communication will fail.
:::

<img src={require("./img/connection_inverter.png").default} width="480" />

**Connect Heat Pump**

Select the appropriate connection method based on the SG Ready interface type of the heat pump:

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
  <TabItem value="wire" label="1️⃣ Relay Control" default>

    1. EMH-2 **+** connects to EMH-2 **NO1**  
    2. EMH-2 **COM1** connects to external relay coil +  
    3. EMH-2 **-** connects to external relay coil -  
    4. Relay contact connects to heat pump  

    <img src={require("./img/connection_heat_pump1.png").default} width="480" />

    > - Controls whether +12V is supplied to the relay coil via DO (NO1/COM1), indirectly controlling the heat pump  
    > - Suitable for high-power or more stable control scenarios  

  </TabItem>

  <TabItem value="wireless" label="2️⃣ Direct Connection">

    EMH-2 DO output (NO1 / COM1) connects directly to the heat pump DI input

    <img src={require("./img/connection_heat_pump2.png").default} width="480" />

    > - Directly switches the signal via internal relay output  
    > - Suitable for low-current control scenarios  

  </TabItem>
</Tabs>

### 3.3 Insert 4G SIM Card

Insert the SIM card according to the diagram near the slot. The metal contacts should face upward, and the notched edge should face outward. Push the card in until it locks into place.

<img src={require("./img/sim_card.png").default} width="240" />

### 3.4 Power Connection

Use the original power adapter and plug the DC connector into the DC power port of the EMH-2 device.

<img src={require("./img/power_on.png").default} width="360" />
