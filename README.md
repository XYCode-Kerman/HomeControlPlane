# 家庭控制中心 | HomeControlPlane

家庭控制中心（HomeControlPlane）简称HCP，是一个基于MQTT和HTTP协议的智能家居控制中心。HCP在MQTT和HTTP协议的基础上定义了一种新的应用层协议HomeControlProtocol（简称HCPL）。HCPL是以**广泛兼容、便捷易用**为初衷而设计的，任何基于HCPL协议的智能家居设备均可介入HCP，实现多种功能。

## 安装

WIP

## HCPL协议

HTTP版本：[ApiFox文档](https://apifox.com/apidoc/shared-0617b72b-cc4c-413c-ae5e-4ebacf7c63df)

MQTT版本：已废弃

> 注：MQTT版本可通过发送如下JSON字符串到服务器实现等价于HTTP版本的功能。
>
> ```json
> {
>     "path": "HTTP版本的路径",
>     "method": "HTTP版本的请求方法（可选，默认GET）",
>     "headers": ["HTTP版本的请求headers（可选）"],
>     "payload": {"HTTP版本的": "请求负载"},
> }
> ```
>
> 返回等价于HTTP版本的返回。
