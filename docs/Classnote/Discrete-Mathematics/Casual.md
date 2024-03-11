---
    comments: true
---


# 琐记

---

&emsp;&emsp;记录一些琐碎的知识点，主要是不熟悉的知识点和易错点。

!!! question "待解决的问题"
    * 两个不同的量词（一个存在一个任意）是不可以交换的，那么两个相同的量词能否交换？
    * 取反$\neg$和推出$\rightarrow$哪一个优先级更高？

* **For any** 在逻辑翻译中有歧义，因为英语中any有时是some的意思。

* 怎么把无关的项从Quantifier中去除：

$$
    \forall x(P(x) \wedge Q) \equiv \forall xP(x) \wedge Q \\
    \forall x(P(x) \vee Q) \equiv \forall xP(x) \vee Q \\
    \exists x(P(x) \wedge Q) \equiv \exists xP(x) \wedge Q \\
    \exists x(P(x) \vee Q) \equiv \exists xP(x) \vee Q \\
    \forall x(Q \rightarrow P(x)) \equiv Q \rightarrow \forall xP(x) \\
    \exists x(Q \rightarrow P(x)) \equiv Q \rightarrow \exists xP(x) \\
    \space \\
    \text{The formula below have changes on quantifier.} \\
    \forall x(P(x) \rightarrow Q) \equiv \exists xP(x) \rightarrow Q \\
    \exists x(P(x) \rightarrow Q) \equiv \forall xP(x) \rightarrow Q \\
$$
> 记忆方法：直接拆括号，对于最后两个式子，因为$P(x)$在前，把推导符号转换成析取的时候要取反，取反前置会导致谓词改变。

* 必要条件和推出符号的关系
&emsp;&emsp;一些翻译题中会出现"necessary condition","only if"字样，需要翻译成"implies"符号，它们的关系是：

> The necessary condition of $A$ is $B$ —— $A \rightarrow B$

> $A$ holds only if $B$ holds &emsp;&emsp;&emsp;&emsp;&emsp;—— $A \rightarrow B$

* 逻辑符号的优先级

&emsp;&emsp;需要注意的是，推出符号$\rightarrow \leftarrow \leftrightarrow$的优先级要大于合取析取$\wedge \vee$，所以在表示隐含关系时，尽量能写括号就写括号。比如$(p \vee q) \rightarrow r$

* 前束范式转换步骤（prenex normal form）
1. 如果发现无关的部分有变量名复用（如$\exist xP(x) \rightarrow \forall xP(x)$）则需要改变变量名，避免变量名重复。
2. 通过上述的谓词公式，把$\forall$和$\exists$提到最前面。注意谓词的前后顺序，实际上带谓词的变量本身就省略了一层括号。例如$\exist xP(x) \rightarrow \forall yP(y) \equiv \forall y\exist x(P(x) \rightarrow P(y))$

* 证伪可以用反例，不一定硬上公式转化。