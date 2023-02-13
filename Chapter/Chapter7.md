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

# 微分方程
- 定义：微分方程的解是指使方程成立的函数，特解指不含任意常数的解

## §1 一阶微分方程
1. 可分离变量的微分方程 
  - 定义：设$\frac{dy}{dx}=f(x,y)$若$f(x,y)=\phi_1(x)\phi_2(y)$则称为可分离变量的微分方程
  - 解法：$\frac{dy}{dx}=\phi_1(x)\phi_2(y) \rightarrow \frac{dy}{\phi_2(y)}=\phi_1(x)dx \rightarrow \int \frac{dy}{\phi_2(y)}=\int \phi_1(x)dx +C$

2. 齐次微分方程
  - 设$\frac{dy}{dx}=f(x,y)$若$\frac{dy}{dx}=\phi(\frac{y}{x})$则称为齐次微分方程
  - 解法：令$u=\frac{y}{x},y=ux,\frac{dy}{dx}=u+x\frac{du}{dx} \Rrightarrow $代入求解

3. 一阶齐次线性微分方程
  - 定义：形如$\frac{dy}{dx}+p(x)y=0$称为一阶齐次线性微分方程
  - 解法：通解公式$y=ce^{-\int p(x)dx}，c$为任意常数

4. 一阶非齐次线性微分方程
  - 定义：形如：$\frac{dy}{dx}+p(x)y=Q(x)$
  - 解法：通解公式：$y=[\int Q(x)e^{\int p(x)dx}dx]e^{-\int p(x)dx}$


## §2 可降阶的高阶微分方程

1. $y^{(n)}=Q(x),(n\geq2)$(没难度)

2. $f(x,y,y'')=0$
  解法：令$\frac{dy}{dx}=p,\frac{d^2y}{dx^2}=\frac{dp}{dx}$

3. $f(y,y',y'')=0$
  解法：令$\frac{dy}{dx}=p,\frac{d^2y}{dx^2}=p\frac{dp}{dy}$

## §3 高阶微分方程
- **定义**

  $n$阶齐次线性微分方程：

  $y^{(n)}+····+a_{n-1}y'+a_ny=0 ——（1）$

  $n$阶非齐次线性微分方程：

  $y^{(n)}+····+a_{n-1}y'+a_ny=f(x)——（2）$

  若$f(x)=f_1(x)+f_2(x)$则可分解为以下两个方程：

  $y^{(n)}+····+a_{n-1}y'+a_ny=f_1(x)——（2.1）$

  $y^{(n)}+····+a_{n-1}y'+a_ny=f_2(x)——（2.2）$

- **高阶线性微分方程解的结构**
  
  1. 设$\phi _1(x),···,\phi_s(x)$ 为$(1)$的一组解，则$k_1\phi _1(x)+···+k_s\phi _s(x)$也为$(1)$的解

  2. 若$\phi_1(x),\phi_2(x)$分别为$(1),(2)$的两个解，则$\phi_1(x)+\phi_2(x)$为$(2)$的解
  
  3. 若$\phi_1(x),\phi_2(x)$为$(2)$的两个解，则$\phi_1(x)-\phi_2(x)$为$(1)$的解
  
  4. 若$\phi_1(x),\phi_2(x)$分别为$(2.1),(2.2)$的两个解，则$\phi_1(x)+\phi_2(x)$为$(2)$的解
  
  5. 设$\phi _1(x),···,\phi_s(x)$ 为$(2)$的一组解，则$k_1\phi _1(x)+···+k_s\phi _s(x)$为$(2)$的解的充要条件是$k_1+···+k_s=1$
  
  6. 设$\phi _1(x),···,\phi_s(x)$ 为$(2)$的一组解，则$k_1\phi _1(x)+···+k_s\phi _s(x)$为$(1)$的解的充要条件是$k_1+···+k_s=0$
  
  7. 设$\phi _1(x),···,\phi_n(x)$ 为$(1)$的线性无关解，则$k_1\phi _1(x)+···+k_n\phi _n(x)$为$(1)$的通解
  
  8. 设$\phi _1(x),···,\phi_n(x)$ 为$(1)$的线性无关解，$\phi _0(x)$为$(2)$的一个特解，则$k_1\phi _1(x)+···+k_n\phi _n(x)+\phi _0(x)$为$(2)$的通解

- 高级常系数线性微分方程
  
  1. $y''+py'+qy=0,p,q$为常数 
   解法：
   - 列出$\lambda ^2+p\lambda+q=0$
   - $\Delta>0，$通解为$y=C_1e^{\lambda_1x}+C_2e^{\lambda_2x}$
   - $\Delta=0，$通解为$y=C_1e^{\lambda_1x}+C_2xe^{\lambda_1x}$
   - $\Delta<0，$解为$\alpha \pm \beta i,$通解为$y=e^{\alpha x}(C_1cos\beta x+C_2sin\beta x)$
  
  2. $y''+py'+qy=P_n(x)e^{kx},p,q$为常数
   解法：
   - 列出$\lambda ^2+p\lambda+q=0$
   - 设$y_0(x)=x^l(a_nx^n+···+a_1x+a_0)e^{kx},(a_nx^n+···+a_1x+a_0)$与$P_n(x)$次数相同
   - $k\neq \lambda _1,k\neq \lambda _2:l=0$
   - $k = \lambda _1,k\neq \lambda _2:l=1$
   - $k= \lambda _1 = \lambda _2:l=2$
   
   例题：求$y''+y'-2y=2xe^{-x}$

   [答案](../pic/7.1.jpg)

