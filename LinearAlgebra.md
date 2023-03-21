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

## 目录：

[第一章：行列式](#行列式)

[第二章：矩阵](#矩阵)

# 行列式

## 第一种概念：几何意义

**概念**：二阶行列式可看成两个二维向量组成的，其值为以两向量为临边的平行四边形的面积；三阶行列式可看成由三个三维向量组成，其值为三个向量为边组成的面积

**性质**：

- $\lvert A\rvert$=$\lvert A^T\rvert$，及行列式中行列地位相同
- 若行列式中某行全为 0 则值为 0
- 若行列式中两行（列）成比例，则值为 0
- 若某行或某列有公因子则可提出
- 单行可加性
- 行列式中两行（列）互换，反号
- 行列中某行的某倍加到另一行上值不变

## 第二种概念：逆序数法

见老汤笔记

## 第三种概念：行列式展开定理

**余子式**：记作 $M_{ij}$；

**代数余子式**：记作$A_{ij}=(-1)^{i+j}M_{ij}$

$$\lvert A\rvert=\sum _{i=1}^{n}a_{ij}A_{ij}$$

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
    C & B
 \end{vmatrix}=
 \begin{vmatrix}
    A & c\\
    0 & B
 \end{vmatrix}=\lvert A \rvert \lvert B \rvert$$

$$\begin{vmatrix}
    0 & A\\
    B & 0
 \end{vmatrix}=
 \begin{vmatrix}
    0 & A\\
    B & C
 \end{vmatrix}=
 \begin{vmatrix}
    C & A\\
    B & 0
 \end{vmatrix}=(-1) ^{mn} \lvert A \rvert \lvert B \rvert$$

 （四）范德蒙德行列式

 $$\begin{vmatrix}
  1 & 1 & \cdots & 1 \\
  x_1 & x_2 & \cdots & x_n\\
  x_1^2 & x_2^2 & \cdots & x_n^2\\
  \cdots & \cdots & \cdots & \cdots\\
  x_1^{n-1} & x_2^{n-1} & \cdots & x_n^{n-1}\\
 \end{vmatrix}=\prod _{1 \leq i<j \leq n}(x_j-x_i)$$

 
 ## 行列式习题,仅技巧型

 （一）**标准爪型**：
   
   解题方法：通过倍数加减变换消边上的爪子

   [例题](LApic/l1.1.jpg)

 （二）**行（列）和相等**

   解题方法：行和或列和相等则相加提公因式，再去化简

   [例题](LApic/l2.2.jpg)

 （三）**异爪型**

   解题方法：1.阶数不高的直接展开 2.用递推法

   [例题](LApic/l3.3.jpg)

 （四）**抽象型行列式的计算**
   解题方法：要熟练地把线性组合表示成矩阵乘积的形式

   [例题](LApic/l4.4.jpg)

[返回目录](#目录)

# 矩阵

## 矩阵的基本运算

 （一）加法：两个同型矩阵对应元素相加

 （二）数乘矩阵

   $$k\begin{pmatrix}
    a_{11} & a_{12}\\
    a_{21} & a_{22}
   \end{pmatrix}=
   \begin{pmatrix}
    ka_{11} & ka_{12}\\
    ka_{21} & ka_{22}
   \end{pmatrix}$$

  （三）运算律

   $$\begin{split}
      A+B&=B+A \\
      (A+B)+C&=A+(B+C)\\
      k(A+B)&=kA+kB
   \end{split}$$
    
   注：
   
   $$\lvert kA \rvert =k^n \lvert A \rvert$$

  （四）矩阵的乘法
  
   > 设 $A_{m \times s},B_{s \times n}$ ，即 $A$ 的列数必须等于 $B$ 的行数， $AB$ 为 $m\times n$ 阶矩阵

   $$\begin{split}
    (AB)C &=A(BC) \qquad(1)\\
    A(B+C)&=AB+BC \qquad(2)\\
    (kA)B& =A(kB) \qquad(3)
   \end{split}$$
   
   注：$AB \neq BA;AB=0$ 得不出 $A or B=0;AB=AC$ 不得$B=C$

  （五）转置矩阵

   > 转置矩阵为将矩阵的行列互换得到的矩阵

   $$\begin{split}
    (A^T)^T&=A \qquad(1)\\
    (kA)^T&=kA^T \qquad(2)\\
    (A+B)^T&=A^T+B^T \qquad(3)\\
    (AB)^T&=B^TA^T \qquad(4)\\
    m=n \text{时} \lvert &A^T \rvert =\lvert A \rvert \qquad(5)
   \end{split}$$

 （六）向量的内积与正交
  
  - 内积
   > 设 $\alpha=[a_1,a_2,\cdots,a_n]^T,\beta=[b_1,b_2,\cdots,b_n]^T$

   $$(\alpha,\beta)=\alpha^T \beta= \sum _{i=1}^n a_ib_i$$

  - 正交
   > 当$(\alpha,\beta)=\alpha^T \beta = 0$ 时称 $\alpha,\beta$ 两向量正交

  - 向量的模

   $$||\alpha||=\sqrt{\sum _{i=1}^na_i^2}$$

   > $\lvert \lvert \alpha\rvert \rvert=1$ 时称为单位向量

  - 标准正交向量组
   > 向量组满足以下，则称为标准正交向量组

   $$a_i^Ta_j=\begin{cases}
    0,i \neq j\\
    1, i=j
   \end{cases}$$

 （七）施密特正交化（正交规范化）过程
   > 线性无关向量组 $\alpha_1,\alpha_2$ 正交化公式为：

   $$\begin{split}
    &\beta _1= \alpha _1 \qquad (1)\\
    &\beta _2 = \alpha _2 - \frac{(\alpha_2,\beta_1)}{(\beta_1,\beta_2)}\beta 1 \qquad (2)\\
    &\gamma_1=\frac{\beta _1}{||\beta _1||},\gamma_2=\frac{\beta _2}{||\beta _2||} \qquad (3)
   \end{split}$$

   > $\gamma_1,\gamma_2$ 为标准正交向量组

 （八）矩阵的幂
   
   > 矩阵的方不能靠经验公式

   $$\begin{split}
    (A+B)^2&=(A+B)(A+B)\\
    (A+B)(A-B)&=A^2+BA-AB-B^2\\
    f(x)=a_0+a_1x+\cdots +a_mx^m,&f(A)=a_0E+a_1A+\cdots+a_mA^m
   \end{split}$$

 （九）方阵乘积的行列式

   $$\lvert AB \rvert=\lvert A \rvert \lvert B \rvert$$

   正交矩阵：$AA^T=E,A$ 的行（列）向量组为标准正交向量组

   [返回目录](#目录)