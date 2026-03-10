### FUNCIÓN EXPONENCIAL
Sea $a \in \mathbb{R}$ tal que $a>0 \land a \neq 1$.

Se define la función exponencial de base $a$ como: $$f:\mathbb{R} \rightarrow \mathbb{R}^+/f(x)=a^x$$
Condiciones fundamentales:
- $a>0$ (para que la potencia esté definida en $\mathbb{R}$)
- $a \ne 1$ (porque si $a=1$, la función sería constante)

Propiedades básicas:
1. $a^0=1$
2. $a^1=a$
3. $a^x \cdot a^y=a^{x+y}$
4. $\frac{a^x}{a^y}=a^{x-y}$
5. $(a^x)^r=a^{x \cdot y}$

Dominio: $\mathbb{R}$
Imagen: $\mathbb{R}^+=(0,\infty)$

Observación importante: $$a^x>0,\forall x\in \mathbb{R}$$
Si:
- $a>1 \Rightarrow$ la función es creciente.
- $0 < a < 1 \Rightarrow$ la función es decreciente.
### DEFINICIÓN FORMAL DE LOGARITMO
Sea $a>0,a \neq 1$.

Se define el logaritmo en base $a$ como la función inversa de la exponencial: $$\log_{a}:\mathbb{R}^+ \rightarrow \mathbb{R}$$
Definición formal: $$\log_{a}(x)=y \Leftrightarrow a^y=x$$
Es decir: $$\log_{a}(x) \text{ es el único número real y tal que }a^y=x$$
Condición fundamental: $$x>0$$
Porque la función exponencial sólo toma valores positivos.

Dominio: $\mathbb{R}^+$
Imagen: $\mathbb{R}$
### EXPONENCIAL Y LOGARITMO SON INVERSAS
Por definición de función inversa: $$a^{\log_{a}(x)}=x, \forall x>0$$
$$\log_{a}(a^x)=x, \forall x \in \mathbb{R}$$
Justificación formal:
Si $$y=\log_{a}(x)$$
por definición: $$a^y=x$$
luego $$a^{\log_{a}(x)}=x$$
Y recíprocamente, si $$x=a^t$$
entonces $$\log_{a}(x)=\log_{a}(a^t)=t$$
Esto es exactamente la definición de funciones inversas.
### PROPIEDADES DEL LOGARITMO
Todas se demuestran usando propiedades de potencias.

Sea $a>0,a \neq 1,x>0,y>0$.

###### Producto
$$\log_{a}(xy)=\log_{a}(x)+\log_{a}(y)$$
Demostración:
Sea 
$$\log_{a}x=m \Rightarrow a^m=x$$$$\log_{a}y=n \Rightarrow a^n=y$$
Entonces: $$xy=a^m \cdot a^n=a^{m+n}$$
Por definición de logaritmo: $$\log_{a}(xy)=m+n$$
$$= \log_{a}x+\log_{a}y$$
###### Cociente
$$\log_{a}(\frac{x}{y})=\log_{a}x-\log_{a}y$$
Demostración:
$$\frac{x}{y}=\frac{a^m}{a^n}=a^{m-n}$$
Luego: $$\log_{a}(\frac{x}{y})=m-n$$
###### Potencia
$$\log_{a}(x^r)=r \cdot \log_{a}x$$
Demostración: $$x=a^m \Rightarrow x^r=(a^m)^r=a^{m \cdot r}$$
Luego: $$\log_{a}(x^r)=m \cdot r=r \cdot \log_{a}x$$
### CONDICIONES FUNDAMENTALES
Nunca olvidar escribir: $a>0 \land a \neq {1}$, $x>0$
Si no se colocan estas condiciones en una demostración formal, está incompleta.
### PROPIEDADES IMPORTANTES
###### Cambio de base
$$\log_{a}x=\frac{\log_{b}x}{\log_{b}a}$$
###### Logaritmo de 1
$$\log_{a}1=0, \text{ por que }a^0=1$$
###### Logaritmo de la base
$$\log_{a}a=1$$