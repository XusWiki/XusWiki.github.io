# 2.1 折现现金流方法的应用
折现现金流考虑两点：①折现后的值；②使用什么折现率。考虑问题①要利用 NPV & IRR；考虑问题②要掌握多种收益率的计算方法。

## NPV & IRR
NPV:


<center><img src="http://latex.codecogs.com/png.latex?NPV=PV-CF_{0}=\sum^{N}_{t=0}\frac{CF_{t}}{(1+r)^{t}}"></center>

IRR:


<center><img src="http://latex.codecogs.com/png.latex?NPV=\sum^{N}_{t=0}\frac{CF_{t}}{(1+IRR)^{t}}=0"></center>

基于 NPV & IRR 的决策：
- 独立项目（independent project）：选择 NPV 为正，IRR 大于要求收益率的项目；
- 互斥项目（mutually exclusive project）：若 NPV 与 IRR 结论冲突，选择 NPV 较大的项目

## 折现率
银行贴现收益率是一个折现率，用于计算 T-bill；HPY 是持有期收益率（而非年华的收益率）；如果要年化 HPY，则要使用 EAY；EAY 和 MMY 是年化的 HPY，EAY 使用复利（365 天），MMY 使用单利（360 天）；

持有期收益（holding period return, HPR）／持有期收益率（holding period yield, HPY）：由两部分组成，①资本利得，②红利。


<center><img src="http://latex.codecogs.com/png.latex?HPY=\frac{P_{t}-P_{t-1}+CF_{t}}{P_{t-1}}"></center>

有效年利率（effective annual yield, EAY）：EAY 把 HPR 换算为年收益率，便于比较各种金融资产。


<center><img src="http://latex.codecogs.com/png.latex?EAY=(1+HPY)^{\frac{365}{t}}-1"></center>

银行贴现收益率（bank discount yield）：


<center><img src="http://latex.codecogs.com/png.latex?r_{BD}=\frac{F-P}{F}\times\frac{360}{t}"></center>

货币市场收益率（money market yield）：


<center><img src="http://latex.codecogs.com/png.latex?r_{BD}=\frac{F-P}{P}\times\frac{360}{t}"></center>

债券等价收益率（bond equivalent yield, BEY）


<center><img src="http://latex.codecogs.com/png.latex?P=\frac{C}{1+y}+\frac{C}{(1+y)^2}+\dots+\frac{C+M}{(1+y)^n}"></center>

## 加权收益率
货币加权收益率（money-weighted rate of return）：求出符合条件的 R；以现金流为加权。


<center><img src="http://latex.codecogs.com/png.latex?V_{0}=\frac{C_{1}}{1+R_{D}}+\frac{C_{2}}{(1+R_{D})^{2}}+\dots+\frac{C_{N}+V_{N}}{(1+R_{D})^{N}}"></center>

时间加权收益率（time-weighted rate of return）/几何平均：


<center><img src="http://latex.codecogs.com/png.latex?R_{T}=[(1+R_{P1})\times(1+R_{P2})\times \dots \times(1+R_{PN})]^{\frac{1}{N}}-1"></center>

## 留言
[gimmick:Disqus](xuswiki.disqus.com)