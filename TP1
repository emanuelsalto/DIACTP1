# Trabajo práctico 1

**Ejercicio 1.-**
$\hspace{2mm}$Se conoce la PDE que describe la estática de una barra particular cuya rigidez axial y fuerzas aplicadas son conocidas.

$$\ u''(x)+1=0\ ,\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }\text{  }   x ∈ [0; 1]$$

 **a.** $\hspace{2mm}$*Cálculo de la solución exacta:* 
 
$$\frac{d}{dx}u'(x)+1=0$$

$$\int du'(x)=-\int dx$$
$$u'(x)=-x +\Bbb C_1 \text{ } \text{ } \text{ } \Rightarrow\text{ }\text{ }\text{ }\text{ Deformación}$$
$$\frac {du(x)}{dx}=-x+\Bbb C_1$$

$$\int du=-\int xdx + \int \Bbb C_1 dx$$
$$u(x)=-\frac {x^2}{2} + \Bbb C_1 x+ \Bbb C_2\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }\text{ Desplazamiento}$$


- Aplicando las condiciones de borde:

$$1=-1+\Bbb C_1\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }\Bbb C_1=2$$
$$0=0+2\cdot 0+\Bbb C_2 \text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text { }\Bbb C_2 =0$$

- Quedando entonces:

$$u(x)= -\frac {x^2}{2} + 2x\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{y}\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\varepsilon=u'(x)=2-x$$

**b.** $\hspace{2mm}$*Analizando un elemento diferencial de barra:*
 
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1thnNfozgsrJnn2Cu2uyAJId42P8olrqt" alt="Sumatoria de fuerzas sobre elemento diferencial de barra - CTM">
</p>


$$\left( \sigma+  \frac{ \partial \sigma}{\partial x}dx\right)A+\rho bA \text{ }dx - \sigma A= 0 \text{ }\text{ }\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }\text{ }\text{ }\sigma' + \rho b = 0$$

$$\sigma = E\varepsilon = E\frac{ du}{dx}\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }\sigma =E(2-x)   $$

$$\sigma' = \frac{d2E}{dx}-E\frac{dx}{dx}\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }\sigma' =-E$$
$$\therefore -E + \rho b = 0\text{ }\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }\text{ }E=\rho b$$

También tenemos que: 
$$\sigma(x)=\frac{F(x)}{A}=E\frac{du(x)}{dx} \text{ }\text{ }$$ 

- Aplicando nuevamente las condiciones de borde:

$\hspace{5mm}$  En  $x =0$

$$-E\frac{du(0)}{dx}=\frac{F_1}{A}\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }-E\cdot2=\frac{F_1}{A}\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }F_1=-2EA$$

$\hspace{5mm}$  En  $x =1$


$$\text{ }\text{ }\text{ }E\frac{du(1)}{dx}=\frac{F_2}{A}\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }E\cdot1=\frac{F_2}{A}\text{ }\text{ }\text{ }\Rightarrow\text{ }\text{ }\text{ }F_2=EA$$





**c.** $\hspace{2mm}$*Cálculo del error*
- Solución exacta:
$$u(L/2)=-\left(\frac{1}{2}\right)^2\cdot\frac{1}{2}+2\cdot\frac{1}{2}$$

$$u(L/2)=-\frac{1}{8}+1$$

$$u(L/2)=\frac{3}{8}=0,875$$

- Solución aproximada:

$\hspace{2mm}$La solución aproximada se obtiene al realizar una interpolación lineal a partir de conocer los desplazamientos en los nodos.
$\hspace{2mm}$Para un punto cualquiera de la barra, la expresión para el desplazamiento axial es:
$$u=N \mathbf u$$

$$
u=\begin{bmatrix}\frac{L-x}{L} & \frac{x}{L}\end{bmatrix} \begin{Bmatrix}u_1\\u_2\end{Bmatrix}
$$
$\hspace{2mm}$Donde $N$ es una matriz conformada por las funciones de forma que, en este caso, seran dos. Cada función $N_i$ describe como $u$ varía con $x$ cuando el correspondiente grado de libertad $u_i$ vale uno, mientras el otro vale cero.

