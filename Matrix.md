# Matrix

<img src="https://latex.codecogs.com/gif.latex?\left[_y^x\right],\%20\left[_{c\%20;\%20d}^{a\%20;\%20b}\right],\%20\left[_{c\%20;\%20d}^{a\%20;\%20b}\right]+\left[_{g\%20;\%20h}^{e\%20;\%20f}\right],\%20\left[_{c\%20;\%20d}^{a\%20;\%20b}\right]\cdot\left[_{g\%20;\%20h}^{e\%20;\%20f}\right],\%20..." />

## Definition


<img src="https://latex.codecogs.com/gif.latex?\text{Soit}\%20\text{un}\%20\text{corps}\%20\text{K}=\left(E_K,\%20+,\%20\cdot\right)\%20" />
<img src="https://latex.codecogs.com/gif.latex?\left(\text{Genre}\%20\text{K}_{\mathbb{C}}=\left(\mathbb{C},\%20+,\%20\cdot\right),\%20\text{K}_{\mathbb{R}}=\left(\mathbb{R},\%20+,\%20\cdot\right),\%20\text{K}_{\mathbb{Q}}=\left(\mathbb{Q},\%20+,\%20\cdot\right),\%20...\right)" />

Une matrice est un tableau rectangulaire de <img src="https://latex.codecogs.com/gif.latex?n_{\in\mathbb{N}^{\ast}}" /> lignes sur <img src="https://latex.codecogs.com/gif.latex?p_{\in\mathbb{N}^{\ast}}" /> colonnes contenant des éléments du corps K.

Chaque élément de K contenu dans la matrice est appelé un "coefficient de la matrice"

Vu que pour définir (déclarer) une matrice, on a besoin de savoir
- le type de coefficients qu'il y a dedans, c'est à dire l'ensemble d'appartenance des coefficients
- le nombre de lignes, genre n de N*
- le nombre de colonnes, genre p de N*

On peut la définir en la notant

<img src="https://latex.codecogs.com/gif.latex?\text{Let}\%20A=\left(a_{i,j}\in\text{K}\right)_{._{j\in\left[1,\%20p\right]_{\mathbb{N}}}^{i\in\left[1,\%20n\right]_{\mathbb{N}}}}" />
Enfin, l'ensemble des matrices n x p qu'il est possible de constituer avec les éléments d'un corps K est noté

<img src="https://latex.codecogs.com/gif.latex?M_{n,\%20p}\left(\text{K}\right)" />
<img src="https://latex.codecogs.com/gif.latex?\left(\text{genre}\%20M_{2,\%203}\left(\mathbb{Q}\right)\%20\text{ou}\%20M_{2,\%201}\left(\mathbb{R}\right),\%20\text{etc}\right)" />

Du coup on peut aussi déclarer une matrice n x p sur K en faisant (plus clair pour moi)

<img src="https://latex.codecogs.com/gif.latex?\text{Let}\%20A\in%20M_{n,\%20p}\left(\text{K}\right)" />

et accéder aux coefficients avec la notation <img src="https://latex.codecogs.com/gif.latex?A_{i,j}\%20" /> (genre <img src="https://latex.codecogs.com/gif.latex?A_{2,3}" /> pour accéder au coefficient de la ligne 2 colonne 3)

Finalement, pour une matrice de n x p sur K, si on considère que chaque ligne est un ensemble ordonné de p éléments de K (c'est à dire un p-uplet d'éléments de K), alors chaque ligne d'une matrice est un élément de 
<img src="https://latex.codecogs.com/gif.latex?\text{K}^p" />.
Du coup, une matrice c'est un ensemble ordonné de lignes (un n-uplet de lignes), c'est à dire qu'on peut considérer que c'est un élément de <img src="https://latex.codecogs.com/gif.latex?\left(K^p\right)^n" />.

