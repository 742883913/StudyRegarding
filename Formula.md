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

# 第一章：函数，极限与连续

## 三角类：

$$\begin{split}
    &\sec ^2x=1+\tan ^2x\\
    &\csc ^2x=1+\cot ^2x\\
    &\arcsin x+\arccos x=\frac{\pi}{2}\\
    &\arctan x+arccot x=\frac{\pi}{2}
\end{split}$$

## 奇偶类：

- 偶数个奇函数之积为偶函数，奇数个奇函数之积为奇函数

## 周期性：

- 两周期函数之和的周期为他俩周期的最小公倍数

## 极限类：

- 数列有极限的充要条件:

$$\lim _{n\to +\infty}X_{2n-1}=\lim _{n\to +\infty}X_{2n}$$

- 数列极限的保号性

$$\lim _{n\to +\infty}X_{2n}=a(a>0) \rightarrow\exists N,n>N,X_n>0$$

- 当 $x\to 0$

$$\begin{split}
    &x\sim \sin x,\ln(1+x),e^x-1\\
    &1-\cos x\sim\frac{1}{2}x^2\\
    &(1+x)^{a}-1\sim ax\\
    &x\sim \sin x,\tan x,\arcsin x,\arctan x\\
    &x-\sin x\sim \frac{1}{6}x^3\\
    &x-\arcsin x\sim -\frac{1}{6}x^3\\
    &x-\arctan x\sim \frac{1}{3}x^3\\
    &x-\tan x\sim -\frac{1}{3}x^3\\
    &x-\ln (1+x)\sim \frac{1}{2}x^2\\
    &\lim _{x\to 0}\frac{a^x-1}{x}=\ln a
\end{split}$$


- 重要极限

$$\begin{split}
    &\lim _{n\to \infty}n^{\frac{1}{n}}=1\\
    &\lim _{x\to 0}(1+x)^{\frac{1}{x}}=e\\
\end{split}$$

- 常用泰勒公式

$$\begin{split}
    &e^x=\sum _{n=0}^{\infty} \frac{x^n}{n!}+0(x^n)\\
    &\sin x=\sum _{n=1}^{\infty}(-1)^{n-1}\frac{x^{2n-1}}{(2n-1)!}+o(x^{2n-1})\\
    &\cos x=\sum _{n=0}^{\infty}\frac{x^{2n}}{(2n)!}+o(x^{2n})\\
    &\ln (1+x)=\sum _{n=1}^{\infty}(-1)^{n-1}\frac{x^{n}}{n}+0(x^n)\\
    &(1+x)^a=\sum _{n=1}^{\infty} \frac{a(a-1)\cdots (a-n+1)}{n!}x^n+0(x^n)
\end{split}$$

