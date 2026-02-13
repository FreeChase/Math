- [chapter4 极限问题](#chapter4-极限问题)
  - [**极限的运算法则**:](#极限的运算法则)
- [chapter5 连续性和可导性](#chapter5-连续性和可导性)
  - [夹逼定理](#夹逼定理)
  - [介值定理](#介值定理)
  - [最大值最小值定理](#最大值最小值定理)
  - [函数可导](#函数可导)
- [chapter6 求微分问题](#chapter6-求微分问题)
  - [求导的基本形式](#求导的基本形式)
  - [多次幂求导](#多次幂求导)
  - [通过乘积法则求积函数的导数](#通过乘积法则求积函数的导数)
  - [通过商法则求商函数的导数](#通过商法则求商函数的导数)
- [chapter7 三角函数的极限和导数](#chapter7-三角函数的极限和导数)
- [chapter11 洛必达法则](#chapter11-洛必达法则)
  - [类型 A：分式形式](#类型-a分式形式)
  - [类型 B1：求差形式](#类型-b1求差形式)
  - [类型 B2：乘积形式](#类型-b2乘积形式)
  - [类型 C：指数形式](#类型-c指数形式)
- [chapter15 积分](#chapter15-积分)
  - [伸缩级数](#伸缩级数)
- [chapter16 定积分](#chapter16-定积分)
  - [定积分规则](#定积分规则)
- [chapter17 微积分基本定理](#chapter17-微积分基本定理)
- [chapter24 泰勒多项式、泰勒级数和幂级数导论](#chapter24-泰勒多项式泰勒级数和幂级数导论)
- [chapter30 微分方程](#chapter30-微分方程)
  - [可分离变量](#可分离变量)


## chapter4 极限问题


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

>法则跟求极限不一样，不能看成$h'(x)=f'(x)g'(x)$<br>
>极限是$\lim_{x->a}f(x)$<br>
>求导是$\lim_{h\rightarrow0}\frac{f(x+h)-f(x)}{h}$

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


这是一份为你整理好的、排版清晰的《洛必达法则类型的总结》Markdown 文件。

我已经帮你修复了原文本中因 OCR 扫描识别错误导致的乱码（例如把  识别成了 `§1`，把减号识别成了 `¡` 等），并将所有的数学公式转化为标准的 LaTeX 格式，方便你阅读和复习。

---


### 类型 A：分式形式

如果极限是分式的形式，例如：

$$\lim_{x \to a} \frac{f(x)}{g(x)}$$

要检查该形式是否为不定式。如果该分式为  或 ，使用洛必达法则：

$$\lim_{x \to a} \frac{f(x)}{g(x)} \overset{\text{L'H}}{=} \lim_{x \to a} \frac{f'(x)}{g'(x)}$$

> **注意**：在求导的过程中，**请不要使用商的求导法则！** 现在，为求解这个新的极限，可能需要再次使用洛必达法则。

---

### 类型 B1：求差形式

如果是求差的极限，例如：
$$\lim_{x \to a} (f(x) - g(x))$$

该形式为$\infty - \infty$。求解该极限的方法是**通分**或**同时乘以并除以一个共轭表达式**，从而转化为**类型 A**。

---

### 类型 B2：乘积形式

如果极限是乘积的形式，例如：

$$\lim_{x \to a} f(x)g(x)$$

该形式为 。选择两个因式中较简单的那个**取倒数把它移到分母**（尽量不要选用对数做分母，把它留在分子）。这样就转化为：

$$\lim_{x \to a} f(x)g(x) = \lim_{x \to a} \frac{g(x)}{1/f(x)}$$

这是典型的**类型 A**。

---

### 类型 C：指数形式


如果极限为指数的形式，并且该指数的底和指数部分都含变量，例如：


$$
\lim_{x \to a} f(x)^{g(x)}
$$


首先，我们**取其对数**：


$$
\lim_{x \to a} \ln\left(f(x)^{g(x)}\right) = \lim_{x \to a} g(x)\ln(f(x))
$$

这样转化为**类型 B2 或 A**（或者转化后的结果不是不定式，这时不得不想其他的技巧）。一旦你已经求解出来了，这时，就有：

$$
\lim_{x \to a} \ln\left(f(x)^{g(x)}\right) = L
$$

然后再**两边同时取指数**，可得：

$$
\lim_{x \to a} f(x)^{g(x)} = e^L
$$


## chapter15 积分

### 伸缩级数

$$
\sum_{j=a}^{b} (f(j) - f(j-1)) = f(b) - f(a-1).
$$
变种1

$$
\sum_{j=1}^{n} j = \frac{n(n+1)}{2}.
$$

变种2

$$
\sum_{j=1}^{n} j^2 = \frac{1}{3} \left( n^3 + \frac{3n(n+1)}{2} - n \right).
$$

## chapter16 定积分
**定积分** (Definite Integral)定积分的核心是一个数值（Number）。

- 定义： 定积分是黎曼和的极限。它表示将一个区间 $[a, b]$ 切分成无数个细小的长方形，计算这些长方形面积之和的极限。
- 符号： 写作 $\int_{a}^{b} f(x)\mathrm{d}x$。其中 $a$ 和 $b$ 是积分的上下限，告诉我们要计算哪一段。
- 几何意义： 它代表曲线 $y=f(x)$、$x$轴以及直线 $x=a$ 和 $x=b$ 所围成的面积（如果有反函数，也可以看作是与 y 轴围成的面积）。
- 结果： 计算出来的结果是一个具体的数字（例如 $5, -3, \pi$ 等）。

**不定积分** (Indefinite Integral)，在微积分第二基本定理中提到了其核心概念——反导数 (Antiderivative)。不定积分的核心是一个函数（Function）。
- 概念： 不定积分是求导的逆运算。它的目的是寻找一个函数 $F(x)$，使得 $F'(x) = f(x)$。
- 关联： 在你的笔记图片中，被称为“$f$ 的任意一个反导数”。
- 结果： 计算出来的结果是一个函数（通常包含一个常数 $C$，即 $F(x) + C$），代表了一簇曲线。


$$
    \int_{a}^{b} f(x)\mathrm{d}x.
$$

这就是定积分. 你可以把它读为 “函数 $f(x)$ 对于 $x$ 从 $a$ 到 $b$ 的积分”. 表达式 $f(x)$ 叫做**被积函数**


$$
\int_{a}^{b} f(x)\mathrm{d}x = \lim_{\text{mesh}\to 0} \sum_{j=1}^{n} f(c_j)(x_j - x_{j-1}),
$$
其中 $a = x_0 < x_1 < \dots < x_{n-1} < x_n = b$ 并且对于每一个 $j=1,\dots,n$ 都有 $c_j$ 在 $[x_{j-1}, x_j]$ 内.

### 定积分规则

**规则1**：

如果翻转积分, 即调换积分上下限, 需要在这个积分前面加个负号
$$
\int_{b}^{a} f(x)\mathrm{d}x = - \int_{a}^{b} f(x)\mathrm{d}x.
$$

**规则2**：
$$
\int_{a}^{a} f(x)\mathrm{d}x = 0
$$

**规则3**：

**可以把一个积分表达式分成两部分**
$$
\int_{a}^{b} f(x)\mathrm{d}x = \int_{a}^{c} f(x)\mathrm{d}x + \int_{c}^{b} f(x)\mathrm{d}x.
$$

**规则4**：

常数可以被移到积分表达式的外边

$$
\int_{a}^{b} C f(x)\mathrm{d}x = C \int_{a}^{b} f(x)\mathrm{d}x.
$$


**规则5**：

和或差的积分等于积分的和或差

$$
\int_{a}^{b} (f(x) + g(x))\mathrm{d}x = \int_{a}^{b} f(x)\mathrm{d}x + \int_{a}^{b} g(x)\mathrm{d}x.
$$

**规则6**：

如果 $f$ 存在反函数, $\int_{A}^{B} f^{-1}(y)\mathrm{d}y$ 就是由函数 $y = f(x)$、直线 $y = A$ 和 $y = B$ 以及 $y$ 轴所围成的面积 (平方单位).

$$
\int_{A}^{B} x\mathrm{d}y
$$

## chapter17 微积分基本定理

**微积分的第一基本定理**: 

如果函数 $f$ 在闭区间 $[a, b]$ 上是连续的, 定义 $F$ 为
$$
F(x) = \int_{a}^{x} f(t)\mathrm{d}t, \quad x \in [a, b]
$$
则 $F$ 在开区间 $(a, b)$ 内是可导函数, 而且 $F'(x) = f(x)$.

简而言之，可以总结为
$$
\frac{\mathrm{d}}{\mathrm{d}x} \int_{a}^{x} f(t)\mathrm{d}t = f(x).
$$


**微积分的第二基本定理**: 

如果函数 $f$ 在闭区间 $[a, b]$ 上是连续的, $F$ 是 $f$ 的任意一个反导数 (关于 $x$), 那么有
$$
\int_{a}^{b} f(x)\mathrm{d}x = F(b) - F(a).
$$


**导数和积分公式**
1. 幂函数 (Power Rule)
$$\frac{\mathrm{d}}{\mathrm{d}x} x^a = a x^{a-1}$$
$$\int x^a \mathrm{d}x = \frac{x^{a+1}}{a+1} + C \quad (\text{如果 } a \neq -1)$$
2. 对数函数 (Logarithms)
$$\frac{\mathrm{d}}{\mathrm{d}x} \ln(x) = \frac{1}{x}$$
$$\int \frac{1}{x} \mathrm{d}x = \ln|x| + C$$

3. 指数函数 (Exponentials)
$$\frac{\mathrm{d}}{\mathrm{d}x} e^x = e^x$$
$$\int e^x \mathrm{d}x = e^x + C$$
4. 一般指数函数 (Base-b Exponentials)
$$\frac{\mathrm{d}}{\mathrm{d}x} b^x = b^x \ln(b)$$
$$\int b^x \mathrm{d}x = \frac{b^x}{\ln(b)} + C$$
5. 正弦与余弦 (Sine & Cosine)
$$\frac{\mathrm{d}}{\mathrm{d}x} \sin(x) = \cos(x)$$
$$\int \cos(x) \mathrm{d}x = \sin(x) + C$$
6. 余弦与正弦 (Cosine & Sine)
$$\frac{\mathrm{d}}{\mathrm{d}x} \cos(x) = -\sin(x)$$
$$\int \sin(x) \mathrm{d}x = -\cos(x) + C$$
7. 正切与正割 (Tangent & Secant)
$$\frac{\mathrm{d}}{\mathrm{d}x} \tan(x) = \sec^2(x)$$
$$\int \sec^2(x) \mathrm{d}x = \tan(x) + C$$
8. 正割与正割正切 (Secant & Secant-Tangent)
$$\frac{\mathrm{d}}{\mathrm{d}x} \sec(x) = \sec(x) \tan(x)$$
$$\int \sec(x) \tan(x) \mathrm{d}x = \sec(x) + C$$


## chapter24 泰勒多项式、泰勒级数和幂级数导论


**泰勒近似定理**: 
若 $f$ 在 $x=a$ 光滑, 则在所有次数为 $N$ 或更低的多项式中, 当 $x$ 在 $a$ 附近时, 最近似于 $f(x)$ 的是
$$
P_N(x) = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 +
$$
$$
\frac{f^{(3)}(a)}{3!}(x-a)^3 + \dots + \frac{f^{(N)}(a)}{N!}(x-a)^N.
$$
用求和号表示该公式为：
$$P_N(x) = \sum_{n=0}^{N} \frac{f^{(n)}(a)}{n!} (x-a)^n.$$

>光滑：可以无限次求导下去。（比如 $e^x, \sin x$，这是泰勒级数最喜欢的函数）

**泰勒定理**: 
关于 $x=a$ 的 $N$ 阶余项
$$R_N(x) = \frac{f^{(N+1)}(c)}{(N+1)!}(x-a)^{N+1},$$
其中 $c$ 是介于 $x$ 与 $a$ 之间的一个数.注意数 $c$ 依赖于 $x$ 和 $N$, 一般不能确定! 

由于 $f(x) = P_N(x) + R_N(x)$, 则我们可以写为
$$f(x) = \sum_{n=0}^{N} \frac{f^{(n)}(a)}{n!} (x-a)^n + \frac{f^{(N+1)}(c)}{(N+1)!}(x-a)^{N+1}.$$


## chapter30 微分方程

### 可分离变量
方程 $\frac{\mathrm{d}y}{\mathrm{d}x}  = ky$ 可重新整理为
$$\frac{1}{ky}\mathrm{d}y = \mathrm{d}x,$$