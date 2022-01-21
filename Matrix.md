# Matrix

<img src="https://latex.codecogs.com/gif.latex?\left[_y^x\right],\%20\left[_{c\%20;\%20d}^{a\%20;\%20b}\right],\%20\left[_{c\%20;\%20d}^{a\%20;\%20b}\right]+\left[_{g\%20;\%20h}^{e\%20;\%20f}\right],\%20\left[_{c\%20;\%20d}^{a\%20;\%20b}\right]\cdot\left[_{g\%20;\%20h}^{e\%20;\%20f}\right],\%20..." />

## Definition

<img src="https://latex.codecogs.com/gif.latex?\text{Soit}\%20\text{un}\%20\text{corps}\%20\text{K}=\left(E_K,\%20+,\%20\cdot\right)\%20" />
<img src="https://latex.codecogs.com/gif.latex?\left(\text{Genre}\%20\text{K}_{\mathbb{C}}=\left(\mathbb{C},\%20+,\%20\cdot\right),\%20\text{K}_{\mathbb{R}}=\left(\mathbb{R},\%20+,\%20\cdot\right),\%20\text{K}_{\mathbb{Q}}=\left(\mathbb{Q},\%20+,\%20\cdot\right),\%20...\right)" />

<img src="https://latex.codecogs.com/gif.latex?\text{Une}\%20\text{matrice}\%20\text{est}\%20\text{un}\%20\text{tableau}\%20\text{rectangulaire}\%20\text{de}\%20n_{\in\mathbb{N}^{\ast}}\%20\text{lignes}\%20\text{sur}\%20\text{p}_{\in\mathbb{N}^{\ast}}\%20\text{colonnes}\%20\text{contenant}\%20\text{des}\%20\text{elements}\%20\text{de}\%20\text{K}" />

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
* Une matrice qui ne contient que des 0 s'appelle une **matrice nulle** (la matrice nulle <img src="https://latex.codecogs.com/gif.latex?N\in%20M_{n,p}\left(\text{K}\right)\%20" /> c'est l'élément neutre du monoïde <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" />)

## Square matrix

Une matrice est dite carrée si son nombre de lignes est égal à son nombre de colonnes (donc si n = p)

Dans une matrice carrée, il y a un truc particulier qu'on appèlle la **diagonale de la matrice** qui est l'ensemble des éléments <img src="https://latex.codecogs.com/gif.latex?\left\{A_{1,1},\%20A_{2,2},\%20A_{3,3},\%20...\%20,\%20A_{n,n}\right\}" />

## Equal (=) operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?=\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{c_{\in\mathbb{N}^{\ast}},\%20d_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> qui teste l'égalité de 2 matrices renvoit vrai si:
- les 2 matrices ont un nombre de lignes identique
- les 2 matrices ont un nombre de colonnes identique
- si les coefficients sont identiques un à un, c'est à dire si <img src="https://latex.codecogs.com/gif.latex?\forall\left(i,j\right)\in\left(\mathbb{N}^{\ast}\right)^2,\%20M_{1_{i,j}}=M_{2_{i,j}}" />


Cette fonction est associative

## Plus (+) unary operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?+\left(A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> renvoit juste la matrice. C'est une fonction identité.

## Plus (+) binary operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?+\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> qui prend 2 matrices pour les additionner, déjà ne fonctionne (n'est définie) que pour des **matrices de même taille**. Ca sert à rien d'additionner des matrices de tailles différentes avec cette fonction + ca ne marche pas.

Elle renvoit une matrice dont chaque coeffient est égal à la somme des coefficients correspondants dans les matrices passées en argument, c'est à dire que la fonction <img src="https://latex.codecogs.com/gif.latex?=\left(M_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20M_{2_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> renvoit une matrice <img src="https://latex.codecogs.com/gif.latex?A_{res}=\left(a_{i,j}=M_{1_{i,j}}+M_{2_{i,j}}\right)_{._{j\in\left[1,\%20b\right]}^{i\in\left[1,\%20a\right]}}" />

Elle est:
* associative
* commutative

## Scalar multiplication (*) operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?\times\left(\lambda_{\in\text{K}}\%20,\%20A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> ou <img src="https://latex.codecogs.com/gif.latex?\cdot\left(\lambda_{\in\text{K}}\%20,\%20A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> qui prend en argument un scalaire de K et une matrice de n x p sur K, retourne la matrice passée en argument, mais avec tous ses coefficients multipliés par k. C'est à dire que la fonction renvoit une matrice <img src="https://latex.codecogs.com/gif.latex?A_{res}=\left(a_{i,j}=k\cdot%20A_{i,j}\right)_{._{j\in\left[1,p\right]}^{i\in\left[1,n\right]}}" />.

