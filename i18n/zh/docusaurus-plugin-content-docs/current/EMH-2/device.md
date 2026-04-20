---
title: 系统接入与设备管理
description: todo
---

# 系统接入与设备管理

## 1. 概述

固件架构平台是一套针对家庭能源管理中心进行监控和运维的本地系统，旨在帮助客户实现全面的设备实时运行状态、设备参数监视及展示，同时通过官方策略、自动化策略等功能提升能源利用率、舒服度、运维稳定性，实现精细化管理。

---

## 2. 登录与账户管理

### 2.1 账号获取

用户在首次使用时，可通过查看设备铭牌（设备机身底部）获取设备登录账号信息：
- 设备登录用户名
- 初始密码（默认密码）
- 设备序列号（SN）


### 2.2 登录 Web 页面

用户可通过浏览器访问设备本地 Web 页面进行系统登录，支持有线连接方式和局域网连接方式。

<img src={require("./img/web_login.png").default} width="960" /> 

import Tabs from '@theme/Tabs';
import TabItem from '@theme/TabItem';

<Tabs>
  <TabItem value="wire" label="1️⃣ 有线连接方式" default>
    1. 接通设备电源，并通过网线将设备 WAN 口与 PC WAN 口连接，确保两者处于同一局域网内  
    2. 在浏览器地址栏输入：http://169.254.254.254 ，并按下 Enter 键 
    3. 进入登录页面后，选择所在国家/地区 
    4. 输入用户名及密码，点击【登录】进入系统

  </TabItem>
  <TabItem value="wireless" label="2️⃣ 局域网连接方式">
    适用于设备已完成配网（通过 APP 接入网络）后的访问方式。
    
    操作步骤如下：
    1. 根据上一章APP使用步骤的介绍，在移动端APP中完成设备添加及网络配置
    2. 在APP中进入设备详情页面，查看设备当前 IP地址
    3. 确保PC与设备处于同一局域网环境（同一路由器下）
    4. 在浏览器地址栏输入设备IP地址（如：192.168.xxx.xxx）
    5. 输入用户名及密码，点击【登录】进入系统

    <img src={require("./img/app1.jpeg").default} width="240" /> 
    <img src={require("./img/app2.jpeg").default} width="240" /> 
    <img src={require("./img/app3.jpeg").default} width="240" /> 

    局域网访问方式依赖设备已成功联网，若无法访问，请优先检查设备网络状态或使用有线连接方式登录。
    
  </TabItem>
</Tabs>


:::warning
请谨慎选择国家，首次选择后不允许变更。
<img src={require("./img/select_country.png").default} width="240" /> 
:::

### 2.3 首次登录修改密码

为保障设备及账户安全，用户在首次登录系统时，需按照系统提示修改初始密码后方可继续使用。
<img src={require("./img/change_password.png").default} width="960" /> 


**功能说明**

首次登录后，系统将自动弹出“安全风险提示”窗口，要求用户完成密码修改操作。该步骤为强制流程，未完成修改将无法进入系统。

**操作步骤**

用户需依次填写以下信息：
- **旧密码**：输入当前登录所使用的初始密码 
- **新密码**：设置新的登录密码 
- **确认密码**：再次输入新密码以确认一致 

填写完成后，点击【确定】完成密码修改。


:::info 密码设置要求
建议密码满足以下要求：
- 包含大小写字母、数字及特殊字符 
- 长度不少于8位 
- 避免使用简单或常见密码（如123456、admin等） 
:::


:::warning
- 密码为设备管理的重要凭证，请务必妥善保管 
- 如遗忘密码，无法通过系统找回，仅可通过设备 **RESET** 按钮恢复出厂设置 
- 执行 RESET 操作后： 
    - 密码将恢复为初始密码 
    - 设备相关配置需要重新设置 
:::


:::tip
- 建议记录并安全保存密码信息 
- 可定期更换密码以提升系统安全性 
- 避免多人共享同一账号密码 
:::

密码修改成功后，系统将回到登录页面，重新输入新的用户名和密码后登录，用户可继续进行设备配置与管理操作。

### 2.4 忘记密码

在登录系统时，如用户忘记管理密码，可通过“**忘记密码**”查阅密码重置方法。
<img src={require("./img/forget_password.png").default} width="360" /> 



**功能说明**

