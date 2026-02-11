

## 极限问题


**定理1**：
$$
    \lim_{x\rightarrow \infty} \frac{C}{x^n} = 0,C为常数   \tag{1}
$$

### **极限的运算法则**:
1. 乘法的极限 = 极限的乘积

    $$\lim (A \times B) = (\lim A) \times (\lim B)$$


2. 除法的极限 = 极限的商 (前提是分母不为0)

    $$\lim (\frac{A}{B}) = \frac{\lim A}{\lim B}$$


3. 加法的极限 = 极限的和
   $$\lim (A+B) = \lim A + \lim B$$

4. 参数“联动”问题，通常发生在不定式 (Indeterminate Forms) 的情况下。<br>
**联动**的情况比如：<br>
$\infty - \infty$ （无穷减无穷）$0 \times \infty$ （零乘无穷）$\frac{\infty}{\infty}$ （无穷除无穷）<br>
**不联动**的情况比如：
$$
    \lim_{x\rightarrow\infty}\frac{\frac{x^3+1}{x^4}x^4}{\frac{x^8+1}{x^9}x^9}
$$

## chapter5 连续性和可导性

定义：
$$
如果 \lim_
{x\rightarrow a}f(x)=f(a), 函数 f 在点 x = a 处连续
$$

### 夹逼定理
写成公式就是：
$$\lim_{x \to a} f(x) = L$$
等价于（必须要同时满足）：<br>
左极限 ($a^-$)： $\lim_{x \to a^-} f(x) = L$<br>
右极限 ($a^+$)： $\lim_{x \to a^+} f(x) = L$<br>
如果左边趋向于 0，右边趋向于 1，那么这个总极限就是不存在**DNE**

### 介值定理

如果$f$在$[a,b]$上连续, 并且$f (a) < 0$且$f (b) > 0$, 那么在区间
$(a,b)$上至少有一点$c$, 使得$f (c) = 0$.<br>代之以$f (a) > 0 且 f (b) < 0$, 同样成立

### 最大值最小值定理
如果$f$在$[a,b]$上连续, 那么$f$在$[a,b]$上至少有一个
最大值和一个最小值.


### 函数可导

- 如果一个函数$f$在$x$上可导，那么它在$x$上连续.
- **可导函数必连续**. 不过要记住, **连续函数并不总是可导的**




## chapter6 求微分问题

### 求导的基本形式
$$
    f'(x) = \lim_{h\rightarrow 0}\frac{f(x+h) - f(x)}{h}
$$

### 多次幂求导

$$
    \frac{d}{dx}x^n=nx^{n-1}
$$