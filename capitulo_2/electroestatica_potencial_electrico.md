# Potencial eléctrico

Una de las consecuencias de que el campo eléctrico $\mathbf{E}$ sea irrotacional,

```{math}
:label: e_rot_cero
\vec{\nabla} \times \mathbf{E} =0,
```

y que por lo tanto sea el gradiente de una función, $\mathbf{E}=\vec{\nabla} \phi$ , es que la integral del campo en un camino cerrado es cero,

```{math}
:label: int_e_cero
\oint \mathbf{E} \cdot d \vec{l}=0.
```

Ya que el campo eléctrico representa a la fuerza sobre una carga de prueba $Q$, es decir, $\mathbf{F}=Q \mathbf{E}$, que la integral de camino cerrada sea cero significa que la fuerza es conservativa. A la integral la podemos interpretar como el trabajo que realiza esta fuerza y por lo tanto define la energía potencial asociada a la fuerza electroestática. Que sea conservativa significa que esta integral solo depdende del estado inicial y final. Si tomamos al punto $\mathbf{O}$ como referencia para calcular la integral, podemos definir el **potencial eléctrico** $V(\mathbf{r})$ como

```{math}
:label: definicion_potencial_electrico
V(\mathbf{r})=-\int_{\mathbf{O}}^{\mathbf{r}} \mathbf{E} \cdot d \vec{l}.
```

Una vez que fijamos el punto de referencia $\mathbf{O}$, el potencial eléctrico solo depende de la posición $\mathbf{r}$.

Ya que esta es una energía potencial, únicamente las diferencias de potencial tienen significado físico, al calcular la diferencia encontramos que


```{math}
:label: delta_potencial_electrico_0
V(\mathbf{b})-V(\mathbf{a})=-\int_{\mathbf{O}}^{\mathbf{b}} \mathbf{E} \cdot d \vec{l}+\int_{\mathbf{O}}^{\mathbf{a}} \mathbf{E} \cdot d \vec{l}.
```

Si ahora cambiamos el orden de integración en la integral de $v(\mathbf{a})$, obtenemos

```{math}
:label: delta_potencial_electrico_1
V(\mathbf{b})-V(\mathbf{a})=-\int_{\mathbf{O}}^{\mathbf{b}} \mathbf{E} \cdot d \vec{l}-\int_{\mathbf{a}}^{\mathbf{O}} \mathbf{E} \cdot d \vec{l}.
```
Finalmente vemos que podemos juntar las dos integrales en una sola:

```{math}
:label: delta_potencial_electrico
V(\mathbf{b})-V(\mathbf{a})=-\int_{\mathbf{a}}^{\mathbf{b}} \mathbf{E} \cdot d \vec{l}.
```
**El teorema fundamental del cálculo para gradientes**,

```{math}
:label: teorema_gradientes
V(\mathbf{b})-V(\mathbf{a})=\int_{\mathbf{b}}^{\mathbf{a}} (\vec{\nabla} V)  \cdot d \vec{l},
```

nos permite relacionar al gradiente del potencial eléctrico con el campo eléctrico

```{math}
:label: relacion_campo_y_potencial
\mathbf{E}(\mathbf{r})=-\vec{\nabla} V(\mathbf{r}) .
```
De esta manera identificamos al potencial con la función escalar que al calcular su gradiente nos permite obtener el campo eléctrico. El potencial tiene la ventaja sobre el campo eléctrico de que el potencial tan solo es una función escalar y no necesitamos realizar cálculos para cada componente de un vector como es el caso con el campo eléctrico.

## Cambio de punto de referencia para el potencial

Analicemos que sucede si cambiamos el punto de referencia $\mathbf{O}$ a otro punto $\mathbf{O}'$. Con el nuevo punto de referncia tenemos un nuevo potencial



```{math}
:label: referencia_potencial_0
V'(\mathbf{r})=-\int_{\mathbf{O'}}^{\mathbf{r}}  \mathbf{E} \cdot d \vec{l}
```

Si ahora tomamos el siguiente camino

