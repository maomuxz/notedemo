#  1 Mobius变换

## 1.1 基本定义及其代数性质

$Mobius\text{变换是复分析中常用的一种分式型线性变换,定义为:}$

$f:\mathbb{C}\to\mathbb{C},\mathbb{z} \leadsto  \displaystyle\frac{az+b}{cz+d},\,$ 其中 $:\det{\begin{bmatrix} a & b \\ c & d \\\end{bmatrix}} \neq0$

>Proposition1.1 $:\text{全体} Mobius\text{变换关于复合运算构成群,记作}PGL(2,\mathbb{C})$

Proof $:$

$\text{记}\,f_{i}(z):=\displaystyle \frac{a_iz+b_i}{c_iz+d_i},i=1,2\, , \,\text{结合律显然成立}$

$1^{\circ}\;\text{单位元 }: \mathcal{E}(z)=z=\displaystyle\frac{z+0}{0+1},\text{而}\det \begin{bmatrix} 1 & 0 \\ 0 & 1 \\\end{bmatrix} =1$

$\quad \text{故}\;\mathcal{E} \in PGL(2,\mathbb{C})\,:\,\forall \;f_1\in PGL(2,\mathbb{C}):\;\mathcal{E}\circ f_1=f_1(z)=\displaystyle \frac{a_1\mathcal{E}(z)+b_1}{c_1\mathcal{E}(z)+d_1}=f_1\circ\mathcal{E}(z)$

$2^{\circ}\;\text{逆元 }:\,\forall \;f_1\in PGL(2,\mathbb{C})\;\text{取}\,f_1^{-1}(z)=\displaystyle \frac{d_1z-b_1}{a_1-c_1z}$