De la même manière, si on raisonne suivant le point de vue où chaque colonne est un ensemble ordonné de n éléments de K (c'est à dire un n-uplet d'éléments de K),
alors chaque colonne d'une matrice est un élément de 
<img src="https://latex.codecogs.com/gif.latex?\text{K}^n" />. Du coup, une matrice c'est un ensemble ordonné de colonnes (un p-uplet de colonnes), c'est à dire qu'on peut considérer que c'est un élément de <img src="https://latex.codecogs.com/gif.latex?\left(K^n\right)^p" />.

<img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)\sim\left(\text{K}^p\right)^n\sim\left(\text{K}^n\right)^p" />

* Une matrice qui n'a qu'une seule ligne s'appelle une **matrice ligne**
* Une matrice qui n'a qu'une seule colonne s'appelle une **matrice colonne**
* Une matrice qui ne contient que des 0 (c'est à dire que des éléments neutres <img src="https://latex.codecogs.com/gif.latex?e_{\left(E_{\text{K}},+\right)}" /> du groupe <img src="https://latex.codecogs.com/gif.latex?\left(E_{\text{K}},+\right)" />) s'appelle une **matrice nulle** 
  * la matrice nulle <img src="https://latex.codecogs.com/gif.latex?N\in%20M_{n,p}\left(\text{K}\right)\%20" /> c'est l'élément neutre du groupe <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" />
  * On peut noter la matrice nulle de taille n x p sur un corps K, <img src="https://latex.codecogs.com/gif.latex?N_{n,p,\text{K}}" />
  * on peut définir une fonction <img src="https://latex.codecogs.com/gif.latex?N_{\varnothing}\left(M_{n,p}\left(\text{K}\right)\right)" /> qui retourne la matrice nulle de l'ensemble de matrices <img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)" />:

<img src="https://latex.codecogs.com/gif.latex?N_{\varnothing}:_{_{\%20\%20\%20\%20\%20\%20\%20M_{n,p}\left(\text{K}\right)\%20\%20\%20\%20\rightarrow\%20\%20\%20\%20\%20\%20\%20N_{n,p,\text{K}}}}^{\cup_{._{p\in\mathbb{N}^{\ast}}^{n\in\mathbb{N}^{\ast}}}\left(M_{n,p}\left(\text{K}\right)\right)\%20\%20\rightarrow\%20\%20\cup_{._{p\in\mathbb{N}^{\ast}}^{n\in\mathbb{N}^{\ast}}}\left(\left\{N_{n,p,\text{K}}\right\}\right)}" />



## Square matrix

Une matrice est dite carrée si son nombre de lignes est égal à son nombre de colonnes (donc si n = p)

On peut déclarer une matrice carrée classiquement en faisant:

<img src="https://latex.codecogs.com/gif.latex?\text{Let}\%20A\in%20M_{n,n}\left(\text{K}\right)" />

genre:

<img src="https://latex.codecogs.com/gif.latex?\text{Let}\%20A\in%20M_{4,4}\left(\mathbb{R}\right)" />

mais pour aller plus vite on peut ne spécifier qu'un seul indice, genre:

<img src="https://latex.codecogs.com/gif.latex?\text{Let}\%20A\in%20M_n\left(\text{K}\right)" />

par exemple:

<img src="https://latex.codecogs.com/gif.latex?\text{Let}\%20A\in%20M_{4}\left(\mathbb{R}\right)" />

Moi je trouve pas ça ultra intuitif mais pourquoi pas.

Du coup le terme <img src="https://latex.codecogs.com/gif.latex?M_{n_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)" /> désigne l'ensemble des matrices carrées n x n sur K

Dans une matrice carrée, il y a un truc particulier qu'on appèlle la **diagonale de la matrice** qui est l'ensemble des éléments <img src="https://latex.codecogs.com/gif.latex?\left\{A_{1,1},\%20A_{2,2},\%20A_{3,3},\%20...\%20,\%20A_{n,n}\right\}" /> c'est à dire, formellement, <img src="https://latex.codecogs.com/gif.latex?\left\{A_{i,j}\%20\%20|\%20\%20i=j\right\}" />

---

## Equal (=) operator of matrix

<img src="https://latex.codecogs.com/gif.latex?=:\%20_{\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\left(A,\%20B\right)\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\rightarrow\%20\left\{\text{True}\%20\text{if}\%20A\%20=B,\%20\text{False}\%20\text{if}\%20A\ne%20B\right\}}^{\left(M_{a_{\in\mathbb{N}^{\ast}},b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\times%20M_{c_{\in\mathbb{N}^{\ast}},d_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\right)\%20\rightarrow\%20\left\{\text{True},\%20\text{False}\right\}}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?=\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{c_{\in\mathbb{N}^{\ast}},\%20d_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> qui teste l'égalité de 2 matrices renvoit vrai si:
- les 2 matrices ont un nombre de lignes identique
- les 2 matrices ont un nombre de colonnes identique
- si les coefficients sont identiques un à un, c'est à dire si <img src="https://latex.codecogs.com/gif.latex?\forall\left(i,j\right)\in\left(\mathbb{N}^{\ast}\right)^2,\%20M_{1_{i,j}}=M_{2_{i,j}}" />


Cette fonction est associative

---

## Plus (+) unary operator of matrix

<img src="https://latex.codecogs.com/gif.latex?+:_{\%20\%20\%20\%20\%20\%20\%20\%20A\%20\%20\%20\%20\%20\%20\%20\%20\rightarrow\%20\%20\%20\%20\%20\%20\%20\%20A}^{M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20\%20\rightarrow\%20M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?+\left(A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> renvoit juste la matrice. C'est une fonction identité.

---

## Plus (+) binary operator of matrix

<img src="https://latex.codecogs.com/gif.latex?+:_{\%20\%20\%20\%20\%20\%20\left(A_1,A_2\right)\%20\%20\%20\%20\%20\%20\%20\%20\rightarrow\%20\%20A_{res}=\left(a_{i,j}=A_{1_{i,j}}+A_{2_{i,j}}\right)_{._{j\in\left[1,p\right]}^{i\in\left[1,n\right]}}}^{\left(M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\right)^2\%20\%20\rightarrow\%20M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?+\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{a,b}\left(\text{K}\right)}}\right)" /> qui prend 2 matrices pour les additionner, déjà ne fonctionne (n'est définie) que pour des **matrices de même taille**. Ca sert à rien d'additionner des matrices de tailles différentes avec cette fonction + ca ne marche pas.

Elle renvoit une matrice dont chaque coeffient est égal à la somme des coefficients correspondants dans les matrices passées en argument, c'est à dire que la fonction <img src="https://latex.codecogs.com/gif.latex?+\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{a,b}\left(\text{K}\right)}}\right)" /> renvoit une matrice <img src="https://latex.codecogs.com/gif.latex?A_{res}=\left(a_{i,j}=M_{1_{i,j}}+M_{2_{i,j}}\right)_{._{j\in\left[1,\%20b\right]}^{i\in\left[1,\%20a\right]}}" />

Elle est:
* associative
* commutative
* la matrice nulle <img src="https://latex.codecogs.com/gif.latex?N_{a,b,\text{K}}" /> est l'élément neutre du groupe <img src="https://latex.codecogs.com/gif.latex?\left(M_{a,b}\left(\text{K}\right),\%20+\right)" />

---

## Scalar multiplication (*) operator of matrix

<img src="https://latex.codecogs.com/gif.latex?\times\%20\%20or\%20\%20\cdot\%20:\%20_{\%20\%20\left(\lambda\%20,\%20\%20A\right)\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\rightarrow\%20A_{res}=\left(a_{i,j}=k\cdot%20A_{i,j}\right)_{._{j\in\left[1,m\right]}^{i\in\left[1,n\right]}}}^{\left(\%20\text{K}\%20\times\%20M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20\right)\%20\rightarrow\%20M_{n,p}\left(\text{K}\right)}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?\times\left(\lambda_{\in\text{K}}\%20,\%20A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> ou <img src="https://latex.codecogs.com/gif.latex?\cdot\left(\lambda_{\in\text{K}}\%20,\%20A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> qui prend en argument un scalaire de K et une matrice de n x p sur K, retourne la matrice passée en argument, mais avec tous ses coefficients multipliés par k. C'est à dire que la fonction renvoit une matrice <img src="https://latex.codecogs.com/gif.latex?A_{res}=\left(a_{i,j}=k\cdot%20A_{i,j}\right)_{._{j\in\left[1,p\right]}^{i\in\left[1,n\right]}}" />.

Elle est
* associative
* commutative
* distributive sur le + binaire matriciel


* l'élément neutre <img src="https://latex.codecogs.com/gif.latex?e_{\left(E_{\text{K}},+\right)}" /> du groupe <img src="https://latex.codecogs.com/gif.latex?\left(E_{\text{K}},+\right)" /> est une sorte d'**élément absorbant** <je sais pas si c'est vraiment le terme consacré>, c'est à dire que <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in\left(M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\right),\left(\%20e_{\left(E_{\text{K}},+\right)}\times%20A=N_{n,p,\text{K}}\right)" />.
  * en l'occurence si <img src="https://latex.codecogs.com/gif.latex?K=\mathbb{R}" />, on a <img src="https://latex.codecogs.com/gif.latex?e_{\left(\mathbb{R},+\right)}=0" />, et du coup <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in\left(M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\mathbb{R}\right)\right),\left(\%200\times%20A=N_{n,p,\text{K}}\right)" />

* la matrice nulle <img src="https://latex.codecogs.com/gif.latex?N_{n,p,\text{K}}" /> est un **élément absorbant**, c'est a dire que <img src="https://latex.codecogs.com/gif.latex?\forall\left(k,n,p\right)\in\left(\text{K}\times\mathbb{N}\times\mathbb{N}\right),\%20\left(k\cdot%20N_{n,p,\text{K}}=N_{n,p,\text{K}}\right)" />

* l'élément neutre <img src="https://latex.codecogs.com/gif.latex?e_{\left(E_{\text{K}},\times\right)}" /> du groupe <img src="https://latex.codecogs.com/gif.latex?\left(E_{\text{K}},\times\right)" /> est un **élément neutre** de l'opération, c'est à dire que <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in\left(M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\right),\%20\left(e_{\left(E_{\text{K}},\times\right)}\cdot%20A=A\right)" />
  * en l'occurence, si <img src="https://latex.codecogs.com/gif.latex?K=\mathbb{R}" />, on a <img src="https://latex.codecogs.com/gif.latex?e_{\left(\mathbb{R},\times\right)}=1" />, et du coup <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in\left(M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\mathbb{R}\right)\right),\%20\left(1\cdot%20A=A\right)" />

<C'est pas un groupe parce que c'est pas une loi de composition interne, du coup faudrait investiguer les espaces vectoriels pour voir si ca pourrait coller avec la definition et avoir un truc analogue aux magmas pour parler correctement des elements neutres et des elements absorbants>

---

## Minus (-) unary operator of matrix

<img src="https://latex.codecogs.com/gif.latex?-:_{\%20\%20\%20\%20\%20\%20\%20\%20A\%20\%20\%20\%20\%20\%20\%20\rightarrow\%20\%20\%20\%20\left(-1\right)\cdot%20A}^{M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20\rightarrow\%20M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?-\left(A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> qui prend 1 matrice pour retourner son "opposé", retourne tout simplement la matrice passée en argument multipliée par le scalaire -1 (en réalité c'est -1 si on est genre dans R ou Z etc, mais de manière générale c'est l'opposé dans le groupe <img src="https://latex.codecogs.com/gif.latex?\left(E_{\text{K}},+\right)" /> de l'élément neutre <img src="https://latex.codecogs.com/gif.latex?e_{\left(E_{\text{K}},\times\right)}" /> du groupe <img src="https://latex.codecogs.com/gif.latex?\left(E_{\text{K}},\times\right)" />, mais t'as compris la logique du truc), c'est à dire <img src="https://latex.codecogs.com/gif.latex?-1\cdot%20A" />

Du coup, toute matrice <img src="https://latex.codecogs.com/gif.latex?A\in%20M_{n,p}\left(\text{K}\right)" /> a une matrice <img src="https://latex.codecogs.com/gif.latex?A'\in%20M_{n,p}\left(\text{K}\right)\%20\%20|\%20\%20A'=-A" /> (tu vois venir le truc, on va y revenir plus tard mais yes le magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" /> est un groupe)

---

## Minus (-) binary operator of matrix

<img src="https://latex.codecogs.com/gif.latex?-:_{\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\left(A_1,\%20A_2\right)\%20\%20\%20\%20\%20\%20\rightarrow\%20A_1+\left(-\left(A_2\right)\right)}^{M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20\times\%20M_{n,p}\left(\text{K}\right)\%20\rightarrow\%20M_{n,p}\left(\text{K}\right)}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?-\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> retourne une matrice <img src="https://latex.codecogs.com/gif.latex?A_{res}=A_1+\left(-1\cdot%20A_2\right)" />

Comme pour le + binaire matriciel, la fonction - binaire matricielle ne prend que 2 matrices **de même taille**.

Du coup, <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in%20M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right),\%20\left(A-A\right)=\left(A+\left(-e_{\left(\text{K},\times\right)}\cdot%20A\right)\right)=N_{n,p,\text{K}}" /> où <img src="https://latex.codecogs.com/gif.latex?N_{n,p,\text{K}}" /> est la matrice nulle de dimension n x p.

Autrement dit, A-A=matrice nulle

Et du coup, vu que, dans le magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" />,
- l'opération <img src="https://latex.codecogs.com/gif.latex?+\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" />, qui est une loi de composition interne, est associative
- qu'il y a un élément neutre qui est la matrice nulle de dimensions n x p
- que toute matrice <img src="https://latex.codecogs.com/gif.latex?A\in%20M_{n,p}\left(\text{K}\right)" /> dispose dans <img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)" /> d'une matrice <img src="https://latex.codecogs.com/gif.latex?A'\%20\%20|\%20\%20\left(A'=-A\right)" />

-> le magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" /> est donc **un groupe** (c'est même un groupe commutatif vu que le plus binaire matriciel est commutatif)

---

## Matrix multiply (*) operator of matrix

<img src="https://latex.codecogs.com/gif.latex?\times%20or\%20\cdot\%20:_{\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\left(A_1,\%20A_2\right)\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\rightarrow\%20A_{res}=\left(a_{i,j}=\sum_{k=1}^pA_{i,k}\times%20A_{k,j}\right)_{._{j\in\left[1,q\right]}^{i\in\left[1,n\right]}}}^{M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20\times\%20M_{p,q_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)\%20\rightarrow\%20M_{n,q}\left(\text{K}\right)}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?\times\left(A_{1_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{p_{\in\mathbb{N}^{\ast}},\%20q_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> ou <img src="https://latex.codecogs.com/gif.latex?\cdot\left(A_{1_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{p_{\in\mathbb{N}^{\ast}},\%20q_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> est une fonction qui prend en argument **une matrice n x p sur K**, et **une matrice p x q sur K**, et retourne **une matrice n x q sur K**. Ca veut dire que: 
- cette fonction n'est **pas commutative**
- la taille de colonnes de la 1ère matrice doit être égale à la taille de lignes de la 2e  matrice, c'est obligé sinon ca ne fonctionne pas. Ça sert à rien de vouloir multiplier 2 matrices dont la taille de colonne de la première n'est pas égale à la taille de ligne de la 2e, ça ne marche pas.

La matrice retournée sera donc une matrice n x q sur K, dont chaque coefficient est généré comme suit:
- on multiplie un à un chaque coefficient de la **1ère ligne de la 1ère matrice** par chaque coefficient de la **1ère colonne de la 2e matrice**, et on somme chaque résultat &#8594; ça nous donne le coefficient (1, 1) de la matrice de retour
- on multiplie un à un chaque coefficient de la **première ligne de la première matrice** par chaque coefficient de la **2e colonne de la 2e matrice**, et on somme chaque résultat &#8594; ça nous donne le coefficient (1, 2) de la matrice de retour
- ...
- on multiplie un à un chaque coefficient de la **première ligne de la première matrice** par chaque coefficient de la **n-ième colonne de la 2e matrice**, et on somme chaque résultat ==> ça nous donne le coefficient (1, n) de la matrice de retour
- &#8594; on a donc toute la première ligne de notre matrice de retour
- On recommene la même chose avec la **2e ligne de la première matrice** &#8594; on a la 2e ligne de notre matrice de retour
- On recommene la même chose avec la **3e ligne de la première matrice** &#8594; on a la 3e ligne de notre matrice de retour
- ...
- On recommene la même chose avec la **p-ième ligne de la première matrice** &#8594; on a la p-ième ligne de notre matrice de retour
- &#8594; On a donc toute notre matrice de retour
- On boit un coup parce qu'on a galéré comme jaja



En gros, formellement, la matrice de retour c'est la matrice

<img src="https://latex.codecogs.com/gif.latex?A_{res}=\left(a_{i,j}=\sum_{k=1}^p\left(A_{1_{i,k}}\cdot%20A_{2_{k,\%20j}}\right)\right)_{._{j\in\left[1,q\right]}^{i\in\left[1,n\right]}}" />

Du coup, pour résumer:

<img src="https://latex.codecogs.com/gif.latex?\times\left(A_{1_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{p_{\in\mathbb{N}^{\ast}},\%20q_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> 
ou 
<img src="https://latex.codecogs.com/gif.latex?\cdot\left(A_{1_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{p_{\in\mathbb{N}^{\ast}},\%20q_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" />

&#8595;

<img src="https://latex.codecogs.com/gif.latex?A_{res}=\left(a_{i,j}=\sum_{k=1}^p\left(A_{1_{i,k}}\cdot%20A_{2_{k,\%20j}}\right)\right)_{._{j\in\left[1,q\right]}^{i\in\left[1,n\right]}}" />


### Remarques sur la multiplication matricielle:
- elle n'est pas commutative
- elle est associative
- elle est distributive sur le + binaire matriciel (comme l'est l'opérateur scalaire de multiplication matriciel)
- la matrice nulle est un élément annulateur, c'est à dire que <img src="https://latex.codecogs.com/gif.latex?A_{\in%20M_{n,p}\left(\text{K}\right)}\cdot%20N=N" />
- La **matrice identité** <img src="https://latex.codecogs.com/gif.latex?I_n\in%20M_{n,n}\left(\text{K}\right)" /> est telle que <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in%20M_{n,p}\left(\text{K}\right),\%20\left(I_n\cdot%20A\right)=A" /> (c'est un peu comme un élément neutre de <img src="https://latex.codecogs.com/gif.latex?\left(M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right),\%20\times\right)" /> mais que dans un sens)

- La **matrice identité** <img src="https://latex.codecogs.com/gif.latex?I_p\in%20M_{p,p}\left(\text{K}\right)" /> est telle que <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in%20M_{n,p}\left(\text{K}\right),\%20\left(A\cdot%20I_p\right)=A" /> (c'est un peu comme un élément neutre de <img src="https://latex.codecogs.com/gif.latex?\left(M_{n_{\in\mathbb{N}^{\ast}},p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right),\%20\times\right)" /> mais que dans un sens)

  - &#8594; Du coup, le magma <img src="https://latex.codecogs.com/gif.latex?\left(\text{K},\times\right)" /> n'a pas forcément d'élément neutre, dans le sens où si on a <img src="https://latex.codecogs.com/gif.latex?n\ne%20p" />, alors on peut faire <img src="https://latex.codecogs.com/gif.latex?I_n\times%20A_{\in%20M_{n,p}\left(\text{K}\right)}" /> mais pas <img src="https://latex.codecogs.com/gif.latex?A_{\in%20M_{n,p}\left(\text{K}\right)}\times%20I_n" /> car dans le second cas le nombre de colonne du premier terme n'est pas égal au nombre de lignes du second terme, et de même pour <img src="https://latex.codecogs.com/gif.latex?I_p" /> 
  
  - &#8594; le seul cas où <img src="https://latex.codecogs.com/gif.latex?I_n" /> pourra effectivement être un élément neutre du magma <img src="https://latex.codecogs.com/gif.latex?\left(\text{K},\times\right)" /> c'est quand <img src="https://latex.codecogs.com/gif.latex?n=p" />, c'est à dire quand il s'agit d'un **magma de matrices carrées** 
  
  - &#8594; du coup, le magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n_{\in\mathbb{N}^{\ast}},n}\left(\text{K}\right),\%20\times\right)" /> est unifère avec comme élément neutre <img src="https://latex.codecogs.com/gif.latex?I_n" />. Ce magma étant unifère, associatif <CF POUR PLUS TARD QUAND ON AURA DÉCRIT LE SYMETRIQUE D'UNE MATRICE POUR SAVOIR SI CA FAIT UN GROUPE OU PAS>

- si on prend 2 vecteurs de dimension <img src="https://latex.codecogs.com/gif.latex?n_{\in\mathbb{N}^{\ast}}" />, par exemple <img src="https://latex.codecogs.com/gif.latex?\vec{u}=\left(u_{x_{\in\mathbb{R}}},u_{y_{\in\mathbb{R}}}\right)_{\left(O,\%20\vec{e_x},\vec{e_y}\right)}" /> et <img src="https://latex.codecogs.com/gif.latex?\vec{v}=\left(v_{x_{\in\mathbb{R}}},v_{y_{\in\mathbb{R}}}\right)_{\left(O,\%20\vec{e_x},\vec{e_y}\right)}" /> qui seraient 2 vecteurs de dimension 2, et qu'on fait leur produit scalaire (c'est à dire <img src="https://latex.codecogs.com/gif.latex?\vec{u}\cdot\vec{v}=\left|\vec{u}\right|\cdot\left|\vec{v}\right|\cdot\cos\left(\vec{u},\vec{v}\right)=u_x\cdot%20v_x+u_y\cdot%20v_y" />), finalement ça revient à prendre le vecteur <img src="https://latex.codecogs.com/gif.latex?\vec{u}" /> et à le caster en une matrice ligne <img src="https://latex.codecogs.com/gif.latex?M_{\vec{u}}=\left[u_x\%20;\%20u_y\right]" />, prendre le vecteur <img src="https://latex.codecogs.com/gif.latex?\vec{v}" /> et à le caster en un matrice colonne <img src="https://latex.codecogs.com/gif.latex?M_{\vec{v}}=\left[_{v_y}^{v_x}\right]" />, et enfin à faire un produit des 2 matrices <img src="https://latex.codecogs.com/gif.latex?M_{\vec{u}}\cdot%20M_{\vec{v}}=u_x\cdot%20v_x+u_y\cdot%20v_y=\vec{u}\cdot\vec{v}" />.
- Le fait que le produit de 2 matrices donne la matrice nulle **NE SIGNIFIE PAS** que l'une des 2 matrices est la matrice nulle (on ne peut pas faire d'analogie avec les rééls où quand on a (ab = 0), alors (a=0 ou b=0) ). Il y a masse contres-exemples où 2 matrices non nulles qu'on multiplie entre elles donne une matrice nulle.

