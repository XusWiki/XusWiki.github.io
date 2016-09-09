# 2.7 假设检验

# 步骤
1. 说明假设；
2. 确定合适的**检验统计量**以及**概率分布**；
3. 书名显著性水平；
4. 阐述决策规则；
5. 收集数据、计算相应的检验统计量；
6. 统计决策；
7. 做出经济／投资决策

## 原假设&备择假设
- 原假设（null hypothesis）：想要**拒绝**的假设（原假设只能“拒绝”或“不拒绝”，不能“接受”）<center><img src="http://latex.codecogs.com/png.latex?H_{0}"></center>
- 备择假设（alternative hypothesis）：拒绝原假设后得到结论<center><img src="http://latex.codecogs.com/png.latex?H_{a}"></center>

单尾检验（one-tailed test） vs. 双尾检验（two-tailed test）

## 检验统计量①
检验统计量：计算自样本，用于决定是否拒绝原假设。

- 已知样本方差：<center><img src="http://latex.codecogs.com/png.latex?Test\ Statistic=\frac{\bar{X}-\mu_{0}}{\frac{\sigma}{\sqrt{n}}}"></center>
- 未知样本方差：<center><img src="http://latex.codecogs.com/png.latex?Test\ Statistic=\frac{\bar{X}-\mu_{0}}{\frac{s}{\sqrt{n}}}"></center>

检验统计量的三个属性：
1. 检验统计量计算自样本统计量，并非查表得出；
2. 服从正态分布、t 分布、卡方分布、F 分布（样本统计量是随机变量 → 检验统计量是随机变量）；
3. 一般公式只适用于 z 分布、t 分布

## 关键值②
关键值：例如在正态分布中，随机变量有 X% 的可能性**落于 Y 个标准差之内**；Y 就是关键值。

1. 和服从的分布有关；
2. 和显著性水平有关（α）；
3. 考虑是双尾检验还是单尾检验（e.g. 单尾检验的 5% 显著性水平等于双尾检验的 10% 显著性水平）

## 判断规则（是否拒绝原假设）
### 方法 1 基于检验统计量与关键值
1. 确定是单尾检验／双尾检验；
2. 画出**分布**①与**拒绝域（面积等于显著性水平）**②；根据拒绝域求出**关键值**③；
3. **计算检验统计量**（test statistics），观察其是否落在拒绝域内；然，则拒绝原假设；不然，则不拒绝原假设

### 方法 2 基于 p 值（p value）和显著性水平
∵ P 值是可以拒绝原假设的最小显著性水平。
∴ p < α，检验统计量落在拒绝域，拒绝原假设；p > α，不拒绝原假设

## Error Type I／Error Type II
第一类错误：原假设正确，拒绝原假设，“错杀好人”；
第二类错误：原假设错误，不拒绝原假设，“放过坏人”

缩小第一类错误的概率会增大第二类错误的概率；规定的第一类错误的概率（e.g. 5%）就是显著性水平；检验的势（power of the test）：原假设错误的情况，下不犯第二类错误的概率<center><img src="http://latex.codecogs.com/png.latex?Power\ of\ the\ Test=1-P(Type\ II\ Error)"></center>

## 检验均值／方差
|检验类型|具体情况|检验统计量|分布|
|:---|:---|:---:|:---:|
|均值检验|单一正态分布，方差已知|<center><img src="http://latex.codecogs.com/png.latex?Z=\frac{\bar{x}-\mu_{0}}{\frac{\sigma}{\sqrt{n}}}"></center>|<center><img src="http://latex.codecogs.com/png.latex?N(0,1)"></center>|
||单一正态分布，方差未知|<center><img src="http://latex.codecogs.com/png.latex?t_{n-1}=\frac{\bar{x}-\mu_{0}}{\frac{s}{\sqrt{n}}}"></center>|<center><img src="http://latex.codecogs.com/png.latex?t(n-1)"></center>|
||双正态分布，独立样本，方差未知但相等|<center><img src="http://latex.codecogs.com/png.latex?t=\frac{\bar{x}_{1}-\bar{x}_{2}-(\mu_{1}-\mu_{2})}{(\frac{s^{2}_{p}}{n_{1}}-\frac{s^{2}_{p}}{n_{2}})^{\frac{1}{2}}}"></center>|<center><img src="http://latex.codecogs.com/png.latex?t(n_{1}+n_{2}-1)"></center>|
||双正态分布，独立样本，方差未知不相等|<center><img src="http://latex.codecogs.com/png.latex?t=\frac{\bar{x}_{1}-\bar{x}_{2}-(\mu_{1}-\mu_{2})}{(\frac{s^{2}_{1}}{n_{1}}-\frac{s^{2}_{2}}{n_{2}})^{\frac{1}{2}}}"></center>|<center><img src="http://latex.codecogs.com/png.latex?t=(\frac{(\frac{s_{1}^{2}}{n_{1}}+\frac{s_{2}^{2}}{n_{2}})^{2}}{\frac{(s^{2}_{1}/{n_1})^{2}}{n_1}+\frac{(s^{2}_{2}/{n_2})^{2}}{n_2}})"></center>|
||两个非独立总体，成对检验|<center><img src="http://latex.codecogs.com/png.latex?t=\frac{\bar{d}-\mu_{0}}{s_{\bar{d}}}"></center>|<center><img src="http://latex.codecogs.com/png.latex?t=(n-1)"></center>|
|方差检验|单一正态分布|<center><img src="http://latex.codecogs.com/png.latex?\chi^{2}_{n-1}=\frac{(n-1)s^{2}}{\sigma^{2}_{0}}"></center>|<center><img src="http://latex.codecogs.com/png.latex?\chi^{2}(n-1)"></center>|
||双正态分布，独立样本|<center><img src="http://latex.codecogs.com/png.latex?F=\frac{s^{2}_{1}}{s^{2}_{2}}"></center>|<center><img src="http://latex.codecogs.com/png.latex?F(n_{1}-1,n_{2}-1)"></center>|