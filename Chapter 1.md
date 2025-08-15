# 第 1 章　电路元件与电路基本定律
## 1.1　电流、电压与电功率
### 电流
- 定义：$i=\dfrac{\mathrm{d}q}{\mathrm{d}t}$，其中 $\mathrm{d}q$ 是 $\mathrm{d}t$ 时间内通过截面的电荷量。
- 方向：正电荷运动的方向。
- 单位：
	- 电荷：库［仑］$\pu{C}$；
	- 电流：安［培］$\pu{A}$，$\pu{1A}=\pu{1C}/\pu{1s}$。
- **参考方向**：任意假设的电流方向，在图中导线上标出。$i_{ab}=-i_{ba}$。如图。
  ![[current-direction.png]]
### 电压
- 定义：$u_{ab}=\dfrac{\mathrm{d}W_{ab}}{\mathrm{d}q}$，其中 $\mathrm{d}W_{ab}$ 是电场力将电荷 $\mathrm{d}q$ 从 $a$ 移动到 $b$ 所做的功。
- 单位：伏［特］$\pu{V}$。
- **电位**（**电势**）：任选一点为 **参考点**（零电位点），则其他点到参考点的电压称为电位，记为 $\varphi$。电压又称电位差或电位降：$u_{ab}=\varphi_a-\varphi_b$。
- **参考方向**：任意假设，在图中用箭头或正负极标出，若由节点 $a$ 指向 $b$，或 $a$ 为正极 $b$ 为负极，则 $\varphi_{ab}$ 为正方向。有 $u_{ab}=\varphi_a-\varphi_b=-(\varphi_b-\varphi_a)=-u_{ba}$。如图。
  ![[voltage-direction.png]]
### 电动势
- 定义：$e=\dfrac{\mathrm{d}W}{\mathrm{d}q}$，其中 $\mathrm{d}W$ 是电源将电荷 $\mathrm{d}q$ 从负极经电源内部移到正极所做的功。
- 单位：$\pu{V}$。
- 方向：从低电位到高电位，与电压方向相反。
### 电功率
- 定义：$p=\dfrac{\mathrm{d}W}{\mathrm{d}t}$，其中 $\mathrm{d}W$ 是在 $\mathrm{d}t$ 时间内 **消耗或吸收** 的功率。
- **计算**：由 $\mathrm{d}W=u \mathrm{d}q=ui \mathrm{d}t$ 得，$p=ui$。在 **关联参考方向**（$u,i$ 同方向，如下图 (a)）下，$p=ui$ 计算的是 **吸收功率**；在非关联参考方向（如下图 (b)）下，计算的是 **发出功率**。若吸收功率为负值，则绝对值为发出功率，反之亦然。
  ![[reference-direction.png]]
- 单位：瓦［特］$\pu{W}$，$\pu{1W}=\pu{1J}/\pu{1s}=\pu{1V}\cdot\pu{1A}$。
- 做功的计算：在 $t_0$ 到 $t$ 时间内，电路吸收或发出的功为 $W(t)=\displaystyle\int_{t_0}^{t}p(\xi)\mathrm{d}\xi=\displaystyle\int_{t_0}^{t}u(\xi)i(\xi)\mathrm{d}\xi$。
## 1.2　电阻元件

- 电路符号：如下图，其中 (a) 为固定电阻，其他为可变电阻，(b) 与 (c) 含义相同，(d) 是一种三端可变电阻，但其可用如图 (e) 的两个二端电阻表示。
  ![[resistance-symbol.png]]
- 欧姆定律：线性二端口电阻的端口电压与电流之间遵循 **欧姆定律**：若 $u,i$ 参考方向相同，则有 $$u=Ri$$或 $$i=Gu,$$其中参数 $R$ 称为 **电阻** 或电阻系数，$G$ 称为 **电导** 或电导系数。显然 $RG=1$。
- 单位：
	- 电阻：欧［姆］$\pu{\Omega}$，$\pu{1\Omega}=\pu{1V}/\pu{1A}$；
	- 电导：西［门子］$\pu{S}$，$\pu{1S}=\pu{1A}/\pu{1V}$。
