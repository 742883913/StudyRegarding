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
# 导数与微分

## §1 导数定义

$$f'(a)=\lim_{x \to a}\frac{f(x)-f(a)}{x-a}=\lim_{\Delta x \to 0}\frac{\Delta y}{\Delta x}$$

这就体现导数和极限之间的关系，导数与极限可以互相转化。

**注意：** 可导一定连续而连续不一定可导。所以一些题目我们就要考虑可导和连续的性质如：

1. 连续：$\lim_{x \to a}f(x)=f(a)$

2. 可导：$f(a-0)=f(a+0)$

## §2 可微定义
如果$f(x_0+\Delta x)-f(x_0)=A\Delta x+o(\Delta x)$则称$f(x)$在$x=x_0$可微。

**注解:** 
- 可导与可微互为充要条件
- $dy=df(x)=f'(x)dx$

## §3 基本公式及题目类型

### 常见基本公式（仅列举易混淆的）
- $(a^x)'=a^xlna$
- $(log_ax)'=\frac{1}{xlna}$
- $(arcsinx)'=\frac{1}{\sqrt{1-x^2}}$
- $(arccosx)'=-\frac{1}{\sqrt{1-x^2}}$
- $(arctanx)'=\frac{1}{1+x^2}$
- $(arccotx)'=-\frac{1}{1+x^2}$

### 题目类型
- 定义研究导数型

  灵活运用

$$f'(x)=\lim_{\Delta x \to 0}\frac{f(x+\Delta x)-f(x)}{\Delta x}$$

- 显函数求导（考验基本功）

- 隐函数求导（考验可微和可导）
- 参数方程确定的函数求导

$$\begin{cases}
    x=\phi(t)\\
    y=\Phi(t)
\end{cases}$$

$$\frac{dy}{dx}=\frac{dy/dt}{dx/dt}=\frac{\Phi '(t)}{\phi'(t)}$$

- 分段函数求导

  要考虑区间连接处的连续性