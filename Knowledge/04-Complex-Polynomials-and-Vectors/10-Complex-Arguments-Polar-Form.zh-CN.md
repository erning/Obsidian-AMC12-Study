---
title: 复数辐角与极坐标形式
tags:
  - AMC12
  - 知识点
---

# 复数辐角与极坐标形式

## 辐角

非零复数 $z=x+iy$ 的辐角 $\theta$ 满足

$$
z=|z|(\cos\theta+i\sin\theta).
$$

所有辐角为

$$
\arg z=\theta+2k\pi.
$$

主辐角通常选在 $(-\pi,\pi]$ 或 $[0,2\pi)$，具体取决于题目约定。由点的象限判断 $\theta$ 的正负和参考角，不能只用 $\arctan(y/x)$ 而忽略象限。

## 辐角的乘法法则

对非零复数，

$$
\arg(zw)=\arg z+\arg w\pmod{2\pi},
$$

$$
\arg\left(\frac zw\right)
=\arg z-\arg w\pmod{2\pi}.
$$

幂满足

$$
\arg(z^n)=n\arg z\pmod{2\pi}.
$$

当题目要求某个象限或某个角度范围时，完成模 $2\pi$ 化简后再选代表值。

## 极坐标形式

$$
z=r\operatorname{cis}\theta
=r(\cos\theta+i\sin\theta).
$$

乘以 $r$ 是缩放，乘以 $\operatorname{cis}\phi$ 是旋转 $\phi$。因此复数乘法把长度和方向分离：

$$
|zw|=|z||w|,
\qquad
\arg(zw)=\arg z+\arg w.
$$

## 复数方程中的辐角

若

$$
z^n=w=R\operatorname{cis}\phi,
$$

则

$$
|z|=R^{1/n},
\qquad
\arg z=\frac{\phi+2k\pi}{n},
\quad k=0,\ldots,n-1.
$$

所有根在一个圆上等角分布。若只需其中一个根，仍要根据题目指定的象限或主辐角筛选。

## 共轭与辐角

若

$$
z=r\operatorname{cis}\theta,
$$

则

$$
\bar z=r\operatorname{cis}(-\theta).
$$

共轭反射复平面中的点到实轴另一侧，模长不变。

## 常见陷阱

- 用 $\arctan(y/x)$ 得到错误象限。
- 忘记辐角只在模 $2\pi$ 意义下确定。
- 求根时漏掉 $k=1,\ldots,n-1$ 的分支。
- 将实部、虚部与模长、辐角混淆。
- 角度模 $360^\circ$ 或模 $2\pi$ 后没有检查题目要求的代表范围。

## 关联题目

- [[Problems/2021-A/Q13.zh-CN.md|2021-A-Q13]]
- [[Problems/2021-B/Q18.zh-CN.md|2021-B-Q18]]
