---
title: System Operation
description: todo
---

# System Operation

## 1. Before Powering On

1. Before officially powering on, use a multimeter to confirm whether the power supply output voltage is within the normal power supply range.
2. Secure the controller power connector.
3. Connect the wiring harness connector to the corresponding interface.
4. Connect the communication port connector to the corresponding interface.
5. The system is powered normally.

After completing the above steps, you can use the host computer software provided by our company or observe the LED indicator status to verify whether the controller is operating normally.


## 2. LED Status

<table><thead>
  <tr>
    <th>Indicator</th>
    <th>Status</th>
    <th>Description</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="2">PWR</td>
    <td>Red LED off</td>
    <td>No power / Power-on failure / System program error</td>
  </tr>
  <tr>
    <td>Red LED solid on</td>
    <td>System is operating normally</td>
  </tr>
  <tr>
    <td rowspan="4">4G</td>
    <td>Green LED off</td>
    <td>4G not enabled or SIM card not detected</td>
  </tr>
  <tr>
    <td>Green LED blinking slowly</td>
    <td>Data transmission in progress</td>
  </tr>
  <tr>
    <td>Green LED blinking rapidly</td>
    <td>4G connection failed or communication interrupted</td>
  </tr>
  <tr>
    <td>Green LED solid on</td>
    <td>4G dial-up connection established successfully</td>
  </tr>
  <tr>
    <td rowspan="3">ALM</td>
    <td>Red LED off</td>
    <td>No alarm</td>
  </tr>
  <tr>
    <td>Red LED blinking slowly</td>
    <td>System notification or minor alarm detected</td>
  </tr>
  <tr>
    <td>Red LED blinking rapidly</td>
    <td>Major system alarm detected</td>
  </tr>
  <tr>
    <td rowspan="3">RUN</td>
    <td>Green LED off</td>
    <td>Abnormal server connection</td>
  </tr>
  <tr>
    <td>Green LED blinking slowly</td>
    <td>Connecting to the server</td>
  </tr>
  <tr>
    <td>Green LED solid on</td>
    <td>Server connection is normal</td>
  </tr>
</tbody>
</table>

> **Note:**
> - Slow blinking: LED on for 1 second and off for 1 second.
> - Rapid blinking: LED on for 100 ms and off for 100 ms.