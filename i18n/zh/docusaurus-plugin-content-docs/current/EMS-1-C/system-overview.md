---
title: 系统运行
description: todo
---

# 系统运行

## 1. 上电前检查

1. 正式上电前，用万用表确认电源输出电压是否在正常供电范围内。  
2. 固定好控制器电源连接器。  
3. 将线束连接器连接至对应接口。  
4. 将通讯端口连接器连接至对应接口。  
5. 系统正常供电。  

完成上述步骤后，可使用我司提供的上位机软件或观察 LED 指示灯状态，以验证控制器运行状态是否正常。

## 2. LED灯状态含义

<table><thead>
  <tr>
    <th>指示灯</th>
    <th>状态</th>
    <th>含义</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="3">ALM</td>
    <td>红灯灭</td>
    <td>无告警</td>
  </tr>
  <tr>
    <td>红灯慢闪</td>
    <td>系统发生提示/次要告警</td>
  </tr>
  <tr>
    <td>红灯常亮</td>
    <td>系统发生重要告警</td>
  </tr>
  <tr>
    <td rowspan="3">NET</td>
    <td>绿灯灭</td>
    <td>服务器连接异常</td>
  </tr>
  <tr>
    <td>绿灯慢闪</td>
    <td>服务器连接中</td>
  </tr>
  <tr>
    <td>绿灯常亮</td>
    <td>服务器连接正常</td>
  </tr>
  <tr>
    <td rowspan="2">PWR</td>
    <td>绿灯灭</td>
    <td>未上电/上电失败/系统程序异常</td>
  </tr>
  <tr>
    <td>绿灯常亮</td>
    <td>服务器连接正常</td>
  </tr>
  <tr>
    <td rowspan="4">4G</td>
    <td>绿灯灭</td>
    <td>4G未启用或者未检测到SIM卡</td>
  </tr>
  <tr>
    <td>绿灯快闪</td>
    <td>4G未连接或通信中断</td>
  </tr>
  <tr>
    <td>绿灯慢闪</td>
    <td>数据传输中</td>
  </tr>
  <tr>
    <td>绿灯常亮</td>
    <td>4G拨号成功</td>
  </tr>
</tbody>
</table>

> 说明：
> - 慢闪：1S亮，1S灭
> - 快闪：100mS亮，100mS灭