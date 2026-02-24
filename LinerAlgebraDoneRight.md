
- [chapter1 Vector Space](#chapter1-vector-space)
- [chapter2 finite-dimensional vector space](#chapter2-finite-dimensional-vector-space)
- [chapter3 liner map](#chapter3-liner-map)


## chapter1 Vector Space




**定义1.10：*列表* (list)，*长度* (length)**

* 假设 $n$ 是一个非负整数。一个**长度**为 $n$ 的**列表**是 $n$ 个元素的有序集合（这些元素可能是数字、其他列表或更抽象的对象）。
* 两个列表相等，当且仅当它们具有相同的长度，并且以相同的顺序包含相同的元素。
  

**1.11 定义：$\mathbf{F}^n$，*坐标* (coordinate)**

$\mathbf{F}^n$ 是所有由 $\mathbf{F}$ 中元素组成的长度为 $n$ 的列表的集合：


$$\mathbf{F}^n = \{(x_1, \dots, x_n) : x_k \in \mathbf{F} \text{ 对于 } k = 1, \dots, n\}$$

对于 $(x_1, \dots, x_n) \in \mathbf{F}^n$ 以及 $k \in \{1, \dots, n\}$，我们称 $x_k$ 是 $(x_1, \dots, x_n)$ 的第 $k$ 个*坐标*。






**1.20 定义：*向量空间* (vector space)**

一个**向量空间**是指一个集合 $V$，连同在 $V$ 上定义的加法和标量乘法，使得以下性质成立：

* **交换律 (commutativity)**
对于所有的 $u, v \in V$，有 $u + v = v + u$。
* **结合律 (associativity)**
对于所有的 $u, v, w \in V$ 以及所有的 $a, b \in \mathbf{F}$，有 $(u + v) + w = u + (v + w)$ 且 $(ab)v = a(bv)$。
* **加法单位元 (additive identity)**
存在一个元素 $0 \in V$，使得对于所有的 $v \in V$，有 $v + 0 = v$。
* **加法逆元 (additive inverse)**
对于每一个 $v \in V$，存在 $w \in V$ 使得 $v + w = 0$。
* **乘法单位元 (multiplicative identity)**
对于所有的 $v \in V$，有 $1v = v$。
* **分配律 (distributive properties)**
对于所有的 $a, b \in \mathbf{F}$ 以及所有的 $u, v \in V$，有 $a(u + v) = au + av$ 且 $(a + b)v = av + bv$。



**1.21 定义**：*向量* (vector)，*点* (point)

向量空间的元素被称为*向量*或*点*。


这是一张关于实向量空间和复向量空间的定义的图片，是对我们前面讨论过的“域 $\mathbf{F}$”的具体化落地。它的完整翻译和 Markdown 格式如下：

**1.22 定义：*实向量空间* (real vector space)，*复向量空间* (complex vector space)**

* 定义在 $\mathbf{R}$（实数域）上的向量空间称为**实向量空间**。
* 定义在 $\mathbf{C}$（复数域）上的向量空间称为**复向量空间**。




**1.24 定义：**：

记号 (notation)：$\mathbf{F}^S$
- 如果 $S$ 是一个集合，那么 $\mathbf{F}^S$ 表示从 $S$ 映射到 $\mathbf{F}$ 的所有函数的集合。
- 对于 $f, g \in \mathbf{F}^S$，它们的和 (sum) $f + g \in \mathbf{F}^S$ 是由下式定义的函数：

  $$(f + g)(x) = f(x) + g(x)$$
  对所有的 $x \in S$ 成立。
-  对于 $\lambda \in \mathbf{F}$ 以及 $f \in \mathbf{F}^S$，它们的乘积 (product) $\lambda f \in \mathbf{F}^S$ 是由下式定义的函数：
    $$(\lambda f)(x) = \lambda f(x)$$
    对所有的 $x \in S$ 成立。


这张图片的完整翻译如下：

**1.29 记号：$V$**

在本书的其余部分中，$V$ 表示定义在 $\mathbf{F}$ 上的向量空间。

---

**定义3**：

**加法逆元的唯一性**

**证明**：

假设 $V$ 是一个向量空间。令 $v \in V$。假设 $w$ 和 $w'$ 都是 $v$ 的加法逆元 (additive inverses)。那么
$$w = w + 0 = w + (v + w') = (w + v) + w' = 0 + w' = w'.$$
因此 $w = w'$，这正是我们想要证明的（证毕）。


## chapter2 finite-dimensional vector space

**定义1**：

多项式 (polynomial)，$\mathcal{P}(\mathbf{F})$

- 一个函数 $p: \mathbf{F} \to \mathbf{F}$ 被称为系数在 $\mathbf{F}$ 中的多项式，如果存在 $a_0, \dots, a_m \in \mathbf{F}$ 使得
$$
    p(z) = a_0 + a_1z + a_2z^2 + \dots + a_mz^m
$$

 对所有的 $z \in \mathbf{F}$ 成立。

- $\mathcal{P}(\mathbf{F})$ 是所有系数在 $\mathbf{F}$ 中的多项式的集合。



**2.17 定义：*线性相关* (linearly dependent)**

* $V$ 中的一个向量列表被称为**线性相关**的，如果它不是线性无关的。
* 换句话说，$V$ 中的向量列表 $v_1, \dots, v_m$ 是线性相关的，如果存在不全为 0 的 $a_1, \dots, a_m \in \mathbf{F}$，使得 $a_1v_1 + \dots + a_mv_m = 0$。


这张图片的完整翻译和 Markdown 格式如下：

**2.34 基的长度与基的选择无关 (basis length does not depend on basis)**

一个有限维向量空间的任意两个基具有相同的长度。
>这个定理的大白话翻译就是：对于同一个空间，无论你用什么千奇百怪的方式去挑选“基准向量”，只要它们够资格成为一组“基”，那么这组基准向量的总数量绝对是固定不变的。


这张图片的完整翻译和 Markdown 格式如下：

**2.35 定义：*维度* (dimension)，$\dim V$**

* 一个有限维向量空间的**维度**是指该向量空间的任意一个基的长度。
* 有限维向量空间 $V$ 的维度记作 $\dim V$。
>维度的大小即 基准基 分量的数量

## chapter3 liner map


**本章的通用假设** (standing assumptions for this chapter)
- $F$表示 $R$（实数集或）$C$（复数集）。
- $U$、$V$ 和 $W$ 表示 F 上的向量空间。

简单来说，线性映射（Linear Map） 就是一种特殊的“函数”或者“变换规则”。假设有一个映射 $T$，它把向量空间 $V$ 里的元素（输入）变成向量空间 $W$ 里的元素（输出）。我们要管这个 $T$ 叫“线性映射”，它就必须且只需绝对服从两条铁律：
1. 可加性 (Additivity)如果你把两个输入先加起来，然后再扔进这个映射里，它的结果必须等于把这两个输入分别扔进去处理后，再把结果加起来。数学表达： 对于 $V$ 中的任意向量 $u$ 和 $v$，都必须满足：
   $$T(u + v) = T(u) + T(v)$$
2. 齐次性 / 比例性 (Homogeneity)如果你把一个输入放大或缩小 $\lambda$ 倍，然后再扔进映射里，它的结果必须等于先把原输入扔进去处理，然后再把结果放大或缩小 $\lambda$ 倍。数学表达： 对于 $V$ 中的任意向量 $v$ 和任意标量 $\lambda$，都必须满足：
   $$T(\lambda v) = \lambda T(v)$$



**定义：线性映射的矩阵** (matrix of a linear map)

$\mathcal{M}(T)$假设 $T \in \mathcal{L}(V, W)$，且 $v_1, \dots, v_n$ 是 $V$ 的一组基 (basis)，$w_1, \dots, w_m$ 是 $W$ 的一组基。$T$ 关于这些基的矩阵 (matrix) 是一个 $m \times n$ 的矩阵 $\mathcal{M}(T)$，其元素 $A_{j,k}$ 由下式定义：
$$
T v_k = A_{1,k} w_1 + \dots + A_{m,k} w_m.
$$
如果基 $v_1, \dots, v_n$ 和 $w_1, \dots, w_m$ 在上下文中不够明确，那么就使用记号 $\mathcal{M}(T, (v_1, \dots, v_n), (w_1, \dots, w_m))$。