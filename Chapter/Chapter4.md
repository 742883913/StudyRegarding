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

**学习本章前重要的三角关系示(哥们老记不住的)：**

$$\begin{cases}
    secx=\frac{1}{cosx}\\
    cscx=\frac{1}{sinx}
\end{cases}$$

$$\begin{cases}
    (secx)^2=1+(tanx)^2\\
    (cscx)^2=1+(cotx)^2
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
    \int \sqrt{a^2-x^2}dx=\frac{a^2}{x}arcsin\frac{x}{a}+\frac x 2 \sqrt{a^2-x^2}+c
\end{cases}$$

**所有公式皆可用第二类换元积分法证明**