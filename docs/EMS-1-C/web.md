---
title: Web Interface Operation
description: todo
---

# Web Interface Operation

## 1. System Overview

The system is mainly used for local debugging of C&I Energy Manager, including data display, warning and fault alarm, configuration modification and instruction issuance, configuration strategy, and historical data viewing and export.

- This product is displayed and interacted in web form and supports Windows, Linux, and Android (including mobile phones and tablets).
- The standard resolution is 1366*768, and you can freely zoom in/out the browser, or you can freely adjust it by zooming in/out in the browser.

:::info Browser
The system does not support UC Browser, and it is recommended to use Google Chrome.
:::

:::warning
- Please do not use a resolution lower than the standard resolution, otherwise, the content may not be displayed properly.
- Please do not use devices with too small a screen size, as this may result in incomplete display of some content.
:::

## 2. Login Steps

### 2.1 Network Links

The product uses LAN network communication and supports WiFi or network port connection:

- Wi-Fi connection: Select the device's default SSID (IGEN_WIFI) from the Wi-Fi list on your computer and enter the password (12345678).
- For network port connection, simply plug into the gateway's LAN port.

<img src={require("./img/lan_ports.png").default} />


### 2.2 Log in to the web interface

Make sure the network and network port are connected properly, open the browser and enter the following address to access the Web host computer:

- Wi-Fi connection login address: https://192.168.123.10:33333/index.html
- LAN port login address: https://172.19.130.109:33333/index.html
- WAN port login address: https://172.19.140.109:33333/index.html

When connecting to the device through a network port, you need to set the computer's IP address to the same IP network segment as the device's corresponding network port in order to access the Web management interface.

<img src={require("./img/login.png").default} width="600"/>

### 2.3 Account and Password

The product adopts the "one machine, one password" format. Each product has its own independent password and cannot be used interchangeably. The account number and initial login password are printed on the shell label, as shown below:

- Account: admin
- Password: 1234

<img src={require("./img/label.png").default} width="240"/>

Please use the default initial login password for the first time login. After logging in, the Web interface will force you to change your password, as shown below.

<img src={require("./img/change_default_password.png").default} width="720"/>

:::warning
Currently, the product has only one login account and multiple accounts cannot be added. Please keep your password safe after changing it.
:::

## 3. Top status bar

### 3.1 Language Switching

The Web host computer currently supports switching between Chinese and English. Click the <img src={require("./img/language_icon.png").default} width="20" style={{verticalAlign: "middle"}}/> language option and select the required language from the drop-down list.

<img src={require("./img/select_language.png").default} width="720"/>

### 3.2 Help

Click the <img src={require("./img/help_icon.png").default} width="20" style={{verticalAlign: "middle"}}/> icon to download the user manual.

<img src={require("./img/download_guide.png").default} width="720"/>


### 3.3 Message Notification

Click the <img src={require("./img/notification_icon.png").default} width="20" style={{verticalAlign: "middle"}}/> icon to view read and unread messages.

Click **View All** to open more historical messages, and one-click reading operation is also supported.

<img src={require("./img/message1.png").default} width="720"/>
<img src={require("./img/message2.png").default} width="720"/>


### 3.4 Logout

Click **Log out** to return to the login interface.

<img src={require("./img/logout.png").default} width="720"/>


## 4. Data Overview

The overview interface contains five data panels, and the displayed content will change dynamically depending on whether the system is configured with charging piles/photovoltaic.

① Mainly display the data of the day and the cumulative data  
② Mainly displays the earnings of the past 7 days  
③ Current power flow  
④ Current alarm information  
⑤ The power curve of the day. Click the switch button below to temporarily display or hide the curve.  

<img src={require("./img/dashboard.png").default} width="720"/>


## 5. Equipment Monitoring

### 5.1 PCS

This interface displays the data and status of the PCS. You can click the Customize button in the upper right corner to execute commands and configurations.

<img src={require("./img/pcs1.png").default} width="720"/>

The password 1234 is required for execution.

