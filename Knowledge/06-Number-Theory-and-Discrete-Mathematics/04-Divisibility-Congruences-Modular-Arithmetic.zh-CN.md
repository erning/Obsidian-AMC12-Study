---
title: 整除、同余与模运算
tags:
  - AMC12
  - 知识点
---

# 整除、同余与模运算

## 整除与同余

对整数 $a,b$，若存在整数 $k$ 使 $b=ak$，则记作 $a\mid b$。同余

$$
a\equiv b\pmod m
$$

等价于 $m\mid(a-b)$，也等价于 $a,b$ 除以 $m$ 的余数相同。模运算中可以安全地加、减和乘：

$$
a\equiv b\pmod m\Longrightarrow a+c\equiv b+c\pmod m,
$$

$$
ac\equiv bc\pmod m.
$$

因此可以在每一步把数替换成较小的余数。

## 最大公因数与逆元

欧几里得算法利用

$$
\gcd(a,b)=\gcd(b,a\bmod b)
$$

反复取余求最大公因数。扩展欧几里得算法还能找到整数 $x,y$，使

$$
ax+by=\gcd(a,b).
$$

当 $\gcd(a,m)=1$ 时，$a$ 在模 $m$ 下有逆元 $a^{-1}$，满足 $aa^{-1}\equiv1\pmod m$。此时同余方程 $ax\equiv b\pmod m$ 可以乘以逆元求解。

## 约分与中国剩余定理

从 $ac\equiv bc\pmod m$ 约去 $c$ 需要谨慎。若 $\gcd(c,m)=1$，可以直接约去；一般情况下只能得到

$$
a\equiv b\pmod{m/\gcd(c,m)}.
$$

若模数两两互质，系统

$$
x\equiv a_1\pmod{m_1},\quad x\equiv a_2\pmod{m_2},\quad\ldots
$$

由中国剩余定理在模 $m_1m_2\cdots$ 下有唯一解。解题时常先用小模数筛选，再代入剩余条件；若模数不互质，还需检查各条件在公共因子下是否相容。

## 整除性与周期

常用的十进制判别法包括：末位判断 $2$、$5$，末两位判断 $4$、$25$，末三位判断 $8$、$125$，各位数字和判断 $3$、$9$。对较长的数，也可以利用

$$
10^k\pmod m
$$

的周期，把数字按块处理。

幂模计算可反复平方并每一步取模。例如求 $a^{13}\pmod m$，写成 $13=8+4+1$，分别计算 $a^2,a^4,a^8$ 后相乘。若发现 $a^t\equiv1\pmod m$，指数可以按 $t$ 的周期化简，但必须确认周期确实适用于当前底数。

## 易错点

- 同余式中的“除法”不是普通分数约分；只有可逆元素才可以直接除。
- $a\equiv b\pmod m$ 不意味着 $a=b$，而是只在模 $m$ 的视角下相同。
- 余数应取标准范围 $0,1,\ldots,m-1$，负数取模时先改写成等价的正余数。
- 使用中国剩余定理前要检查模数是否互质，或检查不互质条件的相容性。

## 关联题目

- [[Problems/2024-A/Q11.zh-CN.md|2024-A-Q11]]
- [[Problems/2024-B/Q04.zh-CN.md|2024-B-Q04]]
- [[Problems/2024-B/Q14.zh-CN.md|2024-B-Q14]]
- [[Problems/2025-B/Q02.zh-CN.md|2025-B-Q02]]
- [[Problems/2025-B/Q05.zh-CN.md|2025-B-Q05]]
- [[Problems/2025-B/Q09.zh-CN.md|2025-B-Q09]]
- [[Problems/2025-B/Q19.zh-CN.md|2025-B-Q19]]
- [[Problems/2025-B/Q23.zh-CN.md|2025-B-Q23]]
- [[Problems/2023-A/Q03.zh-CN.md|2023-A-Q03]]
- [[Problems/2023-A/Q20.zh-CN.md|2023-A-Q20]]
- [[Problems/2023-A/Q22.zh-CN.md|2023-A-Q22]]
- [[Problems/2023-A/Q24.zh-CN.md|2023-A-Q24]]
- [[Problems/2023-B/Q15.zh-CN.md|2023-B-Q15]]
- [[Problems/2023-B/Q23.zh-CN.md|2023-B-Q23]]
- [[Problems/2023-B/Q24.zh-CN.md|2023-B-Q24]]
- [[Problems/2022-A/Q04.zh-CN.md|2022-A-Q04]]
- [[Problems/2022-A/Q16.zh-CN.md|2022-A-Q16]]
- [[Problems/2022-A/Q23.zh-CN.md|2022-A-Q23]]
- [[Problems/2022-B/Q03.zh-CN.md|2022-B-Q03]]
- [[Problems/2022-B/Q06.zh-CN.md|2022-B-Q06]]
- [[Problems/2022-B/Q15.zh-CN.md|2022-B-Q15]]
- [[Problems/2022-B/Q20.zh-CN.md|2022-B-Q20]]
- [[Problems/2022-B/Q23.zh-CN.md|2022-B-Q23]]
- [[Problems/2021-A/Q08.zh-CN.md|2021-A-Q08]]
- [[Problems/2021-A/Q25.zh-CN.md|2021-A-Q25]]
- [[Problems/2021-B/Q07.zh-CN.md|2021-B-Q07]]
- [[Problems/2021-B/Q25.zh-CN.md|2021-B-Q25]]
- [[Problems/2020-A/Q04.zh-CN.md|2020-A-Q04]]
- [[Problems/2020-A/Q08.zh-CN.md|2020-A-Q08]]
- [[Problems/2020-A/Q21.zh-CN.md|2020-A-Q21]]
- [[Problems/2020-B/Q04.zh-CN.md|2020-B-Q04]]
- [[Problems/2020-B/Q07.zh-CN.md|2020-B-Q07]]
- [[Problems/2020-B/Q21.zh-CN.md|2020-B-Q21]]
- [[Problems/2020-B/Q24.zh-CN.md|2020-B-Q24]]
