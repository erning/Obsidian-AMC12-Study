---
title: 多项式因式分解与恒等变形
tags:
  - AMC12
  - 知识点
---

# 多项式因式分解与恒等变形

## 常用恒等式

平方差：

$$
a^2-b^2=(a-b)(a+b).
$$

完全平方：

$$
a^2\pm2ab+b^2=(a\pm b)^2.
$$

立方和与差：

$$
a^3-b^3=(a-b)(a^2+ab+b^2),
$$

$$
a^3+b^3=(a+b)(a^2-ab+b^2).
$$

更一般地，

$$
x^n-y^n=(x-y)(x^{n-1}+x^{n-2}y+\cdots+y^{n-1}),
$$

而 $n$ 为奇数时 $x^n+y^n$ 可被 $x+y$ 整除。

## 因式定理与余式定理

若 $f(r)=0$，则 $x-r$ 是 $f(x)$ 的因子。若

$$
f(x)=(x-r)q(x)+s,
$$

则

$$
s=f(r).
$$

遇到“某个数是根”“除以某个一次式的余数”或“确定未知系数”时，先使用这两个定理，而不是完整展开。

## 换元与结构识别

复杂表达式常可设

$$
t=x+\frac1x,\qquad t=x^2+x+1,
$$

或把 $x^2$、$x^3$ 看成整体。换元后优先寻找平方差、完全平方和或低次多项式。

若出现

$$
x^4+ax^2+b,
$$

可令 $t=x^2$，化为关于 $t$ 的二次式，再检查 $t\ge0$。

## 交错和与等比结构

交错幂和常来自

$$
\frac{x^n+1}{x+1}
=x^{n-1}-x^{n-2}+\cdots-x+1
\qquad(n\text{ 为奇数}).
$$

先用等比和公式，再因式分解，常能把看似高次的式子转为连续区块或二进制幂的和。

## 根与因子

多项式的根和因子一一对应。若已知若干根 $r_1,\ldots,r_k$，则

$$
(x-r_1)\cdots(x-r_k)
$$

是多项式的因子。实系数多项式中的非实根必须同时出现共轭根，故对应实二次因子。

若整数多项式的首项系数为 $a$、常数项为 $c$，有理根 $p/q$（最简）满足

$$
p\mid c,\qquad q\mid a.
$$

## 恒等变形的检验

恒等式必须对所有定义域内的变量成立。可以：

- 展开两边并比较系数；
- 移到一边因式分解；
- 代入足够多的值作检查，但数值检查不能替代证明；
- 记录除法、根式和分母带来的限制。

若只在若干个根处相等，不能断言两个多项式恒等。

## 常见陷阱

- 只看最高次项就判断两个多项式相等。
- 因式分解时漏掉常数项或符号。
- 换元后忘记 $t$ 的范围，例如 $t=x^2\ge0$。
- 使用有理根定理时没有约分 $p/q$。
- 开平方或约分导致定义域改变，却没有保留排除值。

## 关联题目

- [[Problems/2024-A/Q01.zh-CN.md|2024-A-Q01]]
- [[Problems/2024-A/Q06.zh-CN.md|2024-A-Q06]]
- [[Problems/2024-A/Q09.zh-CN.md|2024-A-Q09]]
- [[Problems/2024-A/Q15.zh-CN.md|2024-A-Q15]]
- [[Problems/2024-A/Q17.zh-CN.md|2024-A-Q17]]
- [[Problems/2024-A/Q23.zh-CN.md|2024-A-Q23]]
- [[Problems/2025-A/Q17.zh-CN.md|2025-A-Q17]]
- [[Problems/2025-A/Q25.zh-CN.md|2025-A-Q25]]
- [[Problems/2025-B/Q03.zh-CN.md|2025-B-Q03]]
- [[Problems/2025-B/Q08.zh-CN.md|2025-B-Q08]]
- [[Problems/2023-A/Q12.zh-CN.md|2023-A-Q12]]
- [[Problems/2023-B/Q06.zh-CN.md|2023-B-Q06]]
- [[Problems/2023-B/Q14.zh-CN.md|2023-B-Q14]]
- [[Problems/2022-A/Q14.zh-CN.md|2022-A-Q14]]
- [[Problems/2022-A/Q15.zh-CN.md|2022-A-Q15]]
- [[Problems/2022-A/Q17.zh-CN.md|2022-A-Q17]]
- [[Problems/2022-A/Q21.zh-CN.md|2022-A-Q21]]
- [[Problems/2022-B/Q03.zh-CN.md|2022-B-Q03]]
- [[Problems/2022-B/Q04.zh-CN.md|2022-B-Q04]]
- [[Problems/2022-B/Q08.zh-CN.md|2022-B-Q08]]
- [[Problems/2022-B/Q14.zh-CN.md|2022-B-Q14]]
- [[Problems/2021-A/Q09.zh-CN.md|2021-A-Q09]]
- [[Problems/2021-A/Q12.zh-CN.md|2021-A-Q12]]
- [[Problems/2021-A/Q18.zh-CN.md|2021-A-Q18]]
- [[Problems/2021-A/Q20.zh-CN.md|2021-A-Q20]]
- [[Problems/2021-A/Q22.zh-CN.md|2021-A-Q22]]
- [[Problems/2021-B/Q10.zh-CN.md|2021-B-Q10]]
- [[Problems/2021-B/Q16.zh-CN.md|2021-B-Q16]]
- [[Problems/2021-B/Q20.zh-CN.md|2021-B-Q20]]
- [[Problems/2020-A/Q02.zh-CN.md|2020-A-Q02]]
- [[Problems/2020-A/Q09.zh-CN.md|2020-A-Q09]]
- [[Problems/2020-A/Q13.zh-CN.md|2020-A-Q13]]
- [[Problems/2020-A/Q15.zh-CN.md|2020-A-Q15]]
- [[Problems/2020-A/Q19.zh-CN.md|2020-A-Q19]]
- [[Problems/2020-B/Q02.zh-CN.md|2020-B-Q02]]
- [[Problems/2020-B/Q06.zh-CN.md|2020-B-Q06]]
- [[Problems/2020-B/Q08.zh-CN.md|2020-B-Q08]]
- [[Problems/2020-B/Q17.zh-CN.md|2020-B-Q17]]
- [[Problems/2020-B/Q20.zh-CN.md|2020-B-Q20]]
- [[Problems/2020-B/Q22.zh-CN.md|2020-B-Q22]]
