##### Definición
Una ecuación cuadrática en $R$ es: $ax^2+bx+c=0$, con $a,b,c \in R$ y $a \neq 0$.
- a = coeficiente cuadrático
- b = coeficiente lineal
- c = término independiente
##### Deducción por completar cuadrados
Partimos de: $$ax^2+bx+c=0 \text{, con } a \neq 0$$
1. Pasamos $c$ al segundo miembro: $$ax^2+bx=-c$$
2. Dividimos por $a$: $$x^2+(\frac{b}{a})x=\frac{-c}{a}$$
3. Sumamos el cuadrado de la mitad del coeficiente lineal:
La mitad de $\frac{b}{a}$ es $\frac{\frac{b}{a}}{2}=\frac{b}{2a}$.
Sumamos $(\frac{b}{2a})^2$ en ambos miembros.
$$x^2+(\frac{b}{a})x+(\frac{b}{2a})^2=\frac{-c}{a}+(\frac{b}{2a})^2$$
4. El primer miembro es un Trinomio Cuadrado Perfecto: $$(x+\frac{b}{2a})^2=\frac{b^2}{4a^2}-\frac{c}{a}$$
5. Llevamos a común denominador: $$(x+\frac{b}{2a})^2=\frac{(b^2-4ac)}{4a^2}$$
6. Aplicamos raíz cuadrada[^1]: $$|x+\frac{b}{2a}|=\frac{\sqrt{b^2-4ac}}{2|a|}$$
7. Despejando $x$: $$x=\frac{-b \pm \sqrt{ b^2-4ac }}{2a}$$
Esta es la fórmula general.
##### Discriminante
Se define: $\triangle=b^2-4ac$
Es la expresión bajo la raíz.

Naturaleza de las raíces:
- Si $\triangle>0$
$\sqrt{ \triangle }$ es real positivo.
Dos soluciones reales distintas.
- Si $\triangle=0$
$\sqrt{ \triangle }=0$.
Una única solución real (raíz doble).
- Si $\triangle < 0$
No existe $\sqrt{ \triangle }$ en $R$.
No hay solución real.

Esto sale directamente de la fórmula.

##### Observación sobre el coeficiente principal 
El signo de $a$ no modifica la naturaleza de las raíces (eso depende solo de $\triangle$).
Pero sí influye en:
- El signo de $-\frac{b}{a}$
- El signo de $\frac{c}{a}$
- El comportamiento gráfico (concavidad de la parábola)
Si $a>0$, la parábola abre hacia arriba.
Si $a<0$, la parábola abre hacía abajo.
##### Forma normalizada
Dividiendo por $a \neq 0$: $x^2+\frac{b}{a}x+\frac{c}{a}=0.$
En esta forma:
Suma de raíces = $-$coeficiente de x
Producto de raíces = término independiente
##### Relaciones entre raíces
Si $x_{1}$ y $x_{2}$ son soluciones de: $ax^2+bx+c=0$
Entonces:
$x_{1}+x_{2}=\frac{-b}{a}$
$x_{1}\cdot x_{2}=\frac{c}{a}$

Demostración: Se obtiene sumando y multiplicando las expresiones de la fórmula general.

Consecuencia importante, la forma factorizada es: $a(x-x_{1})(x-x_{2})=0$.

- Sea $ax^2+bx+c=0$, con $a \neq 0$ y sean $r_{1},r_{2} \in R$ sus raíces.
###### Identidad entre discriminante y diferencia de raíces
Identidad útil: $(r_{1}-r_{2})^2=(r_{1}+r_{2})^2-4r_{1}r_{2}$
Sustituyendo las relaciones: $(r_{1}-r_{2})^2=(-\frac{b}{a})^2-4\frac{c}{a}$
$= \frac{b^2}{a^2}-4\frac{c}{a}$
$=\frac{b^2-4ac}{a^2}$
Por lo tanto: $(r_{1}-r_{2})^2=\frac{\triangle}{a^2}$
Consecuencia: $|r_{1}-r_{2}|=\frac{\sqrt{ \triangle }}{|a|}$
###### Demostración formal desde factorización
Si $r_{1},r_{2}$ son raíces, entonces: $a(x-r_{1})(x-r_{2})=0$.
Desarrollamos: $a[x^2-(r_{1}+r_{2})x+r_{1}r_{2}]=0$.
Distribuyendo: $ax^2-a(r_{1}+r_{2})x+ar_{1}r_{2}=0$.
Comparando coeficiente con: $ax^2+bx+c=0$.
Obtenemos: $-a(r_{1}+r_{2})=b$ y $ar_{1}r_{2}=c$.
Dividiendo por $a$: $r_{1}+r_{2}=-\frac{b}{a}$ y $r_{1}r_{2}=\frac{c}{a}$.
###### Recíproco
Si conocemos S y P tales que:
$r_{1}+r_{2}=S$
$r_{1}r_{2}=P$

