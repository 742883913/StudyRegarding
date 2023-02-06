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