

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
$$
    \frac{d}{dx}x=1
$$

$$
    \frac{d}{dx}C= 0
$$


### 通过乘积法则求积函数的导数

**乘积法则(版本 1)**:
$$
如果 h(x) = f(x)g(x), 那么 h'(x) = f'(x)g(x) + f(x)g'(x)
$$

**乘积法则 (版本 2)**:

如果 $y = uv$,则有  
$$
\frac{dy}{dx}= v \frac{du}{dx} + u \frac{dv}{dx}
$$

**乘积法则 (三个变量)**:

如果$y=uvw$,则有
$$
    \frac{dy}{dx}=\frac{du}{dx}vw+u\frac{dv}{dx}w+uv\frac{dw}{dx}
$$

### 通过商法则求商函数的导数
**商法则 (版本 1)**:

 $\quad$ 如果 $h(x) = \frac{f(x)}{g(x)}$, 那么
 $$
 h'(x) = \frac{f'(x)g(x) - f(x)g'(x)}{(g(x))^2}.
 $$


**商法则 (版本 2)**:

$\quad$ 如果 $y = \frac{u}{v}$, 那么
$$\frac{dy}{dx} = \frac{v \frac{du}{dx} - u \frac{dv}{dx}}{v^2}.$$

**链式求导法则 (版本 1)**:
 
$\quad$ 如果 $h(x) = f(g(x))$, 那么 $h'(x) = f'(\ g(x)\ )g'(x)$.

**链式求导法则 (版本 2)**:

$\quad$ 如果 $y$ 是 $u$ 的函数, 并且 $u$ 是 $x$ 的函数, 那么
$$\frac{dy}{dx} = \frac{dy}{du}\frac{du}{dx}.$$


## chapter7 三角函数的极限和导数

**极限1：**
$$
\lim_{x \to 0} \frac{\sin(x)}{x} = 1.
$$


**极限2**:
$$\lim_{x \to 0} \frac{\tan(x)}{x} = \lim_{x \to 0} \frac{\frac{\sin(x)}{\cos(x)}}{x} = \lim_{x \to 0} \left( \frac{\sin(x)}{x} \right) \left( \frac{1}{\cos(x)} \right) = (1) \left( \frac{1}{1} \right) = 1.

$$
这样就证明了
$$\lim_{x \to 0} \frac{\tan(x)}{x} = 1.
$$


## chapter11 洛必达法则

**洛必达法则**：

如果 $f(a) = g(a) = 0$, 那么 
$$
\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}
$$
注意：适用于  $\frac{0}{0}$ 或 $\frac{\infty}{\infty}$ 型未定式