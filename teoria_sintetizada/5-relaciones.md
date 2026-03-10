### DEFINICIÓN FORMAL DE RELACIÓN
Sea $A$ un conjunto.

Una **relación binaria sobre A** es un subconjunto del producto cartesiano $A \times A$.
Formalmente: $R \subseteq A \times A$

Recordemos que: $A \times A=$ {$(a,b):a \in A \land b \in A$}

Si $(a,b) \in R$, escribimos $\text{a R b}$.
Si $(a,b) \notin R$, escribimos $\text{a /R b}$

**Ejemplo:** Sea $A=Z$ y definimos $R=$ {$(a,b)\in Z \times Z:a-b \text{ es par}$}
Entonces $R \subseteq Z \times Z$.
### PROPIEDADES DE UNA RELACIÓN
Sea $R \subseteq A \times A$.
Todas las propiedades deben poder escribirse con cuantificadores.
###### Reflexiva
$R$ es reflexiva si: $\forall a \in A:(a,a)\in R$

Es decir: $\forall a \in A: \text{a R a}$
###### Simétrica
$R$ es simétrica si: $\forall a,b \in A:(a,b)\in R \Rightarrow (b,a)\in R$

Es decir: $\forall a,b \in A: \text{a R b} \Rightarrow \text{b R a}$
###### Antisimétrica
$R$ es antisimétrica si: $\forall a,b\in A:[(a,b)\in R\land(b,a)\in R]\Rightarrow a=b$

Es decir: $\text{a R b} \land \text{b Ra} \Rightarrow a=b$
###### Asimétrica
$R$ es asimétrica si: $\forall a,b \in A:(a,b)\in R \Rightarrow(b,a)\notin R$

Es decir: $\text{a R b} \Rightarrow \sim(\text{b R a})$

**Observación importante:** Toda relación asimétrica es antisimétrica, pero no recíprocamente.
###### Transitiva
$R$ es transitiva si: $\forall a,b,c \in A:[(a,b)\in R \land (b,c)\in R]\Rightarrow(a,c) \in R$

Es decir: $\text{a R b } \land \text{ b R c} \Rightarrow \text{a R c}$
### ORDEN PARCIAL
Una relación $R \subseteq A \times A$ es un **orden parcial** si es:
- Reflexiva
- Antisimétrica
- Transitiva

Formalmente: $R$ es orden parcial $\Leftrightarrow$
1. $\forall a\in A: \text{a R a}$
2. $\forall a,b \in A: \text{a R b } \land \text{ b R a} \Rightarrow a=b$
3. $\forall a,b,c \in A: \text{a R b } \land \text{ b R c} \Rightarrow \text{a R c}$

**Ejemplos:**

En $Z$, la relación "$\leq$" es un orden parcial porque:
- $a \leq a$ (reflexiva)
- $a\leq b \land b\leq a \Rightarrow a=b$ (antisimétrica)
- $a \leq b \land b \leq c \Rightarrow a \leq c$ (transitiva)

Sea $A=P(X)$ (conjunto partes).
Definimos $R=$ {$(A,B):A\subseteq B$}
Entonces $\subseteq$ es un orden parcial.
Se demuestra usando la definición: $A \subseteq B \Leftrightarrow \forall x: x \in A \Rightarrow x \in B$

Demostración formal de que $(P(X),\subseteq)$ es orden parcial.
Sea $A,B,C \subseteq X.$
1. Reflexividad:
Queremos probar $A \subseteq A.$
Por definición de inclusión: $A \subseteq A \Leftrightarrow \forall x:(x \in A \Rightarrow x \in A).$
Sea $x \in A$. Entonces $x \in A$ (verdad trivial).
Luego $A \subseteq A.$
2. Antisimetría:
Supongamos $A \subseteq B \land B \subseteq A.$
Entonces:
$\forall x:x \in A \Rightarrow x \in B$
$\forall x:x \in B \Rightarrow x \in A.$
Luego: $\forall x:x \in A \Leftrightarrow x \in B.$
Por definición de igualdad de conjuntos: $A=B$.
3. Transitividad:
Supongamos $A \subseteq B \land B \subseteq C.$
Sea $x \in A.$
Como $A \subseteq B$, entonces $x \in B.$
Como $B \subseteq C$, entonces $x \in C.$
Luego $A \subseteq C.$

