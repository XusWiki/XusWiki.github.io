# 2.3 数理统计
## Fundamental Concepts
1. 描述性统计：求解数据的统计量、描述数据形式；
2. 推断性计量：预测和判断

<center><img src="http://latex.codecogs.com/png.latex?Statistics\left\{\begin{matrix}Descriptive\ statistics\ (1)\\Statistical\ Inference\ (2)\end{matrix}\right." title="\left\{\begin{matrix}1\\2\end{matrix}\right." /></center>

### 总体&样本
1. 总体（population）→ 总体参数（population parameter）：想要知道；
2. 样本（sample）→ 样本统计量（sample statistics）：实际得到 → 估计总体参数

<center><img src="http://latex.codecogs.com/png.latex?sample\in population,sample\ size\leqslant population\ size"></center>

### 测量等级
1. 名义分类（nominal scale）：分类不排序；
2. 排序分类（ordinal scale）：分类并排序；
3. 区间分类（interval scale）：分类并排序、排序差值相等；
4. 比率分类（ratio scale）：分类并排序、排序差值相等、有绝对零点

## Central Tendency（中心趋势）
<center><img src="http://latex.codecogs.com/png.latex?Central\ Tendency\left\{\begin{matrix}Mean\ (1)\left\{\begin{matrix}Arithmetic\ Mean\\Geometric\ Mean\\Weighted\ Mean\\Harmonic\ Mean\end{matrix}\right\\Mode\ (2)\\Median\ (3)\end{matrix}\right." title="\left\{\begin{matrix}1\\2\end{matrix}\right." /></center>

### Mean
- 算术平均数：

<center><img src="http://latex.codecogs.com/png.latex?\bar{X}=\sum_{i=1}^{N}\frac{X_{i}}{N}"></center>

- 几何平均数：

<center><img src="http://latex.codecogs.com/png.latex?G=\sqrt[n]{X_{1}\times X_{2}\times \dots \times X_{n}}"></center>

- 加权平均数：

<center><img src="http://latex.codecogs.com/png.latex?\bar{X}=\sum_{i=1}^{N}w_{i}X_{i}"></center>

<center><img src="http://latex.codecogs.com/png.latex?\sum_{i=1}^{N}w_{i}=1"></center>

- 调和平均数（倒数的平均数）：

<center><img src="http://latex.codecogs.com/png.latex?\bar{X}_{n}=n/\sum_{i=1}^{N}\frac{1}{X_i}"></center>

### Mode
众数：出现次数最多的观测值；众数可以不唯一。

### Median
中位数：当出现两个数处在中间位置，中位数为这两个数的均值。

## Quantile（分位数）
分位数：将数据分割为相等数量的部分。
1. 四分位数（quartile）；
2. 五分位数（quintile）；
3. 十分位数（deciles）；
4. 百分位数（percentile）

<center><img src="http://latex.codecogs.com/png.latex?L_{y}=(n+1)\times \frac{y}{100}"></center>

分位数不包含被包含在分位内（结束一个数时 50% 分位数，一定有 50% 的数据出现在它左边）；如果分位数的序数是一个分数时，分位数应为①前一个数加上②后一个数与前一个数的差值乘以分数。

## Dispersion（离散程度）

<center><img src="http://latex.codecogs.com/png.latex?Dispersion\left\{\begin{matrix}Range\\Mean\&space;Absolute\&space;Deviation\\Variance\\Standard\&space;Deviation\end{matrix}\right." title="Dispersion\left\{\begin{matrix}Range\\Mean\ Absolute\ Deviation\\Variance\\Standard\ Deviation\end{matrix}\right." /></center>

- Range（极差）：最大值减最小值；

<center><img src="http://latex.codecogs.com/png.latex?Range=Maximum\ Value-Minimum\ Value"></center>

- Mean Absolute Deviation（均差绝对偏差，MAD）：

<center><img src="http://latex.codecogs.com/png.latex?MAD=(\sum_{i=1}^{N}\left | R_{i}-\bar{R} \right |)/n"></center>

- Variance（方差）：注意总体分母为 N，样本分母为（n-1）。

总体方差：
<center><img src="http://latex.codecogs.com/png.latex?Var(R)=\sigma^{2}=[\sum_{I=1}^{N}(R_i-\mu_{R})^{2}]/N"></center>

<center><img src="http://latex.codecogs.com/png.latex?\mu_{R}=\sum_{I=1}^{N}R_{I}/N"></center>

样本方差：
<center><img src="http://latex.codecogs.com/png.latex?s^2=\sum_{I=1}^{N}(x_{I}-\bar{x})^2/(n-1)"></center>

总体标准差：
<center><img src="http://latex.codecogs.com/png.latex?\sigma=\sqrt{\sigma^2}"></center>

样本标准差：
<center><img src="http://latex.codecogs.com/png.latex?s=\sqrt{\sum_{I=1}^{N}(x_{I}-\bar{x})^2/(n-1)}"></center>

## 切比雪夫不等式
随机分布的分布可能性；**无论何种分布**，个体落在均值周围 K 个标准差内的概率。

<center><img src="http://latex.codecogs.com/png.latex?P(\left | X-\mu \right |\leqslant K\sigma)\geqslant 1-\frac{1}{k^2}"></center>

## 变异系数&夏普比率
变异系数：标准差与均值的比率；标准化**不同规模样本的波动率**。

<center><img src="http://latex.codecogs.com/png.latex?CV=\frac{s}{X}"></center>

夏普比率：单位风险带来的收益。

<center><img src="http://latex.codecogs.com/png.latex?Sharpe\ Ratio=\frac{\bar{R_p}-\bar{R_f}}{\sigma_p}"></center>

## 偏度&峰度

### Skewness（偏度）
1. positively skewed（正偏）：均值 > 中位数；均值 > 众数；
2. Normal distribution（正态分布）；
3. negatively skewed（负偏）：均值 < 中位数；均值 < 众数

### Kurtosis（峰度）
1. lepto kurtic（高峰）→ “高峰肥尾”；
2. Platy kurtic（低峰）

Excess kurtosis（超额峰度）：因为正态分布的峰度为 3，超额峰度等于（K - 3）。
