#  Interpolation Numérique
- [But_de_TP](#But_de_TP)
- [Introduction](#Introduction)
- [Principe_de_l_interpolation_polynomiale](#Principe_de_l_interpolation_polynomiale)
> - [Principe_de_l_interpolatio_de_Lagrange](#Principe_de_l_interpolation_de_Lagrange)
> - [Principe_de_phénomène_de_Runge](#Principe_de_phénomène_de_Runge)
> - [Principe_de_polynome_de_Newton](#Principe_de_polynome_de_Newton)
- [Conclusion](#conclusion)
### But de TP

- Etudier les polynomes d'interpolation.

- Etudier leur  principe de fonctionnements.

- Interpréter les résultats obtenues.
### Introduction

> En mathématiques, en analyse numérique, l'interpolation polynomiale est une technique d'interpolation d'un ensemble de 
  
 données ou d'une fonction par un polynôme. En d'autres termes, étant donné un ensemble de points , on cherche un polynôme 
    
 qui passe par tous ces points, et éventuellement vérifie d'autres conditions, de degré si possible le plus bas.




### Principe_de_l_interpolation_polynomiale:



*  Principe_de_l_interpolation_de_Lagrange:

Le polynôme d’interpolation de Lagrange P(x) est le polynôme unique d’ordre n, qui passe exactement par ces (n+1) points,il permettent d'interpoler une série de points par un polynome:
> Soient <img src="https://render.githubusercontent.com/render/math?math=(x_0,y_0), \ldots,(x_k,y_k),\ldots ,(x_n,k_n)">  , le polynôme d'interpolation de Lagrange associés à ces points supports est défini par :
<img src="https://render.githubusercontent.com/render/math?math=\displaystyle P_n(x)=\sum_{k=0}^{n%2B1} y_kL_k(x)">

avec


<img src="https://render.githubusercontent.com/render/math?math=L_{0}(x)=\displaystyle\frac{(x-x_1)(x-x_2)\ldots(x-x_{n})}{(x_0-x_1)(x_0-x_2)\ldots(x_0-x_{n})}">

et 


<img src="https://render.githubusercontent.com/render/math?math=L_{k}(x)=\displaystyle\frac{(x-x_1)(x-x_2)\ldots(x-x_{k-1})(x-x_{k%2B1})\ldots(x-x_{n})}{(x_k-x_0)(x_k-x_1)\ldots(x_k-x_{k-1})(x_k-x_{k %2B 1})\ldots(x_k-x_{n})}">


 pour 
 
 <img src="https://render.githubusercontent.com/render/math?math=k\in \{1,\ldots,n\}">



*  Principe_de_phénomène_de_Runge:

Dans le domaine mathématique de l'analyse numérique, le phénomène de Runge se manifeste dans le contexte de l'interpolation polynomiale, en particulier l'interpolation de Lagrange. Avec certaines fonctions (même analytiques), l'augmentation du nombre n de points d'interpolation ne constitue pas nécessairement une bonne stratégie d'approximation.

*  Principe_de_polynome_de_Newton :

l'interpolation newtonienne, est une méthode d'interpolation polynomiale permettant d'obtenir le polynôme de Lagrange comme combinaison linéaire de polynômes de la « base newtonienne ».

l'interpolation polynomiale dans une base de Newton est une combinaison linéaire de polynômes appartenant à cette base.
### Conclusion
> * L’interpolation designe la construction d’une courbe `a partir de donnée d’un nombre fini de
points, ou d’une fonction `a partir de  donnée d’un nombre fini de valeurs.
* La solution du probléme d’interpolation passe nécessairement et au minimum par les points prescrits et peut necessiter de
respecter des contraintes supplémentaires.
L’interpolation doit ˆetre distinguée de l’approximation, qui consiste alors `a trouver la fonction
la plus proche possible d’une série de donnees. Dans le cas de l’approximation, il n’est en général
plus imposé de passer exactement par les points initiaux. Cependant, une confusion est souvent possible et l’on parle ´egalement d’approximation de la fonction pour désigner les valeurs (estimées) issues d’une interpolation.