- 耗能元件：设 $u,i$ 关联参考方向，由 $p=ui=Ri^2=Gu^2$ 可知，如果 $R,G>0$，则 $p$ 非负，为 **耗能元件**。
- 焦耳定律：导体或半导体电阻吸收电能转化为热能，能量大小为 $$W=\int_{-\infty}^{t}u(\xi)i(\xi)\mathrm{d}\xi=R \int_{-\infty}^{t}i^2(\xi)\mathrm{d}\xi=G \int_{-\infty}^{t}u^2(\xi)\mathrm{d}\xi.$$
- 无源元件：电阻只能吸收电能，不能发出电能。
- 负电阻：$R,G<0$，从而 $u,i$ 关联参考方向时 $p\le0$，对外提供电能，属于 **有源元件**。
- 非线性电阻：$u,i$ 不成正比，$u-i$ 图象不是过原点的直线。例：半导体二极管，$i=I_0(\mathrm{e}^{u/U_T}-1)$。
## 1.3　电容元件

- 电容器的构成：电容器由两块用介质绝缘的金属板组成，如下图，其中 $\varepsilon$ 为介质的介电常数。
  ![[capacitor-structure.png]]
- 电路符号：在电路模型中，用电容元件表示理想化的电容器，其电路符号如下图，其中 (a) 表示固定电容，(b) 表示可变电容。
  ![[capacitor-symbol.png]]
- 储能元件：当在电容器两端施加电压时，两极板上聚集等量的正负电荷，极板之间产生电场，储存有电场能量。对于理想化的电容，当电源移去后，电荷和电场可以继续存在，从而储存电荷和电场能，即电容是储能元件。
- **电容元件的 $q-u$ 特性**：若介质的介电常数与电场强度无关，则称其为 **线性介质**，如空气、陶瓷、云母、胶木等都是线性介质。填充有线性介质的电容称为 **线性电容**，其 $q-u$ 关系为：$$q=Cu.$$其中，$C$ 是 **电容［系数］**。
- 单位：电容 $C$ 的 SI 单位为法［拉］$\pu{F}$，$\pu{1F}=\pu{1C}/\pu{1V}$。法拉很大，故使用时通常用毫法（$\pu{mF}$）、微法（$\pu{\upmu F}$）等。
- 电容的大小：对于上面图中的平行板电容器，其电容为 $C=\dfrac{\varepsilon A}{d}$。线性电容元件的电容为常量。
- $C$ 与 $i,u,q$ 的计算：
	- $q(i)$ 关系：$q(t)=\displaystyle\int_{-\infty}^{t}i(\xi)\mathrm{d}\xi$，即 $t$ 时刻的电荷量是电流充、放电积累的结果。故电容属于 **记忆元件**。
	- $i(u)$ 和 $u(i)$ 关系：设 $u,i$ 为关联参考方向，则：
		- $i=\dfrac{\mathrm{d}q}{\mathrm{d}t}=C \dfrac{\mathrm{d}u}{\mathrm{d}t}$，即电流与电压变化率成正比。若施加直流电压，则电流为零，相当于开路。
		- $u(t)=\dfrac{q(t)}{C}=\dfrac{1}{C}\displaystyle\int_{-\infty}^{t}i(\xi)\mathrm{d}\xi$，即 $t$ 时刻的 $u$ 是该时刻以前 $i$ 对 $u$ 影响的积累。若研究的是某一时刻 $t_0$ 之后的情况，则 $u(t)=u(t_0)+\dfrac{1}{C}\displaystyle\int_{t_0}^{t}i(\xi)\mathrm{d}\xi$，其中 $u(t_0)$ 称为初始电压。
	  $u,i$ 关系为微、积分的关系，故电容属于 **动态元件**。
- 功率与能量：输入线性电容的功率为 $p=ui=u\cdot C \dfrac{\mathrm{d}u}{\mathrm{d}t}$，故 $t$ 时刻吸收的总能量为 $$W _{\mathrm{e}}(t)=\int_{-\infty}^{t}p(\xi)\mathrm{d}\xi=\int_{-\infty}^{t}\left(Cu \frac{\mathrm{d}u}{\mathrm{d}\xi}\right)\mathrm{d}\xi=C \int_{-\infty}^{t}u \mathrm{d}u=\frac{1}{2}Cu^2,$$其中 $t=-\infty$