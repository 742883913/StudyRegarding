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

- [第一讲：随机事件与概率](#第一讲随机事件与概率)
  - [概念及基础公式](#概念及基础公式)
  - [古典概型](#古典概型)
  - [几何概型](#几何概型)
  - [概率的基本性质和公式](#概率的基本性质和公式)
  - [事件的独立性](#事件的独立性)
  - [伯努利试验](#伯努利试验)
- [第二讲：一维随机变量及其分布](#第二讲一维随机变量及其分布)
  - [随机变量及其分布函数的概念、性质及应用](#随机变量及其分布函数的概念性质及应用)
  - [常见的随机变量](#常见的随机变量)
  - [常见的随机变量分布类型](#常见的随机变量分布类型)
  - [一维随机变量函数的分布](#一维随机变量函数的分布)



# 第一讲：随机事件与概率

## 概念及基础公式

（一） $AB \neq \emptyset$ ，则称他们俩相容。 

（二）$AB = \emptyset$ ，则称他俩互斥；对立事件：两个事件必有一个发生。

（三）

$$\begin{split}
    &A-B=A\bar{B}=A-AB\\
    &A\cap(B\cup C)=(A\cap B) \cup (A\cap C)\\
    &A\cup (B\cap C)=(A\cup B) \cap (A\cup C)\\
    &A \cap (B-C)=A\cap B-A\cap C\\
    &\overline{A\cap B}=\bar{A}\cup \bar{B};\overline{A\cup B}=\bar{A}\cap \bar{B}
\end{split}$$

（四）频率： $\frac{k}{n}$ ；概率：随着试验基数越来越大，频率就越接近概率

## 古典概型

特点：（1）只有有限个样本点；（二）每个样本点发生的可能性都一样

排列：

$$A^m_n=\frac{n!}{(n-m)!}$$

组合：

$$C^m_n=\frac{n!}{(n-m)!m!}$$

## 几何概型

特点：（1）样本空间是个可度量的区域（2）每个样本点发生的可能性一样

## 概率的基本性质和公式

**（一）性质**

有界性： $P(A)=0 \neq A=\emptyset ;P(A)=1 \neq A=\Omega$

单调性：$A \subset B\rightarrow P(B-A)=P(B)-P(A)$

> $\sqrt{P(A)P(B)}\leq \frac{P(A)+P(B)}{2},P(A\lvert B)=\frac{P(AB)}{P(A)}   \geq P(AB)$

**（二）公式**

加法公式： 

$$P(A \cup B)=P(A)+P(B)-P(AB)$$

$$P(A \cup B \cup C)=P(A)+P(B)+P(C)-P(AB)-P(AC)-P(BC)+P(ABC)$$

>若 $A,B,C$ 为互不相容事件，则$P(A \cup B \cup C)=P(A)+P(B)+P(C)$

减法公式：

$$P(A-B)=P(A)-P(AB)=P(A\overline{B})$$

条件概率公式：

$$P(B\lvert A)=\frac{P(AB)}{P(A)}$$

> 所有公式都适用于条件概率公式如：$P(A-B\lvert C)=P(A\lvert C)-P(AB\lvert C)$

乘法公式：

$$P(AB)=P(A)P(B\lvert A)$$

>三项相乘：$P(ABC)=P(A)P(B\lvert A)P(C\lvert AB)$

条件概率公式（知因求果）：

$$\bigcup ^n_{i=1}A_i=\Omega,P(B)=\sum ^n_{i=1}P(A_i)P(B\lvert A_i)$$

贝叶斯公式（知果求因）:

$$\bigcup ^n_{i=1}A_i=\Omega,P(A_j\lvert B)=\frac{P(A_j)P(B\lvert A_j)}{\sum ^n_{i=1}P(A_i\lvert B)}$$

## 事件的独立性

**（一）定义**

设 $A,B$ 为两个事件，如果 $P(AB)=P(A)P(B)$ 则称事件$A,B$ 互相独立

> 如果$P(AB)=P(A)P(B),P(AC)=P(A)P(C),P(BC)=P(B)P(C),P(ABC)=P(A)P(B)P(C)$ 则称互相独立，若最后一个条件没有则称为两两独立

## 伯努利试验

特点：

（一）只有两种对立结果
（二）每次实验的概率不变
（三）实验独立重复进行 $n$ 次

# 第二讲：一维随机变量及其分布

## 随机变量及其分布函数的概念、性质及应用

（一）分布函数的概念

设 $X$ 是随机变量， $x$ 是任意实数，称函数 $F(x)=P\lbrace X\leq x\rbrace,x\in R$ 为随机变量的分布函数，或称 $X$ 服从 $F(x)$ 分布，记作 $X\sim F(x)$

（二）性质

1. $F(x)$ 是 $x$ 的单调不减函数，对任意 $x_1<x_2 \rightarrow F(x_1)<F(x_2)$

2. $F(x)$ 是右连续函数，即 $F(x+0)=F(x)$ 

3. $F(-\infty)=0,F(+\infty)=1$

（三）分布函数的应用

$$\begin{split}
  &P\lbrace X\leq a\rbrace=F(a)\\
  &P\lbrace X< a\rbrace=F(a-0)\\
  &P\lbrace X= a\rbrace=F(a)-F(a-0)
\end{split}$$

## 常见的随机变量

（一）离散型随机变量

如果随机变量 $x$ 只能取有限个 $x_1,x_2,\cdots$ 则称 $X$ 为离散型随机变量，称

$$P\lbrace X= x_i\rbrace=P_i,i=1,2,\cdots$$

为其分布列、分布率或概率分布，记为 $X\sim p_i$ 概率分布常常用表格形式或矩阵形式表示，即

$X$|$x_1\qquad x_2\qquad \cdots$
---|---
$P$|$p_1\qquad p_2\qquad \cdots$

数列 $p_i$ 是离散型概率分布的充要条件是: $p_i\geq 0,\sum P_i=1$

设离散型随机变量 $X$ 的概率分布为 $P\lbrace X= x_i\rbrace=P_i$ ，则其分布函数

$$\begin{split}
  &F(x)=P\lbrace X\leq x\rbrace=\sum P\lbrace X= x_i\rbrace\\
  &P\lbrace X= x_i\rbrace=P\lbrace X\leq x_i\rbrace-P\lbrace X< x_i\rbrace=F(x_i)-F(x_i-0)\\
  &P\lbrace a<X\leq b\rbrace=P\lbrace X\leq b\rbrace -P\lbrace X\leq a\rbrace=F(b)-F(a)
\end{split}$$

（二）连续型随机变量

如果随机变量的分布函数能表达为

$$F(x)=\int ^x_{-\infty}f(t)dt$$

其中 $f(x)$ 为非负可积函数，则称其为连续性随机变量，称 $f(x)$ 为概率密度，记为 $X\sim f(x)$ 

改变 $f(x)$ 有限个点 $f(x)$仍是概率密度

$$P\lbrace a<X< b\rbrace=P\lbrace a<X\leq b\rbrace=P\lbrace a\leq X< b\rbrace=P\lbrace a\leq X\leq b\rbrace=\int ^b_a f(t)dt=F(b)-F(a)$$

## 常见的随机变量分布类型

（一）离散型

（1）$0-1$ 分布 $B(1,p)$

 如果 $X$ 的概率分布为 

 $$X\sim \begin{pmatrix}
  0 & 1\\
  p & 1-p
 \end{pmatrix}$$

 则称 $X$ 服从参数为 $p$ 的 $0-1$ 分布

（2）二项分布 $B(n,p)$ ($0-1$ 分布进行 $n$ 次)

 $X$ 的概率分布为 
 
 $$P\lbrace X=k\rbrace =C_n^Kp^k(1-p)^{n-k}$$

（3）泊松分布 $P(\lambda)$

 $\lambda$ 为强度参数， $X$ 的概率分布为 
 
 $$P\lbrace X=k\rbrace =\frac{\lambda ^k}{k!}e^{-\lambda}$$

（4）几何分布 $G(p)$ （首中即停止）

 $X$ 的概率分布为 
 
 $$P\lbrace X=k\rbrace =(1-p)^{k-1}p$$

（二）连续型

（1）均匀分布 $U(a,b)$

 $X$ 的概率密度和分布函数分别为 

 $$f(x)=\begin{cases}
  \frac{1}{b-a},a<x<b\\
  0\quad ,others
 \end{cases}$$

 $$F(x)=\begin{cases}
  0\quad ,x<a\\
  \frac{x-a}{b-a},a\leq x<b\\
  1\quad ,x\geq b
 \end{cases}$$

（2）指数分布 $E(\lambda)$

 $\lambda$ 为失效率，$X$ 的概率密度和分布函数分别为 

 $$f(x)=\begin{cases}
  \lambda e^{-\lambda x},x>0\\
  0\quad ,others
 \end{cases}$$

 $$F(x)=\begin{cases}
  1-e^{-\lambda x},x>0\\
  0\qquad ,others
 \end{cases}$$
 
（3）正态分布 $N(\mu,\sigma ^2)$

 $X$ 的概率密度为

 $$f(x)=\frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{1}{2}(\frac{x-\mu}{\sigma})^2},x\in (-\infty,+\infty),\mu\in (-\infty,+\infty),\sigma\in (0,+\infty)$$

 $f(x)$ 关于 $x=\mu$ 对称，并在此处有最大值,如图

 <div align="center"><img src="./PPic/ZTFB.jpg" width="400"></div>

 当 $\mu=0,\sigma=1$ 称为标准正态分布，概率密度和分布函数分别为

  $$\phi(x)=\frac{1}{\sqrt{2\pi}}e^{-\frac{1}{2}x^2},x\in (-\infty,+\infty)$$

  $$\Phi (x)=\frac{1}{\sqrt{2\pi}}\int_{-\infty}^xe^{=\frac{t^2}{2}}dt$$

 $$\Phi (0)=\frac{1}{2}, \Phi (-x)=1-\Phi (x)$$

 若 $X$ 满足标准正态分布， $P\lbrace X>\mu _0\rbrace =\alpha$ 则称 $\mu _0$ 为上 $\alpha$ 分位点 

 若 $X\sim N(\mu,\sigma ^2)$:

 $$\begin{split}
  &F(x)=P\lbrace X\leq k\rbrace =\Phi (\frac{x-\mu}{\sigma})\\
  &F(\mu -x)+F(\mu +x)=1\\
  &P\lbrace a<X<b\rbrace= \Phi (\frac{b-\mu}{\sigma})-\Phi (\frac{a-\mu}{\sigma})\\
  &aX+b\sim N(a\mu+b,a^2\mu ^2)
 \end{split}$$

## 一维随机变量函数的分布

（一）概念

 设 $X$ 为随机变量，函数 $y=g(x)$ 则以随机变量为自变量的函数也是随机变量，称为随机变量 $X$ 的函数

（二）随机变量函数的分布

（1）离散型 到 离散型

$X$ 的概率分布为 $P\lbrace X= x_i\rbrace =p_i$ ，则 $X$ 的函数 $Y=g(X)$ 也是离散型随机变量，其概率分布为 $P\lbrace Y=g(x_i)\rbrace =p_i$

$$Y\sim \begin{pmatrix}
  g(x_1) & g(x_2) & \cdots\\
  p_1 & p_2 & \cdots 
\end{pmatrix}$$

若有的值相同，则合并为一项

（2）连续型 到 连续型

$$F_Y(y)=P\lbrace Y\leq y\rbrace =P\lbrace g(X)\leq y\rbrace=\int _{g(x)\leq y}f_X(x)dx$$

概率密度等于分布函数求导。









