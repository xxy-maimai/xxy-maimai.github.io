+++
date = '2026-07-13T10:55:47+08:00'
draft = false
title = '带空气阻力下落运动v-t关系式推导'
+++

哎。心酸。本来在我朋友的博客上写过了一次这个东西。结果经历一周访问不了他也不修。我只能提着昨日种种千辛万苦。  
但是我居然™的从ai聊天记录里翻出来了这篇，虽然翻出来的计算结果是错的，但是我能再改改用。可惜的是还有两篇找不到。我还得自己写一遍。不过那两篇一个是高考题。一个是未解决的问题。无所吊谓说是。  
正文：  
我们受力分析：
$$mg-f=ma$$
将$f=\frac{1}{2}\rho Sv^2$代入，并且写为微分形式：
$$\frac{1}{m}(mg-\frac{1}{2}\rho Sv^2) = \frac{dv}{dt}$$
分离变量：
$$dt=\frac{m}{mg-\frac{1}{2}\rho Sv^2}\cdot dv$$
积分：
$$\int dt=\int \frac{m}{mg-\frac{1}{2}\rho Sv^2} dv$$
接下来处理积分问题。
$$\int \frac{m}{mg-\frac{1}{2}\rho Sv^2}dv=m\int\frac{1}{mg-\frac{1}{2}\rho Sv^2}dv$$
我们研究如下形式的积分：
$$\int \frac{1}{a-bv^2}dv=\int\left(\frac{A}{\sqrt{a}+\sqrt{b}v}+\frac{B}{\sqrt{a}-\sqrt{b}v}\right)dv$$
通分，得到$$\sqrt{a}(A+B)+\sqrt{b}v(B-A)=1$$
则
$$
\begin{cases}
\sqrt{a}\,(A+B)=1 \\ 
B-A=0
\end{cases}
$$
解得$$A=B=\frac{1}{2\sqrt{a}}$$
代回积分式，整理得到
$$\frac{1}{2\sqrt{ab}}\left(\int \frac{1}{v+\sqrt{\frac{a}{b}}}dv - \int \frac{1}{v-\sqrt{\frac{a}{b}}}dv\right)$$
积分并整理得到$$\frac{1}{2\sqrt{ab}}\ln\left|\frac{\sqrt{a}+\sqrt{b}v}{\sqrt{a}-\sqrt{b}v}\right|+C$$
代入$a=mg$，$b=\frac{1}{2}\rho S$得到原积分等于
$$t=\frac{m}{\sqrt{2\rho mgS}}\ln\left|\frac{\sqrt{2mg}+\sqrt{\rho S}v}{\sqrt{2mg}-\sqrt{\rho S}v}\right|$$
亦即
$$t=\frac{m}{\sqrt{2\rho mgS}}\ln\left|\frac{\sqrt{2mg}+\sqrt{\rho S}v}{\sqrt{2mg}-\sqrt{\rho S}v}\right|$$
推导完毕。  
P.S.反解的话，我懒得搞了。好像可以用反双曲正切搞？随便了。