### Remarque sur les matrices identités:

Les matrices identités d'un ensemble de matrices <img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)" />, sont les matrices telles que si on les multiplie par n'importe quelle matrice <img src="https://latex.codecogs.com/gif.latex?A\in%20M_{n,p}\left(\text{K}\right)" />, l'opération retourne <img src="https://latex.codecogs.com/gif.latex?A" />.

Formellement, on peut dire qu'une matrice identité d'un ensemble de matrices <img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)" /> c'est une matrice <img src="https://latex.codecogs.com/gif.latex?I\%20\%20|\%20\%20\left(\forall%20A\in%20M_{n,p}\left(\text{K}\right),\%20\left(\left(I\cdot%20A=A\right)\%20\vee\%20\left(A\cdot%20I=A\right)\right)\right)" />

**Attention**, si une matrice I est une matrice identité de <img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)" /> **ça ne veut pas forcément dire** qu'elle-même appartient à  <img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)" />**

En réalité, une matrice identité est **forcément une matrice carrée**, dont tous les coefficients de la diagonale sont égal à 1 et dont tous les autres coefficients sont égal à 0.

On note la matrice identité de taille n x n (où n sont des entiers non nuls bien évidemment) <img src="https://latex.codecogs.com/gif.latex?I_n" />.

Du coup <img src="https://latex.codecogs.com/gif.latex?I_n\in%20M_{n,n}\left(\text{K}\right)" />.

