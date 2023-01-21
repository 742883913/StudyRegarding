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

[中值定理](#中值定理)

[洛必达法则](#洛必达法则)

[极值点、凹凸性及渐近线判断与弧微分](#1-极值点判断)

# 第三章：一元函数微分学应用

## 中值定理
- 罗尔定理：
  $$\begin{cases}
   f(x)\in [a,b] \\
   f(x)在(a,b)内可导\\
   f(a)=f(b)
  \end{cases}$$

一定满足存在$\xi \in (a,b),使f'(\xi )=0$
- 拉格朗日中值定理：
  $$\begin{cases}
   f(x)\in [a,b] \\
   f(x)在(a,b)内可导
  \end{cases}$$

一定满足存在$\xi \in (a,b),使f'(\xi )=\frac{f(b)-f(a)}{b-a}$
- 柯西中值定理
  $$\begin{cases}
   f(x),g(x)\in [a,b] \\
   f(x),g(x)在(a,b)内可导\\
   g(x)\neq 0
  \end{cases}$$

一定存在$\xi \in (a,b),使\frac{f'(\xi )}{g'(\xi)}=\frac{f(b)-f(a)}{g(b)-g(a)}$

## 洛必达法则
  $$\begin{cases}
   f(x),g(x)在x=a的去心邻域内可导且g'(x)\neq 0\\
   \lim_{x \to a}f(x)=0,\lim_{x \to a}g(x)=0\\
   \lim_{x \to a}\frac{f'(x)}{g'(x)}=A
  \end{cases}$$

则

$$\lim_{x \to a}\frac{f(x)}{g(x)}=A$$

**注意**：洛必达后无极限，不代表原函数$\lim_{x \to a}\frac{f(x)}{g(x)}$ 无极限。

## 泰勒公式
- 定义自己看
- 常见等价公式自己看（狗头）（敲起来有点麻烦）

## §1 极值点判断

方法：
1. 方法一: 通过 $f'(x)=0$ 判断左右导数大小
2. 方法二：

  $$f'(x_0)=\begin{cases}
    f(x_0)>0 ，极小值点\\
    f(x_0)<0 ，极大值点
  \end{cases}$$
  
## §2 凹凸性判断
1. 方法一:
   
   (一)凸：$f(\frac{x_1+x_2}{2})>\frac{f(x_1)+f(x_2)}{2}$
   
   (二)凹：$f(\frac{x_1+x_2}{2})<\frac{f(x_1)+f(x_2)}{2}$

2. 方法二：$f(x)\in [a,b],(a,b)内二阶可导$

  $$\begin{cases}
    f''(x)>0(a<x<b), f(x)在(a,b)上为凹函数\\
    f''(x)<0(a<x<b), f(x)在(a,b)上为凸函数
  \end{cases}$$
   
## §3 渐近线判断
- 水平渐近线： 
  
  $$\lim_{x \to \infty}f(x)=A$$
 
 ,y=A为水平渐近线

- 铅直渐近线：  
 
 $$f(a-0)=\infty or f(a+0)=\infty or \lim_{x \to a}f(x)=\infty$$
   
   ，x=a为铅直渐近线

- 斜渐近线：
   
   $$\lim_{x \to \infty}\frac{f(x)}{x}=a,\lim_{x \to \infty}[f(x)-ax]=b$$ 
   
   ,则y=ax+b为斜渐近线

**注意**：  
（1）铅直渐近线一定存在间断点  
（2）水平渐近线与斜渐近线在同一区间上互斥  

## §4 弧微分(弧元素)
- 定义  
  -  直角坐标下：
  
  $$ds=\sqrt{(dx)^2+(dy)^2}=\sqrt{1+(\frac{dy}{dx})^2}=\sqrt{1+(f'(x))^2}dx$$
  
  -  参数方程下：
  
  $$\begin{cases}
    x=\phi(t)\\
    y=\Phi(t)
  \end{cases}$$  
  
  $$ds=\sqrt{(\frac{dx}{dt})^2+(\frac{dy}{dt})^2}dt=\sqrt{(\phi'(t))^2+(\Phi'(t))^2}dt$$
- 曲率和曲率半径
   -  曲率：
  
  $$k=\frac{y''}{(1+(y')^2)^\frac{3}{2}}$$
  
   - 曲率半径： 
  
  $$R=\frac{1}{k}$$