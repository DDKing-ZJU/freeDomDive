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

* 必要条件和推出符号的关系
&emsp;&emsp;一些翻译题中会出现"necessary condition","only if"字样，需要翻译成"implies"符号，它们的关系是：

> The necessary condition of $A$ is $B$ —— $A \rightarrow B$
> $A$ holds only if $B$ holds &emsp;&emsp;&emsp;&emsp;&emsp;—— $A \rightarrow B$

* 逻辑符号的优先级

&emsp;&emsp;需要注意的是，推出符号$\rightarrow \leftarrow \leftrightarrow$的优先级要大于合取析取$\wedge \vee$，所以在表示隐含关系时，尽量能写括号就写括号。比如$(p \vee q) \rightarrow r$