```{math}
:label: referencia_potencial_1
V'(\mathbf{r})=-\int_{\mathbf{O'}}^{\mathbf{O}}  \mathbf{E} \cdot d \vec{l}-\int_{\mathbf{O}}^{\mathbf{r}}  \mathbf{E} \cdot d \vec{l},
```

la primera integral es una constante, mientras que la segunda integral es el potencial que habíamos definido originalmente

```{math}
:label: referencia_potencial_2
V'(\mathbf{r})=k+V(\mathbf{r}) 
```

Estas dos definiciones del potencial solo son diferentes en la suma de una constante, ambas definiciones son físicamente equivalentes ya que, como habiamos mencionado anteriormente, **solo las diferencias de potencial tienen significado físico**.


El punto de referencia $\mathbf{O'}$ se escoge en un lugar donde el campo sea cero. Para una distribución de carga finita esto significa que el cero de potencial está en una superficie muy alejada, o dicho de otra manera, en el infinito. Para una distribución de carga infinita no hay un lugar en donde el campo sea cero, por lo que se toma un punto de referencia arbitrario pero conveniente para la descripción del sistema.


## El potencial eléctrico y el principio de superposición

Este principio parte de que las fuerzas eléctricas son aditivas por pares, es decir se suman las fuerzas debido a cada fuente de campo. Para la carga de prueba $q_0$, la fuerza aplicada $\mathbf{F}_0$ debido a $N$ cargas, $q_{1},q_2,q_3, \ldots$ es

```{math}
:label: aditivadad_fuerzas
\mathbf{F}_0=\mathbf{F}_{01}+\mathbf{F}_{02}+\cdots,
```

en donde hemos usado la ley de Coulomb para calcular la fuerza \mathbf{F}_{0i} a una distancia $\mathbf{r}_{0i}=\mathbf{r}_{0}-\mathbf{r}_{i}$. Al dividir esta expresión entre la carga prueba, obtenemos el campo eléctrico total en la posición $\mathbf{r}$ de la carga de prueba,


```{math}
:label: aditivadad_campos
\mathbf{E}(\mathbf{r})=\mathbf{E}_{01}+\mathbf{E}_{02}+\cdots.
```

Al integrar esta última expresión sobre un camino obtenemos el potencial eléctrico debido a $N$ cargas puntuales,


```{math}
:label: aditivadad_potenciales
V(\mathbf{r})=V_{01}+V_{02}+\cdots,
```

con una suma escalar en vez de una suma vectorial.

## Unidades del potencial eléctrico

Ya que el campo eléctrico tiene unidades


```{math}
:label: unidades_campo
[\mathbf{E}]=\frac{[\mathbf{F}]}{[Q]}.
```

Para el SI esto corresponde a Newtons sobre Coulomb. Ya que el potencial es básicamente el campo por una distancia


```{math}
:label: unidades_potencial
[V]=\frac{[F][L]}{[Q]},
```

en el SI esto es Joules sobre Coulomb. A las unidades del potencial eléctrico en el SI se le llaman volts V

```{math}
:label: definición volts
V=\frac{J}{C}.
```

## Ejemplo 2.7 (Potencial de un cascarón esférico calculado por medio del campo eléctrico)

Encuentre el potencial dentro y fuera de un cascarón esférico de radio $R$ con una carga superficial uniforme. Escoja el punto de referencia al infinito. a) Fuera de la esfera, b) Dentro de la esfera

```{admonition} Nota
El ejercicio se resuelve en clase, se recomienda que el lector intente resolverlo por su cuenta y tome la respuesta como guía.
```

Respuesta inciso a:

```{math}
:label: solucion_ejemplo_2.7.a
v(\mathbf{r}) = \frac{1}{4 \pi \epsilon_{0}} \frac{q}{r}.
```

Respuesta inciso b:

```{math}
:label: solucion_ejemplo_2.7.b
v(\mathbf{r}) = \frac{1}{4 \pi \epsilon_{0}} \frac{q}{R}.
```

Ya que dentro de la esfera el potencial no depende de la posición y es el mismo en todas partes, se dice que estamos en una región equipotencial.


## Ecuación de Poisson y Laplace

## El potencial de una distribución de carga (localizada)

## Ejemplo 2.8

## Condiciones de frontera