Elle est
* associative
* commutative
* distributive sur le + binaire matriciel


* le réél 0 est un élément anulateur, c'est à dire que <img src="https://latex.codecogs.com/gif.latex?0\times%20A=N" />
* la matrice nulle est un élément anulateur, c'est a dire que <img src="https://latex.codecogs.com/gif.latex?k_{\in\mathbb{R}}\times%20N=N" />
* 1 est l'élément neutre du magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20\cdot\right)=\left(M_{n,p}\left(\text{K}\right),\%20\times\right)" />, c'est à dire que <img src="https://latex.codecogs.com/gif.latex?\forall%20A\in%20M_{n,\%20p}\left(\text{K}\right),\%201\times%20A=A" />

<je sais pas si c'est un groupe>


## Minus (-) unary operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?-\left(A_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}\right)" /> qui prend 1 matrice pour retourner son "opposé", retourne tout simplement la matrice passée en argument multipliée par le scalaire -1, c'est à dire <img src="https://latex.codecogs.com/gif.latex?-1\cdot%20A" />

Du coup, toute matrice <img src="https://latex.codecogs.com/gif.latex?A\in%20M_{n,p}\left(\text{K}\right)" /> a une matrice <img src="https://latex.codecogs.com/gif.latex?A'\in%20M_{n,p}\left(\text{K}\right)\%20\%20|\%20\%20A'=-A" /> (tu vois venir le truc, on va y revenir plus tard mais yes le magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" /> est un groupe)

## Minus (-) binary operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?-\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> retourne une matrice <img src="https://latex.codecogs.com/gif.latex?A_{res}=A_1+\left(-1\cdot%20A_2\right)" />

Du coup, <img src="https://latex.codecogs.com/gif.latex?A-A=A+\left(-1\cdot%20A\right)=N" /> où N est la matrice nulle de dimension n x p

Et du coup, vu que, dans le magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" />,
- l'opération <img src="https://latex.codecogs.com/gif.latex?+\left(A_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" />, qui est une loi de composition interne, est associative
- qu'il y a un élément neutre qui est la matrice nulle de dimensions n x p
- que toute matrice <img src="https://latex.codecogs.com/gif.latex?A\in%20M_{n,p}\left(\text{K}\right)" /> dispose dans <img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)" /> d'une matrice <img src="https://latex.codecogs.com/gif.latex?A'\%20\%20|\%20\%20\left(A'=-A\right)" />

-> le magma <img src="https://latex.codecogs.com/gif.latex?\left(M_{n,p}\left(\text{K}\right),\%20+\right)" /> est donc **un groupe** (c'est même un groupe commutatif vu que le plus binaire matriciel est commutatif)

## Matrix multiplication (*) operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?\times\left(A_{1_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{p_{\in\mathbb{N}^{\ast}},\%20q_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> ou <img src="https://latex.codecogs.com/gif.latex?\cdot\left(A_{1_{\in%20M_{n_{\in\mathbb{N}^{\ast}},\%20p_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20A_{2_{\in%20M_{p_{\in\mathbb{N}^{\ast}},\%20q_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> est une fonction qui prend en argument **une matrice n x p sur K**, et **une matrice p x q sur K**, et retourne **une matrice n x q sur K**. Ca veut dire que: 
- cette fonction n'est **pas commutative**
- la taille de colonnes de la 1ère matrice doit être égale à la taille de lignes de la 2e  matrice, c'est obligé sinon ca ne fonctionne pas. Ça sert à rien de vouloir multiplier 2 matrices dont la taille de colonne de la première n'est pas égale à la taille de ligne de la 2e, ça ne marche pas.

La matrice retournée sera donc une matrice n x q sur K, dont chaque coefficient est généré comme suit:
- on multiplie un à un chaque coefficient de la **1ère ligne de la 1ère matrice** par chaque coéfficient de la **1ère colonne de la 2e matrice**, et on somme chaque résultat &#8594; ça nous donne le coefficient (1, 1) de la matrice de retour
- on multiplie un à un chaque coefficient de la **première ligne de la première matrice** par chaque coéfficient de la **2e colonne de la 2e matrice**, et on somme chaque résultat &#8594; ça nous donne le coefficient (1, 2) de la matrice de retour
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



