### DEFINICIONES FORMALES
###### Definición de función
Sean $A$ y $B$ conjuntos.

Una función $f:A\rightarrow B$ es una relación que a cada elemento $x\in A$ le asigna **un único** elemento $y\in B$.

Se escribe: $$f:A \rightarrow B,\text{ }y=f(x)$$
Condición esencial: $$\forall x\in A,\exists! y\in B \text{ tal que } y=f(x).$$
El símbolo $\exists!$ significa "existe único".
###### Dominio
El dominio de $f$, denotado $\mathrm{Dom}(f)$, es el conjunto de partida $A$.
###### Imagen
La imagen de $f$, denotada $\mathrm{Im}(f)$, es: $$\mathrm{Im}(f)=\{ f(x)\in B:x \in A\}$$
O sea, el subconjunto de $B$ que realmente es alcanzado.
###### Función inyectiva
$f:A \rightarrow B$ es inyectiva si: $$\forall x_{1},x_{2}\in A:f(x_{1})=f(x_{2})\Rightarrow x_{1}=x_{2}$$
Equivalente: $$x_{1}\ne x_{2} \Rightarrow f(x_{1})\ne f(x_{2})$$
###### Función sobreyectiva
$f:A \rightarrow B$ es sobreyectiva si: $$\forall y\in B,\exists x \in A: f(x)=y$$
Es decir: $$\mathrm{Im}(f)=B$$
**Observación:** La sobreyectividad depende del codominio declarado.
Ejemplo: $f(x)=x^2$
- No es sobreyectiva si $f:\mathbb{R} \rightarrow \mathbb{R}$
- Si es sobreyectiva si $f:\mathbb{R} \rightarrow [0,\infty)$
###### Función biyectiva
Es inyectiva y sobreyectiva simultáneamente.
###### Función inversa
Si $f:A \rightarrow B$ es biyectiva, entonces existe una función $$f^{-1}:B \rightarrow A$$
tal que: $$f^{-1}(f(x))=x$$ $$f(f^{-1}(y))=y$$
###### Procedimiento para hallar la inversa
Sea $f:A \rightarrow B$ biyectiva
1. Escribir $y=f(x)$
2. Intercambiar $x \leftrightarrow y$
3. Despejar $y$
4. Verificar dominio e imagen

Aclarar:
$\mathrm{Dom}(f^{-1})=\mathrm{Im}(f)$
$\mathrm{Im}(f^{-1})=\mathrm{Dom}(f)$
###### Función compuesta
Sean $f:A \rightarrow B$ y $g:B \rightarrow C$.
La composición es: $$g\circ f:A \rightarrow C$$
definida por: $$(g \circ f)(x)=g(f(x))$$
La composición $g \circ f$ está bien definida si y solo si: $\mathrm{Im}(f)\subseteq \mathrm{Dom}(g)$

Dominio de la composición: $\mathrm{Dom}(g \circ f)=\{ x \in \mathrm{Dom}(f):f(x)\in \mathrm{Dom}(g) \}$

###### Función cociente
Si $f$ y $g$ son funciones con mismo dominio y $g(x) \neq 0$ para todo $x$, entonces: $$(\frac{f}{g})(x)=\frac{f(x)}{g(x)}$$
Dominio: $$\mathrm{Dom}(\frac{f}{g})=\{ x\in \mathrm{Dom}(f) \cap \mathrm{Dom}(g):g(x)\ne 0 \}$$
### DEMOSTRACIONES
###### Demostración 1
Si $f$ y $g$ son inyectivas $\Rightarrow$ $g \circ f$ es inyectiva.

Sea $(g \circ f)(x_{1})=(g \circ f)(x_{2})$

Entonces: $$g(f(x_{1}))=g(f(x_{2}))$$
Como $g$ es inyectiva: $$f(x_{1})=f(x_{2})$$
Como $f$ es inyectiva: $$x_{1}=x_{2}$$
Por lo tanto: $$g \circ f \text{ es inyectiva.}$$
###### Demostración 2
Función lineal con $m \neq 0$ es biyectiva.

Sea: $$f(x)=mx+b$$
**Inyectividad**

Supongamos: $$f(x_{1})=f(x_{2})$$
Entonces: $$mx_{1}+b=mx_{2+b}$$
Restando $b$: $$mx_{1}=mx_{2}$$
Como $m\ne 0$: $$x_{1}=x_{2}$$
Luego es inyectiva.

**Sobreyectividad**

Sea $y \in \mathbb{R}$.
Buscamos $x$ tal que: $$y=mx+b$$
Entonces: $$x=\frac{y-b}{m}$$
Como existe para todo $y$, es sobreyectiva.

Luego es biyectiva.
###### Restricción para que exista inversa
Una función tiene inversa si y solo si es biyectiva.

Si no es inyectiva, no se puede definir una inversa funcional porque un mismo valor tendría dos preimágenes.

Ejemplo:
$f(x)=x^2$ en $\mathbb{R}$ no es inyectiva.
Pero si se restringe a: $$f:[0,\infty) \rightarrow [0,\infty]$$
entonces sí es inyectiva y admite inversa $\sqrt{ x }$.
###### Demostración: una cuadrática no es inyectiva
Sea $f(x)=ax^2+bx+c$ con $a \neq 0$
Sea $h=-\frac{b}{2a}$
Sea $t \neq 0$

Definimos:
$x_{1}=h+t$
$x_{2}=h-t$

Entonces $x_{1} \neq x_{2}$
Y: $f(x_{1})=f(x_{2})$

Luego $f$ no es inyectiva en $\mathbb{R}$.
### DOMINIO
###### Dominio de una función racional
Si: $$f(x)=\frac{P(x)}{Q(x)}$$
Entonces: $$\mathrm{Dom}(f)=\{ x\in \mathbb{R}: Q(x)\ne 0 \}$$
Nunca puede anularse el denominador.
###### Dominio de $\log(x-k)$
El argumento debe ser positivo: $$x-k>0$$$$x>k$$
Dominio: $$(k,\infty)$$
###### Dominio de $\tan(x)$
$$\tan(x)=\frac{\sin(x)}{\cos(x)}$$
Debe cumplirse: $$\cos(x) \neq 0$$
Sabemos que: $$\cos(x)=0 \Leftrightarrow x=\frac{\pi}{2}+k\pi$$
Por lo tanto: $$\mathrm{Dom}(\tan)=\mathbb{R}-\{ \frac{\pi}{2}+k\pi:k \in \mathbb{Z} \}$$
###### Dominio de raíz
Si $f(x)=\sqrt{ g(x) }$, entonces:

$\mathrm{Dom}(f)=\{ x \in \mathbb{R}:g(x) \geq 0 \}$.
###### Dominio combinado
Si $f(x)=\sqrt{ \frac{P(x)}{Q(x)} }$, entonces:

1. $Q(x) \neq 0$
2. $\frac{P(x)}{Q(x)} \geq 0$

Debe resolverse sistema de condiciones.
### CASOS TÍPICOS
###### Función constante
Sea $f(x)=c$.
- No es inyectiva si $\mathrm{Dom}(f)$ tiene más de un elemento.
- Es sobreyectiva $\Leftrightarrow$ el codominio es {$c$}.
###### Función valor absoluto
Sea $f(x)=|x|$.

No es inyectiva en $\mathbb{R}$ porque: $|a|=|-a|$ con $a \neq 0$.
Pero es inyectiva si se restringe a $[0,\infty)$.
