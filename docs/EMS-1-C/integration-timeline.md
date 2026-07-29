---
title: Integration Timeline
description: todo
---

# Integration Timeline

<table><thead>
  <tr>
    <th>Device Type</th>
    <th>Common Devices</th>
    <th>Integration Protocol</th>
    <th>Integration Timeline</th>
    <th>Remarks</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="3">Power Conversion System (PCS)</td>
    <td>Mainstream PCS Brands<br />(Standard Protocol)</td>
    <td>Modbus RTU/TCP<br />CAN</td>
    <td>3 days</td>
    <td>1. Requires register debugging and control logic verification</td>
  </tr>
  <tr>
    <td>Mainstream PCS Brands<br />(Non-standard Protocol)</td>
    <td>IEC 61850</td>
    <td>10–20 days</td>
    <td>
      1. Requires modeling, ICD import, and system integration testing<br />
      2. New protocol stack development is relatively complex and takes longer for the first migration<br />
      3. The timeline can be reduced by 50% for subsequent projects
    </td>
  </tr>
  <tr>
    <td>Niche / New PCS Brands<br />(Non-standard Protocol)</td>
    <td>Proprietary Custom Protocol</td>
    <td>10–15 days</td>
    <td>
      1. Requires register debugging and control logic verification<br />
      2. Protocols from niche brands may be less mature, resulting in longer debugging time
    </td>
  </tr>
  <tr>
    <td rowspan="2">Battery Management System (BMS)</td>
    <td>Mainstream BMS</td>
    <td>Modbus RTU/TCP<br />CAN</td>
    <td>3 days</td>
    <td>1. Standard data integration</td>
  </tr>
  <tr>
    <td>Customized BMS</td>
    <td>Proprietary Protocol</td>
    <td>3–5 days</td>
    <td>1. Requires custom integration development</td>
  </tr>
  <tr>
    <td>PV Inverter</td>
    <td>String / Central Inverter</td>
    <td>Modbus RTU/TCP</td>
    <td>2 days</td>
    <td>1. Standard data integration</td>
  </tr>
  <tr>
    <td>Energy Meter</td>
    <td>Multi-function Energy Meter</td>
    <td>Modbus RTU/TCP<br />DL/T645</td>
    <td>1 day</td>
    <td>1. Standard data integration</td>
  </tr>
  <tr>
    <td rowspan="2">Temperature Control System</td>
    <td>Liquid Cooling Unit</td>
    <td>Modbus RTU/TCP</td>
    <td>2 days</td>
    <td>1. Standard data integration</td>
  </tr>
  <tr>
    <td>Air Conditioner</td>
    <td>Modbus RTU/TCP</td>
    <td>2 days</td>
    <td>1. Standard data integration</td>
  </tr>
  <tr>
    <td rowspan="2">EV Charger</td>
    <td>Mainstream EV Chargers / Charging Stations</td>
    <td>Modbus RTU/TCP</td>
    <td>4 days</td>
    <td>1. Standard data integration and power scheduling</td>
  </tr>
  <tr>
    <td>Niche / New Brands EV Chargers</td>
    <td>Modbus RTU/TCP</td>
    <td>6–8 days</td>
    <td>1. Standard data integration and power scheduling</td>
  </tr>
  <tr>
    <td rowspan="2">Microgrid / Off-grid Applications</td>
    <td>Pure Microgrid (VF/VSG)</td>
    <td>Modbus RTU/TCP</td>
    <td>10 days</td>
    <td>1. Includes microgrid forming, islanding, frequency and voltage regulation logic</td>
  </tr>
  <tr>
    <td>Grid-connected / Off-grid Switching<br />Circuit Breaker / ATS / STS</td>
    <td>Modbus / Dry Contact</td>
    <td>10 days</td>
    <td>1. Includes interlocking and mode switching logic; high control complexity and mostly customized requirements</td>
  </tr>
  <tr>
    <td>Diesel Generator</td>
    <td>Generator Set</td>
    <td>Modbus RTU</td>
    <td>10 days</td>
    <td>1. Includes start/stop control and power matching</td>
  </tr>
  <tr>
    <td>Grid Dispatch</td>
    <td>Industrial Park / Grid Control Center</td>
    <td>IEC 104</td>
    <td>20–30 days</td>
    <td>
      1. Upstream integration with station-level control systems<br />
      2. First protocol migration requires longer development time<br />
      3. The timeline can be reduced by 50% for subsequent projects
    </td>
  </tr>
  <tr>
    <td>Third-party Platform</td>
    <td>Cloud Platform, Energy Management System</td>
    <td>MQTT / HTTP</td>
    <td>20–30 days</td>
    <td>
      1. Direct cloud integration is not recommended due to difficulties in after-sales support and upgrades<br />
      2. Cloud-to-cloud integration is recommended
    </td>
  </tr>
  <tr>
    <td rowspan="7">Strategy Algorithms</td>
    <td>Custom Charge/Discharge Strategy</td>
    <td>/</td>
    <td>/</td>
    <td rowspan="6">1. Existing standard algorithms generally do not require additional development</td>
  </tr>
  <tr>
    <td>Peak-Valley Arbitrage</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>Demand Management</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>Reverse Power Protection</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>Renewable Energy Utilization</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>Dynamic Transformer Capacity Expansion</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>Custom Strategy</td>
    <td>/</td>
    <td>/</td>
    <td>1. Custom algorithms or other complex non-standard applications require separate evaluation and discussion</td>
  </tr>
</tbody></table>
