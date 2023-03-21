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

# 行列式

## 第一种概念：几何意义

**概念**：二阶行列式可看成两个二维向量组成的，其值为以两向量为临边的平行四边形的面积；三阶行列式可看成由三个三维向量组成，其值为三个向量为边组成的面积

**性质**：

$$\begin{cases}
    \|A\|=\|A^T\|,及行列式中行列地位相同\\
    若行列式中某行全为0则值为0\\
    若行列式中两行（列）成比例，则值为0\\
    若某行或某列有公因子则可提出\\
    单行可加性\\
    行列式中两行（列）互换，反号\\
    行列中某行的某倍加到另一行上值不变
\end{cases}$$

## 第二种概念：逆序数法

见老汤笔记

## 第三种概念：行列式展开定理

**余子式**：记作$M_{ij}；$**代数余子式**：记作$A_{ij}=(-1)^{i+j}M_{ij}$

$$\|A\|=\sum _{i=1}^{n}a_{ij}A_{ij}$$

**几个重要行列式**：

 （一）：主对角线行列式等于主对角线之积

 （二）：副对角线行列式=$(-1)^{\frac{n(n-1)}{2}}a_{1n}a_{2,n-1}····$
 （三）：拉普拉斯展开式：$A$为$m$阶矩阵，$B$为$n$阶矩阵

 $$\begin{vmatrix}
    A & 0\\
    0 & B
 \end{vmatrix}=
 \begin{vmatrix}
    A & 0\\
    0 & B
 \end{vmatrix}$$