<img src={require("./img/pcs2.png").default} width="720"/>

Under certain conditions, you can use custom configuration instructions to issue specific instructions. The specific interface is as follows. If you need to perform special operations, please contact our technical support.

<img src={require("./img/pcs3.png").default} width="720"/>


### 5.2 BMS 

This screen displays BMS data. Switch the tabs at the top to view the BMS overview, cluster-level data, and cell data.

- Cluster-level data
  <img src={require("./img/bms1.png").default} width="720"/>

- Individual data (distribution chart view)
  <img src={require("./img/bms2.png").default} width="720"/>

- Single data (table view)
  <img src={require("./img/bms3.png").default} width="720"/>

### 5.3 Electricity Meter

This interface displays the electricity meter data.

<img src={require("./img/meter.png").default} width="720"/>

### 5.4 Air conditioner

This interface is used to display air conditioner data and manage air conditioner configuration.

<img src={require("./img/conditioner1.png").default} width="720"/>
<img src={require("./img/conditioner2.png").default} width="720"/>

## 6. Fault alarm

The fault alarm interface can view the current unresolved faults and historical faults.

In addition, you can filter by device, alarm level, alarm status, and start and end time to quickly obtain the required data.

<img src={require("./img/alarm.png").default} width="720"/>

## 7. Historical data

### 7.1 Revenue Statistics

The interface displays historical revenue data. You can view records for the past 7 days, a whole month, or a whole year from the selected date and support export.

<img src={require("./img/revenue.png").default} width="720"/>

### 7.2 Power statistics

This interface displays electricity consumption data. You can view records for the past 7 days, a whole month, or a whole year from the selected date and support export.

<img src={require("./img/battery.png").default} width="720"/>

### 7.3 Power curve

This interface displays the power change curve, supports daily viewing and data export.

<img src={require("./img/power.png").default} width="720"/>

### 7.4 PCS Curve

This interface displays the PCS change curve. You can select and view data by device name or date, and export it. **Trend analysis** displays data for the selected date, while **comparative analysis** displays data for the selected date and the previous day.

<img src={require("./img/pcs.png").default} width="720"/>

### 7.5 BMS curve

This interface displays BMS data curves. You can select and view data by device name or date, and export them. **Trend analysis** displays data for the selected date, while **comparative analysis** displays data for the selected date and the previous day.

<img src={require("./img/bms.png").default} width="720"/>

### 7.6 Battery cluster curve

This screen displays battery cluster data curves. You can select and view data by device name, cluster number, or date, and export them. **Trend analysis** displays data for the selected date, while **comparative analysis** displays data for the selected date and the previous day.

<img src={require("./img/batteries.png").default} width="720"/>

### 7.7 Battery temperature curve

This interface displays the battery temperature curve. You can view and export the data by device name, cluster N, or date.

<img src={require("./img/battery_temp.png").default} width="720"/>

### 7.8 Battery voltage curve

This interface displays the battery voltage curve. You can view and export the curve by device name, cluster N, or date.

<img src={require("./img/battery_voltage.png").default} width="720"/>

### 7.9 Electricity meter report

This interface displays meter charge and discharge data. You can select and view data by device name, start and end time, and export it.

<img src={require("./img/meter_energy.png").default} width="720"/>

## 8. Policy Configuration

### 8.1 Strategy Display

This interface displays the currently running strategy, and you can view the power values and SOC curve changes during the day by selecting a date. The bottom shows the strategy, strategy priority, and time period for the day.

<img src={require("./img/strategy.png").default} width="720"/>

### 8.2 Policy Management

The policy management interface is shown in the figure below:  

① Modify the selection for the current month.  
② Add a policy.  
③ View, edit, or delete all created policies.  

<img src={require("./img/strategy_management.png").default} width="720"/>

### 8.3 Policy addition and modification

As shown in the figure below, in the policy add/edit interface:

**① Basic information**: Each strategy type must be filled in

