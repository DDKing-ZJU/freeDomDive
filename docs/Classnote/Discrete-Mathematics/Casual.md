---
    comments: true
---


# 琐记

---

&emsp;&emsp;记录一些琐碎的知识点，主要是不熟悉的知识点和易错点。

!!! question "待解决的问题"
    * 两个不同的量词（一个存在一个任意）是不可以交换的，那么两个相同的量词能否交换？

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