$\quad \text{则}\;f_1^{-1}\circ f_1=\displaystyle \frac{d_1\cdot \displaystyle \frac{a_1z+b_1}{c_1z+d_1}-b_1}{a_1-c_1\cdot \displaystyle \frac{a_1z+b_1}{c_1z+d_1}}= \begin{vmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{vmatrix}z(c_1z+d_1)^{-1}\begin{vmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{vmatrix}^{-1}(c_1z+d_1)
$

$\quad \quad \quad \quad \qquad\!=\mathcal{E}(z)=f\circ f_1^{-1}$


>Proposition1.2 $:PGL(2,\mathbb{C})\simeq GL(\mathbb{C})/\mathbb{C}^{\mathrm{x}}$

Proof $:\;$

$\text{记映射 }: \psi\;:PGL(2,\mathbb{C})\to GL(\mathbb{C})/\mathbb{C}^{\mathrm{x}}\, , \,f(z)=\displaystyle \frac{az+b}{cz+d}\leadsto \begin{bmatrix} a & b \\ c & d \\\end{bmatrix}$

$1^{\circ}\;\text{单射 }:\,\forall \;f_i(z)=\displaystyle \frac{a_iz+b_i}{c_iz+d_i}\in PGL(2,\mathbb{C})\, , \,i=1,2$

$\quad\text{令 }\psi(f_1)=\psi (f_2)\, , \,\text{即 }\begin{bmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{bmatrix} = \begin{bmatrix} a_2 & b_2 \\ c_2 & d_2 \\\end{bmatrix}\quad \text{从而得到 }:a_1=\lambda a_2,b_1=\lambda b_2,c_1=\lambda c_2,d_1=\lambda d_2$

$\quad \text{即 }f_1=\displaystyle \frac{\lambda a_2z+\lambda b_2}{\lambda c_2z+\lambda d_2}=f_2$

$2^{\circ}\;\text{满射 }:\,\forall \;\begin{bmatrix} a & b \\ c & d \\\end{bmatrix}\in GL(\mathbb{C})/\mathbb{C}^{\mathrm{x}}\, , \,f(z)=\displaystyle \frac{az+b}{cz+d}\in GPL(2,\mathbb{C})$

$\quad \text{即 }\begin{bmatrix} a & b \\ c & d \\\end{bmatrix}=\psi(f)$

$3^{\circ}\;\text{同态 }:\,\psi(f_1\circ f_2)=\psi \displaystyle \left\{ \frac{a_1\cdot \displaystyle \frac{a_2z+b_2}{c_2z+d_2}+b_1}{c_1\cdot \displaystyle \frac{a_2z+b_2}{c_2z+d_2}+d_1} \right\}=\psi\displaystyle \left\{ \frac{(a_1a_2+b_1c_2)z+a_1b_2+b_1d_2}{(c_1a_2+d_1c_2)z+c_1b_2+d_1d_2} \right\}$

$\quad \qquad \qquad \qquad \qquad\! =\begin{bmatrix} a_1a_2+b_1c_2 & a_1b_2+b_1d_2 \\ c_1a_2+d_1c_2 & c_1b_2+d_1d_2 \\\end{bmatrix}=\begin{bmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{bmatrix}\cdot \begin{bmatrix} a_2 & b_2 \\ c_2 & d_2 \\\end{bmatrix}$

$\quad \qquad \qquad \qquad \qquad\! =\psi(f_1)\cdot \psi(f_2)$

$\quad \text{即 }\psi \text{是同构}$

**over**

$\text{所以下面我们用 }\,\displaystyle \left<\begin{matrix} a & b \\ c & d \\\end{matrix}\right>\;\text{来表示 }Mobius \text{ 变换的形式矩阵(简称}\,mobius\,\text{阵),并用左乘复变量 }z\text{ 来表示 }Mobius\text{变换}$

$\text{即 }:\;\,\forall \;M=\displaystyle\left<\begin{matrix} a & b \\ c & d \end{matrix}\right>\in PGL(2,\mathbb{C})\, , \,\text{则 }Mz:=\displaystyle\left<\begin{matrix} a & b \\ c & d \end{matrix}\right> z=\displaystyle \frac{az+b}{cz+d}$

$\text{同时 }:\;\text{记 }\det M\equiv \left\vert M \right\vert:=ad-bc\; , \;Tr(M):=a+d$

$\text{并记 }:\; \dot{M}z:=(az+b)\; , \; J(M,z):=cz+d\, , \; \;\text{分别称为 }M\,\text{的上行和自守形式}$

>Lemma1.3 $:\,\forall \;M_1,M_2\in PGL(2,\mathbb{C})\, , \,J(M_1M_2,x)=J(M_1,M_2x)J(M_2,x)$

Proof $:\;Trival$

$\text{根据 }proposition\,1.2\;\text{设 }M_i=\displaystyle\left<\begin{matrix} a_i & b_i \\ c_i & d_i\end{matrix}\right>\; , \,i=1,2\, ,\text{则 }M_1(M_2z)=(M_1M_2)z\, , \,\text{且令 }\,t=M_1z\, , \,\text{就有 }z=M_1^{-1}t$

>Propositon1.3 $:\;\,\forall \;M=\displaystyle\left<\begin{matrix} a & b \\ c & d \end{matrix}\right> \in PGL(2,\mathbb{C})\, , \, z\in \mathbb{C}\, , \,\frac{d}{dz}(Mz)=\displaystyle \frac{\det M}{J^{2}(M,z)}\, , \, \mathcal{Im}(Mz)=\displaystyle \frac{\det M}{J^{2}(M,z)}\cdot \mathcal{Im}(z)$

Proof $:\;Trival$

$\text{考虑 }M=\displaystyle\left<\begin{matrix} a & b \\ c & d \end{matrix}\right>\in PGL(2,\mathbb{R})\;\text{的不动点 }z_1,z_2(\in \mathbb{C})\, , \,\text{以及 }M\text{ 形式矩阵的特征值 }\lambda_1 , \lambda_2(\in \mathbb{C})\, , \,\text{它们两个有如下关系 }:$

Theorem1.4 $:\;\begin{cases} J(M,z_1)=\lambda_1\quad ,\quad \dot{M}z_1=\lambda_1z_1\\ J(M,z_2)=\lambda_2\quad ,\quad \dot{M}z_2=\lambda_2z_2\end{cases}$

Proof $:\;$

$\text{对 }Mz=z\, , \,\text{我们有 }:\;(cz^{2}-(d-a)z+b)=0$

$\text{考虑判别式 }: \Delta=(d-a)^{2}-4bc=Tr^{2}(M)-4\det M$

$\text{从而不失一般性的设 }:\;\begin{cases} z_1=\displaystyle \frac{a-d+\sqrt{\Delta}}{2c}\quad , \quad\lambda_1 = \displaystyle \frac{Tr(M)+\sqrt{\Delta}}{2}\\ z_2=\displaystyle \frac{a-d-\sqrt{\Delta}}{2c}\quad , \quad\lambda_2 = \displaystyle \frac{Tr(M)-\sqrt{\Delta}}{2}\end{cases}$

$\text{从而有 }:\;\begin{cases} \displaystyle \frac{z_1}{\lambda_1}-\displaystyle \frac{z_2}{\lambda_2}=\displaystyle \frac{d}{c}\cdot \frac{\sqrt{\Delta}}{\left\vert M \right\vert }\\ \displaystyle \frac{z_1-z_2}{\lambda_1 - \lambda_2}=\displaystyle \frac{1}{c}\end{cases}\quad \quad \text{联立解得 }:\begin{cases} z_1=\displaystyle \frac{\lambda_1 \lambda_2}{c}\cdot(\displaystyle \frac{1}{\lambda_2}-\displaystyle \frac{\sqrt{\Delta}}{\lambda_1-\lambda_2}\cdot \frac{d}{\left\vert M \right\vert })\\ z_2=\displaystyle \frac{\lambda_1 \lambda_2}{c}\cdot(\displaystyle \frac{1}{\lambda_1}-\displaystyle \frac{\sqrt{\Delta}}{\lambda_1-\lambda_2}\cdot \frac{d}{\left\vert M \right\vert })\end{cases}$

$\text{由韦达定理立马得证}$

**over**

## 1.2 $PGL(2，\mathbb{R})\,$在 $\mathbb{F}[x]$ 上的群作用

$\text{对于 }\mathbb{R}[x]\text{ 我们定义 }PGL(2,\mathbb{R})\text{ 对 }\mathbb{R}[x]\text{ 的群作用 }*:\;PGL(2,\mathbb{R})\mathbf{x}\mathbb{R}[x]\to \mathbb{R}[Mx]\, , \,M*P \leadsto J^{\partial P}(M,x)P(Mx)$

$\text{考虑 }P(x)\overset{\displaystyle n\overset{\Delta}{=}\partial P}{=\!=\!=\!=}\displaystyle \sum_{k=0}^{n}a_kx^{k}\, , \,M=\displaystyle\left<\begin{matrix} a & b \\ c & d \end{matrix}\right>\in PGL(2,\mathbb{R})\, , \,\text{则 }M*P=J^n(M,x)P(Mx)=J^{n}(M,x)\displaystyle \sum_{k=0}^{n}a_k(Mx)^{k}=\displaystyle \displaystyle \sum_{k=0}^{n}a_k(\dot{M}x)^kJ^{n-k}(M,x)$

