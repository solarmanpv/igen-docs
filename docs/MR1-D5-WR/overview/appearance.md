---
title: Appearance
description: Appearance, interface definition, indicator and button descriptions of the MR1-D5 series meters
---

# Appearance

## MR1-D5-W, MR1-D5-WR Appearance and Interface Definition

<div style={{display:'flex', gap:'40px', alignItems:'flex-start', flexWrap:'wrap', margin:'12px 0'}}>
  <img src={require('./img/mr1-appearance.png').default} width="155" alt="MR1-D5-W appearance" />
  <img src={require('./img/mr1-appearance-w.png').default} width="150" alt="MR1-D5-WR appearance" />
</div>

| Interface | Name | Description |
| --- | --- | --- |
| ![Neutral terminal](img/interface-mr1-terminal.png) | N | Neutral terminal, meter power input |
| ![Live terminal](img/interface-mr1-terminal.png) | L | Live terminal, meter power input |
| ![CT port](img/interface-mr1-ct.png) | CT | CT port, CT current sampling port |

## MR3-D5-W, MR3-D5-WR Appearance and Interface Definition

<div style={{display:'flex', gap:'40px', alignItems:'flex-start', flexWrap:'wrap', margin:'12px 0'}}>
  <img src={require('./img/mr3-appearance.png').default} width="135" alt="MR3-D5-W appearance" />
  <img src={require('./img/mr3-appearance-w.png').default} width="170" alt="MR3-D5-WR appearance" />
</div>

| Interface | Name | Description |
| --- | --- | --- |
| ![Neutral terminal](img/interface-mr3-terminal.png) | N | Neutral terminal, meter power input |
| ![Phase A live terminal](img/interface-mr3-terminal.png) | L1 | Phase A live terminal, meter power input |
| ![Phase B live terminal](img/interface-mr3-terminal.png) | L2 | Phase B live terminal, meter power input |
| ![Phase C live terminal](img/interface-mr3-terminal.png) | L3 | Phase C live terminal, meter power input |
| ![CT port](img/interface-mr3-ct.png) | CT | CT port, CT current sampling port |

## MR1-D5-WR, MR3-D5-WR Indicator Descriptions

| Indicator | Meaning | Status Description |
| --- | --- | --- |
| ![Power indicator](img/indicator-power.png) | Power (red) | Steady on: power indicator, the meter is powered normally.<br/>Off: the meter is not powered or is abnormal. |
| ![Network indicator](img/indicator-wifi.png) | Network (WiFi) (green) | Steady on: the device is connected to the cloud platform.<br/>Blinking at 1s intervals: the device is connected to the router or has obtained an IP.<br/>Fast blinking at 100ms intervals: the device is upgrading.<br/>Off: the device is not connected to the router or has not obtained an IP. |
| ![LoRa indicator](img/indicator-rf.png) | LoRa (green) | Steady on: LoRa connection established.<br/>Off: LoRa not connected. |

## MR1-D5-W, MR3-D5-W Indicator Descriptions

| Indicator | Meaning | Status Description |
| --- | --- | --- |
| ![Power indicator](img/indicator-power.png) | Power (red) | Steady on: power indicator, the meter is powered normally.<br/>Off: the meter is not powered or is abnormal. |
| ![Network indicator](img/indicator-wifi.png) | Network (WiFi) (green) | Steady on: the device is connected to the cloud platform.<br/>Blinking at 1s intervals: the device is connected to the router or has obtained an IP.<br/>Fast blinking at 100ms intervals: the device is upgrading.<br/>Off: the device is not connected to the router or has not obtained an IP. |

## Button Description

| Button | Meaning | Function Description |
| --- | --- | --- |
| ![RESET button](img/reset-button.png) | RESET | Long press for 10 seconds to restore factory settings.<br/>All indicators stay on for 2s and then return to normal status. |