**Relación estricta asociada**
Sea $(A,R)$ un orden parcial.
Definimos la relación estricta $R^*$ por: $a\text{ }R^*\text{ }b\Leftrightarrow a \text{ }R\text{ }b \land a\neq b.$
Propiedades:
1. $R^*$ es asimétrica.
Demostración:
Supongamos $a\text{ }R^*\text{ }b.$
Entonces $a\text{ }R\text{ }b$ y $a \neq b.$
Si además $b\text{ }R^*\text{ }a$, entonces $b\text{ }R\text{ }a$ y $b\neq a.$
De la antisimétrica en $R$: $a\text{ }R\text{ }b \land b\text{ }R\text{ }a\Rightarrow a=b.$
Contradicción con $a \neq b.$
Luego $R^*$ es asimétrica.
2. $R^*$ es transitiva.
Sea $a\text{ }R^*\text{ }b$ y $b\text{ }R^*\text{ }c.$
Entonces: $a\text{ }R\text{ }b\land b\text{ }R\text{ }c.$
Por transitividad de $R$: $a\text{ }R\text{ }c.$
Además, si $a=c$, entonces de $a\text{ }R\text{ }b$ y $b \text{ }R\text{ a}$ se obtendría $a=b$ por antisimetría, contradicción con $a\ne b.$
Luego $a \neq c.$
Por tanto $a\text{ }R^*\text{ }c.$
### RELACIÓN DE EQUIVALENCIA
Una relación $R \subseteq A\times A$ es una **relación de equivalencia** si es:
- Reflexiva
- Simétrica
- Transitiva

Formalmente: 
1. $\forall a\in A: \text{a R a}$
2. $\forall a,b \in A: \text{a R b } \Rightarrow \text{ b R a}$
3. $\forall a,b,c \in A: \text{a R b } \land \text{ b R c} \Rightarrow \text{a R c}$

Ejemplo:

En $Z$ definimos: $\text{a R b} \Leftrightarrow a-b \text{ es múltplo de n}$
Es decir: $a \equiv b \text{ (mod n)}$
Esto es relación de equivalencia.

Demostración de que $\equiv(\text{mod n})$ es relación de equivalencia.
Definimos: $\text{a R b} \Leftrightarrow n\text{ | }(a-b).$
1. Reflexiva:
$a-a=0$
$n\text{ | }0$
Luego $\text{a R a}.$
2. Simétrica:
Si $n\text{ | }(a-b)$, entonces $a-b=nk.$
Multiplicando por $-1$: $b-a=-nk$
Luego $n\text{ | }(b-a).$
Por tanto $\text{b R a}.$
3. Transitiva:
Si $n\text{ | }(a-b) \land n\text{ | }(b-c)$, entonces:
$a-b=nk, \forall k \in Z$
$b-c=nm, \forall m \in Z$
Sumando: $a-c=n(k+m), \forall k,m \in Z$
Luego $n \text{ | }(a-c).$
Por tanto: $\text{a R c}.$
###### Teorema
Si $R$ es relación de equivalencia sobre $A$, entonces el conjunto de clases: $A/R=$ {$[a]:a\in A$} es una partición de $A$.

Demostración:
1. Cada $a\in A$ pertenece a su clase $[a]$, pues $R$ es reflexiva.
2. Si $[a]\cap[b]\ne\varnothing$, entonces $[a]=[b].$
Sea $x \in [a]\cap[b].$
Entonces $x\text{ }R\text{ }a\land x\text{ }R\text{ }b.$
Por simetría: $a\text{ }R\text{ }x.$
Por transitividad: $a\text{ }R\text{ }b.$
Luego se demuestra que: $[a]=[b].$
Sea $y\in[a]$. Entonces $y\text{ }R\text{ }a.$
Como $a\text{ }R\text{ }b$, por transitividad $y\text{ }R\text{ }b.$
Luego $y\in[b].$
Así $[a]\subseteq[b].$
Análogamente se prueba $[b]\subseteq[a].$
Luego $[a]=[b].$
3. La unión de todas las clases es $A$, porque todo elemento pertenece a su clase.
### CLASE DE EQUIVALENCIA
Sea $R$ una relación de equivalencia sobre $A$.

