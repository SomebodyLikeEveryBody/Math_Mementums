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

Finalement, pour une matrice de n x p sur K, si on considère que chaque ligne est un ensemble ordonné de p éléments de K (c'est à dire un p-uplet d'éléments de K)
alors chaque ligne d'une matrice est un élément de 
<img src="https://latex.codecogs.com/gif.latex?\text{K}^p" />.
Du coup, une matrice c'est un ensemble ordonné de lignes (un n-uplet de lignes), c'est à dire qu'on peut considérer que c'est un élément de <img src="https://latex.codecogs.com/gif.latex?\left(K^p\right)^n" />

<img src="https://latex.codecogs.com/gif.latex?M_{n,p}\left(\text{K}\right)=\left(K^p\right)^n" />

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


## Minus (-) operator of matrix

La fonction <img src="https://latex.codecogs.com/gif.latex?-\left(M_{1_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}},\%20M_{2_{\in%20M_{a_{\in\mathbb{N}^{\ast}},\%20b_{\in\mathbb{N}^{\ast}}}\left(\text{K}\right)}}\right)" /> qui prend 2 matrice pour les soustraire, c'est pareil elle ne fonctionne qu'avec 2 matrices **de même tailles**. 
