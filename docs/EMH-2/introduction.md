---
title: Product Overview
description: Introduction to the EMH-2 home energy management center, including model information, features, interfaces, and accessories.
---

# Product Overview

## 1. Model Information

This document mainly covers the following product models: EMH-2-RG and EMH-2-R.

**Model Naming Convention**

<img src={require("./img/model.png").default} width="240" />

| No. | Description          | Value                                                  |
| --- | -------------------- | ------------------------------------------------------ |
| ⑴   | Product Identifier   | EMH: Home Energy Management Hub                        |
| ⑵   | Product Generation   | 2: Second-generation product                           |
| ⑶   | Communication Method | R: Supports LoRa communication<br />G: Supports 4G communication |

## 2. Application Scenarios

The EMH-2 is a smart device specifically designed for residential energy management applications. By monitoring, analyzing, and optimizing household energy consumption in real time, it helps users reduce energy costs, save electricity expenses, and improve the intelligence of home energy usage.

The device supports multiple interfaces and can seamlessly integrate with inverters, batteries, EV chargers, SG Ready heat pumps, P1 smart meters, and other devices. It enables centralized control and optimized management of photovoltaic generation, energy storage, EV charging, and household power consumption.

**Typical Applications**

- Designed for residential energy management in Europe, helping users optimize energy usage and improve energy cost efficiency in household scenarios.

## 3. Product Advantages

### Core Value

- **Cost Reduction**: Optimize the use of solar power, battery storage, and grid electricity for the most economical energy consumption.
- **Increased Savings**: Supports energy planning based on electricity tariffs to enable peak-valley arbitrage.
- **Higher Efficiency**: Supports local and remote monitoring and management of home energy systems, improving operation and maintenance efficiency.
- **Better User Experience**: Provides a visualized UI for intuitive display and monitoring of energy data.

### Product Features

- Supports integration with various new energy devices such as inverters, batteries, EV chargers, and heat pumps.
- Supports integrated management and scenario linkage of solar generation, energy storage, EV charging, and household loads.
- Supports multiple communication methods including 4G, WiFi, and Ethernet for uploading data to the cloud platform, enabling convenient remote monitoring and management.
- Built-in local management interface for viewing power generation, energy storage, and electricity consumption locally.
- Supports multiple energy management strategies to optimize energy usage, reduce electricity costs, and improve energy efficiency.
- Complies with the EN18031 IoT cybersecurity standard.

## 4. Product Structure

EMH-2 dimensions (unit: mm, dimensional tolerance ±2%)

<img src={require("./img/size.png").default} width="480" />

## 5. Appearance Overview

<img src={require("./img/appearance.png").default} width="480" />

### Appearance and Interfaces

| No. | Interface                  | Description |
| --- | -------------------------- | ----------- |
| 1   | WAN Port                   | RJ45 Ethernet port (with indicator LEDs). |
| 2   | LAN Port                   | RJ45 Ethernet port (with indicator LEDs). |
| 3   | 3-Bit DIP Switch           | Used to configure the 120Ω termination resistors for the 3 RS485 channels:<br />- ON: Enable 120Ω termination resistor<br />- Default: Disabled |
| 4   | 8Px2 Terminal Connector    | Detailed pin definitions are provided in the table below (*8Px2 Terminal Pin Definitions*). |
| 5   | DC Power Input             | External DC power supply input: DC 5V/2A. |
| 6   | RJ12 Female Port (P1)      | Used to connect a P1 smart meter. |
| 7   | Reset Button (RESET)       | Used to reboot the device or restore factory settings. |
| 8   | Micro SIM Card Slot        | Insert the SIM card with the metal contacts facing upward and the notch facing outward. Only available on the 4G version. |

### 8Px2 Terminal Pin Definitions

<table><thead>
  <tr>
    <th>No.</th>
    <th>Pin Name</th>
    <th>Function</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td>1</td>
    <td>B1</td>
    <td rowspan="2">RS485 Channel 1</td>
    <td>RS485 Channel 1 Data B</td>
  </tr>
  <tr>
    <td>2</td>
    <td>A1</td>
    <td>RS485 Channel 1 Data A</td>
  </tr>
  <tr>
    <td>3</td>
    <td>B2</td>
    <td rowspan="2">RS485 Channel 2</td>
    <td>RS485 Channel 2 Data B</td>
  </tr>
  <tr>
    <td>4</td>
    <td>A2</td>
    <td>RS485 Channel 2 Data A</td>
  </tr>
  <tr>
    <td>5</td>
    <td>B3</td>
    <td rowspan="2">RS485 Channel 3</td>
    <td>RS485 Channel 3 Data B</td>
  </tr>
  <tr>
    <td>6</td>
    <td>A3</td>
    <td>RS485 Channel 3 Data A</td>
  </tr>
  <tr>
    <td>7</td>
    <td>DI1+</td>
    <td rowspan="2">DI Channel 1</td>
    <td>DI Channel 1 Positive Signal</td>
  </tr>
  <tr>
    <td>8</td>
    <td>DI1-</td>
    <td>DI Channel 1 Reference Ground</td>
  </tr>
  <tr>
    <td>9</td>
    <td>DI2+</td>
    <td rowspan="2">DI Channel 2</td>
    <td>DI Channel 2 Positive Signal</td>
  </tr>
  <tr>
    <td>10</td>
    <td>DI2-</td>
    <td>DI Channel 2 Reference Ground</td>
  </tr>
  <tr>
    <td>11</td>
    <td>+</td>
    <td rowspan="2">12V Isolated Power Output</td>
    <td>DC 12V@100mA isolated power output</td>
  </tr>
  <tr>
    <td>12</td>
    <td>-</td>
    <td>Isolated power reference ground</td>
  </tr>
  <tr>
    <td>13</td>
    <td>NO1</td>
    <td rowspan="2">DO Channel 1</td>
    <td>DO Channel 1 Normally Open Terminal</td>
  </tr>
  <tr>
    <td>14</td>
    <td>COM1</td>
    <td>DO Channel 1 Common Terminal</td>
  </tr>
  <tr>
    <td>15</td>
    <td>NO2</td>
    <td rowspan="2">DO Channel 2</td>
    <td>DO Channel 2 Normally Open Terminal</td>
  </tr>
  <tr>
    <td>16</td>
    <td>COM2</td>
    <td>DO Channel 2 Common Terminal</td>
  </tr>
