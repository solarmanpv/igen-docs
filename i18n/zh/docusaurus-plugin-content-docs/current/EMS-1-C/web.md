---
title: Web 页面操作
description: todo
---

# Web 页面操作

## 1. 系统介绍

系统主要用于本地调试 EMS 设备，包含 EMS 设备的数据展示、警告故障报警、配置修改与指令下发、配置策略以及历史数据查看与导出。

- 本产品以 Web 形式展现与交互，支持 Windows、Linux、安卓（包括手机与平板）。
- 标准分辨率 1366*768，可自由放大 / 缩小浏览器，也可以在浏览器通过放大 / 缩小来自由调整。


:::info 浏览器要求
系统不支持 UC 浏览器，推荐使用谷歌浏览器。
:::

:::warning
- 请不要低于标准分辨率，否则将出现无法展示等问题。
- 请不要使用屏幕尺寸过小的设备，会导致部分内容展示不全。
:::

## 2. 登录步骤

### 2.1 网络链接

产品使用局域网网络通信，支持 Wi-Fi 或网口连接：

- Wi-Fi连接：在电脑的WiFi列表中选择设备默认的SSID (IGEN_WIFI)，输入密码（12345678）。
- 使用网口连接时，插入网关 LAN 口即可。

<img src={require("./img/lan_ports.png").default} />


### 2.2 登录 Web 界面

确保网络和网口连接正常，打开浏览器并输入以下地址访问 Web 上位机：

- Wi-Fi 连接登录地址：https://192.168.123.10:33333/index.html
- LAN 口登录地址：https://172.19.130.109:33333/index.html
- WAN 口登录地址：https://172.19.140.109:33333/index.html

通过网口连接设备时，需将电脑的 IP 地址设置至设备对应网口的同一 IP 网段，才能访问 Web 管理界面。

<img src={require("./img/login.png").default} width="600"/>

### 2.3 账号与密码

产品采用“一机一密”形式，每台产品均有其独立密码，且不能互用。账号及初始登录密码印在外壳标贴上，如下图所示：

- 账号：admin
- 密码：1234

<img src={require("./img/label.png").default} width="240"/>

首次登录请使用默认初始登录密码。登录后，Web 界面会强制修改密码，如下图所示。

<img src={require("./img/change_default_password.png").default} width="720"/>

:::warning
目前产品仅有一个登录账号，且无法添加多个账号，密码修改之后请保管好您的密码。
:::

## 3. 顶部状态栏

### 3.1 语言切换

Web 上位机当前支持中英文切换。点击 <img src={require("./img/language_icon.png").default} width="20" style={{verticalAlign: "middle"}}/> 语言选项，并从下拉列表中选择所需语言。

<img src={require("./img/select_language.png").default} width="720"/>

### 3.2 帮助

点击 <img src={require("./img/help_icon.png").default} width="20" style={{verticalAlign: "middle"}}/> 图标下载用户手册。

<img src={require("./img/download_guide.png").default} width="720"/>


### 3.3 消息通知

点击 <img src={require("./img/notification_icon.png").default} width="20" style={{verticalAlign: "middle"}}/> 图标查看已读和未读的消息。

单击**查看全部**可打开更多历史消息，同时支持**一键已读**操作。

<img src={require("./img/message1.png").default} width="720"/>
<img src={require("./img/message2.png").default} width="720"/>


### 3.4 注销

点击**注销登录**退回登录界面。

<img src={require("./img/logout.png").default} width="720"/>


## 4. 数据概览

总览界面包含五个数据板块，显示内容会根据系统是否配置充电桩/光伏而动态变化。  
① 当日数据以及累计数据  
② 近 7 日收益  
③ 当前的功率流向  
④ 当前的告警信息  
⑤ 当日的功率曲线，点击下方开关按钮，可暂时显示或隐藏曲线  

<img src={require("./img/dashboard.png").default} width="720"/>


## 5. 设备监控

### 5.1 PCS

