# Numerical-Analysis
<h1 style="color:#800080;text-decoration:underline "> Introduction :</h1>
<p> en analyse on a besoin beaucoup de fois à résoudre l'équation f(x)=0, qui peut se rammèner à résoudre une équation de type
    
   point fixe:X=g(x). 
    
 ici ona besoin des méthodes itératives qui nécessitent la construction d'une suite réelle(Xn) convergente vers  α : racine de 
 
 f c'est à dire f(x)=0.
 
  les méthodes itératives utilisées sont  la dichotomie , méthode de pont fixe et méthode de newton.  </p>
  
  <strong> la méthode dichotomie: </strong>
  
  La méthode de dichotomie ou méthode de la bissection est, en mathématiques, un algorithme de recherche d'un zéro d'une 
  
  fonction qui consiste à répéter des partages d’un intervalle en deux parties puis à sélectionner le sous-intervalle dans 
  
  lequel existe un zéro de la fonction.
   
   $$ \circ \hspace{0.5cm} Si \hspace{0.5cm} f(a+b2)≤0 \Longrightarrow	α\in [(a+b)/2,b]$$

$$ \circ \hspace{0.5cm} Sinon \hspace{0.5cm} f(a+b2)>0 \Longrightarrow	α\in [a,(a+b)/2]$$

<strong> la méthode de point fixe :</strong>

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
   
   <strong> La méthode de newton :</strong>
   
L'idée est de remplacer la courbe représentative de la fonction par sa tangente.

On part d'un point $x_0$ de l'intervalle de définition de f, et on considère la tangente à la courbe représentative de f en

$(x_0,f(x_0))$. Soit $x_1$ l'abscisse de l'intersection de la tangente avec l'axe des abscisses. 

Puisque la tangente est proche de la courbe, on peut espérer que $x_1$ donne une meilleure estimation d'une solution de 

l'équation f(x)=0 que $x_0$.

On recommence alors le procédé à partir de $x_1$, et on construit par récurrence une suite $(x_n)$ définie par :

$$x_{n+1}=x_n-(f(x_n)/f'(x_n))$$

Soit $g(x)=x-(\frac{f(x)}{f'(x)}) \Longrightarrow x_{n+1}= g(x_n)$
  
<h1 style="color:#800080;text-decoration:underline "> But de TP:</h1>

Dans ce tp on a étudier et comparer les différentes méthodes de résolution d'équation f(x)=0 .
  
  les outils utilisées : 
  
  <strong> anaconda </strong>:
  
  Anaconda est une distribution libre et open source des langages de programmation Python et R appliqué au développement 
  
  d'applications dédiées à la science des données et à l'apprentissage automatique (traitement de données à grande échelle, 
  
  analyse prédictive, calcul scientifique),
  
  qui vise à simplifier la gestion des paquets et de déploiement4. Les versions de paquetages sont gérées par le système de 
  
  gestion de paquets conda. 
  
  <strong> Le langage utilisé : </strong>
 
 python 
