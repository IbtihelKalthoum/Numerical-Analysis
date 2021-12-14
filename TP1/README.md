# TP1 Analyse Numérique
- [But](#But)
- [Introduction](#Introduction)
- [La_méthode_dichotomie](#La_méthode_dichotomie)
- [La_méthode_de_point_fixe](#La_méthode_de_point_fixe)
- [La méthode_de_newton](#La méthode_de_newton)
## But 

Dans ce tp on a étudier et comparer les différentes méthodes de résolution d'équation f(x)=0 .
## Introduction
<p> 
    En analyse on a besoin beaucoup de fois à résoudre l'équation f(x)=0, qui peut se rammèner à résoudre une équation de type point fixe:X=g(x). 
    
 Ici on a besoin des méthodes itératives qui nécessitent la construction d'une suite réelle(Xn) convergente vers  α : racine de 
 
 f c'est à dire f(x)=0.
 
  les méthodes itératives utilisées sont  la dichotomie , méthode de pont fixe et méthode de newton.  </p>
  
   ### La_méthode_dichotomie: 
  
  La méthode de dichotomie ou méthode de la bissection est, en mathématiques, un algorithme de recherche d'un zéro d'une 
  
  fonction qui consiste à répéter des partages d’un intervalle en deux parties puis à sélectionner le sous-intervalle dans 
  
  lequel existe un zéro de la fonction.
  $$ \circ \hspace{0.5cm} Si \hspace{0.5cm} f(a+b2)≤0 \Longrightarrow	α\in [(a+b)/2,b]$$

  $$ \circ \hspace{0.5cm} Sinon \hspace{0.5cm} f(a+b2)>0 \Longrightarrow	α\in [a,(a+b)/2]$$

  ### La_méthode_de_point_fixe :

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
   
   
   ### La méthode_de_newton :
   
L'idée est de remplacer la courbe représentative de la fonction par sa tangente.

On part d'un point x0 de l'intervalle de définition de f, et on considère la tangente à la courbe représentative de f en

(x0,f(x0)). Soit x1 l'abscisse de l'intersection de la tangente avec l'axe des abscisses. 

Puisque la tangente est proche de la courbe, on peut espérer que x1 donne une meilleure estimation d'une solution de 

l'équation f(x)=0 que x0.

On recommence alors le procédé à partir de x1 , et on construit par récurrence une suite xn définie par :

$$x_{n+1}=x_n-(f(x_n)/f'(x_n))$$

Soit $g(x)=x-(\frac{f(x)}{f'(x)}) \Longrightarrow x_{n+1}= g(x_n)$
  

