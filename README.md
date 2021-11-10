# Numerical-Analysis
<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->


- [Requirements](#requirements)
- [TP1](#tp1)
- [TP2](#TP2)
- [TP3](#TP3)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->
## Requirements

* [ANACONDA For windows][ANACONDA] 
* [Jupyter][Jup]

## TP1
<h1 style="color:#800080;text-decoration:underline "> Introduction :</h1>
<p> 
    En analyse on a besoin beaucoup de fois à résoudre l'équation f(x)=0, qui peut se rammèner à résoudre une équation de type point fixe:X=g(x). 
    
 Ici on a besoin des méthodes itératives qui nécessitent la construction d'une suite réelle(Xn) convergente vers  α : racine de 
 
 f c'est à dire f(x)=0.
 
  les méthodes itératives utilisées sont  la dichotomie , méthode de pont fixe et méthode de newton.  </p>
  
   * La méthode dichotomie: 
  
  La méthode de dichotomie ou méthode de la bissection est, en mathématiques, un algorithme de recherche d'un zéro d'une 
  
  fonction qui consiste à répéter des partages d’un intervalle en deux parties puis à sélectionner le sous-intervalle dans 
  
  lequel existe un zéro de la fonction.
   
  $$ \circ \hspace{0.5cm} Si \hspace{0.5cm} f(a+b2)≤0 \Longrightarrow	α\in [(a+b)/2,b]$$

  $$ \circ \hspace{0.5cm} Sinon \hspace{0.5cm} f(a+b2)>0 \Longrightarrow	α\in [a,(a+b)/2]$$

  * La méthode de point fixe :

Le principe de cette méthode consiste à transformer l’équation $f(x) = 0$ en une équation équivalente $g(x) = x$ .

Le point α est alors un point fixe de g. Approcher les zéros de f revient à approcher les points fixes de g. 

Le choix de la fonction g est motivé par les exigences du théorème de point fixe.

En effet, elle doit être contractante dans un voisinage I de α, ce qui revient à vérifier que :

$|g_0(x)| < 1$ sur ce voisinage. Dans ce cas, on construit une suite $(x_n)$ $n \in \mathbb{N}$ définie par :

  $$\left \{
   \begin{array}{r c l}
      x_0 \hspace{0.2cm}dans\hspace{0.2cm} un\hspace{0.2cm} voisinage \hspace{0.2cm}I\hspace{0.2cm}de\hspace{0.2cm}α \\
      ∀ n ≥ 0,\hspace{0.3cm} x_{n+1} = g(x_n) 
   \end{array}
   \right. $$
   
   
   * La méthode de newton :
   
L'idée est de remplacer la courbe représentative de la fonction par sa tangente.

On part d'un point x0 de l'intervalle de définition de f, et on considère la tangente à la courbe représentative de f en

(x0,f(x0)). Soit x1 l'abscisse de l'intersection de la tangente avec l'axe des abscisses. 

Puisque la tangente est proche de la courbe, on peut espérer que x1 donne une meilleure estimation d'une solution de 

l'équation f(x)=0 que x0.

On recommence alors le procédé à partir de x1 , et on construit par récurrence une suite xn définie par :

$$x_{n+1}=x_n-(f(x_n)/f'(x_n))$$

Soit $g(x)=x-(\frac{f(x)}{f'(x)}) \Longrightarrow x_{n+1}= g(x_n)$
  
<h1 style="color:#800080;text-decoration:underline "> But de TP:</h1>

Dans ce tp on a étudier et comparer les différentes méthodes de résolution d'équation f(x)=0 .
  
  les outils utilisées : 
  
 ### Anaconda :
  
  Anaconda est une distribution libre et open source des langages de programmation Python et R appliqué au développement 
  
  d'applications dédiées à la science des données et à l'apprentissage automatique (traitement de données à grande échelle, 
  
  analyse prédictive, calcul scientifique),
  
  qui vise à simplifier la gestion des paquets et de déploiement4. Les versions de paquetages sont gérées par le système de 
  
  gestion de paquets conda. 
  
  ### Le langage utilisé : 
 
 Python 
 
[ANACONDA]: https://www.anaconda.com/products/individual
[Jup]: https://jupyter.org/