La **clase de equivalencia de a** se define como: $[a]=$ {$x \in A: \text{x R a}$}
Es decir: $[x]=$ {$\text{elementos relacionados con x}$}

Propiedad fundamental:

Las clases de equivalencia:
- Son disjuntas o iguales.
- Su unión es todo el conjunto $A$.
- Forman una partición de $A$.
### EJERCICIOS
**A) Determinar si una relación es orden parcial**
Ejemplo:
Sea $R$ en $Z$ definida por: $\text{a R b} \Rightarrow a \text{ divide a }b$
1. Reflexiva:
$a$ divide a $a \rightarrow$ verdadero 
2. Antisimétrica:
Si $a$ divide a $b$ y $b$ divide a $a$, entonces $a=b$ o $a=-b$
En $Z$ no es antisimétrica.
En $N$ si lo es.
3. Transitiva:
Si $a$ | $b$ y $b$ | $c$, entonces $a$ | $c$ $\rightarrow$ verdadero.

Conclusión: En $N$ es orden parcial. En $Z$ no.

**B) Construir relación antisimétrica pero no asimétrica**
Queremos:
- Antisimétrica
- No asimétrica

Ejemplo: Sea $A=$ {$1,2$}.
Definimos: $R=$ {$(1,1),(2,2),(1,2)$}

Verificación:

Antisimétrica:
No ocurre que (1,2) y (2,1) estén ambos.
Luego se cumple.

No asimétrica:
Porque $(1,1)\in R$.
Pero si fuera asimétrica debería cumplirse: $\text{a R a} \Rightarrow \text{imposible}$

Una relación asimétrica nunca puede tener (a,a).

Luego esta relación es antisimétrica pero no asimétrica.

**C) Construir relación con dos clases de equivalencia**
Sea $A=Z$.
Definimos: $a\text{ R }b \Leftrightarrow a-b \text{ es par.}$

Entonces hay exactamente dos clases:
$[0]=$ {$\text{números pares}$}
$[1]=$ {$\text{números impares}$}

Es decir: $Z=[0] \cup [1]$

Dos clases disjuntas.

**D) Expresar propiedades en símbolos**

Reflexiva: $\forall a\in A:(a,a)\in R$
Simétrica: $\forall a,b \in A: (a,b) \in R \Rightarrow (b,a) \in R$
Antisimétrica: $\forall a,b \in A:[(a,b)\in R\land(b,a)\in R]\Rightarrow a=b$
Asimétrica: $\forall a,b \in A:(a,b)\in R \Rightarrow (b,a)\notin R$
Transitiva: $\forall a,b,c\in A:[(a,b)\in R \land(b,c)\in R]\Rightarrow(a,c)\in R$

Orden parcial: $R$ es reflexiva, antisimétrica y transitiva.

Relación de equivalencia: $R$ es reflexiva, simétrica y transitiva.

Clase: $[a]=$ {$x \in A:(x,a)\in R$}
### DIFERENCIAS CONCEPTUALES
**Antisimétrica vs Asimétrica**
Antisimétrica permite $(a,a)$.
Asimétrica lo prohíbe.

**Equivalencia vs Orden Parcial**
Equivalencia $\rightarrow$ simétrica
Orden parcial $\rightarrow$ antisimétrica

Son estructuras distintas.
### CRITERIO PRÁCTICO PARA CONJUNTOS FINITOS
Reflexiva $\Leftrightarrow$ todos los pares $(a,a)$ están.
Simétrica $\Leftrightarrow$ si $(a,b)$ está, entonces $(b,a)$ también.
Antisimétrica $\Leftrightarrow$ no existen $(a,b)$ y $(b,a)$ con $a \ne b.$
Asimétrica $\Leftrightarrow$ no existen pares diagonales ni pares cruzados.
Transitiva $\Leftrightarrow$ si $(a,b)$ y $(b,c)$ están, debe estar $(a,c).$