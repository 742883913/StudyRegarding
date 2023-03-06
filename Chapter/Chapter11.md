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

# 第十一章：曲线和曲面积分

## 第一类曲线积分（对弧长）
（一）$\int _lf(x,y)ds$称为$f(x,y)$在$l$上对弧长的曲线积分

（二）性质：$\int _l1ds=l$其他类似普通积分

（三）计算方法（直角坐标下）：$L=\phi(x)(a<x<b)$

$$\int _lf(x,y)ds=\int_a^bf(x,\phi(x))\sqrt{1+\phi'^2(x)}dx$$

（四）计算方法（极坐标下）：$x=\phi(t),y=\Phi(t)$

$$\int _lf(x,y)ds=\int_{\alpha}^{\beta}f[\phi(t),\Phi(t)]\sqrt{\phi'^2(t)+\Phi'^2(t)}dt$$

## 第二类曲线积分（对坐标）
（一）应用情形（做工）：$dw=\vec{F}·\vec{s},\vec{F}=\{P(x,y), Q(x,y)\},\vec{S}=\{dx,dy\}\r\Rightarrow w=\int _LP(x,y)dx+Q(x,y)dy$

（二）性质:$\int _{L^-}=-\int _L$

（三）解题方法（直角坐标）：$y=\phi(x)$

$$\int _LP(x,y)dx+Q(x,y)dy=\int_{a}^{b}\{P(x,\phi(x))+Q(x,\phi(x))\phi'(x)\}dx$$

（四）解题方法（极坐标）：$x=\phi(t),y=\Phi(t)$

$$\int _LP(x,y)dx+Q(x,y)dy=\int _{\alpha}^{\beta}\{P(\phi(t),\Phi(t))\phi'(t)+Q(\phi(t),\Phi(t))\Phi'(t)\}dt$$

（五）概念：一、单连通区域：逆时针为正；二、双连通区域：外逆内负为正

（六）格林公式：

  - 条件：1.$D$为$xoy$面内连通区域；2. $L$为$D$的正向边界
  - 结论：$\int _LPdx+Qdy=\int \int (\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y})ds$

（七）设$D$为单连通区域；$P(x,y),Q(x,y)$在区域内连续可偏导，则与以下四个等价：

$$\begin{cases}
    曲线积分与路径无关\\
    D内恒有\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}\\
    D内存在函数u(x,y),使du(x,y)=Pdx+Qdy
\end{cases}$$

推论：
 1. 若$\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y},$则原式$=\int _{(x_0,y_0)}^{(x_1,y_1)}Pdx+Qdy=\int _{x_0}^{x_1}P(x,y_0)dx+\int _{y_0}^{y_1}Q(x_1,y)dy$ 
 2. 若$\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y},$则原式$=\int _{(x_0,y_0)}^{(x,y)}Pdx+Qdy=\int _{x_0}^{x}P(x,y_0)dx+\int _{y_0}^{y}Q(x,y)dy$ 