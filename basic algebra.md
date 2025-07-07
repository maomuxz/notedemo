#  Basic algebra

## § 0划分和等价关系
* 0.1 : 集合$\,S\,$的一些非空不交子集的并是$\,S\,$
  则这些子集称为$\,S\,$的一个划分;
* 0.2 : 集合$\,S\times S\,$的非空子集$\,\omega\,$称为一个二元关系,而
  $\,\forall \,a,b \in S\,$,若$\,(a,b)\in \omega$,则称$\,a\,$与$\,b\,$有$\,\omega\,$关系,记作$\,a\omega b$
  反之$\,(a,b)\notin S\,$则称$\,a\,$与$\,b\,$没有$\,\omega\,$关系
* 0.3 : 二元关系$\,\omega\,$称为等价关系,若其满足:$\,\forall  a,b,c \in S\,$
  $\quad\quad\quad$1 )反身性:$\,a \omega a\,$;
  $\quad\quad\quad$2 )对称性:$\,a \omega b \iff b \omega a\,$;
  $\quad\quad\quad$3 )传递性:$\,a \omega b,b \omega c \Rightarrow a \omega c\,$;
  并记$\,\omega\,$为$\,a \sim  b\,$
* 0.4 : 一个有等价关系$\,\sim \,$的集合$\,S\,$,任给$\,a \in S\,$
  记$\,\bar{a}= \left\{ x|x \sim a,x \in S \right\}\,$,称为$\,a\,$的等价类
  $\,a\,$称为该类的一个代表元;
* 0.5 : 任意两个等价类$\, \bar{a},\bar{b}\,$相等$\,\iff a \sim  b\,$;
>proof:
$\quad\quad\quad \Rightarrow:\,$若$\,\bar{a}=\bar{b}\,$,则$\,a\in \bar{a} \Rightarrow a \in \bar{b} \Rightarrow a \sim b$
$\quad\quad\quad \Leftarrow:\,$若$\,a \sim  b\, , \forall \,x \in \bar{a},x \sim  a\Rightarrow x \sim  b$
$\quad\quad\quad\quad\;\,$从而$\,x \in  \bar{b}$
$\quad\quad\quad\quad\;\,$由任意性$\,\bar{a} =\bar{b}$ []
* 0.6 : 集合$\,S\,$关于等价关系$\,\sim \,$的所有等价类构成$\,S\,$的一个划分
  这样的划分称为$\,S\,$关于$\,\sim \,$的商集
>proof:
$\quad\quad\quad$设$\,\bar{a}_1,\bar{a}_2,. . .,\bar{a}_n,. . .\,$是$\,S\,$的全体等价类,根据0.5知道:
$\quad\quad\quad\quad\quad\quad\quad\quad\quad\forall \,i\neq j,\bar{a}_i\cap  \bar{a}_j=\empty$
$\quad\quad\quad$而$\,\forall \,x\in S\,$必$\,\exists \,i,s.t.\,x\in \bar{a}_i\,$,否则由反身性$\,x \sim x\,$知$\,x \in \bar{x}$
$\quad\quad\quad$从而$\,S \subseteq \bigcup\limits_{i=1}^{n} \bar{a}_i\,$,并显然:$\,\bigcup\limits_{i=1}^{n} \bar{a}_i \subseteq  S\,$,于是$\,\bigcup\limits_{i=1}^{n} \bar{a}_i =  S\,$ []
* 0.7 : 二元代数运算:$$