此界面展示 PCS 的数据及状态。可点击右上角自定义配置按钮执行指令与配置。

<img src={require("./img/pcs1.png").default} width="720"/>

执行时需输入口令 1234。

<img src={require("./img/pcs2.png").default} width="720"/>

在特定条件下，可使用自定义配置指令来进行特定指令下发，具体界面如下，如需进行特殊操作可联系我方技术支持。

<img src={require("./img/pcs3.png").default} width="720"/>



### 5.2 BMS 

此界面展示BMS数据。切换顶部的选项卡查看BMS总览，簇级数据和单体数据。

- 簇级数据
  <img src={require("./img/bms1.png").default} width="720"/>

- 单体数据（分布图视图）
  <img src={require("./img/bms2.png").default} width="720"/>

- 单体数据（表格视图）
  <img src={require("./img/bms3.png").default} width="720"/>



### 5.3 电表

此界面展示电表数据。

<img src={require("./img/meter.png").default} width="720"/>

### 5.4 空调

此界面用于展示空调数据，以及管理空调配置。

<img src={require("./img/conditioner1.png").default} width="720"/>
<img src={require("./img/conditioner2.png").default} width="720"/>

## 6. 故障告警

故障告警界面可以查看当前仍未解决的故障以及历史出现过的故障。

另外还可通过设备、告警等级、告警状态、起止时间筛选，快速获取所需数据。

<img src={require("./img/alarm.png").default} width="720"/>

## 7. 历史数据

### 7.1 收益统计

界面展示历史收益数据，可查看选中日期起的近7天、整月或整年的记录并支持导出。

<img src={require("./img/revenue.png").default} width="720"/>

### 7.2 电量统计

此界面展示电量数据，可查看选中日期起的近7天、整月或整年的记录并支持导出。

<img src={require("./img/battery.png").default} width="720"/>

### 7.3 功率曲线

此界面展示功率变化曲线，支持按天查看并可导出数据。

<img src={require("./img/power.png").default} width="720"/>

### 7.4 PCS 曲线

此界面展示PCS变化曲线。支持按设备名称、日期选择查看并支持导出。**趋势分析**查看选中日期当天数据展示，**对比分析**查看选中日期当天和前一天数据展示。

<img src={require("./img/pcs.png").default} width="720"/>

### 7.5 BMS 曲线

此界面展示 BMS 数据曲线。支持按设备名称、日期选择查看并支持导出。**趋势分析**查看选中日期当天数据展示，**对比分析**查看选中日期当天和前一天数据展示。

<img src={require("./img/bms.png").default} width="720"/>

### 7.6 电池簇曲线

此界面展示电池簇数据曲线。支持按设备名称、第N簇、日期选择查看并支持导出。**趋势分析**查看选中日期当天数据展示，**对比分析**查看选中日期当天和前一天数据展示。

<img src={require("./img/batteries.png").default} width="720"/>

### 7.7 电池温度曲线

此界面展示电池温度变化曲线。支持按设备名称、第N簇、日期查看并支持导出。

<img src={require("./img/battery_temp.png").default} width="720"/>

### 7.8 电池电压曲线

此界面展示电池电压变化曲线。支持按设备名称、第N簇、日期查看并支持导出。

<img src={require("./img/battery_voltage.png").default} width="720"/>

### 7.9 电表报表

此界面展示电表充放电量数据。支持按设备名称、起止时间选择查看并支持导出。

<img src={require("./img/meter_energy.png").default} width="720"/>

## 8. 策略配置

### 8.1 策略展示

该界面展示当前运行的策略，并且可以通过选择日期来查看这一天运行时的各个功率数值和SOC曲线变化。最下方展示当日的策略、策略优先级以及时间段。

<img src={require("./img/strategy.png").default} width="720"/>

### 8.2 策略管理

策略管理界面如下图所示：

① 修改当月的选择。  
② 添加策略。  
③ 查看、编辑或删除已创建的所有策略。  

