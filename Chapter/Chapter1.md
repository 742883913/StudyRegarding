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

# 第一章：极限与连续

## 极限
### 极限部分
（尚未完成）


### 无穷小部分
- **定义**：设$\alpha,\beta$都趋于零，若

$$\begin{cases}
  \lim \frac{\beta}{\alpha}=0,\beta=o(\alpha)\\
  \lim \frac{\beta}{\alpha}=k,\beta=O(\alpha)
\end{cases}$$

$\beta=o(\alpha),\beta为\alpha高阶无穷小$；$\beta=O(\alpha)\beta为\alpha同阶无穷小$

- **性质**（仅列举特殊的）：
  
  $$\lim_{n \to \infty}f(x)=A \rightarrow f(x)=A+\alpha$$

  $\alpha \rightarrow 0$



## 间断点与连续
### 连续部分
- **连续的定义**：如果$\lim_{x \to a}f(x)=f(a)$或者$f(a-0)=f(a+0)=f(a)$则f(x)在x=a连续。

- **f(x)在$[a,b]$上连续的性质**:

$$\begin{cases}
  f(x) \text{在(a,b)上连续}\\
  f(a)=f(a+0)\\
  f(b)=f(b-0)
\end{cases}$$

  1. 一定存在最大值和最小值
  2. 一定有界
  3. 零点定理
  4. 介值定理


### 间断点部分
- **间断点定义**：如果$\lim_{x \to a}f(x)\neq f(a)$则$x=a$为$f(x)$间断点
- **间断点种类**：
    
    第一类间断点：$f(a-0)与f(a+0)$存在

    $$\begin{cases}
      f(a-0)=f(a+0) \text{为可去间断点}\\
      f(a-0)\neq f(a+0) \text{为跳跃间断点}
    \end{cases}$$

    第二类间断点：$f(a-0)与f(a+0)$至少一个不存在
  
  **此处题目一般为判断间断点类型与位置**