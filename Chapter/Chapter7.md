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
