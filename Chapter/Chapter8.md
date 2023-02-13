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

# 重积分

## 二重积分

### 性质：

1. $\int \int _D[f(x,y) \pm g(x,y)]dxdy=\int \int _Df(x,y)dxdy+\int \int _Dg(x,y)dxdy$

2. $\int \int _Dkf(x,y)dxdy=k\int \int _Df(x,y)dxdy$

3. $D=D_1+D_2 \Rightarrow \int \int _{D_1}f(x,y)dxdy+\int \int _{D_2}f(x,y)dxdy$

4. $\int \int _Ddxdy=A,A$为$D$的面积

5. 在$D$上有$f(x,y)\leq g(x,y)$则$\int \int _Df(x,y)dxdy \leq \int \int _Dg(x,y)dxdy$,若$f(x)$不恒等于$g(x)$,则 $\int \int _Df(x,y)dxdy < \int \int _Dg(x,y)dxdy$

6. 对称性质：
  - 关于$x$轴对称时，一侧区域为$D_1$:
  
  $$\begin{cases}
    f(x,-y)=-f(x,y),\int \int _Df(x,y)dxdy=0\\
    f(x,-y)=f(x,y),\int \int _Df(x,y)dxdy=2\int \int _{D_1}f(x,y)dxdy
  \end{cases}$$

  - 关于$y$轴对称类似
  
  - 关于$y=x$对称：$\int \int _Df(x,y)dxdy=\int \int _Df(y,x)dxdy$
  
  - 关于$y=-x$对称：$\int \int _Df(x,y)dxdy=\int \int _Df(-y,-x)dxdy$

7. 中值定理：
   设$f(x,y)$在$D$上连续，$A$为$D$面积，则一定存在$(m,n) \in D$使$\int \int _D f(x,y)dxdy=f(m,n)A$