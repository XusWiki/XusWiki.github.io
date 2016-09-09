# 2.4 概率论基础
1. 单一事件：<center><img src="http://latex.codecogs.com/png.latex?0\leqslant P(E) \leqslant 1"></center>
2. 遍历事件／互斥事件：<center><img src="http://latex.codecogs.com/png.latex?\sum_{I=1}^{n}P(E_{i})=1"></center>

## 概率分类
<center><img src="http://latex.codecogs.com/png.latex?\left\{\begin{matrix}(1)\ Objective\ Probability\left\{\begin{matrix}Emprical\ Probability\\Priori\ Probability\end{matrix}\right.\\(2)\ Subjective\ Probability\end{matrix}\right."></center>

经验概率①：根据以前数据，分析未来的可能性；
先验概率①：根据以前数据，分析当时的可能性；
主观概率②：掺入主观意见的概率

## 赔率
- 胜率：<center><img src="http://latex.codecogs.com/png.latex?Odds\ for\ E=\frac{P(E)}{1-P(E)}"></center>
- 赔率：<center><img src="http://latex.codecogs.com/png.latex?Odds\ against\ E=\frac{1-P(E)}{P(E)}"></center>

## 无条件概率&条件概率
无条件概率／边际概率：时间单独发生的概率，不考虑其他事件；
条件概率：已知 B 发生的情况下，A 发生的概率<center><img src="http://latex.codecogs.com/png.latex?P(A\mid B)"></center>

## 加法法则&乘法法则
乘法法则／联合概率（joint probability）：时间同时发生的概率；
- 独立事件：<img src="http://latex.codecogs.com/png.latex?P(AB)=P(A\mid B)\times P(B)=P(B\mid A)\times P(A)">
- 互斥事件：<img src="http://latex.codecogs.com/png.latex?P(AB)=P(A\mid B)\times P(B)=P(B\mid A)\times P(A)=0">

<center><img src="http://latex.codecogs.com/png.latex?P(B\mid A)=\frac{P(AB)}{P(A)}"></center>

<center><img src="http://latex.codecogs.com/png.latex?P(AB)=P(B\mid A)\times{P(A)}"></center>
<center><img src="http://latex.codecogs.com/png.latex?P(AB)=P(A\mid B)\times{P(B)}"></center>

加法法则：两个事件至少有一个发生的概率
<center><img src="http://latex.codecogs.com/png.latex?P(A\ or\ B)=P(A)+P(B)-P(AB)"></center>

### 独立事件
<center><img src="http://latex.codecogs.com/png.latex?P(AB)=P(A)\times P(B)"></center>

## 全概率公式
全概率公式：所有影响因素下时间概率的和。
<center><img src="http://latex.codecogs.com/png.latex?P(A)=P(\frac{A}{S_1})P(S_1)+P(\frac{A}{S_2})P(S_2)+\dots+P(\frac{A}{S_n})P(S_n)"></center>

## 协方差&相关系数
协方差（covariance）：两个随机变量的同向性；一个变量与其自身的协方差是其方差；
<center><img src="http://latex.codecogs.com/png.latex?Cov(X,Y)=E[(X_{i}-\bar{X})(Y_{I}-\bar{Y})]"></center>

相关系数：
<center><img src="http://latex.codecogs.com/png.latex?\rho_{X,Y}=\frac{Cov(X,Y)}{\sigma_{X}\sigma_{Y}}"></center>

## 贝叶斯公式
∵<center><img src="http://latex.codecogs.com/png.latex?P(AB)=P(A)\times P(B)=P(B\mid A)\times P(A)"></center>
∴<center><img src="http://latex.codecogs.com/png.latex?P(A\mid B)=\frac{P(B\mid A)}{P(B)}\times P(A)"></center>

## 计数原理
- 将 n 个物品放在 n 个位置；
<center><img src="http://latex.codecogs.com/png.latex?n!"></center>

- 标号问题（labeling）：n 个物品，需标上 k 个标签；
<center><img src="http://latex.codecogs.com/png.latex?\frac{n!}{n_{1}!\times n_{1}!\times \dots\times n_{k}!}"></center>

- 组合问题；
<center><img src="http://latex.codecogs.com/png.latex?_{n}C_{r}=\frac{n!}{(n-r)!\times r!}"></center>

- 排列问题
<center><img src="http://latex.codecogs.com/png.latex?_{n}P_{r}=\frac{n!}{(1-r)!}"></center>
