##### Definición formal
Para todo $x \in R$,
$|x|=x,\text{si } x\geq 0$
$|x|=-x,\text{si } x < 0$

**Toda demostración debe apoyarse en esta definición** y dividir en casos cuando sea necesario.
###### Propiedad básica de acotación
Para todo $x \in R$ se cumple: $-|x| \leq x \leq |x|$

**Demostración por casos**
- **Caso 1:** $x\geq 0$
Entonces $|x|=x$.
Luego $-x \leq x \leq x$, lo cuál es verdadero.
- **Caso 2:** $x<0$
Entonces $|x|=-x$.
Luego $-(-x) \leq x \leq -x$
Es decir $x \leq x \leq -x$, lo cuál es verdadero porque $x<0$ implica $x\leq -x$.
**Conclusión:** $-|x| \leq x \leq |x|,\forall x \in R.$
##### Demostraciones
###### 1. $|a-b|=|b-a|$
Observamos que: $b-a=-(a-b)$.
Entonces debemos probar: $|x|=|-x|$ para todo $x \in R$.

**Demostración por casos**

**Caso 1:** $x\geq 0$.
Entonces $|x|=x$.
Como $x\geq 0 \Rightarrow -x \leq 0$.
Si $x>0$, entonces $-x<0$ y: $|-x|=-(-x)=x$.
Si $x=0$, trivialmente $|0|=0$ y $|-0|=0$.
Luego $|x|=|-x|$.

**Caso 2:** $x<0$.
Entonces $|x|=-x$.
Ahora $-x>0$ por lo tanto: $|-x|=-x$.
Luego nuevamente $|x|=|-x|$.

**Conclusión:** $|a-b|=|-(a-b)|=|b-a|$.

###### 2. $\sqrt{x^2}=|x|$
**Demostración formal:**

**Caso 1:** $x \geq 0$
Entonces $|x|=x$.
Como $x \geq 0$, se cumple: $\sqrt{x^2}=x$.
Luego $\sqrt{ x^2 }=|x|$.

**Caso 2:** $x < 0$
Entonces $|x|=-x$.
Pero si $x<0 \Rightarrow -x>0$.
Notamos que $x^2=(-x)^2$.
Entonces: $\sqrt{ x^2 }=\sqrt{ (-x)^2 }=-x$.
Pero $-x=|x|$.

**Conclusión:** $\sqrt{ x^2 }=|x|,\forall x \in R$.

###### 3. Propiedad del producto: $|ab|=|a||b|$
**Demostración por análisis de signos**
Se estudian cuatro casos:

1. $a \geq 0$ y $b \geq 0$
Se tiene $|a|=a \land |b|=b$.
Y $ab \geq 0 \Rightarrow |ab|=ab$.
Luego $|ab|=ab=|a||b|$.

2. $a \geq 0$ y $b<0$
Tenemos entonces que $|a|=a \land |b|=-b$.
Y $ab<0 \Rightarrow |ab|=-ab$.
Pero $|a||b|=a(-b)=-ab$.
Luego $|ab|=|a||b|$.

3. $a<0$ y $b \geq 0$
Tenemos: $|a|=-a \land |b|=b$.
Y $ab<0 \Rightarrow |ab|=-ab$.
Pero $|a||b|=(-a)b=-ab$.
Luego $|ab|=|a||b|$.

4. $a<0$ y $b<0$
Tenemos: $|a|=-a \land |b|=-b$.
Y $ab>0 \Rightarrow |ab|=ab$.
Por otro lado $|a||b|=(-a)(-b)=ab$.
Luego $|ab|=|a||b|$.

**Conclusión:** $|ab|=|a||b|$.
###### 4. Desigualdad triangular: $|a+b|\leq|a|+|b|$
Sabemos por definición
$-|a| \leq a \leq |a|$
$-|b| \leq b \leq |b|$

Sumando miembro a miembro: $-|a|-|b| \leq a+b \leq |a|+|b|$
Agrupando: $-(|a|+|b|) \leq a+b \leq |a|+|b|$

