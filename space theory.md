# § 1.space theory
##  1.space
* 1.1 : 集合 $\boldsymbol{X}$,若 $\exists\,d:\boldsymbol{X}^2\rightarrow\mathbb{R}^{+}\cup \left\{0\right\}$ , 且满足：$\\{}\quad\quad\quad1）\forall x,y\in \boldsymbol{X},\quad{}d(x,y)\geq_{}0,\quad{}\text{iff}\;{}x =y\\{}\quad\quad\quad{} 2）\forall x,y\in \boldsymbol{X},\quad{}d(x,y)=d(y,x)\\{}\quad\quad\quad{}3）\forall x,y,z\in \boldsymbol{X},d(x,y)\leq_{}d(x,z)+d(z,y)$
则称$\,\boldsymbol{d}\,$为$\,\boldsymbol{X}\,$的一个度量，而$\,(\boldsymbol{X},\boldsymbol{d})\,$称为一个度量空间，记作$\,ms(\boldsymbol{X},\boldsymbol{d})$
$\\{}$
* 1.2 : $\boldsymbol{Y\,}$是$\,ms(\boldsymbol{X},\boldsymbol{d})\,$的一个子集，则限制$\,\boldsymbol{d}\,$的定义域到$\,\boldsymbol{Y}^2$，并记作$\,\boldsymbol{d}_{\boldsymbol{Y}}$，
得到$\,ms(\boldsymbol{Y},\boldsymbol{d}_{\boldsymbol{Y}})\,$，称为$\,\boldsymbol{X}\,$的子度量空间，$\boldsymbol{d}_{\boldsymbol{Y}}\,$称为由$\,\boldsymbol{d}\,$诱导的度量
$\\{}$
* 1.3 : 若$\,\boldsymbol{d}_{1}$,$\boldsymbol{d}_{2}\,$分别为$\,\boldsymbol{X}\,$上的度量，若$\,\exist{}\,C_1,C_2\in{}\mathbb{R}^{+},s.t.\,\forall{}\,x,y\in{}\boldsymbol{X}\,$
都有:
$\quad\quad\quad\quad\quad\quad{}\,d_2(x,y)\leq{}C_1\,d_1(x,y),\quad{}d_1(x,y)\leq{}C_2\,d_2(x,y)$
则称$\,d_1与d_2\,$等价
$\\{}$
* 1.4 : $ms(\boldsymbol{X},\boldsymbol{d})\,$若序列$\,\left\{x_n\right\}\subseteq \boldsymbol{X}\,$，满足$\,\exists\,N\in \mathbb{N}^{+}\,$，$\forall\,m,n>0,\epsilon>0\,$
总有:
$\quad\quad\quad\quad\quad\quad{}d(x_n,x_m)<\epsilon\,$，则称$\,\left\{x_n\right\}\,$为一个$Cauchy$列$\\{}$若$\,\exists\,x\in \boldsymbol{X}\,s.t.\,\exists \,N\in \boldsymbol{N}^{+},\forall \,n>N,\forall \,\epsilon>0$
均有:
$\quad\quad\quad\quad\quad\quad{}\,d(x_n,x)>0$，则称$\,\left\{x_n\right\}$收敛到$\,x$，记作$\,\left\{x_n\right\}\to x\,$(或$\,\lim\limits_{n \to \infty}x_n=x$)
$\\{}$
* 1.5 : 重要性质：若$\,Cauchy$列有收敛子列，则其必收敛
特别地，如果$\,\boldsymbol{X}\,$中所有$Cauchy$列都收敛，则称其是完备度量空间，记作$\,cms(\boldsymbol{X},\boldsymbol{d})$
>proof:
>$\quad\quad\quad{}$设$\,Cauchy$列$\,\left\{x_n\right\}$. 并设$\,\left\{x_{n_k}\right\}\to x$
$\quad\quad\quad{}$根据定义:$\,\exists \,k_0\in \boldsymbol{N},s.t.\,\forall \,k>k_0\,{,}\,n_k>n_{k_0}\,{,}\forall \,\epsilon_1>0\,{,}d(x_{n_k},x_0)<\epsilon_1$$\\{}\quad\quad\quad\quad\quad\quad\;\;\,{}\exists \,N\in \boldsymbol{N},s.t.\,\forall \,m,n>N\,{,}\,\forall \,\epsilon_2>0\,{,}d(x_m,x_n)<\epsilon_2$
$\quad\quad\quad{}$取$N_0=\max{\left\{n_{k_0},N\right\}}\,$，则$\,\forall \,n_k,n>N_0\,{,}\forall \epsilon\doteq\epsilon_1+\epsilon_2>0$
$\quad\quad\quad\quad\quad{}d(x_n,x_0)\le d(x_n,x_{n_k})+d(x_{n_k}+x_0)=\epsilon$
$\quad\quad\quad{}$此即$\lim\limits_{n \to \infty}x_n=x$ []
---
* 1.6 : $ms(\boldsymbol{X},\boldsymbol{d})$，$\forall \,x_0\in  \boldsymbol{X},\delta\in \mathbb{R}^{+}$定义：$\\{}\quad\quad\quad{} \,\boldsymbol{B}(x_0,\delta):=\left\{x\in \boldsymbol{X}|d(x,x_0)<\delta\right\}$，称为$\,x_0$的一个开球$\\{}\quad\quad\quad{}\boldsymbol{\dot{B}}(x_0,\delta):=\boldsymbol{B}(x_0,\delta)\backslash\left\{x_0\right\}$，称为去心开球
$\\{}$
* 1.7 : $ms(\boldsymbol{X},\boldsymbol{d}),ms(\boldsymbol{Y},\boldsymbol{h}),f:\boldsymbol{X}\to \boldsymbol{Y}\,$，取定$\,x_0\in \boldsymbol{X}$，若满足：$\forall \,\epsilon>0,\exists \,\delta>0,s.t.\,\forall \,x\in \,\boldsymbol{B_{d}}(x_0,\delta)$
都有：$\\{}\quad\quad\quad\quad\quad\quad{}\,f(x)\in \boldsymbol{B_h}(f(x_0),\epsilon)$，则称$\,f\,$在$\,x_0\,$处连续
$\\{}$若$\,f\,$在$\,\boldsymbol{X}\,$处处连续，则称$\,f\,$为$\,\boldsymbol{X}\,$上的连续映射，$\,\boldsymbol{X}\,$上的全体连续映射记作$\,C(x)$
$\\{}$

