# 2.6 抽样和估计
总体 → 抽样（sampling）→ 样本 → 估计（estimation）→ 总体；

- 简单随机抽样（simple random sampling）：每个个体被抽中的几率一致；
- 分层随机抽样（stratified random sampling）：先将总体分割为子集，对每个自己进行简单随机抽样

抽样误差（sampling error）：样本与总体的差异，造成成对总体参数估计的误差 → 样本的统计量是随机变量，为了可信估计总体参数 → 中心极限定理；

## 时间序列&截面数据
1. 时间序列数据：在固定间的时间上，以时间顺序排列的离散数据集合（e.g. 每年／月／日）；
2. 截面数据：某一固定时间点上的一组数据（同一时间点／不排序）

## 中心极限定理
1. 任意总体分布 → 样本（n ≥ 30）均值都为正态分布；
2. 样本**均值的期望值**等于总体均值<center><img src="http://latex.codecogs.com/png.latex?E(\bar{X})=\mu"></center>
3. 样本均值的方差等与总体方差处以样本量<center><img src="http://latex.codecogs.com/png.latex?Var(\bar{X})=\frac{\sigma^2}{n}"></center>

※ 样本均值服从正态分布 → 可以做概率估计；
※ 样本量需要大于 30。

## 标准误
标准误（standard error）:样本均值的标准差（∵ 样本参数是随机变量）；
- 已知总体标准差：<center><img src="http://latex.codecogs.com/png.latex?\sigma_{\bar{x}}=\frac{\sigma}{\sqrt{n}}"></center>
- 未知总体标准差：<center><img src="http://latex.codecogs.com/png.latex?s_{\bar{x}}=\frac{s}{\sqrt{n}}"></center>

## 好的估计量的性质
1. 无偏性：样本参数的期望值等于总体参数；
2. 有效性：方差最小的无偏估计量 → 最小方差无偏估计量／有效估计量 → 方差越小离散程度越小，越接近总体均值；
3. 一致性：样本容量更大的无偏估计量

## 点估计&区间估计
- 点估计：认定某一特定数值为总体参数；
- 区间估计／置信区间：认定总体参数有一定**几率**①处于特定**区间**②
	- 区间：<center><img src="http://latex.codecogs.com/png.latex?\bar{X}\pm Z_{\frac{\alpha}{2}}\times\frac{\sigma}{\sqrt{n}}"></center>
	- 置信度（confidence level）：总体参数处于区间的概率<center><img src="http://latex.codecogs.com/png.latex?1-\alpha"></center>
	- 显著性水平（significance level）：<center><img src="http://latex.codecogs.com/png.latex?\alpha"></center>

## 学生 t 分布
<center><img src="http://latex.codecogs.com/png.latex?t=(\bar{x}-\mu)\times \frac{s}{\sqrt{n}}"></center>

1. t 对称分布，中心周围均值；
2. 一个变量“自由度” = (n - 1)；
3. 低峰肥尾；
4. 自由度 ↑，t 分布逼近正态分布

|类型|检验统计量||
|---|:---:|:---:|
||小样本（n < 30）|大样本（n ≥ 30）|
|正态分布，总体方差已知|z 统计量|z 统计量|
|正态分布，总体方差未知|t 统计量|z 统计量／t 统计量|
|正态分布，总体方差已知|-|z 统计量|
|正态分布，总体方差未知|-|z 统计量／t 统计量|

※方差已知用 z，方差未知用 t，小样本不可求。


## Bias（偏差）
1. 数据挖掘偏差（data-mining bias）：把偶然当成必然；
2. 样本选择偏差（sample selection bias）：因为样本选择过程不能涵盖全部个体造成的偏差；
3. 存活偏差（survivorship bias）：e.g. 股票指数中不包含已经退市、倒闭的企业;
4. 时间间隔偏差（time-period bias）：只检验使结论成立的特定时间段
