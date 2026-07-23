---
title: 适配周期
description: todo
---

# 适配周期

<table><thead>
  <tr>
    <th>设备类型</th>
    <th>常见设备</th>
    <th>接入协议</th>
    <th>适配周期</th>
    <th>备注</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="3">储能变流器</td>
    <td>主流品牌 PCS<br />（标准协议）</td>
    <td>Modbus RTU/TCP<br />CAN</td>
    <td>3 天</td>
    <td>1、需调试寄存器、验证控制逻辑</td>
  </tr>
  <tr>
    <td>主流品牌 PCS<br />（非标协议）</td>
    <td>IEC 61850</td>
    <td>10~20 天</td>
    <td>1、需建模、导入 ICD、联调<br />2、新协议栈较复杂，第一次移植耗时较长<br />3、后期可缩短50%周期</td>
  </tr>
  <tr>
    <td>小众 / 新品牌 PCS<br />（非标协议）</td>
    <td>私有定制协议</td>
    <td>10~15 天</td>
    <td>1、需调试寄存器、验证控制逻辑<br />2、小众品牌协议不成熟，坑多，调试耗时</td>
  </tr>
  <tr>
    <td rowspan="2">电池管理系统</td>
    <td>主流 BMS</td>
    <td>Modbus RTU/TCP<br />CAN</td>
    <td>3 天</td>
    <td>1、标准数据接入</td>
  </tr>
  <tr>
    <td>定制 BMS</td>
    <td>私有协议</td>
    <td>3~5 天</td>
    <td>1、需开发适配</td>
  </tr>
  <tr>
    <td>光伏逆变器</td>
    <td>组串式 / 集中式</td>
    <td>Modbus RTU/TCP</td>
    <td>2 天</td>
    <td>1、标准数据接入</td>
  </tr>
  <tr>
    <td>电表</td>
    <td>多功能电表</td>
    <td>Modbus RTU/TCP<br />DL/T645</td>
    <td>1 天</td>
    <td>1、标准数据接入</td>
  </tr>
  <tr>
    <td rowspan="2">温控系统</td>
    <td>液冷机组</td>
    <td>Modbus RTU/TCP</td>
    <td>2 天</td>
    <td>1、标准数据接入</td>
  </tr>
  <tr>
    <td>空调</td>
    <td>Modbus RTU/TCP</td>
    <td>2 天</td>
    <td>1、标准数据接入</td>
  </tr>
  <tr>
    <td rowspan="2">充电桩</td>
    <td>主流充电桩/充电站</td>
    <td>Modbus RTU/TCP</td>
    <td>4 天</td>
    <td>1、标准数据接入、功率调度</td>
  </tr>
  <tr>
    <td>小众 / 新品牌 充电桩</td>
    <td>Modbus RTU/TCP</td>
    <td>6～8 天</td>
    <td>1、标准数据接入、功率调度</td>
  </tr>
  <tr>
    <td rowspan="2">微网/离网应用</td>
    <td>纯微网（VF/VSG）</td>
    <td>Modbus RTU/TCP</td>
    <td>10 天</td>
    <td>1、微网构网、孤岛、调频调压等逻辑</td>
  </tr>
  <tr>
    <td>并离网切换<br />断路器 / ATS /STS</td>
    <td>Modbus / 硬接点</td>
    <td>10 天</td>
    <td>1、含联锁模式切换等逻辑、控制复杂度高、多为定制化需求</td>
  </tr>
  <tr>
    <td>柴油发电机</td>
    <td>发电机组</td>
    <td>Modbus RTU</td>
    <td>10 天</td>
    <td>1、含启动停止、功率匹配</td>
  </tr>
  <tr>
    <td>电网调度</td>
    <td>园区 / 电网主站</td>
    <td>IEC 104</td>
    <td>20~30 天</td>
    <td>1、站控级向上对接<br />2、第一次协议移植耗时较长<br />3、后期可缩短50%周期</td>
  </tr>
  <tr>
    <td>第三方平台</td>
    <td>云平台、能量管理系统</td>
    <td>MQTT/HTTP</td>
    <td>20~30 天</td>
    <td>1、不推荐边接云，无法售后维护和升级<br />2、推荐云云对接</td>
  </tr>
  <tr>
    <td rowspan="7">策略算法</td>
    <td>自定义充放</td>
    <td>/</td>
    <td>/</td>
    <td rowspan="6">1、已有标准算法一般无需另外开发</td>
  </tr>
  <tr>
    <td>峰谷套利</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>需量管理</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>防逆流</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>新能源消纳</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>变压器动态扩容</td>
    <td>/</td>
    <td>/</td>
  </tr>
  <tr>
    <td>定制策略</td>
    <td>/</td>
    <td>/</td>
    <td>1、定制算法或其它非标复杂应用，请单独评审沟通</td>
  </tr>
</tbody></table>