点击登录页面的【忘记密码】入口后，系统将弹出密码重置提示窗口，引导用户通过设备本体进行密码恢复操作。

**重置方式**

当忘记管理密码时，可通过设备上的复位按钮恢复出厂密码：
- 找到设备机身上的 **RESET** 复位按钮 
- 使用针状工具长按 **5–10 秒** 
- 设备将恢复为出厂默认密码 

<img src={require("./img/reset_button.png").default} width="360" /> 


:::tip
- RESET 按钮通常位于设备侧面或底部（如上图所示） 
- 长按过程中请保持设备通电状态 
- 松开按钮后设备将自动完成重置 
:::


:::warning
- 恢复出厂设置后，原有自定义配置可能会丢失 
- 建议重置后及时重新设置密码，确保设备安全 
- 若多次操作无效，请检查设备状态或联系技术支持
:::

### 2.5 语言切换

在系统首页，将鼠标移动至 <img src={require("./img/language_icon.png").default} width="25" style={{verticalAlign: "middle"}}/> 上，在下拉菜单中选择语言。

<img src={require("./img/language.png").default} width="180" /> 

---

## 3. 设备接入配置

在系统中完成设备接入，是实现能源数据采集与管理的前提。用户可通过“添加设备”功能，将现场设备接入至平台进行统一管理。

### 3.1 添加设备（基础信息配置）

登录系统后，进入【**HEMS配置**】模块，在“**能源设备**”页签中点击右上角【**添加设备**】按钮，系统弹出“添加设备”窗口。

**页面功能说明**

1. 点击【**刷新支持清单**】，系统将更新当前支持接入的设备类型及型号列表，用于匹配最新设备库信息。
2. 用户需依次填写以下信息：

   | 参数 | 说明 |
   | ---- | ---- |
   | 设备类型 | 用于选择设备所属类别（如逆变器、电表、储能设备等），决定后续可选品牌及型号范围。    |
   | 设备品牌 | 选择设备制造商或品牌名称。     |
   | 设备型号 | 在所选品牌下，选择对应的设备型号。    |
   | 设备端口 | 指设备通信所使用的接口类型或通信通道（如RS485、P1、LAN、LoRa等），用于建立设备与系统之间的数据通信连接。    |


:::warning
- 请确保所选设备型号与实际设备一致，否则可能导致通信失败 
- 若未找到对应型号，可尝试点击“刷新支持清单”更新设备库 
- 设备端口需与实际接线方式及通信协议匹配 
- 建议在接入前确认设备已正常上电并具备通信条件
:::

### 3.2 通信参数设置

在完成设备基本信息选择后，点击【**下一步**】进入通信参数配置页面。本页面用于设置设备与系统之间的通信参数，是确保数据正常采集的关键步骤。
 
**参数说明**

:::note
该配置页面根据不同品牌型号设备会动态变化，以下为添加逆变器设备的参数案例。
:::

用户需根据设备实际通信配置，填写以下参数：

| 参数     | 说明                 |
| -------- | -------------------- |
| 波特率   | 表示通信传输速率，单位为 bps（如 1200、2400、4800、9600 等）。                                     |
| 校验位   | 用于数据校验的方式，常见包括：<br />- NONE（无校验）<br />- EVEN（偶校验）<br />- ODD（奇校验） |
| 数据位   | 表示每帧数据的有效数据位长度，常见为 5、6、7、8 位。                                              |
| 停止位   | 用于标识数据帧结束，常见为 1 或 2 位。                                                              |
| 通信地址 | 即设备在通信总线中的地址（如 Modbus 地址）<br /> **提示**：同一通信总线下地址必须唯一，通常默认为1，具体以设备实际设置为准。|
 
填写完成后，点击【**确定**】完成设备添加。如需修改前一步设备信息，可点击【上一步】返回。


:::warning
- 通信参数必须与设备实际设置完全一致，否则设备无法识别 
- 同一 RS485 总线中，**通信地址不可重复** 
- 若通信失败，优先检查： 
    - 波特率是否一致 
    - 地址是否正确 
    - 接线（A/B 极性）是否正确 

:::

:::info
若还需要添加设备，请重复以上动作，最大可添加设备为 **10** 台。
:::

### 3.3 设备接入结果与管理

完成设备添加及通信参数配置后，系统将返回“能源设备”列表页面，已接入设备将以卡片形式进行展示。

#### 设备状态说明

