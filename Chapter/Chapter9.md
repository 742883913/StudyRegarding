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

# 第九章级数
## 常数项级数
#### 定义：
1. 若$\{a_n\}$为数列，则$\sum_{n=1}^{\infty}a_n$为常数项级数
2. $S_n=a_1+···+a_n,\lim _{n \to \infty}S_n=\sum_{n=1}^{\infty}a_n$

#### 收敛基本性质

1. $$\sum_{n=1}^{\infty}a_n=A,\sum_{n=1}^{\infty}b_n=B\rightarrow\sum_{n=1}^{\infty}(a_n+b_n)=A+B$$

2. $$\sum_{n=1}^{\infty}ka_n=k\sum_{n=1}^{\infty}a_n$$

3. 加、减、改变有限项不改变级数敛散性
4. 添加任意括号后提高收敛性

5. $$\sum_{n=1}^{\infty}a_n=s \Rightarrow \lim _{n \to \infty}a_n=0,\lim _{n \to \infty}s_n=s$$

#### P级数
1. 定义：形如$\sum_{n=1}^{\infty}\frac{1}{n^p}$的叫$P$级数,其中$p=1$时称为调和级数

2. 敛散性：
   
   $$\begin{cases}
    发散，p\leq1\\
    收敛，p>1
    \end{cases}$$

#### 几何级数（等比数列之和）
$$\begin{cases}
    发散,q \geq 1\\
    收敛，q <1
\end{cases}$$

#### 正项级数
1. 定义：$\sum_{n=1}^{\infty}a_n,a_n\geq0,$（$a_n$有几项负的不影响）称为正项级数。

2. 性质：（一）$s_n$单调递增；（二）${s_n}$有上界则$\sum_{n=1}^{\infty}a_n$收敛

3. 比较审敛法：
   
   $$\begin{cases}
    a_n\leq b_n,\sum_{n=1}^{\infty}b_n 收敛\Rightarrow\sum_{n=1}^{\infty}a_n收敛\\
    a_n\leq b_n,\sum_{n=1}^{\infty}a_n发散\Rightarrow\sum_{n=1}^{\infty}b_n发散
   \end{cases}$$

   **若$\lim_{x \to \infty}\frac{b_n}{a_n}=l(0<l<+\infty)$,他们的敛散性相同**


   $$\begin{cases}
    x \geq 0,sinx\leq x\\
    x>-1,x\geq ln(x+1)\\
    e^x\geq x+1
   \end{cases}$$
4. 比值法：设$\lim_{n \to \infty}\frac{a_{n+1}}{a_n}=A$
   
   $$\begin{cases}
    A<1,收敛\\
    A=1,未知\\
    A>1,发散
   \end{cases}$$

5. 根值审敛法：设$\lim_{n \to \infty}\sqrt[n]{a_n}=A$

    $$\begin{cases}
    A<1,收敛\\
    A=1,未知\\
    A>1,发散
    \end{cases}$$

#### 交错级数
1. 定义：形如$\sum_{n=1}^{\infty}(-1)^na_n$称为交错级数
2. 审敛法：
   $a_n$单调递减，$\lim_{n \to \infty}a_n=0$，则$\sum_{n=1}^{\infty}(-1)^na_n$收敛

#### 幂级数
1. 定义：幂级数形如
   $$\begin{cases}
    a_0+a_1x+a_2x^2+···=\sum_0^{\infty}a_nx^n\\
    a_0+a_1(x-x_0)+a_2(x-x_0)^2+···=\sum_0^{\infty}a_n(x-x_0)^n
   \end{cases}$$

   一切的收敛点构成收敛域；一切的发散点构成发散域

2. 阿贝尔定理：
   
   $\exists R,|x|<R$绝对收敛,$|x|>R$发散，$R$称为收敛半径

3. 收敛半径的计算：
   $\sum_0^{\infty}a_nx^n$,若$\lim_{n \to \infty}|\frac{a_{n+1}}{an}|=\rho,lim_{n\to \infty}\sqrt[n]{|a_n|}=\rho$

   $$\begin{cases}
    \rho=0 \rightarrow R=+\infty\\
    \rho = +\infty \rightarrow R=0，收敛域为\{0\}\\
    0<\rho<+\infty \rightarrow R=\frac{1}{\rho},注意讨论端点
   \end{cases}$$

4. 解题性质：设$s(x)=\sum_0^{\infty}a_nx^n,x\in (-R,R)$
  
   - 逐项可导性(收敛半径保持不变):

      $$s'(x)=(\sum_0^{\infty}a_nx^n)'=\sum_0^{\infty}(a_nx^n)'$$

   - 逐项可积性(收敛半径不变)：

      $$\int^x_0s(x)=\int^x_0\sum_0^{\infty}a_nx^ndx=\sum_0^{\infty}\int^x_0a_nx^ndx$$

5. 常见多项式展开：
  
 $$\begin{cases}
  e^x=1+x+\frac{x^2}{2!}+···+\frac{x^n}{n!}=\sum_0^{\infty}\frac{x^n}{n!}\\
  sinx=x-\frac{x^3}{3!}+\frac{x^5}{5!}-···+\frac{(-1)^n}{(2n+1)!}x^{2n+1}=\sum_0^{\infty}\frac{(-1)^n}{(2n+1)!}x^{2n+1}\\
  cosx=1-\frac{x^2}{2!}+\frac{x^4}{4!}-···+\frac{(-1)^n}{(2n)!}x^{2n}=\sum_0^{\infty}\frac{(-1)^n}{(2n)!}x^{2n}\\
  \frac{1}{1-x}=1+x+x^2+···+x^n=\sum_0^{\infty}x^n,(-1<x<1)\\
  \frac{1}{1+x}=1-x+x^2-···+(-1)^nx^n=\sum_0^{\infty}(-1)^nx^n,(-1<x<1)\\
  ln(1+x)=x-\frac{x^2}{2}+\frac{x^3}{3}+···+\frac{(-1)^{n-1}}{n}x^n=\sum_1^{\infty}\frac{(-1)^{n-1}}{n}x^n,(-1<x\leq 1)\\
  -ln(1-x)=\sum_{n=1}^{\infty}\frac{x^n}{n},(-1\leq x<1)\\
  1-\frac{1}{2}+\frac{1}{3}+····=ln2
 \end{cases}$$

 