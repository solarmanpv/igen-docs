---
title: Feature List
description: todo
---

# Feature List

<table><thead>
  <tr>
    <th>Feature Category</th>
    <th>Feature Module</th>
    <th>Feature Details</th>
    <th>EMS-1-P</th>
    <th>Remarks</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="4">Data Acquisition</td>
    <td>Analog Data Acquisition</td>
    <td>Three-phase voltage / current / active power / reactive power / frequency acquisition</td>
    <td>✅</td>
    <td>Supports standard Modbus protocol and DIO data acquisition</td>
  </tr>
  <tr>
    <td>Analog Data Acquisition</td>
    <td>Cell voltage / temperature / SOC / SOH acquisition</td>
    <td>✅</td>
    <td>Supports rack-level and PACK-level data acquisition</td>
  </tr>
  <tr>
    <td>Digital Status Acquisition</td>
    <td>Switch status, contactor status, and alarm signal acquisition</td>
    <td>✅</td>
    <td>Supports standard digital input signals</td>
  </tr>
  <tr>
    <td>Energy Metering</td>
    <td>Cumulative charge/discharge energy and peak/flat/valley energy statistics</td>
    <td>✅</td>
    <td>Supports energy meter integration</td>
  </tr>

  <tr>
    <td rowspan="4">Device Control</td>
    <td>Basic Control</td>
    <td>Energy storage system start/stop and charge/discharge mode switching</td>
    <td>✅</td>
    <td>Basic modes such as constant power charging/discharging</td>
  </tr>
  <tr>
    <td>Power Regulation</td>
    <td>Active/reactive power command control</td>
    <td>✅</td>
    <td>Supports continuous adjustment from 0% to 100%</td>
  </tr>
  <tr>
    <td>Grid-connected / Off-grid Switching</td>
    <td>Grid-connected / off-grid mode switching control</td>
    <td>⚙️</td>
    <td>Requires PCS support</td>
  </tr>
  <tr>
    <td>Multi-device Parallel Operation</td>
    <td>Multi-cabinet cluster power distribution and current sharing control</td>
    <td>✅</td>
    <td>Dedicated function for station-level control</td>
  </tr>

  <tr>
    <td rowspan="4">Operation Strategies</td>
    <td>Basic Strategies</td>
    <td>Scheduled charge/discharge and SOC maintenance</td>
    <td>✅</td>
    <td>Built-in standard function</td>
  </tr>
  <tr>
    <td>Peak-Valley Arbitrage</td>
    <td>Automatic charge/discharge based on time-of-use electricity tariffs</td>
    <td>✅</td>
    <td>Built-in standard function</td>
  </tr>
  <tr>
    <td>Demand Management</td>
    <td>Maximum demand limitation and peak shaving</td>
    <td>✅</td>
    <td>Built-in standard function</td>
  </tr>
  <tr>
    <td>Reverse Power Protection</td>
    <td>PV energy utilization and self-consumption optimization</td>
    <td>✅</td>
    <td>Built-in standard function</td>
  </tr>

  <tr>
    <td rowspan="3">Protection and Alarms</td>
    <td>Level 1 Protection</td>
    <td>Overvoltage / undervoltage / overcurrent / overtemperature alarms and shutdown</td>
    <td>✅</td>
    <td>Fault shutdown and alarm reporting</td>
  </tr>
  <tr>
    <td>Level 2 Protection</td>
    <td>Insulation detection, liquid leakage detection, and smoke concentration detection</td>
    <td>⚙️</td>
    <td>Requires connection of corresponding sensors</td>
  </tr>
  <tr>
    <td>Fault Records</td>
    <td>Fault alarm storage, operation data, and SOE event records</td>
    <td>✅</td>
    <td>Local storage capacity ≥10,000 records</td>
  </tr>

  <tr>
    <td rowspan="3">Communication Protocols</td>
    <td>Southbound Communication</td>
    <td>Modbus RTU/TCP</td>
    <td>✅</td>
    <td>Built-in standard function</td>
  </tr>
  <tr>
    <td>Southbound Communication</td>
    <td>IEC 61850 MMS</td>
    <td>❌</td>
    <td>Requires ICD model import and configuration</td>
  </tr>
  <tr>
    <td>Northbound Communication</td>
    <td>IEC 103 / IEC 104 Protocol</td>
    <td>❌</td>
    <td>Requires protocol stack migration</td>
  </tr>

  <tr>
    <td rowspan="2">Human-Machine Interaction</td>
    <td>Local Monitoring</td>
    <td>Local parameter configuration and status monitoring</td>
    <td>✅</td>
    <td>Standard Web interface included</td>
  </tr>
  <tr>
    <td>Remote Monitoring</td>
    <td>Cloud platform data integration (UniEnergy)</td>
    <td>✅</td>
    <td>Standard MQTT interface</td>
  </tr>

  <tr>
    <td rowspan="2">Log and Maintenance</td>
    <td>Parameter Management</td>
    <td>Parameter read/write and setting group switching</td>
    <td>✅</td>
    <td>Built-in standard function</td>
  </tr>
  <tr>
    <td>Upgrade and Maintenance</td>
    <td>Remote firmware upgrade and log export</td>
    <td>✅</td>
    <td>Built-in standard function</td>
  </tr>
</tbody></table>
