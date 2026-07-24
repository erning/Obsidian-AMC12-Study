---
title: Heron 公式与内切圆半径
tags:
  - AMC12
  - 知识点
---

# Heron 公式与内切圆半径

## Heron 公式

三角形三边为 $a,b,c$，半周长为

$$
s=\frac{a+b+c}{2}.
$$

面积由 Heron 公式给出：

$$
\boxed{K=\sqrt{s(s-a)(s-b)(s-c)}}.
$$

使用前必须满足三角形不等式：

$$
|a-b|<c<a+b.
$$

若不满足，根式中的因子可能不对应非退化三角形。

## 内切圆半径

若内切圆半径为 $r$，则把三角形分成三个以 $r$ 为高的小三角形：

$$
K=\frac12ar+\frac12br+\frac12cr
=rs.
$$

因此

$$
\boxed{r=\frac Ks}.
$$

将 Heron 公式代入可得

$$
r=\sqrt{\frac{(s-a)(s-b)(s-c)}s}.
$$

这在已知三边求内切半径时很方便。

## 高与面积

以边 $a$ 为底，对应高为

$$
h_a=\frac{2K}{a}.
$$

三条高满足

$$
h_a:h_b:h_c=\frac1a:\frac1b:\frac1c.
$$

因此最短边对应最高的高，最长边对应最低的高。

## 特殊三角形

等边三角形边长为 $a$ 时：

$$
K=\frac{\sqrt3}{4}a^2,
\qquad
r=\frac{\sqrt3}{6}a,
\qquad
h=\frac{\sqrt3}{2}a.
$$

直角三角形两直角边为 $u,v$、斜边为 $w$ 时：

$$
K=\frac12uv,
\qquad
r=\frac{u+v-w}{2}.
$$

## 常见陷阱

- 把半周长 $s$ 写成周长。
- Heron 公式中漏掉某个 $(s-a)$ 因子。
- 没有先检查三角形不等式。
- 将内切半径误当成某条高。
- 已知面积和一条边时，忘记 $h=2K/a$。

## 关联题目

- [[Problems/2024-A/Q24.zh-CN.md|2024-A-Q24]]
- [[Problems/2024-B/Q24.zh-CN.md|2024-B-Q24]]
