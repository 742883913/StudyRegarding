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

# 静电场

## 库伦定律

$$\vec{F}=\frac{1}{4\pi \epsilon _0}\frac{q_1q_2}{r^2}\vec{e_0}$$

$\epsilon _0$ 真空电容量， $\vec{e_0}$ 表示方向的单位向量

## 电场强度

$$E=\frac{F}{q}$$

- 对于电场的叠加：

通过计算点电荷在该位置的受力，来计算该点的电场强度。现假设一个带电体，电荷体密度为 $\rho$

$$dE=\frac{E}{q_0}=\frac{\vec{e_0}}{4\pi\epsilon _0}\frac{dq}{r^2}=\frac{\vec{e_0}}{4\pi\epsilon _0}\frac{\rho dv}{r^2}$$

$$E=\int _v \frac{\vec{e_0}}{4\pi\epsilon _0}\frac{\rho}{r^2}dv$$