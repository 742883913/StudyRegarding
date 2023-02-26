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

## 第十章：空间解析几何

#### 定义：
1. 方向角：向量与$x,y,z$轴的夹角记为方向角分别为$\alpha,\beta,\gamma$
2. 方向余弦：方向角的余弦

    $$\begin{cases}
        cos\alpha=\frac{a_1}{\sqrt{a_1^2+b_1^2+c_1^2}}\\
        cos\beta=\frac{b_1}{\sqrt{a_1^2+b_1^2+c_1^2}}\\
        cos\gamma=\frac{c_1}{\sqrt{a_1^2+b_1^2+c_1^2}}\\
        cos^2\alpha+cos^2\beta+cos^2\gamma=1\\
        \vec{a}^0=\{cos\alpha,cos\beta,cos\gamma\}
    \end{cases}$$

#### 向量运算
1. 数量积：$\vec{a}·\vec{b}=\|\vec{a}\|\|\vec{b}\|cos<\vec{a},\vec{b}>$

2. 向量积:（一）方向：右手定则；（二）大小：$\|\vec{a}\times \vec{b}\|=\|\vec{a}\|\|\vec{b}\|sin<\vec{a},\vec{b}>$

3. 代数运算：
   
   $$\begin{cases}
    \vec{a}·\vec{b}=a_1a_2+b_1b_2+c_1c_2\\
    \vec{a}\times \vec{b}=\{b_1c_2-b_2c_1,a_2c_1-a_1c_2,a_1b_2-a_2b_1\}
   \end{cases}$$

4. 性质说明：
   
   - $\vec{a}·\vec{a}=\|\vec{a}^2\|$
   
   - $\vec{a}·\vec{b}=0\rightarrow$两向量平行
   
   - $\vec{a}\times \vec{b}=-\vec{b}\times \vec{a}$
   
   - $\vec{a}\times \vec{b}=\vec{0}\rightarrow\vec{a}//\vec{b}$
   
   - $\|\vec{a}\times \vec{b}\|=2S_{\Delta}$