Entonces la ecuación cuyas raíces son $r_{1}$ y $r_{2}$ es: $x^2-Sx+P=0$.
Y si el coeficiente principal no es 1: $a(x^2-Sx+P)=0$.
###### Casos
1. Raíces opuestas
Si $r_{1}=-r_{2}$
$\Rightarrow r_{1}+r_{2}=0 \Rightarrow -\frac{b}{a}=0 \Rightarrow b=0.$
Conclusión: La ecuación tiene raíces opuestas $\Leftrightarrow b=0$.
2. Raíces reciprocas
Si $r_{2}=\frac{1}{r_{1}}$
Entonces: $r_{2}r_{1}=1 \Rightarrow \frac{c}{a}=1 \Rightarrow c=a.$
Condición necesaria y suficiente: $c=a$.
3. Raíces iguales (raíz doble)
Si $r_{1}=r_{2}$
Entonces: $\triangle=0$
Y además: $r_{1}=r_{2}=-\frac{b}{2a}$.
###### Signos de las raíces
Sin calcular las raíces explícitamente se puede deducir:
- Si $r_{1}r_{2}>0 \rightarrow$ las raíces tienen el mismo signo.
- Si $r_{1}r_{2}<0 \rightarrow$ tienen signos opuestos.

Y usando la suma:
- Si $r_{1}r_{2}>0$ y $r_{1}+r_{2}>0 \rightarrow$ ambas positivas.
- Si $r_{1}r_{2}>0$ y $r_{1}+r_{2}<0 \rightarrow$ ambas negativas.

Para que ambas raíces sean reales y positivas:
1. $\triangle\geq0$
2. $r_{1}r_{2}>0$
3. $r_{1}+r_{2}>0$

Para que ambas raíces sean reales y negativas:
1. $\triangle\geq 0$
2. $r_{1}r_{2}>0$
3. $r_{1}+r_{2}<0$
##### Aplicaciones frecuentes
1. Si $c=a$
Entonces: $x_{1} \cdot x_{2}=\frac{c}{a}=\frac{a}{a}=1$.
Por lo tanto: $x_{1} \cdot x_{2}=1$.
Eso significa que una raíz es el recíproco de la otra.
2. Condición para solución única
La ecuación tiene solución única $\Leftrightarrow \triangle=0$.
Es decir: $b^2-4ac=0$.
3. Condición para que tenga dos soluciones reales
$b^2-4ac>0$
4. Condición para que no tenga solución real
$b^2-4ac<0$
##### Análisis con parámetro
Puede aparecer: $ax^2+bx+c(k)=0$, o coeficientes que dependen de $k$, que miedoo.
Se procede así:
1. Calcular $\triangle(k)$
2. Analizar el signo de $\triangle(k)$
3. Resolver la desigualdad correspondiente
Ejemplo: Determinar $k$ para que la ecuación tenga solución única.
Se impone $\triangle=0$ y se resuelve en $k$.

[^1]: **Observación**
	El valor absoluto aparece porque: $\sqrt{ 4a^2 }=2|a|$
	Luego, al despejar $x$, el valor absoluto se elimina introduciendo el símbolo $\pm$: $x+\frac{b}{2a}=\pm \frac{\sqrt{ b^2-4ac }}{2a}$
	Es decir, el $\pm$ "absorbe" el efecto del valor absoluto.
