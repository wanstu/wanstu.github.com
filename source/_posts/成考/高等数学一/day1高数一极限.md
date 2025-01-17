---
title: day1高数一极限
date: 2024-05-23 00:00:00
---
# 准备

> 略

# 考情分析(00:02:32 - 00:33:42)

> 略

# 极限与连续(00:33:42 - end)

> 本节内容 天一成考 高等数学(一) p1 - p5

## 定义(00:33:42 - 00:39:49)

>  略

## 运算法则(00:39:49 - 00:42:33)
若 $\lim\limits_{x \to x_0}f(x)=A, \lim\limits_{x \to x_0}g(x)$ = B ，则
- 和差的极限等于极限的和差
  $\lim\limits_{x \to x_0}[f(x) \pm g(x)] = \lim\limits_{x \to x_0}f(x) \pm \lim\limits_{x \to x_0}g(x) = A \pm B$
- 乘积的极限等于极限的乘积
  $\lim\limits_{x \to x_0}[f(x) * g(x)] = \lim\limits_{x \to x_0}f(x) * \lim\limits_{x \to x_0}g(x) = A * B $
   
- 商的极限等于极限的商
  当 $b \neq 0$ 时，$\lim\limits_{x \to x_0} \frac{\lim\limits_{x \to x_0}f(x)}{\lim\limits_{x \to x_0}g(x)} = \frac{A}{B} $

> 常数的极限等于常数 $\lim\limits_{x \to x_0} C = C$

## 求极限(00:42:33 - end)

### 代入法(00:42:33 - 01:17:06)
  **分母不为零**时可用代入法求极限
  > $\lim\limits_{x \to 1} \frac{2x}{3x - 2} = \frac{2}{1} = 2$