</tbody></table>

### LED Indicator Description

<table><tbody>
  <tr>
    <th colspan="2">Indicator</th>
    <th colspan="3">Operating Status</th>
  </tr>
  <tr>
    <td>Icon</td>
    <td>Description</td>
    <td>On</td>
    <td>Blinking</td>
    <td>Off</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/power.png").default} width="25" style={{verticalAlign: "middle"}}/> </td>
    <td>Power / System Status Indicator</td>
    <td>1. After power-on, all 6 LEDs light up for 30 seconds and then turn off, indicating successful startup.<br />2. Remaining solid on indicates system program error.</td>
    <td>System operating normally</td>
    <td>Power-on failure / system error</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/cloud.png").default} width="40" style={{verticalAlign: "middle"}}/> </td>
    <td>Server Connection Indicator</td>
    <td>Connected to server successfully</td>
    <td>Connecting to server</td>
    <td>Server connection failed</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/net.png").default} width="30" style={{verticalAlign: "middle"}}/> </td>
    <td>Router / Base Station Connection Indicator</td>
    <td>Connected successfully</td>
    <td>Connecting</td>
    <td>4G disabled / connection failed</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/lora.png").default} width="30" style={{verticalAlign: "middle"}}/> </td>
    <td>LoRa Indicator</td>
    <td>Indicates connection status between the collector and LoRa sub-devices / also compatible with Bluetooth connection indication; solid on means connected normally</td>
    <td>LoRa/Bluetooth communication active</td>
    <td>Connection failed</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/com.png").default} width="80" style={{verticalAlign: "middle"}}/> </td>
    <td>Serial Port Indicator</td>
    <td>RS485 device connected normally</td>
    <td>N/A</td>
    <td>Connection failed</td>
  </tr>
  <tr>
    <td style={{ textAlign: "center" }}> <img src={require("./img/p1.png").default} width="25" style={{verticalAlign: "middle"}}/> </td>
    <td>P1 Indicator</td>
    <td>Connected normally</td>
    <td>N/A</td>
    <td>Connection failed</td>
  </tr>
</tbody>
</table>

> **Firmware Upgrade:** During firmware upgrade, the COM and P1 indicators blink simultaneously. The system will automatically reboot after the upgrade is completed.

### Button Description

<table>
<tbody>
  <tr>
    <th rowspan="2">Button</th>
    <td>Reset</td>
    <td>Short press the RESET button (duration &lt; 10s): release the button after all indicators light up, and the device will reboot.</td>
  </tr>
  <tr>
    <td>Reload</td>
    <td>Press and hold the RESET button (duration ≥ 10s): keep holding until all indicators turn off, then release to restore factory settings.</td>
  </tr>
</tbody>
</table>

## 6. Accessories

### Power Adapter

Supplied with a European-standard AC power adapter as the mains input power source. It uses a DC 2.5 connector (cable length: 1m) to power the EMH-2.

<img src={require("./img/power_cable.png").default} width="240" />

| Input Characteristics | Minimum | Rated Value      | Maximum |
| --------------------- | ------- | ---------------- | ------- |
| Input Voltage         | 90Vac   | 100Vac~240Vac    | 264Vac  |
| Input Frequency       | 47Hz    | 50Hz/60Hz        | 63Hz    |

<table><thead>
  <tr>
    <th colspan="2">Rated Load</th>
    <th rowspan="2">Output Voltage</th>
  </tr>
  <tr>
    <th>Minimum</th>
    <th>Maximum</th>
  </tr></thead>
<tbody>
  <tr>
    <td>0.1A</td>
    <td>2A</td>
    <td>+5V±5%</td>
  </tr>
</tbody>
</table>

### P1 Meter Cable

Supplied with a standard 1.5m RJ12 connection cable.

<img src={require("./img/p1_cable.png").default} width="360" />