* 1.8 : $ms(\boldsymbol{X},\boldsymbol{d}),ms(\boldsymbol{Y},\boldsymbol{h}),f:\boldsymbol{X}\to \boldsymbol{Y}$，若满足：$\,\forall \,\epsilon>0,\exists \,\delta>0,\forall \,x,y\in \boldsymbol{X}$
只要$\,d(x,y)<\delta$，就有:
$\quad\quad\quad\quad\quad\quad{}h(f(x),f(y))<\epsilon$，则称$\,f\,$一致连续
$\\{}$
* 1.9 : $ms(\boldsymbol{X},\boldsymbol{d}),ms(\boldsymbol{Y},\boldsymbol{h}),f:\boldsymbol{X}\to \boldsymbol{Y}$，若满足：$\,\exists \,H\in \mathbb{R}^{+},\alpha\in \mathbb{N},s.t.\,\forall \,x_1,x_2\in \boldsymbol{X}$
都有:
$\quad\quad\quad\quad\quad\quad \boldsymbol{h}(f(x_1),f(x_2))\le H·\boldsymbol{d^{\alpha}}(x_1,x_2)$
则称$\,f\,$为$\,\alpha\,$阶$H\ddot{o}lder$连续
特别地，$\,\alpha=1$时称为$Lip$连续，并称$\,H\,$为$Lip$常数，记作$L$
$\\{}$
* 1.10 $Heine$定理 : $ms(\boldsymbol{X},\boldsymbol{d}),ms(\boldsymbol{Y},\boldsymbol{h}),f:\boldsymbol{X}\to \boldsymbol{Y}$，取$\,x_0\in \boldsymbol{X}$,则：
$\quad{}f\,$在$\,a\,$处连续$\iff$任取$\,\left\{x_n\right\}\subseteq \boldsymbol{X}$,若$\,x_n\to x_0$,则$\,\left\{f(x_n)\right\}\to f(x_0)$
>proof:
$\quad\quad\quad{}$
---
* 1.11 $Banach$不动点定理 : 若$\,cms(\boldsymbol{X},\boldsymbol{d}),f:\boldsymbol{X}\to \boldsymbol{X}\,$是一个$\,Lip\,$常数小于$\,1\,$的$\,Lip\,$函数，即满足：
$\quad\quad\quad{} \exists \,0<\tau<1,\forall \,x_1,x_2\in \boldsymbol{X}$，均有：$\boldsymbol{d}(f(x_1),f(x_2))\le \tau \boldsymbol{d}(x_1,x_2)$
则$\,\exists !x_0<\boldsymbol{X},s.t.\,f(x_0)=x_0$，称$\,x_0\,$为$\,f\,$的一个不动点，而$\,f\,$称为一个压缩映射
>proof:
$\quad\quad\quad{}$
---