<table><tbody>
  <tr>
    <th>Strategy Type</th>
    <td>You can choose "new energy consumption strategy", "peak shaving and valley filling strategy", "AI strategy", "anti-back flow strategy" and "demand management strategy".</td>
  </tr>
  <tr>
    <th>Policy Templates</th>
    <td>It is used to quickly fill in all the data below. You can use the preset blank template or load a similar template you have created.</td>
  </tr>
  <tr>
    <th>Control unit</th>
    <td>Select the unit that needs to be regulated by the current policy.</td>
  </tr>
  <tr>
    <th>Policy Name</th>
    <td>Enter a name for the policy.</td>
  </tr>
</tbody>
</table>

**② Trigger conditions**

<table><tbody>
  <tr>
    <th>Charge</th>
    <td>Set the charging type (grid tracking, fixed mode) and threshold. If you choose fixed mode, you also need to enter the power.</td>
  </tr>
  <tr>
    <th>Discharge</th>
    <td>Set the discharge type (load tracking, fixed mode) and threshold. If you select fixed mode, you also need to enter the power.</td>
  </tr>
</tbody>
</table>

**③ Boundary conditions**

<table><tbody>
  <tr>
    <th>SOC range</th>
    <td>Set lower and upper limits.</td>
  </tr>
  <tr>
    <th>Anti-back flow</th>
    <td>Set the trigger value, limit value, and limit method (allow charging, stop discharging).</td>
  </tr>
  <tr>
    <th>Demand limitation</th>
    <td>Set the trigger value, limit value, and limit method (allow charging, stop discharging).</td>
  </tr>
</tbody>
</table>

**④ Date and priority**

<table><tbody>
  <tr>
    <th>Effective period</th>
    <td>The range is 00:00 ~ 24:00.</td>
  </tr>
  <tr>
    <th>Time range</th>
    <td>You can add as many non-contiguous ranges as you like.</td>
  </tr>
  <tr>
    <th>Priority</th>
    <td>P0~P9, the highest priority is P0.</td>
  </tr>
</tbody>
</table>

<img src={require("./img/strategy_modification.png").default} width="720"/>

## 9. System Management

### 9.1 Basic Information

- Power station name: Enter the power station name.
- Power plant region: Select a province, city, or district.
- Detailed address: Fill in the address by yourself.
- Time zone setting: range: UTC-12 ~ UTC+12.
- Currency unit: Currently only US dollar, euro and RMB.

<img src={require("./img/basic_info.png").default} width="720"/>

### 9.2 Device Management

#### 9.2.1 Unit Management

Before adding a device, you need to set the unit and name. When adding devices later, you need to select the device based on the unit type.

<img src={require("./img/unit_management.png").default} width="720"/>

#### 9.2.2 Equipment List

You can filter and view by unit and device type.

<img src={require("./img/device_list.png").default} width="720"/>