---

## Scalar power (^) operator of matrix

<img src="https://latex.codecogs.com/gif.latex?\wedge:\%20_{\%20\%20\%20\%20\%20\%20\%20\%20\%20\%20\left(A\%20,\%20\%20\lambda\right)\%20\rightarrow\%20\%20_{\lambda\ne0\%20\rightarrow\%20\left(A\times%20A\times%20A\times...\%20\times%20A\right)=A^{\lambda}}^{\lambda=0\%20\rightarrow\%20I_n}}^{M_{n_{\in\mathbb{N}^{\ast}},n}\left(\text{K}\right)\%20\times\%20\mathbb{N}\%20\rightarrow\%20M_{n,n}\left(\text{K}\right)}" />

La fonction <img src="https://latex.codecogs.com/gif.latex?\wedge\left(A_{\in%20M_{a_{\in\mathbb{N}^{\ast}},a}\left(\text{K}\right)},\%20\lambda_{\in\mathbb{N}}\right)" />  qui prend une matrice et un entier naturel, déjà ne fonctionne (n'est définie) que pour des **matrices carrées**. Ca sert à rien de pow des matrices non carrés avec cette fonction ca ne marche pas.

Cette fonction retourne <img src="https://latex.codecogs.com/gif.latex?A\times%20A\times%20A\times...\times%20A\%20=A^{\lambda}" /> (A multiplié par A, lambda fois)

### Remarques:
* <img src="https://latex.codecogs.com/gif.latex?A^0=I_n" />, la matrice identité de <img src="https://latex.codecogs.com/gif.latex?M_{n,n}\left(\text{K}\right)" />
* <img src="https://latex.codecogs.com/gif.latex?\left(A_{\in%20M_{n,n}\left(\text{K}\right)}+B_{\in%20M_{n,n}\left(\text{K}\right)}\right)^2=A\%20^2+B^2+\left(A\cdot%20B\right)+\left(B\cdot%20A\right)" /> (car pour rappel, la fonction de multiplication matricielle n'est pas commutative)
* Une matrice A telle que <img src="https://latex.codecogs.com/gif.latex?\exists%20k\in\mathbb{N}\%20\%20\%20|\%20\%20\%20A^k=N" />, une matrice nulle, est dite **matrice nilpotente**

---

## Inversion (/) operator of matrix

j'ai vidé le compost et les poubelles mais maintenant je suis tout fatigué et je dois aller bosser demain donc je vais faire dodo biz


# Matrix commutation

Quand on dit que 2 matrices A et B commutent, ça veut dire que <img src="https://latex.codecogs.com/gif.latex?\left(A\cdot%20B\right)=\left(B\cdot%20A\right)" />, c'est à dire que **pour ces 2 matrices en particulier**, la fonction de multiplication matricielle est commutative.

Dans ce cas, on peut avoir une adaptation de la formule du binôme de Newton à ces matrices, avec

<img src="https://latex.codecogs.com/gif.latex?\left(A+B\right)^{\lambda}=\sum_{k=0}^{\lambda}\left(A^k\cdot%20B^{\left(\lambda-k\right)}\right)=\sum_{k=0}^{\lambda}\left(B^k\cdot%20A^{\left(\lambda-k\right)}\right)" />

Du coup, une matrice identité de <img src="https://latex.codecogs.com/gif.latex?M_{n,n}\left(\text{K}\right)" /> (ensemble de matrices carrées) commute avec n'importe quelle matrice carrée de l'ensemble <img src="https://latex.codecogs.com/gif.latex?M_{n,n}\left(\text{K}\right)" />
