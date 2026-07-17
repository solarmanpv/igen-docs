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
    <th>State</th>
    <th>Meaning</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="3">ALM</td>
    <td>Red light off</td>
    <td>No alarm</td>
  </tr>
  <tr>
    <td>Red light flashing slowly</td>
    <td>System prompt/minor alarm</td>
  </tr>
  <tr>
    <td>Red light flashing quickly</td>
    <td>A major alarm occurs in the system</td>
  </tr>
  <tr>
    <td rowspan="3">NET</td>
    <td>Green light off</td>
    <td>Server connection abnormal</td>
  </tr>
  <tr>
    <td>Green light flashing slowly</td>
    <td>Connecting to server</td>
  </tr>
  <tr>
    <td>Green light solid on</td>
    <td>Server connection normal</td>
  </tr>
  <tr>
    <td rowspan="2">PWR</td>
    <td>Green light off</td>
    <td>No power / Power-on failed / System program abnormal</td>
  </tr>
  <tr>
    <td>Green light solid on</td>
    <td>Server connection normal</td>
  </tr>
  <tr>
    <td rowspan="4">4G</td>
    <td>Green light off</td>
    <td>4G not enabled or SIM card not detected</td>
  </tr>
  <tr>
    <td>Green light flashing quickly</td>
    <td>4G is not connected or the communication is interrupted</td>
  </tr>
  <tr>
    <td>Green light flashing slowly</td>
    <td>Data transmission in progress</td>
  </tr>
  <tr>
    <td>Green light solid on</td>
    <td>4G dial-up successful</td>
  </tr>
</tbody></table>

> **Note:**
> - Slow blinking: LED on for 1 second and off for 1 second.
> - Rapid blinking: LED on for 100 ms and off for 100 ms.