## 2 $\,ms\,$上的集合
* 2.1 : $\,ms(\boldsymbol{X},\boldsymbol{d})\,,A \subseteq \boldsymbol{X}\,$, 则定义:
$\quad\quad\quad 1)\,$内点 : 若$\,\exists \,\delta>0\, , s.t.\boldsymbol{B}(x,\delta) \subset A$
$\quad\quad\quad 2)\,$外点 : 若$\,\exists \,\delta>0\, , s.t.\boldsymbol{B}(x,\delta) \subset A^{s}$
$\quad\quad\quad 3)\,$内点 : 若$\,\forall  \,\delta>0\, , s.t.\boldsymbol{B}(x,\delta)\cap A \neq \empty\, , \boldsymbol{B}(x,\delta)\cap A^{s} \neq \empty$
  $\,A\,$的全体内点记作$\,int\,A\,$ , 全体边界点记作$\,\partial A$
$\quad\quad\quad 4)\,$内点 : 若$\,\forall  \,\delta>0\, , s.t.\dot{\boldsymbol{B}}(x,\delta) \cap A\neq \empty$
$\quad\quad\quad 5)\,$内点 : 若$\,\forall  \,\delta>0\, , s.t.\dot{\boldsymbol{B}}(x,\delta) \cap A= \empty$
  $\,A\,$的全体聚点记作$\,A^{d}\,$称为导集,并记$\,\bar{A}=A\cup A^{d}\,$称为$\,A\,$的闭包
$\\{}$
* 2.2 : $\,ms(\boldsymbol{X},\boldsymbol{d})\, , \forall \,A \subset X\,$, 若 :
$\quad\quad\quad 1)\,$开集 : 若$\,int A=A$
$\quad\quad\quad 2)\,$闭集 : 若$\,\bar{A}=A$
  可列个闭集的并称为$\,F_\sigma$集 , 可列个开集的交称为$\,G_\delta$集
$\\{}$
* 2.3 : $\quad\, 1)\,$内点一定是聚点,即$\, intA \subset A$
$\quad\quad\quad 2)$边界点是聚点或者孤立点
$\quad\quad\quad 3)$闭包等于集合与其边界的并,即$\,\bar{A}=A\cup \partial A$
$\quad\quad\quad 4)$外点一定不是聚点和孤立点,孤立点一定是边界点
$\quad\quad\quad 5)\,ms(\boldsymbol{X},\boldsymbol{d})$上点开球一定是开集
$\quad\quad\quad 6)$开集的有限交和任意并仍为开集
$\quad\quad\quad\;\;\;$闭集的有限并和任意交仍为闭集
>trival
---
* 2.4 : $\,ms(\boldsymbol{X},\boldsymbol{d})\, , S \subset \boldsymbol{X} $
$\quad\quad\quad 1)\,\partial S\,$必为闭集
$\quad\quad\quad 2)\, int S\,$必为开集 , 且为包含于$\,S\,$的最大开集
$\quad\quad\quad 3)\, (S^{d})^d \subset S^{d}$
  推论 : $\,\bar{S}\,$必为闭集
$\quad\quad\quad 4)$开集的补集为闭集 , 闭集的补集为开集
>proof:
---
* 2.5 : $\,ms(\boldsymbol{X},\boldsymbol{d})\, , A \subset \boldsymbol{X}$
$\quad\quad\quad 1)\,$完备性 : $\, A\,$中所有$\,Cauchy\,$列都收敛
  若$\,ms(\boldsymbol{X},\boldsymbol{d})\,$是完备的 , 则称$\,\boldsymbol{d}\,$为完备度量 , $\,\boldsymbol{X}\,$为完备度量空间 , 记作$\,cms(\boldsymbol{X},\boldsymbol{d})$