**Adding and editing devices:**
- Unit: The options in the drop-down box are based on the [unit management configuration](#921-unit-management).
- Equipment Type: Varies according to the type of unit it belongs to.
- Device Name: Give the device a name.
- Equipment Manufacturer: The manufacturer of the equipment.
- Communication type: Currently supports modbus-RTU, modebus-TCP, CAN, DLT, ZVPP. The selected protocol type will determine the specific configuration parameters to be filled in below. The parameter requirements corresponding to each protocol are as follows:
  - Modbus-RTU: COM, baud rate, parity, data bits, stop bits.
  - Modbus-TCP, ZVPP: IP address, port number.
  - can: CAN port, baud rate.
  - Dlt: Dlt address.
- Device Address: The address of the device.

<img src={require("./img/device_modification.png").default} width="720"/>

### 9.3 Network Configuration

#### 9.3.1 WLAN

Enter/modify the SSID and password.

<img src={require("./img/wlan.png").default} width="720"/>

#### 9.3.2 Mobile data

- Monthly data package: the amount of data available per month (unit: GB).
- Network mode: Auto, 2G, 3G, 4G.
- APN mode: automatic mode, manual mode.
- Authentication type: CHAP, manual mode.
- When the APN mode is manual, you need to fill in: APN, dial-up number, user name, and user password.

<img src={require("./img/mobile.png").default} width="720"/>

#### 9.3.3 WAN

- If you obtain the IP automatically, you do not need to fill in the following content.
- If the IP address is not obtained automatically, you need to fill in: IP address, subnet mask, gateway address, preferred DNS server, and alternative DNS server.


#### 9.3.4 LAN

Configure whether to automatically obtain IP addresses. If you manually obtain IP addresses, you need to enter the IP address, subnet mask, and gateway address.

<img src={require("./img/lan.png").default} width="720"/>

### 9.4 Forwarding Configuration

Not currently available.

### 9.5 Electricity Price Management

#### 9.5.1 Grid electricity prices

View electricity prices by month/day. Click to enter edit mode to edit.
- View by month: Select a year from the drop-down box.
- View by day: Select the year and month from the drop-down box.

<img src={require("./img/grid_price.png").default} width="720"/>

#### 9.5.2 Photovoltaic grid-connected electricity price

Modify the photovoltaic grid-connected electricity price.

<img src={require("./img/pv_price.png").default} width="720"/>

#### 9.5.3 Charging pile electricity price

Modify the electricity price of charging piles.

<img src={require("./img/charging_pile_price.png").default} width="720"/>

#### 9.5.4 Time period management

① Filter and view time period data by year.  
② Click to select a time period. The timeline color chart below will change according to the selected time period. Click **Add** to add, click **X** to delete, and click **Edit** on the right to modify.  
③ Displays the time period configured for the year selected in ① and the time period it selected.  

<img src={require("./img/price_period1.png").default} width="720"/>

④ Click **Configure** to enter the following interface, where you can add or edit time periods. The time periods on this interface correspond to the list in Figure ② above.

<img src={require("./img/price_period2.png").default} width="720"/>

⑤ Click **Edit** to enter the following interface (or click Add in ②).

Name the template, configure the time period, and select "Peak/Off-peak" or "No charge" from the drop-down box. After saving, the new template will be displayed in the area shown in Figure ②.

<img src={require("./img/price_period3.png").default} width="720"/>

#### 9.5.5 Modification Record

List all modification records. Clicking View Electricity Price will display an interface similar to [9.5.1](#951-grid-electricity-prices) for viewing modification contents.

<img src={require("./img/price_history1.png").default} width="720"/>
<img src={require("./img/price_history2.png").default} width="720"/>


### 9.6 Equipment maintenance

#### 9.6.1 Software upgrade

1. Click **Upload** to open the file selection dialog box for selecting the upgrade file to upload.
   <img src={require("./img/upgrade1.png").default} width="720"/>

2. After selecting the device, click the **Upgrade** button to start the upgrade.
   <img src={require("./img/upgrade2.png").default} width="720"/>

3. The device that starts the upgrade will update the target version and upgrade progress. During the upgrade process, no other operations can be performed.


#### 9.6.2 Security Settings

- Login information: Modify the current user's login password.
- Built-in WLAN information: Modify whether to enable, and set the SSID and password.

<img src={require("./img/security.png").default} width="720"/>

#### 9.6.3 System time

- Time zone setting: UTC-12 ~ UTC+12
- Date and time: Fill in the date and time
- Clock source: NTP, management system, none

<img src={require("./img/system_time.png").default} width="720"/>

#### 9.6.4 Point table management

Not currently available.

#### 9.6.5 System Maintenance

<img src={require("./img/maintenance.png").default} width="720"/>

#### 9.6.6 Device topology

If you need to view or edit the device topology, please click this link to jump to the dedicated interface. This page does not provide direct operation functions.

<img src={require("./img/topology1.png").default} width="720"/>

View and edit interface: Click the return and confirmation buttons in ① to return to the browsing interface. The browsing interface does not have the various components on the left, and cannot be operated or edited. It can only be viewed.

<img src={require("./img/topology2.png").default} width="720"/> -->
