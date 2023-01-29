<head>
  <script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
  <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
      tex2jax: {
      skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
      inlineMath: [['$','$']]
      }
    });
  </script>
</head>

[定义](#1-定义)

[定积分一般性质](#2-定积分一般性质)

[基本定理](#3-定积分基本定理)

[定积分特殊性质](#4-定积分特殊性质)

# 第五章：定积分及其应用

## §1 定义
设 $f(x)$ 在 $[a,b]$ 上有界，$\lambda = max${$\xi_1,\xi_2,...,\xi_n$},则 $\lim_{\lambda \to 0}f(\xi _i)\Delta \xi_i$ 为 $f(x)$ 在 $[a,b]$ 上的积分。

## §2 定积分一般性质
- $\int^a_af(x)dx=0$

- $\int^b_af(x)dx=-\int^a_bf(x)dx$

- $\int^b_af(x)+g(x)dx=\int^b_af(x)dx+\int^b_ag(x)dx$

- $\int^b_amf(x)dx=m\int^b_af(x)dx$

- $\int^c_af(x)dx=\int^b_af(x)dx+\int^c_bf(x)dx$

- **几何性质**

  $$\begin{cases}
      f(x)\geq 0,\int^b_af(x)dx=s\\
      f(x)\leq 0,\int^b_af(x)dx=-s
  \end{cases}$$

  $f(x)$ 有正有负的时候 $\int^b_af(x)dx=s_正-s_负$

- $f(x),g(x)$ 在 $[a,b]$ 可积，且 $f(x)>g(x)$ ，则 $\int^b_af(x)dx>\int^b_ag(x)dx$

- $f(x),\lvert f(x)\rvert$ 在 $[a,b]$ 可积$\rightarrow \lvert\int^b_af(x)dx\rvert\leq \int^b_a\lvert f(x)\rvert dx$

- **积分中值定理**

  $f(x) \in [a,b],f(x) $ 在 $[a,b]$ 可积，一定存在$\xi \in [a,b] \rightarrow \int^b_af(x)dx=f(\xi)(b-a)$

![](../pic/Chapter5.1.jpg)

## §3 定积分基本定理

- **积分中值定理推论(拉格朗日版）**

  $f(x) \in [a,b],f(x) $ 在 $[a,b]$ 可积，一定存在$\xi \in (a,b)\rightarrow \int^b_af(x)dx=f(\xi)(b-a)$

  **例题**
  $f(x) \in c[0,1],f(x)$在$(0,1)$可导$,f(0)=\int^1_0f(x)dx,$证明：$\exists \xi \in (0,1),f'(\xi)=0$

  [答案](../pic/Chaper5.3.jpg)

- 牛顿莱布尼兹定理
  $\int^b_af(x)dx=F(b)-F(a)$

## §4 定积分特殊性质
- $f(x)$ 在 $[0,1]$ 上可积

  $$\lim_{n \to \infty}\frac 1 n \displaystyle \sum^n_{i=1}f(\frac {i-1} n)=\lim_{n \to \infty}\frac 1 n \displaystyle \sum^n_{i=1}f(\frac i n)=\int^1_0f(x)dx$$

  注意$x=\frac i n$,这个只能在分子分母皆齐，分母比分子高一次的情况下使用

  **例题**

  $$\lim_{n \to \infty}\frac{1^2+2^2+...+n^2}{n^3}$$

  [答案](../pic/Chapter5.2.jpg)
  
- **$\int^a_{-a}f(x)dx=\int^a_0f(x)+f(-x)dx$**

- **$\int^{\frac \pi 2}_0f(sinx)dx=\int^{\frac \pi 2}_0f(cosx)dx$**
  
  **例题**
  $\int^1_0\frac 1 {x+\sqrt{1-x^2}}dx$

  [答案](../pic/Chapter5.6.jpg)

- $I_n=\int^{\frac \pi 2}_0sin^nxdx=\int^{\frac \pi 2}_0cos^nxdx$

  $$\begin{cases}
    I_n=\frac{n-1}nI_{n-2}\\
    I_0=\frac{\pi}{2}\\
    I_1=1
  \end{cases}$$

  例如：$I_4=\frac{3}{4} * \frac{1}{2} * \frac{\pi}{2}$

  **例题**：$\int^{\frac{\pi}2}_{-\frac{\pi}2}(\frac{sin^4x}{1+e^x})dx$

  [答案](../pic/Chapter5.7.jpg)

- $\int^{\pi}_0f(sinx)dx=2\int^{\frac{\pi}2}_0f(sinx)dx$

- $\int^{\pi}_0xf(sinx)dx=\frac{\pi}2\int^{\pi}_0f(sinx)dx$

- $f(x)$是以T为周期的可积函数，则：

  $$\begin{cases}
    \int^{a+T}_af(x)dx=\int^{T}_0f(x)dx\\
    \int^{nT}_0f(x)dx=n\int^{T}_0f(x)dx
  \end{cases}$$

## §5 问题类型
- 变积分线问题：
  
  **例题**：$f(x)$连续，$F(x)=\int^x_0(x-t)^2f(t)dt$，求$F''(x)$

  [答案](../pic/Chapter5.4.jpg)

  **例题**：$f(x)$连续，$f(0)=0,f'(0)=\pi,$求

  $$\lim_{x \to 0}\frac{\int^x_0tf(x^2-t^2)dt}{x^4}$$

  [答案](../pic/Chapter5.5.jpg)