#### 练习
1. $\lim\limits_{x \to \frac{\pi}{2}}\frac{2x - 1}{sinx}$
  解： $\frac{\pi - 1}{sin \frac{\pi}{2}} = \pi- 1$
  根据正弦/余弦函数图象：
  ![17165090588061716509057847.png](http://img.wanstu.cn/utools-tc/2024/524/17165090588061716509057847.png)
  可得 $sin\frac{\pi}{2} = 1$
  
2. $\lim\limits_{x \to 2} \frac{x^2 + 5}{x - 3}$
    解： $\frac{4 + 5}{2 - 3} = \frac{9}{-1} = -9$

3. $\lim\limits_{x \to 1} \frac{sinx}{x}$
    解： $\frac{sin1}{1} = 1$

4. $\lim\limits_{x \to 1}\frac{2x^2 + 6x - 1}{3x^2 + 5x + 6}$
    解： $\frac{2 + 6 - 1}{3 + 5 + 6} = \frac{7}{14} = \frac{1}{2}$

5. $\lim\limits_{x \to \sqrt{3}}\frac{x^2 - 3}{x^4 + x^2 + 1}$
    解： $\frac{0}{9 + 3 + 1} = 0$

6. $\lim\limits_{x \to 1}\frac{2x}{x^2 - 3}$
    解： $\frac{2}{-2} = -1$

#### 真题
1. $\lim\limits_{x \to 0} \frac{x}{cosx}$
    解： $\frac{0}{1} = 0$
    根据正弦/余弦函数图象：
    ![17165090588061716509057847.png](http://img.wanstu.cn/utools-tc/2024/524/17165090588061716509057847.png)
    可得 $cos0 = 1$

2. $\lim\limits_{x \to \frac{\pi}{2}}\frac{cos2x}{x}$
    解： $\frac{cos\pi}{\frac{\pi}{2}} = \frac{-1}{\frac{\pi}{2}} = -\frac{2}{\pi}$
    根据正弦/余弦函数图象：
    ![17165090588061716509057847.png](http://img.wanstu.cn/utools-tc/2024/524/17165090588061716509057847.png)
    可得 $cos\pi = -1$

3. $\lim\limits_{x \to 1}\frac{2x}{x^3 - 3}$
   解： $\frac{2}{-2} = -1$

4. $\lim\limits_{x \to -1}\frac{x + 1}{x^2 + 1}$
   解： $\frac{0}{2} = 0$

5. $\lim\limits_{x \to 1}\frac{x^3 - 5x + 2}{x^2 - 2}$
   解： $\frac{1 - 5 + 2}{1 - 2} = \frac{-2}{-1} = 2$

- **休息(01:03:52 - 01:12:43)**

6. $\lim\limits_{x \to 0}\frac{x - 1}{2x^2 + 3}$
   解： $\frac{-1}{3} = -\frac{1}{3}$

7. $\lim\limits_{x \to 1}\frac{3x^4 + x^2 -2}{4x^2 + 5x -8}$
   解： $\frac{3 + 1 - 2}{4 + 5 - 8} = \frac{2}{1} = 2 $

### 约去为零公因子法(01:17:06 - 01:33:10)
> 找出并约掉分子分母中为**零**的公因子

#### 练习
1. $\lim\limits_{x \to 1}\frac{x^2+x-2}{x^2-1}$
   解： $\frac{(x - 1)(x + 2)}{(x - 1)(x + 1)} = \frac{x + 2}{x + 1} = \frac{3}{2}$
   分子使用[十字相乘法](https://zhuanlan.zhihu.com/p/440324474)得出

2. $\lim\limits_{x \to 1}\frac{x^4 - 1}{x^3 - 1}$
   解： $\frac{(x^2)^2 - 1}{(x - 1)(x^2 + x + 1)} = \frac{(x^2 - 1)(x^2 + 1)}{(x - 1)(x^2 + x + 1)} = \frac{(x - 1)(x + 1)(x^2 + 1)}{(x - 1)(x^2 + x + 1)} = \frac{(x + 1)(x^2 + 1)}{(x^2 + x + 1)} = \frac{4}{3}$
   > $a^3-b^3 = (a - b)(a^2 + ab + b^2)$

3. $\lim\limits_{x \to 1}(\frac{1}{x - 1} - \frac{2}{x^2 - 1})$
   解： $\frac{1}{x - 1} - \frac{2}{(x - 1)(x + 1)} = \frac{x + 1}{(x - 1)(x + 1)} - \frac{2}{(x - 1)(x + 1)} = \frac{x - 1}{(x - 1)(x + 1)} = \frac{1}{x  +1} = \frac{1}{2}$

### 分子分母同时除最高次项 (01:33:10 - 01:36:53)

#### 练习
1. $\lim\limits_{x \to \infty}\frac{2x^5 - x + 1}{x^5 - 1}$
   解： $\frac{2 - \frac{1}{x^4} + \frac{1}{x^5}}{1 - \frac{1}{x^5}} = \frac{2 - 0 + 0}{1 - 0} = 2$

### <mark>等价代换法</mark>
#### 定义
当 $x \to x_0(x \to \infty)$ 时 $f(x)$ 的极限为 0 则称 $f(x)$ 为 $x \to x_0(x \to \infty)$ 时的**无穷小量** 
> 常数中只有 0 可以看作无穷小
当 $x \to x_0(x \to \infty)$ 时 $f(x)$ 的绝对值无限增大 则称 $f(x)$ 为 $x \to x_0(x \to \infty)$ 时的**无穷大量** 
> 无穷小量(不为 0时)和无穷大量互为**倒数**
#### 无穷小量的比较

设 α，β 都是自变量 x 在同一变化时的无穷小量，且极限 $\lim\limits_{}\frac{α}{β}$ 也是该条件下的极限
1) 若 $\lim\limits_{}\frac{α}{β} = 0$，称 α 是比 β 高阶的无穷小
2) 若 $\lim\limits_{}\frac{α}{β} = \infty$，称 α 是比 β 低阶的无穷小
3) 若 $\lim\limits_{}\frac{α}{β} = c(c \neq 0)$，称 α 是比 β 同阶无穷小；当 c = 1 时，称 α 是比 β 等价无穷小记为 $α \sim β$
   常用等价无穷小代换
   $x \sim sinx \sim ln(1 + x) \sim arcsinx \sim arctanx \sim e^x - 1 \sim tanx$
   $ 1 - cosx \sim \frac{1}{2}x^2 $
   $ (1 + x)^α - 1 \sim ax (α为实常数，α \neq 0)$
   > 并非所有的无穷小都可以比较 如 $ x \to 0 $ 时 x 和 $xsin\frac{1}{x}$ 都是无穷小，就不可比较
> 等价代换法只能用于乘除不能用于加减

#### 练习

1. $\lim\limits_{x \to 1}\frac{sim(x - 1)}{x^2 - 1}$
   解： $\frac{x - 1}{(x - 1)(x + 1)} = \frac{1}{x + 1} = \frac{1}{2}$

2. $\lim\limits_{x \to 0}\frac{1- cosx}{xsinx}$
   解： $\frac{\frac{1}{2}x^2}{x^2} = \frac{1}{2}$

3. $\lim\limits_{x \to 1}\frac{arcsin(x - 1)}{x^3 - 1}$
   解： $\frac{x - 1}{(x - 1)(x^2 + x + 1)} = \frac{1}{x^2 + x + 1} = \frac{1}{3}$

4. $\lim\limits_{x \to 0}\frac{tanx - sinx}{x^3}$
   解： $\frac{\frac{sinx}{cosx} - sinx}{x^3} = \frac{sinx(\frac{1}{cosx} - 1)}{x^3} = \frac{\frac{1}{cosx} - 1}{\frac{x^3}{sinx}} = \frac{1 - cosx}{x^2cosx} = \frac{\frac{1}{2}x^2}{x^2cosx} = \frac{\frac{1}{2}}{cosx} = \frac{1}{2}$
   根据正弦/余弦函数图象：
   ![17165090588061716509057847.png](http://img.wanstu.cn/utools-tc/2024/524/17165090588061716509057847.png)
   可得 $cos0 = 1$


# 本节练习

$\lim\limits_{x \to \frac{\pi}{2}}\frac{2x - 1}{sinx}$


$\lim\limits_{x \to 2} \frac{x^2 + 5}{x - 3}$


$\lim\limits_{x \to 1} \frac{sinx}{x}$


$\lim\limits_{x \to 1}\frac{2x^2 + 6x - 1}{3x^2 + 5x + 6}$


$\lim\limits_{x \to \sqrt{3}}\frac{x^2 - 3}{x^4 + x^2 + 1}$


$\lim\limits_{x \to 1}\frac{2x}{x^2 - 3}$


$\lim\limits_{x \to 0} \frac{x}{cosx}$


$\lim\limits_{x \to \frac{\pi}{2}}\frac{cos2x}{x}$


$\lim\limits_{x \to 1}\frac{2x}{x^3 - 3}$


$\lim\limits_{x \to -1}\frac{x + 1}{x^2 + 1}$


$\lim\limits_{x \to 1}\frac{x^3 - 5x + 2}{x^2 - 2}$


$\lim\limits_{x \to 0}\frac{x - 1}{2x^2 + 3}$


$\lim\limits_{x \to 1}\frac{3x^4 + x^2 -2}{4x^2 + 5x -8}$


$\lim\limits_{x \to 1}\frac{x^2+x-2}{x^2-1}$


$\lim\limits_{x \to 1}\frac{x^4 - 1}{x^3 - 1}$


$\lim\limits_{x \to 1}(\frac{1}{x - 1} - \frac{2}{x^2 - 1})$


$\lim\limits_{x \to \infty}\frac{2x^5 - x + 1}{x^5 - 1}$


$\lim\limits_{x \to 1}\frac{sim(x - 1)}{x^2 - 1}$


$\lim\limits_{x \to 0}\frac{1- cosx}{xsinx}$


$\lim\limits_{x \to 1}\frac{arcsin(x - 1)}{x^3 - 1}$


$\lim\limits_{x \to 0}\frac{tanx - sinx}{x^3}$


# 其他资料

- 正弦/余弦函数图象：
  ![17165090588061716509057847.png](http://img.wanstu.cn/utools-tc/2024/524/17165090588061716509057847.png)
- [十字相乘法](https://zhuanlan.zhihu.com/p/440324474)
- $a^3-b^3 = (a - b)(a^2 + ab + b^2)$