<img src={require("./img/strategy_management.png").default} width="720"/>

### 8.3 策略添加与修改

如下图所示，策略的添加/编辑界面中：

**① 基础信息**：每个策略类型均需填写

<table><tbody>
  <tr>
    <th>策略类型</th>
    <td>可以选择“新能源消纳策略”、“削峰填谷策略”、“AI策略”、“防逆流策略”、“需量管理策略”。</td>
  </tr>
  <tr>
    <th>策略模板</th>
    <td>用于快速填写下方所有数据，可使用预置的空白模板，也可从您已创建的同类模板中载入。</td>
  </tr>
  <tr>
    <th>调控单元</th>
    <td>选择当前策略需要调控的单元。</td>
  </tr>
  <tr>
    <th>策略名称</th>
    <td>填写策略的名称。</td>
  </tr>
</tbody>
</table>

**② 触发条件**

<table><tbody>
  <tr>
    <th>充电</th>
    <td>设置充电类型（电网追踪、固定模式）及阈值。如果选择固定模式，还需填写功率。</td>
  </tr>
  <tr>
    <th>放电</th>
    <td>设置放电类型（负荷追踪、固定模式）及阈值。如果选择固定模式，还需填写功率。</td>
  </tr>
</tbody>
</table>

**③ 边界条件**

<table><tbody>
  <tr>
    <th>SOC范围</th>
    <td>设置下限和上限。</td>
  </tr>
  <tr>
    <th>防逆流</th>
    <td>设置触发值、限制值，以及限制方式（允许充电，停止放电）。</td>
  </tr>
  <tr>
    <th>需量限制</th>
    <td>设置触发值、限制值，以及限制方式（允许充电，停止放电）。</td>
  </tr>
</tbody>
</table>

**④ 日期及优先级**

<table><tbody>
  <tr>
    <th>生效时段</th>
    <td>范围是00:00 ~ 24:00。</td>
  </tr>
  <tr>
    <th>时间范围</th>
    <td>可以添加任意多个不连续的范围。</td>
  </tr>
  <tr>
    <th>优先级</th>
    <td>P0~P9，最高优先级为P0。</td>
  </tr>
</tbody>
</table>

<img src={require("./img/strategy_modification.png").default} width="720"/>

## 9. 系统管理

### 9.1 基础信息

- 电站名称：填写电站名称。
- 电站地区：选择省市区。
- 详细地址：自行填写地址。
- 时区设置：范围UTC-12~UTC+12。
- 货币单位：目前仅有美元、欧元、人民币。

<img src={require("./img/basic_info.png").default} width="720"/>

### 9.2 设备管理

#### 9.2.1 单元管理

添加设备前，需设置单元以及名称。后续添加设备时，需根据单元类型选择设备。

<img src={require("./img/unit_management.png").default} width="720"/>

#### 9.2.2 设备列表

可通过单元和设备类型筛选查看。

<img src={require("./img/device_list.png").default} width="720"/>

