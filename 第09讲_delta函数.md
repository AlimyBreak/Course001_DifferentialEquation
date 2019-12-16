[课程连接](https://www.wanmen.org/courses/586d23485f07127674135df2/lectures/5922ac904b1b0d44114fd145)

***

# 9.1 δ函数

+ 全称:dirac-δ 函数.

+ 函数空间的__基矢__

  + 傅里叶级数
  $$
  f(x) = \sum{a_n\cos(\frac{2\pi nx}{L})} + \sum{b_n\sin(\frac{2\pi nx}{L})}
  $$
  
  + 其他基矢的选择方法
    
    + 俄罗斯方块 离散连续化,用离散的来表示连续的.
    
    + 把$f(x)$展开为一堆俄罗斯方块的叠加
    
    + 需要:位置和高度信息.
    
    + 单位方块就用$\delta$函数表示
    
      + 位置信息
      
      + 单位面积
      
      + 函数性质
      $$
      \int_{-\infty}^{+\infty}\delta(x-x_0)dx = 1
      $$
      
      + 函数无法绘制,但可以用已经有的函数和极限的观点来表示
      $$
      \begin{eqnarray}
      f(x) & = & \frac{1}{\sqrt{2\pi}\sigma}e^{-\frac{(x-x_0)^2}{2\sigma^2}},\sigma\to 0 \\
      f(x) & = & \frac{a_n}{1+(nx)^2},n\to \infty \\
      \end{eqnarray}
      $$
      
      + 我们可以通过已有函数进行构造，但构造时希望原函数具有__任意阶可导性__.
      
      + $\delta(x)$属于广义函数,画不出来,但具有非常好的数学性质.
      
    + $\delta$函数的数学性质
    
      1. 抓取性(卷积不变性)
      $$
      \int_{-\infty}^{+\infty}\delta(x-x_0)f(x)dx = f(x_0)
      $$
      
      2. $\delta$函数的拉普拉斯变换
      $$
      \begin{eqnarray}
      \mathcal{L}(\delta(x-x_0)) & = & \int_{-\infty}^{+\infty}\delta(x-x_0)e^{-sx}dx\\
      &=& e^{-sx_0}
      \end{eqnarray}
      $$
      
      3. $\delta^{n}(x-x_0)$都存在
      $$
      \begin{eqnarray}
      & &\int_{-\infty}^{+\infty} \phi(x)\delta'(x-a)dx\\
      = & &\int_{-\infty}^{+\infty} \phi(x)d\delta(x-a)\\
      = & & \phi(x)\delta(x-a)|_{-\infty}^{+\infty} - \int_{-\infty}^{+\infty} \phi'(x)\delta(x-a)dx\\
      = & & -\phi'(a)
      \end{eqnarray}
      $$
      $$
      \begin{eqnarray}
      & &\int_{-\infty}^{+\infty} \phi(x)\delta^{(n)}(x-a)dx\\
      = & & (-1)^n\phi^{(n)}(a)
      \end{eqnarray}
      $$
    
    