Aplicando las condiciones de borde, tenemos que:
$$
u(x)=\begin{bmatrix}\frac{L-x}{L} & \frac{x}{L}\end{bmatrix} \begin{Bmatrix}0\\\frac{3}{2}\end{Bmatrix}
$$

$$
\therefore \text{ }\text{ }\text{ }\text{ }u(x)=\frac{3}{2}\frac{x}{L} \text{ }\text{ }\text{ }\text{ }\text{ con }\text{ }\text{ }\text{ }L=1 
$$

Quedando entonces:
$$ u(L/2)=\frac{3}{2}\cdot\frac{1}{2}= 0,75$$

- Cálculo del error:

$$ \text{error}= \frac{0,875-0,75}{0,875}\approx 0,14=14\%$$


****
**Ejercicio 2.-**


$$K=\frac{AE}{L}\begin{pmatrix}1 & -1\\-1 & 1\end{pmatrix} \text{ }\text{ }\text{ }\text{ }\text{ }\text{ }\Bbb u=\begin{pmatrix}u_1\\u_2 \end{pmatrix}\text{ }\text{ }\text{ }\text{ }\text{ }\text{ }F=\begin{pmatrix}F_1\\F_2 \end{pmatrix}$$
$$Ku=F$$
**a.** 
- Cálculo del rango de $K$

$$rank(K)=1\text{ }\text{ }\text{ }\rightarrow\text{ }\text{ }\text{ }\text{ya que solo hay una fila linealmente independiente.}$$


- Cálculo del rango de $(K|F)$

$$\frac{AE}{L}\left(
\begin{array}{cc|c}
  1&-1&F_1\\
  -1&1&F_2
\end{array}
\right) \Rightarrow \text{ } \frac{AE}{L}\left(\begin{array}{cc|c} 1&-1&F_1\\
  0&0&F_2+F_1\end{array}
\right)
$$
$$rank(K|F)=2\text{ }\text{ }\text{ }\rightarrow\text{ }\text{ }\text{ }\text{las dos filas son linealmente independientes}$$

$\hspace{2mm}$El rango de la matriz representa los modos de deformación de cuerpo deformable, es decir, los que acumulan energía.
$\hspace{2mm}$Al tener $K$ y $K|F$ distinto rango, el sistema no tendrá solución.

**b.**
El sistema tendrá solución si:

 1.  $F_1=-F_2=F$
 2.  $u_1-u_2=\frac{F}{k}\text{ }\text{ }\text{ }\text{ }\text{ Donde}\text{ }\text{ }\text{ }\text{ }\text{ } k=\frac{AE}{L}$

$\hspace{4mm}\therefore u_1=u_2+\frac{F}{k}$

**c.**$\hspace{2mm}$ *Solución general para un sistema en equilibrio*:


$$Ku=F$$$$\frac{AE}{L}\begin{pmatrix}1 & -1\\-1 & 1\end{pmatrix}\begin{pmatrix}u_1\\u_2 \end{pmatrix}=\begin{pmatrix}F_1\\F_2 \end{pmatrix}$$

$$\frac{AE}{L}\begin{pmatrix}1 & -1\\-1& 1\end{pmatrix}\begin{pmatrix}u_2+\frac{F}{k}\\u_2 \end{pmatrix}=\begin{pmatrix}F\\-F\end{pmatrix}$$

$$\frac{AE}{L}\begin{pmatrix}1 & -1\\0 & 0\end{pmatrix}\begin{pmatrix}u_2+\frac{F}{k}\\u_2 \end{pmatrix}=\begin{pmatrix}F\\0\end{pmatrix}$$

