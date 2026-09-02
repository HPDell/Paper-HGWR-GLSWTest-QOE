# 合并论文大纲

## 拟定标题

**Testing Spatial Heterogeneity in Hierarchical and Geographically Weighted Regression: Theory, Simulation, and a Study of Extracurricular Education in China**

## 一句话主线

本文从条件分布出发界定空间异质性，提出检验 HGWR 模型中 group-level spatially weighted（GLSW）效应空间异质性的 bootstrap 与近似 F 检验，并通过模拟实验和中国家庭子女课外艺术及兴趣课程投资案例验证其统计作用和实证价值。

## 文章结构

### 1. Introduction

- 说明空间异质性与空间自相关虽常同时出现，但不是同一统计对象。
- 引出空间层级数据及 HGWR：HGWR 可以估计空间变化的组层效应，但现有工作缺少判断这种变化是否超出随机误差的正式检验。
- 将 QOE 研究作为贯穿式动机：家庭支出受家庭层和省级因素共同影响，若不检验空间异质性，容易把无显著地理差异的变量错误设为 GLSW 效应。
- 明确三项贡献：条件分布定义；bootstrap 与 F 检验及模拟验证；QOE 案例中的模型设定与实证解释。

### 2. Hierarchical and geographically weighted regression

#### 2.1 Definition

- 给出 GLSW、fixed 和 sample-level random（SLR）三类效应。
- 阐明三类效应分别对应省级空间变化、全局稳定关系和组间随机差异。

#### 2.2 Estimator

- 保留 BFML/back-fitting、权重矩阵、带宽与协方差结构的主要推导。
- 明确 GLSW 局部估计和 hat matrix 是后续异质性检验的对象与推导基础。

### 3. Spatial heterogeneity

#### 3.1 Strong and weak spatial heterogeneity

- 定义 spatial random variable。
- 以条件密度随位置变化定义强空间异质性。
- 以条件期望或其他数值特征随位置变化定义弱空间异质性。

#### 3.2 Spatial non-stationarity and spatial autocorrelation

- 区分条件期望的非平稳性与误差相关结构。
- 说明二者可以共存，但检验目标与解释不同。

#### 3.3 From the definition to the testing logic

- 将弱空间异质性转化为“所有位置的条件期望相同”的原假设。
- 对 GLSW 效应，原假设为同一效应在所有组位置相等，而不是效应等于零。
- 以局部估计值的空间方差衡量偏离齐性的程度。
- 说明 bootstrap 与 F 检验使用相同的检验对象和原假设，仅零分布的获得方式不同。

### 4. Testing spatial heterogeneity in GLSW effects

#### 4.1 Bootstrap-based method

- 在齐性原假设下从拟合模型产生响应变量，重估 HGWR，并比较 GLSW 估计方差。

#### 4.2 Distribution-based F test

- 由 GLSW smoother/hat matrix 推导方差统计量的矩近似与自由度。
- 将 F 检验作为高效主检验，并用 bootstrap 进行交叉验证。

#### 4.3 Simulation

- 保留含真实空间异质 GLSW、空间常量 GLSW、固定效应和 SLR 效应的模拟。
- 报告两类检验对真实异质效应与齐性效应的区分结果。

### 5. Case study: spatial inequalities in extracurricular education investment in China

#### 5.1 Context, data, and outcome

- 简述 QOE、课外课程的市场属性及家庭和省级差异。
- 数据包括 2017/2019 CIEFR-HS、统计年鉴、省级边界和 POI。
- 主响应为每小时课外课程支出；支出占比模型作为稳健性/替代结果。

#### 5.2 Effect specification guided by heterogeneity tests

- 省级候选变量先作为 GLSW 效应拟合。
- 对空间异质性不显著的 Youth Palace Count 不保留 GLSW 设定，改为 fixed effect。
- 对共线性变量作删减或改设 fixed effect；以 HLM 前向选择确定 Region Urban 的 SLR 效应。
- 强调检验服务于模型设定，而不只是拟合后描述。

#### 5.3 Evidence of spatial heterogeneity

- 报告各 GLSW 效应的 F 值与显著性。
- 结合地图说明 GDP Primary、CPI、Gini、General Education Budget、High Educated Population、Engel 和 University Recruitment Ratio 的地区差异。
- 将“整体空间异质性显著”与“某一省局部估计显著”严格区分。

#### 5.4 Household-level findings and substantive interpretation

- 报告家庭总支出、资产、父母教育水平、儿童性别和年龄等固定效应。
- 讨论城市—农村差异的 SLR 效应。
- 保留原稿关于经济发展、教育预算、收入差距与公共课外教育资源的政策讨论，但将措辞限定为关联性证据。

#### 5.5 Alternative outcome and limitations

- 概述支出占比模型：总体方向大体一致，但 Asset 不再显著，CPI 异质性减弱，Engel 异质性增强。
- 说明响应变量代理性、两层结构、省以下地理信息缺失、空间共线性和横截面关联解释等限制。

### 6. Discussion and conclusion

- 回到方法主线：地图上的变化本身不是空间异质性的统计证据。
- 总结定义、两类 GLSW 异质性检验、HGWR 模拟与案例研究的相互支持关系。
- 讨论 bootstrap 计算成本、非 i.i.d. 误差、异质性强度量化、多重检验与因果解释限制。

### Appendix and supplemental material

- 保留 F 检验的计算简化推导。
- 保留 QOE 各省详细系数表和替代响应模型结果于 supplemental material。
