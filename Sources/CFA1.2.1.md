# 2.1 货币时间价值

## Interest Rate 利率
1. Required return rate (要求回报率);
2. Discount rate (折现率);
3. Opportunity cost (机会成本)


<center><img src="http://latex.codecogs.com/png.latex?Required\ Return\ Rate=Risk\textrm{-}free\ Rate + Risk\ Premiums"></center>

<center><img src="http://latex.codecogs.com/png.latex?Nominal\ Risk\textrm{-}free\ Rate=Real\ Risk\textrm{-}free\ Rate + Inflation\ Rate"></center>

<center><img src="http://latex.codecogs.com/png.latex?Risk\ (Premiums)=Liquidity\ Risk+Default\ Risk+Maturity\ Risk"></center>

风险溢价（risk premiums）：流动性风险、违约风险、期限风险。

## EAR 有效年利率
当利率周期与计息周期不一致，需要计算有效年利率（EAR）。

复利 EAR：


<center><img src="http://latex.codecogs.com/png.latex?EAR=(1+\frac{R}{n})^{n}-1"></center>

连续复利 EAR：


<center><img src="http://latex.codecogs.com/png.latex?EAR=e^{r}-1"></center>

## 现值&终值
### 单笔现金流
年单次复利终值：


<center><img src="http://latex.codecogs.com/png.latex?FV=PV\times(1+r)^{n}"></center>
年多次复利终值：


<center><img src="http://latex.codecogs.com/png.latex?FV=PV\times(1+\frac{r}{m})^{m\times n}"></center>
年连续复利终值：


<center><img src="http://latex.codecogs.com/png.latex?FV=PV\times e^{r\times n}"></center>
现值：


<center><img src="http://latex.codecogs.com/png.latex?PV=\frac{FV}{(1+r)^{n}}=FV\times(1+r)^{-n}"></center>

### 年金
年金是本单元重点。不要求掌握公式，但要求在知道`N`、`I/Y`、`PMT`、`FV`、`PV`中任意给定的四个值时，可以**使用计算器**求出另一个值。

普通年金（normal annuity）：


<center><img src="http://latex.codecogs.com/png.latex?F=A\times\frac{(1+i)^{n}-1}{i}"></center>

<center><img src="http://latex.codecogs.com/png.latex?P=A\times\frac{1-(1+i)^{-n}}{i}"></center>

先付年金（annuity due）：


<center><img src="http://latex.codecogs.com/png.latex?F=A\times[\frac{(1+i)^{n+1}-1}{i}-1]"></center>

<center><img src="http://latex.codecogs.com/png.latex?P=A\times[\frac{1-(1+i)^{-(n-1)}}{i}+1]"></center>

递延年金（deferred annuity）：**普通年金的一种特殊形式**，一个 n 期年金的第一期流入现金流，在第 m 期开始。计算终值时与普通年金无差别；计算现值时①先求出这个 n 期年金的限制。②再计算这个现值的 m 期的折现值。

永续年金（perpetuity）：永续年金无法计算终值


<center><img src="http://latex.codecogs.com/png.latex?P=\frac{A}{i}"></center>

## 留言
[gimmick:Disqus](xuswiki.disqus.com)