---
title: "区域及可用区"
description: test
draft: false
weight: 10
---

## 解释说明

### 区域

根据数据中心地理位置划分，不同区域间内网隔离，不能互相访问。

### 可用区

一个区域包括多个可用区，每个可用区都相互独立但网络互通，同一可用区内的主机网络延时更小。如果业务需要同城多活，建议您部署在不同可用区。详情请参考：[区域与可用区文档](https://docs.qingcloud.com/product/region/index)。

## 常见问题

<details>
<summary><p>
 1.如何选择区域？ </p></summary>
<p>
  建议靠近您的业务区域选择区域，可以减少网络时延，提高访问速度。另外，不同区域的资源价格可能有差异，您可以根据价格选择合适的区域。
  </p>
</details>

<details>
<summary><p>
  2.如何选择可用区？
  </p></summary>
<p>
  每个可用区都相互独立，规格相同。如果您初次创建资源，您可选择系统分配。如果您的业务需要同城多活，建议您将主机部署在不同可用区，通过同一个负载均衡器对外提供服务。如果您的云服务器之间需要较低的网络时延，则建议您将它们部署在相同的可用区内。
  </p>
</details>

<details>
<summary><p>
  3.不同区域或不同可用区的云服务器是否可以通过内网相互访问？
  </p></summary>
<p>
  不同区域的云服务器内网互不相通，如果有访问需求，您可以通过绑定公网IP通过公网相互访问或通过隧道服务访问。同区域内不同可用区的云服务器如果处在同一个多可用区部署的私有网络下，可以内网互通。
  </p>
</details>


<details>
<summary><p>
  4.云服务器是否支持区域/可用区迁移？
  </p></summary>
<p>
  不支持，云服务器购买后区域/可用区无法更换。如需迁移云服务器到其他区域，您可以将云服务器制作成镜像，通过跨区域复制将镜像复制到目标区域，再以该镜像创建云服务器，实现区域间的业务迁移。
  </p>
</details>