$$\frac{AE}{L}\begin{pmatrix}1 & -1\\0 & 0\end{pmatrix}\left[u_2\begin{pmatrix}1\\1 \end{pmatrix}+\frac{F}{k}\begin{pmatrix}1\\0 \end{pmatrix}\right]=\begin{pmatrix}F\\0\end{pmatrix}$$
Siendo:
$$\hspace{2mm}u=u_h+u_p$$
Donde:
$$u_h = u_2[1\hspace{2mm}1]^T\hspace{1cm}\rightarrow\hspace{1cm}\text{Solución homogénea}$$
$$u_p = 
\frac{F}{k}[1\hspace{2mm}0]^T\hspace{1cm}\rightarrow\hspace{1cm}\text{Solución particular}$$

****
**Ejercicio 3.-**

**a.** 

$\hspace{2mm}$ La siguiente imagen corresponde a la matriz diagonal D en donde los coeficientes no nulos serán los autovalores de la matriz K.


<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1nvxTEeIngbRVy3VQJmOxKBZUglXP9pmn" alt="Matriz diagonal D">
</p>



$\hspace{2mm}$ En la siguiente imagen se podrá ver la matriz V en donde las columnas corresponden a los autovectores de la matriz K

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1W_Vs5Zh11AKMdHNUfnRB--5rumPOO7Hq" 
    alt="Matriz V">
</p>

**b.** $\hspace{2mm}$ *Cálculo de la solución:*

$\hspace{2mm}$ El objetivo del problema es hallar los desplazamientos de los nodos. Al ya conocer el desplazamiento de uno de ellos (BCs), se procede a reducir el sistema, quedando el mismo de 2x2.
A continuación, se muestra imagen de lo comentado resuelto en Matlab.

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=13Hxz0UjrZreW9i3kLeStsp9VwzTimZUY" 
    alt="Solucion Ej.3">
</p>

**c.** $\hspace{2mm}$ *Cálculo de la matriz flexibilidad:*

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=18SZSD070vaV77099nYOvjDkdtefQ7FJW" 
    alt="Matriz flexibilidad">
</p>

****
**Ejercicio 4.-**

**a.**
$\hspace{2mm}$ Para calcular la capacidad de carga estática máxima se procede primero a realizar un análisis estático de las estructuras, solicitándolas con fuerzas de $1N$. Como al solicitarlas con dicha carga las barras estarán en régimen elástico (es decir que habrá una relación lineal entre la tensión y la deformación), se podrá estimar la carga estática máxima de la siguiente manera: 

$$\frac{\sigma_f\cdot\ P}{\sigma_p}=F$$

$\hspace{2mm}$ Donde $\sigma_f$ es la tensión de fluencia del material, $P$ es la carga de prueba $P=1N$, $\sigma_p$ es la tensión máxima que se alcanza al aplicar la carga de prueba y $F$, la carga estática máxima de la estructura.

*.-Viga Pratt:*

$$\newline$$

$$\frac{250Mpa\cdot\ 1N}{0,02121Mpa}=F$$
$$11786,89N=F$$

-Verificación:

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1dqUY2gYYxXtJ92mMFBNXApo25VasxGI4" 
    alt="Tension axial Viga Pratt con carga critica">
</p>


*.-Viga Howie:*

$$\frac{250Mpa\cdot\ 1N}{0,02Mpa}=F$$
$$12500N=F$$

-Verificación:

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1icrQkLcdJmCZgTZk5ZyER62dLpRX97FP" 
    alt="Tension axial Viga Howie con carga critica">
</p>

**b.**

-Desplazamientos transversales:
$$\newline$$
*-Viga Pratt*
$$\newline$$
$$\newline$$
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1UuIprnFjhfi4awpDsENQv40posZAq7pn" 
    alt="Tension axial Viga Pratt con carga critica">
</p>

$$\newline$$
*-Viga Howie*
$$\newline$$
$$\newline$$
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1VPQ22H_Pje7p7sG1zWayXO_ajqcnQUFS" 
    alt="Tension axial Viga Pratt con carga critica">
</p>