**添加与编辑设备：**
- 所属单元：下拉框选项基于[单元管理配置](#921-单元管理)。
- 设备类型：根据所属单元类型发生变化。
- 设备名称：给设备命名。
- 设备厂家：设备的厂家。
- 通讯类型：目前支持 modbus-RTU、modebus-TCP、can、Dlt、ZVPP，所选协议类型将决定下方需填写的具体配置参数。各协议对应的参数要求如下：
  - modbus-RTU：COM、波特率、奇偶校验、数据位、停止位。
  - modebus-TCP、ZVPP：IP地址、端口号。
  - can：CAN口、波特率。
  - Dlt：Dlt地址。
  - 设备地址：设备的地址。

<img src={require("./img/device_modification.png").default} width="720"/>

### 9.3 网络配置

#### 9.3.1 WLAN

填写/修改SSID和密码。

<img src={require("./img/wlan.png").default} width="720"/>

#### 9.3.2 移动数据

- 月流量套餐：每月可使用流量（单位G）。
- 网络模式：自动、2G、3G、4G。
- APN模式：自动模式、手动模式。
- 身份认证类型：CHAP、手动模式。
- APN模式为手动时需要填写：APN、拨号号码、用于名称、用户密码。

<img src={require("./img/mobile.png").default} width="720"/>

#### 9.3.3 WAN

- 如果是自动获取IP，不用填写下面内容。
- 如果不是自动获取IP，需要填写：IP地址、子网掩码、网关地址、首选DNS服务器、备选DNS服务器。

<img src={require("./img/wan.png").default} width="720"/>

#### 9.3.4 LAN

配置 LAN 是否自动获取 IP。如果是手动获取，则需要填写 IP 地址、子网掩码、网关地址。

<img src={require("./img/lan.png").default} width="720"/>

### 9.4 转发配置

暂未开放

### 9.5 电价管理

#### 9.5.1 电网电价

按月/日查看电价。点击进入编辑模式进行编辑。
- 按月查看：下拉框选择年份。
- 按日查看：下拉框选择年份和月份。

<img src={require("./img/grid_price.png").default} width="720"/>

#### 9.5.2 光伏上网电价

修改光伏上网电价。

<img src={require("./img/pv_price.png").default} width="720"/>

#### 9.5.3 充电桩电价

修改充电桩电价。

<img src={require("./img/charging_pile_price.png").default} width="720"/>

#### 9.5.4 时段管理

① 根据年份筛选查看时间段数据。  
② 单击选中时段，下方时间轴色图会随着选中的时段改变。点击**添加**可以增加，点击**X**可以删除，点击右侧**编辑**可以修改。  
③ 显示①中选择的年份配置的时段以及它选择的时段。  
<img src={require("./img/price_period1.png").default} width="720"/>

④ 点击**配置**进入如下界面，可添加或编辑时段。该界面的时段对应上图②的列表。
<img src={require("./img/price_period2.png").default} width="720"/>

⑤ 点击**编辑**后进入如下界面（或者点击②的添加）。  
为模板命名，配置时间段，并从下拉框中选择“尖峰平谷”或“不计费”。保存后，新模板将显示在图②所示区域。

<img src={require("./img/price_period3.png").default} width="720"/>

#### 9.5.5 修改记录

列出所有修改记录。点击查看电价会展示和[9.5.1](#951-电网电价)相似的界面用于查看修改内容。

<img src={require("./img/price_history1.png").default} width="720"/>
<img src={require("./img/price_history2.png").default} width="720"/>


### 9.6 设备维护

#### 9.6.1 软件升级

1. 点击**上传**打开文件选择对话框，用于选择上传的升级文件。
   <img src={require("./img/upgrade1.png").default} width="720"/>

2. 选中设备之后，点击**升级**按钮开始升级。
   <img src={require("./img/upgrade2.png").default} width="720"/>

3. 开始升级的设备会更新目标版本和升级进度。在升级过程中，无法进行其他操作。

#### 9.6.2 安全设置

- 登录信息：修改当前用户登录密码。
- 内置WLAN信息：修改是否启用，以及设置SSID和密码。

<img src={require("./img/security.png").default} width="720"/>

#### 9.6.3 系统时间

- 时区设置：UTC-12 ~ UTC+12
- 日期与时间：填写日期以及时间
- 时钟源：NTP、管理系统、无

<img src={require("./img/system_time.png").default} width="720"/>

#### 9.6.4 点表管理

暂未开放

#### 9.6.5 系统维护

<img src={require("./img/maintenance.png").default} width="720"/>

#### 9.6.6 设备拓扑

如需查看或编辑设备拓扑，请点击此链接跳转至专用界面。本页面不提供直接操作功能。

<img src={require("./img/topology1.png").default} width="720"/>

查看与编辑界面：点击①的返回和确认按钮，以回到浏览界面。浏览界面没有左侧的各类元件，也无法操作和编辑，仅能查看。

<img src={require("./img/topology2.png").default} width="720"/>
