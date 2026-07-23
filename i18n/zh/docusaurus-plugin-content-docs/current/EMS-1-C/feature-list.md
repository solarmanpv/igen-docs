---
title: 功能清单
description: todo
---

# 功能清单

<table><thead>
  <tr>
    <th>功能大类</th>
    <th>功能模块</th>
    <th>具体功能点</th>
    <th>EMS-1-C</th>
    <th>备注</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="4">数据采集</td>
    <td>模拟量采集</td>
    <td>三相电压 / 电流 / 有功 / 无功 / 频率采集</td>
    <td>✅</td>
    <td>标准 Modbus 协议接入 DIO 采集</td>
  </tr>
  <tr>
    <td>模拟量采集</td>
    <td>电芯电压 / 温度 / SOC/SOH 采集</td>
    <td>✅</td>
    <td>支持簇级、PACK 级</td>
  </tr>
  <tr>
    <td>状态量采集</td>
    <td>开关状态、接触器状态、告警信号采集</td>
    <td>✅</td>
    <td>标准遥信接入</td>
  </tr>
  <tr>
    <td>电能计量</td>
    <td>累计充放电电量、峰平谷电量统计</td>
    <td>✅</td>
    <td>支持电表对接</td>
  </tr>
  <tr>
    <td rowspan="4">设备控制</td>
    <td>基础控制</td>
    <td>储能系统启停、充放电模式切换</td>
    <td>✅</td>
    <td>恒功率充放电等基础模式</td>
  </tr>
  <tr>
    <td>功率调节</td>
    <td>有功 / 无功功率指令下发</td>
    <td>✅</td>
    <td>支持 0~100% 连续调节</td>
  </tr>
  <tr>
    <td>并离网切换</td>
    <td>并网 / 离网模式切换控制</td>
    <td>⚙️</td>
    <td>需 PCS 支持</td>
  </tr>
  <tr>
    <td>多机并联</td>
    <td>多柜集群功率分配、均流控制</td>
    <td>✅</td>
    <td>站控级专属</td>
  </tr>
  <tr>
    <td rowspan="4">运行策略</td>
    <td>基础策略</td>
    <td>定时充放电、SOC 维持</td>
    <td>✅</td>
    <td>标准内置</td>
  </tr>
  <tr>
    <td>峰谷套利</td>
    <td>按时段电价自动充放电</td>
    <td>✅</td>
    <td>标准内置</td>
  </tr>
  <tr>
    <td>需量管理</td>
    <td>最大需量限制、削峰填谷</td>
    <td>✅</td>
    <td>标准内置</td>
  </tr>
  <tr>
    <td>防逆流</td>
    <td>光伏消纳、自发自用</td>
    <td>✅</td>
    <td>标准内置</td>
  </tr>
  <tr>
    <td rowspan="3">保护告警</td>
    <td>一级保护</td>
    <td>过压 / 欠压 / 过流 / 过温告警与停机</td>
    <td>✅</td>
    <td>故障停机，上报告警</td>
  </tr>
  <tr>
    <td>二级保护</td>
    <td>绝缘检测、漏液检测、烟雾浓度检测</td>
    <td>⚙️</td>
    <td>需接入对应传感器即可</td>
  </tr>
  <tr>
    <td>故障记录</td>
    <td>故障告警存储、运行数据、SOE 事件记录</td>
    <td>✅</td>
    <td>本地存储≥10000 条</td>
  </tr>
  <tr>
    <td rowspan="3">通信协议</td>
    <td>南向接入</td>
    <td>Modbus-RTU/TCP</td>
    <td>✅</td>
    <td>标准内置</td>
  </tr>
  <tr>
    <td>南向接入</td>
    <td>IEC 61850 MMS</td>
    <td>❌</td>
    <td>需导入 ICD 模型配置</td>
  </tr>
  <tr>
    <td>北向上传</td>
    <td>IEC103、104 规约</td>
    <td>❌</td>
    <td>需移植协议栈</td>
  </tr>
  <tr>
    <td rowspan="2">人机交互</td>
    <td>本地监控</td>
    <td>本地参数设置、状态查看</td>
    <td>✅</td>
    <td>标配 Web 页面</td>
  </tr>
  <tr>
    <td>远程监控</td>
    <td>云端平台数据对接（能睿）</td>
    <td>✅</td>
    <td>标准 MQTT 接口</td>
  </tr>
  <tr>
    <td rowspan="2">日志运维</td>
    <td>参数管理</td>
    <td>参数读写、定值组切换</td>
    <td>✅</td>
    <td>标准内置</td>
  </tr>
  <tr>
    <td>升级维护</td>
    <td>远程固件升级、日志导出</td>
    <td>✅</td>
    <td>标准内置</td>
  </tr>
</tbody></table>
