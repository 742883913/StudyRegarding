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

# 多元函数微分学
## §1 概念
1. **多元函数连续、可导与可微的关系**
   
   多元函数可微可推出连续与可导；对比一元函数，可微与可导互为充要，并且可推连续。

## §2 求偏导
（一）显函数求导——没有难度

（二）复合函数求导

  重点就是将$z=f(u,v)$画出树形图，多个分支的用$\partial$，一个分支的用$d$

  6.1例题：设$f(u,v)$二阶连续可偏导，且$z=f(t,sint)$,求$\frac{d^2z}{dt^2}$

  [答案](../pic/Chapter6.1.jpg)

（三）隐函数求偏导

  注意看约束条件，比如如果三个未知数，两个约束条件，则可推出两个一元方程

  6.2例题：$y=f(x+t,t^2),F(y,t,x^2+y^2)=0.f,F$连续可偏导，求$\frac{dt}{dx}$

  [答案](../pic/Chapter6.2.jpg)

## §3 找极值点求极值
  1. 找驻点

  $$\begin{cases}
  \frac{\partial z}{\partial x}=0\\
  \frac{\partial z}{\partial y}=0
  \end{cases}$$

  2. 判断极值点类型

   $$\begin{cases}
    A=\frac{\partial ^2z}{\partial x^2}|_{(x_0,y_0)}\\
    B=\frac{\partial ^2z}{\partial x\partial y}|_{(x_0,y_0)}\\
    C=\frac{\partial ^2z}{\partial y^2}|_{(x_0,y_0)}\\
   \end{cases}$$

   若$AC-B^2>0$则为极值点，反之不是极值点。且当$A>0 \rightarrow$极小值点， 反之不是极值点。且当$A<0 \rightarrow$极大值点
   
## §4 条件极值问题
- 方法一（拉格朗日乘数法）
  1. 作$F=f(x,y)+\lambda \Phi(x,y)$
  2. 列方程组，求出$x,y,\lambda$

    $$\begin{cases}
      F_x=f_x+\lambda \Phi _x=0\\
      F_y=f_y+\lambda \Phi _y=0\\
      F_{\lambda}=\Phi(x,y)=0
    \end{cases}$$

- 方法二：参数方程代换

6.3例题：$u=x^2-2y^2+3$在$x^2+4y^2\leq4$下的最大值和最小值

[答案](../pic/6.3.jpg)
 
## §5 几何应用
- 方向导数

  $z=f(x,y),(x,y)\in D,M_0(x_0,y_0)$在$M_0$做一条射线$l$,取$M(x_0+\Delta x,y_0+\Delta y),\rho=\sqrt{(\Delta x)^2+(\Delta y)^2},\Delta z=f(x_0+\Delta x,y_0+\Delta y)-f(x_0,y_0)$，方向余弦$(cos\alpha,cos\beta)$若$l$的向量为$(x,y)$则$cos\alpha=\frac{x}{\sqrt{x^2+y^2}}$

  $$\frac{\partial z}{\partial l}|_(x_0,y_0)=\lim_{\rho \to 0}\frac{\Delta z}{\rho}$$

  $$\frac{\partial z}{\partial l}\rvert_{(x_0,y_0)}=\frac{\partial z}{\partial x}|_(x_0,y_0)*cos\alpha+\frac{\partial z}{\partial y}|_(x_0,y_0)*cos\beta$$

- 梯度(该点处方向导数最大值)
  
  $u=f(x,y,z)$

  $$\nabla u\rvert _{M_0}=(\frac{\partial u}{\partial x},\frac{\partial u}{\partial y},\frac{\partial u}{\partial z})_{M_0}$$