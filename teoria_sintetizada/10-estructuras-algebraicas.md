### SEMIGRUPO
###### Definición
Sea $S \ne \varnothing$ un conjunto y $*:S \times S \rightarrow S$ una operación binaria.

Decimos que $(S,*)$ es un **semigrupo** si se cumple:

$i)$ Cierre: $$\forall a,b\in S:a*b\in S$$
$ii)$ Asociatividad: $$\forall a,b,c\in S:(a*b)*c=a*(b*c)$$
Observación: no se exige existencia de neutro ni de inversos.

Ejemplo:
$(\mathbb{N},+)$ es semigrupo, pues la suma es cerrada y asociativa en $\mathbb{N}$.
### GRUPO
###### Definición
Sea $G \ne \varnothing$ y $*:G\times G \rightarrow G$.

Decimos que $(G,*)$ es un **grupo** si se cumplen:

$i)$ Cierre: $$\forall a,b \in G, a*b\in G$$
$ii)$ Asociatividad: $$\forall a,b,c \in G: (a*b)*c=a*(b*c)$$
$iii)$ Existencia de elemento neutro: $$\exists e \in G \text{ tal que } \forall a \in G: e*a=a*e=a$$
$iv)$ Existencia de inverso: $$\forall a \in G,\exists a^{-1}\in G:a*a^{-1}=a^{-1}*a=e$$
Notación: el par $(G,*)$.

Ejemplo: $(\mathbb{Z},+)$ es grupo.
### UNICIDAD DEL NEUTRO
###### Teorema
En un grupo, el elemento neutro es único
###### Demostración
Sea $e$ y $e'$ neutros en $G$. Entonces:

Por ser $e$ neutro: $e*e'=e'$
Por ser $e'$ neutro: $e*e'=e$
Luego, por transitividad de la igualdad: $e=e'$
### UNICIDAD DEL INVERSO
###### Teorema
En un grupo, el inverso de cada elemento es único.
###### Demostración
Sea $a \in G$ y supongamos que $b$ y $c$ son inversos de $a$. Entonces: $$a*b=b*a=e$$ $$a*c=c*a=e$$
Entonces: $b=b*e \Rightarrow b=b*(a*c)$
Por asociatividad: $b=(b*a)*c$
Como $b*a=e$, resulta: $b=e*c$
Y como $e$ es neutro: $b=c$
### CRITERIO DE SUBGRUPO
###### Teorema (criterio práctico)
Sea $(G,*)$ grupo y $H \subseteq G$.

Si:
$i)$ $H \ne \varnothing$
$ii)$ $\forall a,b\in G,a*b^{-1}\in H$

Entonces $H$ es un subgrupo de $G$.
###### Demostración esquemática formal
1. Como $H \ne \varnothing$, existe $h \in H$.

2. Tomando $a=b=h$, se tiene: $h*h^{-1}\in H$
Pero $h*h^{-1}=e$, luego $e\in H$.

3. Para $a\in H$, como $e \in H$: $a*e^{-1}\in H$
Pero $e^{-1}=e$, luego $a\in H$
y además: $a^{-1}=e*a^{-1}\in H$

4. Si $a,b\in H$, ya sabemos que $b^{-1}\in H$, entonces: $a*(b^{-1})^{-1}=a*b\in H$

Se verifican cierre, neutro e inversos. Luego $H$ es subgrupo.
### GRUPO ABELIANO
###### Definición
Un grupo $(G,*)$ es **abeliano** si además se cumple: $$\forall a,b\in G:a*b=b*a$$
Es decir, la operación es conmutativa.

Ejemplo:
$(\mathbb{Z},+)$ es grupo abeliano.
### ANILLO
###### Definición
Sea $A \ne \varnothing$ con dos operaciones $+$ y $\cdot$.

Decimos que $(A,+,\cdot)$ es un **anillo** si:

$i)$ $(A,+)$ es grupo abeliano.
$ii)$ $(A,\cdot)$ es semigrupo.
$iii)$ Distributividad:$$\begin{aligned} \forall a,&b,c \in A, \\ a\cdot(b+c) & =a\cdot b+a\cdot c \\ (b+c)\cdot a & =b\cdot a+c\cdot a \end{aligned}$$
Observaciones:
- No se exige inverso multiplicativo.
- Puede o no tener neutro multiplicativo.

Ejemplo:
$(\mathbb{Z},+,\cdot)$ es anillo.
### Resumen estructural
$$\text{Semigrupo} \Rightarrow \text{Agrego neutro e inversos} \Rightarrow \text{Grupo} \Rightarrow \text{Agrego conmutatividad} \Rightarrow \text{Grupo abeliano}$$
$$\text{Grupo abeliano + segunda operación distributiva} \Rightarrow Anillo$$
