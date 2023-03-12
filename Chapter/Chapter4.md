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

# 第四章 不定积分

[定义](#1-定义)

[重要基本公式](#2-重要基本公式)

[换元积分法](#3-换元积分法)

[分布积分法](#§4-分部积分法)

[特殊函数的不定积分](#§5-特殊函数的不定积分)

**学习本章前重要的三角关系示(哥们老记不住的)：**

$$\begin{cases}
    secx=\frac{1}{cosx}\\
    cscx=\frac{1}{sinx}
\end{cases}$$

$$\begin{cases}
    (secx)^2=1+(tanx)^2\\
    (cscx)^2=1+(cotx)^2\\
    (sin^2x)'=sin2x
\end{cases}$$

$$\begin{cases}
    (tanx)'=(secx)^2\\
    (secx)'=secx*tanx
\end{cases}$$

## §1 定义
- $F'(x)=f(x)$则称$F(x)$为$f(x)$的原函数
  
  **注意：**
  1. 连续函数一定有原函数
  2. 若$f(x)$有原函数，则一定有无数个原函数

- 不定积分：$\int f(x)dx=F(x)+C$

## §2 重要基本公式

$$\begin{cases}
    \int xe^xdx=(x-1)e^x+c\\
    \int tanxdx=-ln|cosx|+c\\
    \int cotxdx=ln|sinx|+c\\
    \int secxdx=ln|secx+tanx|+c\\
    \int cscxdx=ln|cscx-cotx|+c
\end{cases}$$

$$\begin{cases}
    \int \frac{1}{\sqrt{1-x^2}}dx=arcsinx+c\\
    \int \frac{1}{\sqrt{a^2-x^2}}dx=arcsin\frac x a+c\\
    \int \frac{1}{a^2+x^2}dx=\frac1 a arctan\frac x a+c\\
    \int \frac{1}{\sqrt{x^2+a^2}}dx=ln(x+\sqrt{x^2+a^2})+c\\
    \int \frac{1}{\sqrt{x^2-a^2}}dx=ln|x+\sqrt{x^2-a^2}|+c\\
    \int \frac{1}{x^2-a^2}dx=\frac{1}{2a}ln|\frac{x-1}{x+a}|+c\\
    \int \sqrt{a^2-x^2}dx=\frac{a^2}{2}arcsin\frac{x}{a}+\frac x 2 \sqrt{a^2-x^2}+c
\end{cases}$$

**所有公式皆可用第二类换元积分法证明**

## §3 换元积分法

- **第一类换元积分法：**

$$\int f[\phi(x)]d\phi'(x)=\int f(t)dt=F(t)+c=F[\phi(x)]+c$$

**适用类型** :**无理数$\rightarrow$有理数**

例题：求$\int \sqrt{e^x-1}dx$

- **第二类换元积分法**

$$\int f(x)dx=\int f[\phi(t)]d\phi(t)=\int g(t)dt=G(t)+c=G[\phi^{-1}(x)]+c$$

**适用类型**：平方和差(可以将上面给出的公式全部证明)

$\sqrt{a^2-x^2}\rightarrow 设x=asint$

$\sqrt{x^2+a^2}\rightarrow 设x=atant$

$\sqrt{x^2-a^2}\rightarrow 设x=asect$

## §4 分部积分法

- 公式：

$uv=\int u dv+\int v du \rightarrow \int u dv=uv-\int v du$

**适用类型**
1. $\int 幂函数*指数dx$
2. $\int 幂函数*对数dx$
3. $\int 幂函数*三角dx$
4. $\int 幂函数*反三角dx$
5. 特殊：设原函数为$t$型,会发现积着又回到原函数

  $$\begin{cases}
  \int e^{ax}cosbxdx\\
  \int e^{ax}sinbxdx
  \end{cases}$$

  例题：求$\int e^{-x}cosxdx$

6. 特殊($n$为奇数时)

  $$\begin{cases}
    \int sec^nxdx\\
    \int csc^nxdx
  \end{cases}$$

  例题：1.$\int sec^4xdx$ 2. $\int sec^3xdx$

## §5 特殊函数的不定积分
### 最重要的是保持灵活并不是所有都是这么做！
- **假分式（及分子次数比分母次数大）**：

$$假分式 \rightarrow 多项式+真分式$$

- **真分式**
1. 第一步：$\frac{保持不变}{因式分解}$
2. 拆分(列举特殊情况)

$$\frac{2x+1}{x(x^2+2x+2)}=\frac A x+\frac{Bx+c}{x^2+2x+2}$$

$$\frac{2x+2}{x^3(2x+1)}=\frac{A}{x}+\frac B {x^2}+\frac C {x^3}+\frac D {2x+1}$$

- **三角函数中没有办法的办法（万能公式）**
  
  设
  
  $$tan\frac x 2=u,sinx=\frac{2u}{1+u^2},cosx=\frac{1-u^2}{1+u^2},x=2arctanu,dx=\frac 2 {1+u^2}$$