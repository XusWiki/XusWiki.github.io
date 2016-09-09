# 2.5 常见概率分布
<center><img src="http://latex.codecogs.com/png.latex?Random\ Variable\left\{\begin{matrix}Discrete\ Random\ Variable\ (1)\left\{\begin{matrix}Discrete\ Uniform\ Distribution\ (3)\\Binomial\ Distribution\ (4)\end{matrix}\right.\\Continuons\ Random\ Variable\ (2)\left\{\begin{matrix}Continuons\ Uniform\ Distribution\ (5)\\Normal\ Distribution\ (6)\end{matrix}\right.\end{matrix}\right."></center>

- 离散型随机变量①：可能性取值有限（e.g. 硬币、骰子）；
- 连续型随机变量②：可能性取值无限（e.g. 股票价格）；
- 离散均匀分布③：离散型随机变量，所有可能性概率一致（e.g. 硬币、骰子）；
- 二项分布④：只有两种可能性，可能性可能不一致；
- 连续均匀分布⑤：每个点的可能性一致；
- 正态分布⑥：对称分布；均值 = 中位数 = 众数

二项实验在 n 次试验中，x 次试验成功的概率：
<center><img src="http://latex.codecogs.com/png.latex?p(x)=P(X=x)=_{n}C_{x}\times p^{x}\times(1-p)^{n-x}"></center>

## 正态分布
1. 均值 = 中位数 = 众数；
2. 正态分布可用均值、方差完全描述：<center><img src="http://latex.codecogs.com/png.latex?X\sim N(\mu,\sigma^{2})"></center>
3. 对称分布、偏度为 0、超额峰度为 0

### 置信区间
1. <img src="http://latex.codecogs.com/png.latex?68\%,\ E(x)\pm 1 \sigma">；
2. <img src="http://latex.codecogs.com/png.latex?90\%,\ E(x)\pm 1.65 \sigma">；
3. <img src="http://latex.codecogs.com/png.latex?95\%,\ E(x)\pm 1.96 \sigma">；
4. <img src="http://latex.codecogs.com/png.latex?99\%,\ E(x)\pm 2.58 \sigma">

### 标准正态分布／Z 分布
标准正态分布期望值为 0，标准差为 1：
<center><img src="http://latex.codecogs.com/png.latex?X\sim N(0,1)"></center>

任何一个正态分布可以转换为标准正态分布，转换目的是为了查概率分布表。
<center><img src="http://latex.codecogs.com/png.latex?Z=\frac{X-\mu}{\sigma}"></center>
<center><img src="http://latex.codecogs.com/png.latex?E(\frac{X-\mu}{\sigma})=\frac{E(X)-\mu}{\sigma}=0"></center>
<center><img src="http://latex.codecogs.com/png.latex?Var(\frac{X-\mu}{\sigma})=\frac{Var(X)}{\sigma^{2}}=0"></center>

## 超亏风险&第一安全比率
超亏风险：投资收益率小雨要求回报率的风险。

第一安全比率（SFR）：
<center><img src="http://latex.codecogs.com/png.latex?SFR=\frac{E(R_{P})-R_{L}}{\sigma_{P}}"></center>
夏普比率（SFR 的一种特殊形式）：以无风险利率作为最低要求回报率
<center><img src="http://latex.codecogs.com/png.latex?SFR=\frac{E(R_{P})-R_{f}}{\sigma_{P}}"></center>

1. 计算每个投资组合的 SFR；
2. 选择 SFR 最高的组合

## 对数正态分布
1. 对数正态分布：如果随机变量 X 的自然对数（lnX）符合正态分布，X 符合对数正态分布（X > 0）；
2. 对数正态分布取值范围大于零；
3. 对数正态分布右偏

## 跟踪误差
用于判断基金经理业绩，若果值小于 0，说明这投资组合没有跑赢大盘。
<center><img src="http://latex.codecogs.com/png.latex?Tracking\ Error=Total\ Return-Benchmark\ Return"></center>

## 历史模拟&蒙特卡罗模拟
利用模拟数据求得数据分布情况，并计算平均值（预期收益率）。区别是历史模拟使用历史数据、蒙特卡罗模拟利用计算机生成。
历：优点，简单；缺点，无法处理**没有发生过的情况**；
蒙：优点，**可以处理没有发生过的情况**；缺点，比较复杂；
