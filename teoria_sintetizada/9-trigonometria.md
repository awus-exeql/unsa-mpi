La trigonometría estudia relaciones entre ángulos y longitudes. En esta materia trabajamos en $\mathbb{R}$, interpretando las funciones trigonométricas como funciones reales de variable real.

Tomamos como conjunto universal $\mathbb{R}$.
### DEFINICIÓN GEOMÉTRICA DE SENO Y COSENO
Existen dos enfoques clásicos: triángulo rectángulo y circunferencia unitaria. En la cátedra se adopta la definición mediante circunferencia unitaria porque permite extender las funciones a todo $\mathbb{R}$.

Sea la circunferencia unitaria: $$\mathrm{C}=\{ (x,y) \in \mathbb{R}^2:x^2+y^2=1 \}$$
Sea $\theta \in \mathbb{R}$ un ángulo medido en radianes desde el eje positivo x.

Definición.
Sea $\text{P}=(x,y)$ el punto de intersección entre el lado terminal del ángulo $\theta$ y la circunferencia unitaria.

Definimos: $\sin(\theta)=y$ y $\cos(\theta)=x$

Es decir: $\forall x\in \mathbb{R}$
$\cos(\theta)=$ abscisa del punto correspondiente
$\sin(\theta)=$ ordenada del punto correspondiente

Como el punto pertenece a la circunferencia unitaria, se cumple: $x^2+y^2=1$
Luego: $\cos^2(\theta)+\sin^2(\theta)=1$ (identidad trigonométrica fundamental)
###### Interpretación en triángulo rectángulo
Si $\theta$ es un ángulo agudo de un triángulo rectángulo, entonces:
$\sin(\theta)= \frac{\text{cateto opuesto}}{\text{hipotenusa}}$
$\cos(\theta)= \frac{\text{cateto adyacente}}{\text{hipotenusa}}$

Esta definición es equivalente a la anterior cuando $0< \theta < \frac{\pi}{2}$.
### TANGENTE Y SU DOMINIO
Definición.
Para todo $\theta \in \mathbb{R}$ tal que $\cos(\theta) \ne 0$ definimos: $$\tan(\theta)=\frac{\sin(\theta)}{\cos(\theta)}$$
Luego el dominio de la tangente es: $$\mathrm{Dom}(\tan)=\{ \theta \in \mathbb{R}: \cos(\theta) \ne 0 \}$$
Sabemos que: $\cos(\theta)=0 \Leftrightarrow \theta=(\frac{\pi}{2}+k \cdot \pi) \text{, con }k \in \mathbb{R}$
Por lo tanto: $$\mathrm{Dom}(\tan)=\mathbb{R}-\{ \frac{\pi}{2}+k \cdot \pi:k \in \mathbb{R} \}$$
### AMPLITUD, PERÍODO Y FASE DE $A \cdot \sin(Bx+C)$
Consideramos la función: $f(x)=A \cdot \sin(Bx+C)$, con $A,B,C \in \mathbb{R}$ y $B \ne 0$.
#### Definiciones formales:
###### Amplitud
La amplitud es: $|A|$ 

Justificación: Como $-1 \leq \sin(\theta) \leq 1$, entonces $-|A| \leq A \cdot \sin(\theta) \leq |A|$

Luego la imagen de la función está contenida en: $[-|A|,|A|]$
###### Período
Sabemos que: $\sin(x+2\pi)=\sin(x)$

Buscamos $\mathrm{T}$ tal que: $\sin(B(x+\mathrm{T})+C)=\sin(Bx+C)$

Esto ocurre cuando: $B(x+\mathrm{T})+C=Bx+C+2\pi$
$\Rightarrow B\mathrm{T}=2\pi$
$\Rightarrow \mathrm{T}=\frac{2\pi}{|B|}$

Por lo tanto: Período $= \frac{2\pi}{|B|}$
### Fase (desplazamiento horizontal)
La expresión: $Bx+C=B(x+\frac{C}{B})$

Entonces: $A \cdot \sin(Bx+C)=A \cdot \sin(B(x+\frac{C}{B}))$

El desplazamiento horizontal es: $-\frac{C}{B}$

Se interpreta como un corrimiento:
- Hacia la izquierda si $\frac{C}{B}>0$
- Hacia la derecha si $\frac{C}{B} < 0$
### IDENTIDADES BÁSICAS
###### Identidad fundamental:
$$\sin^2(x)+\cos^2(x)=1$$
Se deduce directamente de la ecuación de la circunferencia unitaria.
###### Identidades derivadas importantes
1. $1+\tan^2(x)=\frac{1}{\cos^2(x)}$
Demostración:
$\tan(x)=\frac{\sin(x)}{\cos(x)}$
$\tan^2(x)=\frac{\sin^2(x)}{\cos^2(x)}$
Entonces: $1+\tan^2(x)$
$= 1+\frac{\sin^2(x)}{\cos^2(x)}$
$=\frac{\cos^2(x)}{\cos^2(x)}+\frac{\sin^2(x)}{\cos^2(x)}$
$=\frac{\cos^2(x)+\sin^2(x)}{\cos^2(x)}$
$=\frac{1}{\cos^2(x)}$

2. $\cos^2(x)=1-\sin^2(x)$
3. $\sin^2(x)=1-\cos^2(x)$
### PERIODICIDAD
$$\sin(x+2\pi)=\sin(x)$$
$$\cos(x+2\pi)=\cos(x)$$
Luego ambas funciones son periódicas de período $2\pi$.

$$\tan(x+\pi)=\tan(x)$$
Luego la tangente es periódica de período $\pi$.