$\quad\quad\quad 2)\,$有界性 : $\,\exists \,\delta>0\, ,s.t.\sup \limits_{x,y\in A}\left\{ \boldsymbol{d}(x,y) \right\} \le \delta$ 
$\quad\quad\quad 3)\,$稠密性 : $\,\forall x\in \boldsymbol{X}\, , \exists \, a \in A\, ,\forall \epsilon>0\, ,s.t.\,\boldsymbol{d}(x,a)<\epsilon$
$\quad\quad\quad 4)\,$连通性 : 不$\,\exists \,$开集$\,U\, , V\,,\,s.t.\,U \cup  V=A\, ,$ 且$\,U \cap  V=\empty$ 
$\quad\quad\quad 5)\,$道路连通性 : $\,\forall \, x,y\in A\, ,\exists\,injection\,f:\left[ 0,1 \right]\to A\, , s.t.\,f(0)=x\, ,f(1)=y $
$\quad\quad\quad 6)\,$紧性 : $\,$
# § 2.Measure theory
##  1.$\,\sigma\!-\!algebra$
* 1.1 : 集合$\,\boldsymbol{S}\,$，若其子集族$\,\Lambda \subseteq 2^S\,$对并集运算满足:
$\quad\quad\quad 1)\;\empty \in \Lambda$
$\quad\quad\quad 2)\;$若$\,A\in \Lambda\,$则$\,A^{c} \in \Lambda$
$\quad\quad\quad 3)\;$对集序列$\left\{ A_\alpha\in \Lambda \right\}_{\alpha \in I}\,$满足:$\bigcup\limits_{\alpha\in I}A_\alpha \in \Lambda\, ,$ 其中$\,I\,$为指标集
则称$\,\Lambda\,$为$\,S\,$的一个$\,algebra\,$
$\\$
 若$\,\#I <\infty\,$则称$\,\Lambda\,$为一个$\,\sigma\!-\!algebra$ , 将这样一个二元组称为一个可测空间$\,Measurable \,space\,$记作$\,(S,\Lambda)$
$\\$
 两个平凡的$\,\sigma\!-\!algebra\,$: $\,2^{S}\,$和$\,\left\{ \empty\,,S \right\} $是任何集合的$\,\sigma\!-\!algebra$
 $\\{}$
* 1.2 : $\, \sigma\!-\!algebra$的交还是$\,\sigma\!-\!algebra$
>trival
---
* 1.3 : 集合$\,S\,$, 设$\,A \subseteq 2^{S}\,$记$\,\Sigma_A \doteq \left\{ \Lambda|A \subseteq \Lambda\,,\Lambda为\sigma\!-\!algebra \right\} $
  则$\,\delta(A) := \bigcap\limits_{\Lambda \in \Sigma_A} \Lambda\,$称为$\,A\,$生成的$\,\sigma\!-\!algebra\,$, 容易验证这是包含$\,A\,$的最小$\,\sigma\!-\!algebra$
 $\,ms(X,d)\,$上全体开集生成的$\,\sigma\!-\!algebra\,$构成的集合称为$\,Borel\!-\!algebra$ , 记作$\boldsymbol{B}(X)$,其元素称为$\,X\,$上的$\,Borel\,$集
$\\{}$
* 1.4 : 上升集序列 : 子集族$\,\left\{ A_n \right\} \subseteq X\,$ 满足 : $\,A_1 \subseteq  A_2\subseteq \cdots\subseteq A_n\subseteq \cdots$ , 并记$\,\overline{\lim\limits_{n \to \infty}}A_n \doteq \bigcup\limits_{n=1}^{\infty}A_n $ 或$\,\left\{ A_n \right\} \uparrow A$ , 其中$\,A =\bigcup\limits_{n=1}^{\infty} A_n$
$\quad\quad$下降集序列 : 子集族$\,\left\{ A_n \right\} \subseteq X\,$ 满足 : $\,A_1 \supseteq  A_2\supseteq \cdots\supseteq A_n\supseteq \cdots$ , 并记$\,\underline{\lim\limits_{n \to \infty}}A_n \doteq \bigcap\limits_{n=1}^{\infty}A_n $ 或 $\,\left\{ A_n \right\} \,\downarrow A$ , 其中$\,A = \bigcap\limits_{n=1}^{\infty}A_n$
$\\$
  单调类 : $\,$