设备添加完成后，默认会显示在设备列表中，但部分功能（如数据查看）需在系统完成通信建立后才可使用。

用户可点击页面右上角<img src={require("./img/refresh_icon.png").default} width="50" style={{verticalAlign: "middle"}}/>，更新设备状态及功能入口。
 
<img src={require("./img/device_list.png").default} width="960" /> 

#### 设备卡片信息说明

每个设备以卡片形式展示，包含以下信息：
- 设备编号 / SN 
- 设备类型 
- 品牌信息 
- 设备型号 

用于快速识别当前已接入设备。

<img src={require("./img/device_card.png").default} width="360" /> 


#### 功能按钮说明

设备卡片底部提供多个操作入口：

**1️⃣ 编辑设备**<img src={require("./img/edit_icon.png").default} width="35" style={{verticalAlign: "middle"}}/>

功能说明：用于修改设备基础信息或通信参数配置。
 
<img src={require("./img/edit_device.png").default} width="360" /> 



**2️⃣ 设备数据查看**<img src={require("./img/view_icon.png").default} width="35" style={{verticalAlign: "middle"}}/>

功能说明：用于进入设备数据页面，查看设备运行数据及通信状态，也可针对当前设备下发控制指令。

:::tip
每种设备显示的数据指标因需求或设备类型有所不同。
:::
 
<img src={require("./img/device_info1.png").default} width="960" /> 
<img src={require("./img/device_info2.png").default} width="960" /> 
<img src={require("./img/device_info3.png").default} width="960" /> 

当设备成功建立通信后，系统将持续采集并更新设备运行数据，用户可通过设备详情页面进行实时监控与数据分析。


 
:::info
- <img src={require("./img/view_icon.png").default} width="35" style={{verticalAlign: "middle"}}/>需在点击【刷新】后才会显示 
- 若未显示，说明系统尚未完成设备通信建立或状态未更新 
:::


**3️⃣ 删除设备**<img src={require("./img/delete_icon.png").default} width="35" style={{verticalAlign: "middle"}}/>

功能说明：用于移除当前设备，删除后需重新添加才可恢复。

---


## 4. 网关设置

在【**HEMS配置**】模块中，进入“**网关设置**”页面，可查看并管理设备的网络连接状态。系统支持多种通信方式，包括 LTE、WLAN、WAN 和 LAN，用于满足不同场景下的联网需求。

<img src={require("./img/gateway_setting.png").default} width="960" /> 


### 4.1 功能概述

该页面以卡片形式展示当前设备的各类网络连接状态，用户可实时查看网络信息，并通过对应入口进行配置与调整。

页面右上角 <img src={require("./img/refresh_icon.png").default} width="50" style={{verticalAlign: "middle"}}/> 按钮用于更新当前网络状态信息。


### 4.2 网络类型说明

<Tabs>
  <TabItem value="lte" label="LTE" default>

    **蜂窝网络**

    用于通过移动通信网络实现设备联网，适用于无有线网络环境或需要远程部署的场景

    主要信息包括：
    - **信号强度**：当前蜂窝信号质量 
    - **SIM卡状态**：是否正常插入 
    - **IP地址**：当前分配的网络地址 

    点击 <img src={require("./img/setting_icon.png").default} width="25" style={{verticalAlign: "middle"}}/> 按钮配置：

    <img src={require("./img/lte_setting.png").default} width="480" /> 
  </TabItem>
  <TabItem value="wlan" label="WLAN">

    **无线网络**

    用于通过WiFi连接网络，适用于有无线网络覆盖的场景

    主要信息包括：
    - **信号强度**：WiFi信号质量 
    - **WiFi名称（SSID）**：当前连接的无线网络名称 
    - **IP地址**：连接后分配的地址 

    点击 <img src={require("./img/setting_icon.png").default} width="25" style={{verticalAlign: "middle"}}/> 按钮配置：

    <img src={require("./img/wlan_setting.png").default} width="480" /> 

  </TabItem>
  <TabItem value="wan" label="WAN">

    **广域网/有线网络**
    
    用于通过网线连接外部网络（如路由器）， 通常为优先推荐的稳定联网方式

    主要信息包括：
    - **连接状态**：是否已成功联网 
    - **IP获取方式**：如DHCP（自动获取） 
    - **IP地址 / 子网掩码 / 网关** 
    - **DNS / 备用DNS** 

    点击 <img src={require("./img/setting_icon.png").default} width="25" style={{verticalAlign: "middle"}}/> 按钮配置：

    <img src={require("./img/wan_setting.png").default} width="480" /> 

  </TabItem>
  <TabItem value="lan" label="LAN">

    **局域网接口**

    用于设备内部网络通信或本地调试。

    主要信息包括：
    - **连接状态**（如：尚未启动） 
    - **IP获取方式** 
    - **IP地址等网络参数** 

    点击 <img src={require("./img/setting_icon.png").default} width="25" style={{verticalAlign: "middle"}}/> 按钮配置： 

    <img src={require("./img/lan_setting.png").default} width="480" /> 

  </TabItem>