**Proposición:** Si $-k \leq x \leq k$ con $k \geq 0 \Rightarrow |x| \leq k$.

Aquí $k=|a|+|b| \geq 0$

Luego: $|a+b| \leq |a|+|b|$.
###### 5. Desigualdad triangular inversa: $||a|-|b||\leq|a-b|$
**Demostración**
Por desigualdad triangular: $|a|=|(a-b)+b|\leq|a-b|+|b|$
Luego: $|a|-|b| \leq |a-b|$ (1).
Intercambiando $a$ y $b$: $|b|=|(b-a)+a|\leq|b-a|+|a|$.
Pero $|b-a|=|a-b|$.
Luego: $|b|-|a|\leq|a-b|$ (2).
De (1) y (2) se obtiene: $-|a-b|\leq|a|-|b|\leq|a-b|$.
Por definición de valor absoluto: $||a|-|b||\leq|a-b|.$
##### Como trabajar correctamente por casos
Cuando aparece $|f(x)|$:
1. Determinar los valores críticos donde $f(x)=0$.
2. Dividir $R$ en intervalos.
3. En cada intervalo reemplazar usando la definición.
4. Resolver la ecuación o desigualdad obtenida.
5. Verificar que las soluciones pertenezcan al intervalo analizado.

**Ejercicio: Resolver $|2x-3|+|x+1|=5$.**

Valores críticos:
$2x-3=0 \Rightarrow x=\frac{3}{2}$.
$x+1=0 \Rightarrow x=-1$.

Dividir $R$ en: $I_{1}=(-\infty,-1)$,$I_{2}=[-1,\frac{3}{2})$, $I_{3}=[\frac{3}{2},\infty)$

- Caso $I_{1}:x<-1$
En este intervalo
$x+1<0 \Rightarrow |x+1|=-(x+1)$.
$2x-3<0$ (porque $x<-1<\frac{3}{2}$) $\Rightarrow |2x-3|=-(2x-3)$

La ecuación queda:
$-(2x-3)-(x+1)=5$
$-2x+3-x-1=5$
$-3x+2=5$
$-3x=3$
$x=-1$
Pero $x=-1 \not\in (-\infty,-1)$.
No hay solución en $I_{1}$.

- Caso $I_{2}:-1 \leq x < \frac{3}{2}$
Aquí
$x+1 \geq 0 \Rightarrow |x+1|=x+1$
$2x-3<0 \Rightarrow |2x-3|=-(2x-3)$

La ecuación:
$-(2x-3)+(x+1)=5$
$-2x+3+x+1=5$
$-x+4=5$
$-x=1$
$x=-1$
Verificación: $-1 \in [-1,\frac{3}{2})$.
Solución válida.

- Caso $I_{3}: x \geq \frac{3}{2}$
En este intervalo
$x+1 \geq 0 \Rightarrow |x+1|=x+1$
$2x-3 \geq 0 \Rightarrow |2x-3|=2x-3$

La ecuación:
$(2x-3)+(x+1)=5$
$3x-2=5$
$3x=7$
$x=\frac{7}{3}$
Verificación: $\frac{7}{3}>\frac{3}{2}$.
Solución válida.

Conclusión
El conjunto solución es: $S=$ {$-1,\frac{7}{3}$}.
##### Caracterización de desigualdades con valor Absoluto
Sea $a\geq0$.
1. $|x|\leq a \Leftrightarrow -a\leq x \leq a$
2. $|x|<a \Leftrightarrow -a<x<a$
3. $|x|\geq a \Leftrightarrow x\leq-a \lor x\geq a$
4. $|x|>a \Leftrightarrow x < -a \lor x>a$

Caso especial
Si $a<0$.
$|x|\leq a$ no tiene solución porque $|x|\geq 0$ para todo $x \in R$.

Ejercicio de ejemplo, resolver $|2x-1|\leq 3.$
Solución:
$|2x-1|\leq 3 \Leftrightarrow -3 \leq 2x-1 \leq 3$
$\Leftrightarrow -2\leq 2x \leq 4 \Leftrightarrow -1\leq x \leq 2.$
Conjunto solución: $S=[-1,2].$
