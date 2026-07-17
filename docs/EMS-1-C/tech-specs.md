---
title: Technical Specifications
description: todo
---

# Technical Specifications

<table><thead>
  <tr>
    <th>Category</th>
    <th>Device Configuration</th>
    <th>Specifications</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="15">Hardware Parameters</td>
    <td>CPU</td>
    <td>RV1126BJ<br />4×ARM Cortex-A53@1.6GHz</td>
  </tr>
  <tr>
    <td>NPU</td>
    <td>Supports INT4/INT8/INT16/FP16 mixed precision computation, with up to 3 Tops of computing power</td>
  </tr>
  <tr>
    <td>Operating System</td>
    <td>Debian12/Ubuntu 22.04</td>
  </tr>
  <tr>
    <td>Memory</td>
    <td>1/2GB DDR4</td>
  </tr>
  <tr>
    <td>eMMC</td>
    <td>8/16GB eMMC</td>
  </tr>
  <tr>
    <td>ETHERNET</td>
    <td>2 × 10/100M ports, one LAN and one WAN</td>
  </tr>
  <tr>
    <td>USB 3.0</td>
    <td>USB-A 3.0*1</td>
  </tr>
  <tr>
    <td>485</td>
    <td>3 × RS485 ports</td>
  </tr>
  <tr>
    <td>CAN</td>
    <td>1 × CAN port</td>
  </tr>
  <tr>
    <td>DI</td>
    <td>4 × DI (dry contact detection)</td>
  </tr>
  <tr>
    <td>AI</td>
    <td>1 × current detection (0–60mA), 1 × voltage detection (0–36V)</td>
  </tr>
  <tr>
    <td>DO</td>
    <td>2 × DO ports</td>
  </tr>
  <tr>
    <td>4G</td>
    <td>FDD-LTE、TDD-LTE</td>
  </tr>
  <tr>
    <td>WiFi</td>
    <td>IEEE 802.11b/g/n/ax(@2.4GHz), Wi-Fi compliant</td>
  </tr>
  <tr>
    <td>BT</td>
    <td>BLE5.2</td>
  </tr>
  <tr>
    <td rowspan="17">Software Parameters</td>
    <td>Southbound Data Access</td>
    <td>Supports access and data protocol adaptation for various devices including BMS, PCS, EMS, PV, I/O systems, etc.</td>
  </tr>
  <tr>
    <td>Northbound Data Upload</td>
    <td>Supports multi-channel encrypted transmission to platforms such as SOLMAN, as well as standard protocol platform access including IEC104, Modbus TCP, etc.</td>
  </tr>
  <tr>
    <td>Parallel Cabinet Management</td>
    <td>≤ 16 units</td>
  </tr>
  <tr>
    <td rowspan="6">Energy Strategies</td>
    <td>Peak shaving and valley filling</td>
  </tr>
  <tr>
    <td>Demand management</td>
  </tr>
  <tr>
    <td>Load tracking + anti-reverse power flow</td>
  </tr>
  <tr>
    <td>Power control</td>
  </tr>
  <tr>
    <td>Renewable energy consumption</td>
  </tr>
  <tr>
    <td>Other customized advanced strategies</td>
  </tr>
  <tr>
    <td rowspan="2">User Configuration</td>
    <td>Local web configuration</td>
  </tr>
  <tr>
    <td>Remote server configuration</td>
  </tr>
  <tr>
    <td rowspan="2">Firmware Upgrade</td>
    <td>Remote upgrade</td>
  </tr>
  <tr>
    <td>Local web upgrade</td>
  </tr>
  <tr>
    <td rowspan="2">Security Mechanism</td>
    <td>Software watchdog</td>
  </tr>
  <tr>
    <td>Hardware watchdog</td>
  </tr>
  <tr>
    <td>Policy Configuration</td>
    <td>Local/Remote Policy Configuration</td>
  </tr>
  <tr>
    <td>Others</td>
    <td>Real-time control, Remote OTA, Breakpoint resume</td>
  </tr>
</tbody></table>