</Tabs>

### 4.3 操作说明

- 每个网络模块底部提供配置入口，可进入对应网络的详细设置页面 
- 用户可根据实际使用场景，启用或关闭对应网络方式 
- 建议仅启用一种主要联网方式，避免网络冲突 

### 4.4 状态说明

| 连接状态        | 颜色       | 说明                         |
| --------------- | ---------- | ---------------------------- |
| 已连接          | 绿色       | 表示网络正常，可进行数据通信 |
| 未启动 / 未连接 | 红色或灰色 | 表示当前网络不可用或未启用   |


:::warning
- 不同网络方式建议根据实际环境选择，避免同时启用多个主通信链路 
- 若网络异常，可点击 <img src={require("./img/refresh_icon.png").default} width="50" style={{verticalAlign: "middle"}}/> 刷新或检查对应网络配置 
- LTE 使用时需确保 SIM 卡正常插入且已开通数据服务 
:::


当网络连接正常后，设备可与云平台或本地系统建立通信，实现数据上传与远程管理功能。


## 5. 接入云服务

在【**HEMS配置**】模块中，进入“**接入云服务**”页面，可配置设备与云平台或第三方平台之间的通信连接，实现数据上云与远程管理功能。
 
<img src={require("./img/cloud_connection.png").default} width="960" /> 


### 5.1 功能概述

本页面用于管理设备的云接入状态，支持启用或关闭云服务，并配置对应的云平台连接参数。
当云服务开启后，设备可将运行数据上传至云端，实现远程监控、数据分析及平台联动。



### 5.2 页面说明

**1️⃣ 云服务开关**

开关位于页面顶部，用于控制设备是否启用云接入功能

- <img src={require("./img/cloud_enabled.png").default} width="100" style={{verticalAlign: "middle"}} /> 开启后：设备将尝试连接云平台
- <img src={require("./img/cloud_disabled.png").default} width="100" style={{verticalAlign: "middle"}} /> 关闭后：设备仅进行本地运行，不上传数据


**2️⃣ 第三方云服务列表**

页面下方展示当前支持接入的云平台信息，例如：
- **平台名称**：Solarman 
- **服务器地址**：access.solarmanpv.com 
- **通信协议**：MQTT 

每个云服务卡片底部提供 <img src={require("./img/setting_icon.png").default} width="25" style={{verticalAlign: "middle"}} /> 配置按钮 

- 开启：设备向该平台发送数据
- 关闭：不向该平台上传数据

**3️⃣ 配置入口**

右侧提供【云服务配置】按钮，用于进入云接入参数配置页面（如账号、密钥、Topic 等）

### 5.3 操作说明

1. 打开“**云服务**”开关 
2. 默认接入Solarman云平台
3. 若需要配置第三方云平台，点击【**云服务配置**】
4. 按要求填写相关参数（如服务器地址、认证信息等） 
5. 保存配置并返回 
 
<img src={require("./img/add_server.png").default} width="480" /> 

### 5.4 状态说明

| 状态 | 说明                         |
| ---- | ---------------------------- |
| 开启 | 设备尝试连接云平台并上传数据 |
| 关闭 | 设备仅本地运行，不进行云通信 |


:::warning
- 使用云服务前，请确保设备网络已正常连接（参考[网关设置](#4网关设置)） 
- 云平台地址及协议需与实际配置一致 
- 若连接失败，请检查： 
    - 网络是否正常 
    - 云平台参数是否正确 
    - 设备是否具备访问外网能力 
:::

当设备成功接入云服务后，用户可通过对应云平台或APP查看设备运行数据，实现远程监控与运维管理。