$$\newline$$
-Tension normal
$$\newline$$
*-Viga Pratt*
$$\newline$$
$$\newline$$
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1MtiKc4suVOxiz9JdQiQPNLRLatV2qEYj" 
    alt="Tension axial Viga Pratt con P=1N">
</p>

$$\newline$$
*-Viga Howie*
$$\newline$$
$$\newline$$
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1e79-2DlZAgZ-Hg9IWj-V7vy7_MUjSxQ0" 
    alt="Tension axial Viga Pratt con P=1N">
</p>

$\hspace{2mm}$ Se puede observar al comparar que para la misma solicitación, los desplazamientos y las tensiones serán mayores en la viga Pratt.

**c.**

-Desplazamientos transversales: 
$$\newline$$
*-Viga Pratt*
$$\newline$$
$$\newline$$


<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1HodbwJskF8jIM_Q3zvXhlgkUoCxQ4rDV" 
    alt="Desplazamientos transversales">
</p>

$$\newline$$
*-Viga Howie*
$$\newline$$
$$\newline$$

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1EzLkh9bULelx3yGPPmDE_GoJuDeoOzHP" 
    alt="Desplazamientos transversales">
</p>

$$\newline$$
-Tensión normal
$$\newline$$
*-Viga Pratt*
$$\newline$$
$$\newline$$

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1C87aV789c2LN0l_vJxEw6fTINtH33_mP" 
    alt="Tension axial Viga Pratt con P=1N">
</p>

$$\newline$$
*-Viga Howie*
$$\newline$$
$$\newline$$

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1uCyOJTHi9nm7ZnrQDYNSTy9sx9bie_WN" 
    alt="Desplazamientos transversales">
</p>

$$\newline$$
$\hspace{2mm}$ Las tensiones y desplazamientos son mayores al cambiar el vínculo simple por uno doble en ambas estructuras.

****

**Ejercicio 5.-**

$\hspace{2mm}$ Se solicitó a las estructuras con una carga de $1N$ en en nodo D. La sección y el material utilizado fueron los mismos que para el punto anterior.


**a.**  *Diagrama de fuerzas* 
$$\newline$$
*-Viga Michell*
$$\newline$$
$$\newline$$

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1QlW1OfeZ1H7Pz3a_g5ptX5wOtDOiVCm3" 
    alt="N Michell">
</p>

$$\newline$$
*-Estructura 2*
$$\newline$$
$$\newline$$
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1qbMuNxRDE3gNAOlbiS6tK6KQC-AqcCiS" 
    alt="N estructura">
</p>

**b.** $\hspace{2mm}$*Cálculo de las secciones de las barras a iso-tensión.*
$$\newline$$
*- Viga Michell*
$$\newline$$
$$\newline$$

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1FNClm3Zsa-41Ce0jXN1_uYTHLvn8zZ8D" 
    alt="N estructura">
</p>

$$\newline$$
*-Estructura 2*
$$\newline$$
$$\newline$$

<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1VWHj1s2Sis6SwbwxUe-bgOin-n1T1i1B" 
    alt="N estructura">
</p>

$\hspace{2mm}$ Se puede observar que para igual estado de cargas, la viga Michell tendrá menor volumen.
$$\newline$$
**c.** $\hspace{2mm}$ *Desplazamiento del punto D*
$$\newline$$
*- Viga Michell*
$$\newline$$
$$\newline$$
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1R42rf_eaHTHsmv6N_HFXcaxKTPLQ91lN" 
    alt="N estructura">
</p>

$$\newline$$
*-Estructura 2*
$$\newline$$
$$\newline$$
<p align="center">
    <img src="https://drive.google.com/uc?export=view&id=1l7EorfNtKgv5pK3WEqCu0-HFlWlNODr5" 
    alt="N estructura">
</p>

$\hspace{2mm}$ Se puede observar que para igual estado de cargas,  el nodo D tiene un desplazamiento menor en la viga Michell.
