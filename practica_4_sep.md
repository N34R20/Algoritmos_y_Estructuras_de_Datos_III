# Practica



## Induccion 

- **Idea**: 

    Para probar que una propiedad $P$ vale para todos los nautrales $n \in \N$, vamos a probar que $P(0)$ es cierto, y que $P(n) \rightarrow P(n+1), \forall n$. Funciona tambien si queremos probar algo para todos los naturales mayores a un cierto $k$.


#### Ejercicio

Probar que $2^n \leq n!$ para todo $n \geq 4$

#### Resolucion

- pruebo $P(0)$

$$P(4) : 2^4 < 4!$$
$$16 < 24$$


- Pruebo que $P(n) \rightarrow P(n+1)$

    Asumo como Hipotesis $2^n < n!$ y quiero ver que $2^{n+1} < (n+1)!$

$$2^{n+1} = 2^n 2 < n! 2 \leq n!(n+1) = (n+1)!$$

$2 \leq n+1$ porque $n \geq 4$


### Induccion completa

### Induccion estructural


## Contrareciproco

- **Idea**: 

    Decir que $\alpha \rightarrow \beta$ es lo mismo que decir  $\neg \beta \rightarrow \neg \alpha$

#### Ejercicio 

Probar que si $n^2$ es par, entonces $n$ tambien lo es.

$n^2$ par $\rightarrow n$ par $\equiv$ $n$ impar $\rightarrow n^2$ impar



## Por absurdo

- **Idea**: 
    Para probar que $\alpha \rightarrow \beta$ vamos a asumir que valen $\alpha$ y $\neg \beta$, para ver luego que esto contradice algun resultado previo

#### Ejercicio

Probar que $\sqrt 2$ es irracional

#### Resolucion

Suponemos que $\sqrt 2 = \frac{a}{b}$ con $a,b\in \Z, (a:b)=1, b\neq0$

$(a:b)=1$ nos dice que a y b son coprimos, no tienen nigun entero comun en la factorizacion


## Por construccion

- **Idea**: 
    Si la formula habla de la existencia de alguna estructura, podemos simplemente explicar como se construye.

#### Ejercicio

Probar que para todo conjunto finito $S \subseteq \N$ vale que existe un polinomio $p$ no nulo tal que $p(s)=0$ para todo $s \in S$


#### Resolucion

$$P_S(x) = \prod_{s \in S}(x-s)$$

$$\forall j \in {1,..,n}, P_s(s_j) = \prod_{s \in S}(s_j-s) = 0$$

## Polemico 

Veamos un ejemplo curioso de una induccion mal hecha

- **Teorema?**
    
    Todo conjunto finito de caballos es de un mismo color

https://en.wikipedia.org/wiki/All_horses_are_the_same_color

#### Ejercicio
identificar que esta mal en la siguiente demostracion

Prueba: hagamos induccion en el tamaño del conjutno $C$ de caballos

Si |C| = 1 el teorema vale

Si $C = \{c_1, ..., c_{n+1}\}$ hacemos lo siguiente:

1. Para $\{c_1, ..., c_n\}$ el teormea vale, por lo que los caballos $c_1, ..., c_n$ son de un mismo color.
2. Para $\{c_n, c_{n+1}\}$ el teorema tambien vale.
3. Como $c_n$ 


## Backtracking


Fibonacci

Cual es la complejidad exacta del algoritmo que implementa Fibonacci recursivamente.


$$Fibo(n) = 
\begin{array}{ll}
1 & \text{si } n =1,2 \\
F(n-1) + F(n-2) & \text{si } n \neq 1,2 
\end{array}$$
