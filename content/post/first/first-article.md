---
date: 2020-03-01
title: Traffic Flow Dynamics读书笔记系列：总是觉得旁边的车开得更快？这是错觉吗？
authors: ["admin"]
links:
  - icon_pack: fab
    icon: weixin
    name: Follow
    url: 'https://mp.weixin.qq.com/s?__biz=MzI1MTUzMDUxMw==&mid=2247483691&idx=1&sn=3946b69168dbff47388c3a1f419b498b&chksm=e9f0dd55de875443fbb46aa4c9aee5a5e0c7ef8b931f596cb531bfc9179c4353bc670f715a01&mpshare=1&scene=1&srcid=&sharer_sharetime=1582970236000&sharer_shareid=dac10d352441ca68e744ca96ba7dc1c0&key=068cf6e98cf9479cf197eb56cf0ec6a65ac51c9e9f95feac3f1cc06ca23688a280e7606f661bfa32ea941bcdea255cd4c3e6ad25dfd8a6aee36c0c4b4d9486bbb077156f9303534bc266cbd52465cd1a&ascene=1&uin=MjUzMzA0MDcwNw%3D%3D&devicetype=Windows+10&version=62080079&lang=zh_CN&exportkey=AeZJwCT3gTjEjcZ1NjfDnuc%3D&pass_ticket=%2FbS0zO1Ubxo93nmUvqf0F50jOcyHTVeGGpLAsEhkZLuhEMfBPq51YTxzlXrWKtnn'
---
总是觉得旁边的车开得更快？这是错觉吗？
=============================
```
Zhang Xiaohui 发自 加里敦
Traffic Flow Dynamics读书笔记系列 | 公众号 通达四方
```

在拥堵的车流中走走停停，旁边车道的车却总能呼啸而过，这可能是很多人曾经遇到过的情境。

然而这到底是错觉还是事实，其中是否蕴含科学道理？

<img src="https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/tan-kaninthanond-VEVfbQtyB8s-unsplash.jpg" alt="real jam" style="zoom:80%;" />

是的，这是错觉，不然哪需要我写这么多:upside_down_face:

其实在1999年，Nature就曾有一篇短篇通讯讨论过这个问题。

作者来自斯坦福大学的HRP(Departments of Health Research and Policy and of Statistics)。

<img src="https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/nature.PNG" alt="nature" style="zoom:80%;" />

可能是作者研究领域的原因，文中对此交通现象的原理并未从交通学科的角度深度挖掘。

因此本文分别从**交通工程学**与**心理生理学**的角度来进行完整的剖析。

## 交通流理论：陷入拥堵的时间总是更多

试想如下两车道场景，存在长度为$L$的交错交通波，灰色部分（记为区域1）以平均速度$V_{1}$缓慢前进。

灰色部分之间的区域2则以一更快的平均速度$V_{2}$前进，即$V_{2}>V_1$。

但两类区域均为拥堵状态（区域2并不是自由流）。

![jam](https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/%E4%BA%A4%E9%94%99.png)

假设此场景的宏观基本图为典型的三角形，且速度调整时间忽略不计（可以认为相应跟驰模型为OVM或是Newell模型）。

因此区域1和区域2分别对应基本图中箭头所示的两点。

![fd](https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/%E5%9F%BA%E6%9C%AC%E5%9B%BE%20%5B2%5D.png)

根据交通波理论，从区域1传至区域2的波速$c$为一恒定值，假定为$-5m/s^2$，即图中的两点连线的斜率。
$$
c=\frac{Q_2-Q_1}{\rho_2-\rho_1}=-5m/s^2
$$
注意到斜率为负数，即此阻塞波的传播方向与车辆行驶方向相反，如下图所示。

![wave](https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/jam.gif)

因此车辆在区域$1$的相对速度为$V_1+|c|$，相应的于区域$1$中渡过的时间为$\tau_1=\frac{L}{V_1+|c|}$。

同理车辆在区域$2$的相对速度为$V_2+|c|$，相应的于区域$2$中渡过的时间为$\tau_2=\frac{L}{V_2+|c|}$。

同时假定$V_1=0$，$V_2=10m/s^2$，因此整体行程时间中挤在拥堵区域的比例为：
$$
\frac{\tau_1}{\tau_1+\tau_2}=\frac{v_2+|c|}{v_1+v_2+2|c|}=\frac{3}{4}
$$
> 即对于任意一辆车来说，在整个行程中有超过50%的时间是陷入缓慢的“爬行”中的。

而两条车道的平均速度是相同的，即使换道也会落入该车道的交通波中，最后的行程时间毫无差别。

因此总觉得旁边车道更快是不符合交通流理论的。



## 心理生理学：视线中的错觉

从生理学的视角来看，人类在驾驶时，视线总是向前的。

![sight](https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/why-kei-8e2gal_GIE8-unsplash.jpg)

所超越的车辆很快会消失在视野中，而超越本车的车辆仍会在视线中留存一段更长的时间。

同时，人们在拥挤交通流中缓慢前行的闲暇时总是会看向相邻车道。

而从心理学的角度来说，人们对于被超越带来的失落感往往大于超车带来的快感。

![loss](https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/marcos-paulo-prado-_aRzwAI1ZeM-unsplash.jpg)

综上才会认为旁边的车道总是比本车道更快。

正如古语所说，这山望着那山高，“ The Grass is Always Greener on the Other Side”。

![grass](https://raw.githubusercontent.com/tjzxh/pics-of-blog/master/phil-goodwin-Ys85uMksDHc-unsplash.jpg)

## Reference

Traffic Flow Dynamics：\
http://www.traffic-flow-dynamics.org/#trafficFlowDynamicsPage

Why cars in the next lane seem to go faster：\
https://www.nature.com/articles/43360

--- **完** ---