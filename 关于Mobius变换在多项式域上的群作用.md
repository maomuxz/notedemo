#  Mobius变换

$Mobius\text{变换是复分析中常用的一种分式型线性变换,定义为:}$

$f:\mathbb{C}\to\mathbb{C},\mathbb{z} |\to \displaystyle\frac{az+b}{cz+d},\,$ 其中 $:\det{\begin{bmatrix} a & b \\ c & d \\\end{bmatrix}} \neq0$

Proposition1.1 $:\text{全体} Mobius\text{变换关于复合运算构成群,记作}PGL(2,\mathbb{C})$

Proof $:\text{记}\,f_{i}(z):=\displaystyle \frac{a_iz+b_i}{c_iz+d_i},i=1,2$
$\text{结合律显然成立}$

$1^{\circ}\;\text{单位元 }: \mathcal{E}(z)=z=\displaystyle\frac{z+0}{0+1},\text{而}\det \begin{bmatrix} 1 & 0 \\ 0 & 1 \\\end{bmatrix} =1$

$\quad \text{故}\;\mathcal{E} \in PGL(2,\mathbb{C})\,:\,\forall \;f_1\in PGL(2,\mathbb{C}):\;\mathcal{E}\circ f_1=f_1(z)=\displaystyle \frac{a_1\mathcal{E}(z)+b_1}{c_1\mathcal{E}(z)+d_1}=f_1\circ\mathcal{E}(z)$

$2^{\circ}\;\text{逆元 }:\,\forall \;f_1\in PGL(2,\mathbb{C})\;\text{取}\,f_1^{-1}(z)=\displaystyle \frac{d_1z-b_1}{a_1-c_1z}$

$\quad \text{则}\;f_1^{-1}\circ f_1=\displaystyle \frac{d_1\cdot \displaystyle \frac{a_1z+b_1}{c_1z+d_1}-b_1}{a_1-c_1\cdot \displaystyle \frac{a_1z+b_1}{c_1z+d_1}}= \begin{vmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{vmatrix}z(c_1z+d_1)^{-1}\begin{vmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{vmatrix}^{-1}(c_1z+d_1)
$

$\quad \quad \quad \quad \qquad\!=\mathcal{E}(z)=f\circ f_1^{-1}$



Proposition1.2 $:PGL(2,\mathbb{C})\simeq GL(\mathbb{C})/\mathbb{C}^{\mathrm{x}}$

Proof $:\;\text{记映射 }: \psi\;:PGL(2,\mathbb{C})\to GL(\mathbb{C})/\mathbb{C}^{\mathrm{x}}\, , \,f(z)=\displaystyle \frac{az+b}{cz+d}|\to \begin{bmatrix} a & b \\ c & d \\\end{bmatrix}$

$1^{\circ}\;\text{单射 }:\,\forall \;f_i(z)=\displaystyle \frac{a_iz+b_i}{c_iz+d_i}\in PGL(2,\mathbb{C})\, , \,i=1,2$

$\quad\text{令 }\psi(f_1)=\psi (f_2)\, , \,\text{即 }\begin{bmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{bmatrix} = \begin{bmatrix} a_2 & b_2 \\ c_2 & d_2 \\\end{bmatrix}\quad \text{从而得到 }:a_1=a_2,b_1=b_2,c_1=c_2,d_1=d_2$

$\quad \text{即 }f_1=f_2$

$2^{\circ}\;\text{满射 }:\,\forall \;\begin{bmatrix} a & b \\ c & d \\\end{bmatrix}\in GL(\mathbb{C})/\mathbb{C}^{\mathrm{x}}\, , \,f(z)=\displaystyle \frac{az+b}{cz+d}\in GPL(2,\mathbb{C})$

$\quad \text{即 }\begin{bmatrix} a & b \\ c & d \\\end{bmatrix}=\psi(f)$

$3^{\circ}\;\text{同态 }:\,\psi(f_1\circ f_2)=\psi \displaystyle \left\{ \frac{a_1\cdot \displaystyle \frac{a_2z+b_2}{c_2z+d_2}+b_1}{c_1\cdot \displaystyle \frac{a_2z+b_2}{c_2z+d_2}+d_1} \right\}=\psi\displaystyle \left\{ \frac{(a_1a_2+b_1c_2)z+a_1b_2+b_1d_2}{(c_1a_2+d_1c_2)z+c_1b_2+d_1d_2} \right\}$

$\quad \qquad \qquad \qquad \qquad\! =\begin{bmatrix} a_1a_2+b_1c_2 & a_1b_2+b_1d_2 \\ c_1a_2+d_1c_2 & c_1b_2+d_1d_2 \\\end{bmatrix}=\begin{bmatrix} a_1 & b_1 \\ c_1 & d_1 \\\end{bmatrix}\cdot \begin{bmatrix} a_2 & b_2 \\ c_2 & d_2 \\\end{bmatrix}$

$\quad \qquad \qquad \qquad \qquad\! =\psi(f_1)\cdot \psi(f_2)$

$\quad \text{即 }\psi \text{是同构}$

$\text{}$