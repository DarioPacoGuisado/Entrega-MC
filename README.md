# Entrega-MC
Una simulación de Cadenas de Markov, siguiendo la guía de clase.

En esta simulación se simulan y visualizan cadenas de Markov en tiempo discreto $T = \mathbb{N}$ y con conjunto de estados finito.

Primero, se simula una Cadena de Markov mediante simular para cada paso una variable discreta $X_n$ que toma los valores ${0, 1... N-1}$ con probabilidad indicada la matriz de transición $P$ y el valor $X_{n-1}$.

Después, se programa la evolución de la distribución marginal de la variable $X_n$, cuando $n \in \mathbb{N}$ crece, partiendo de una distribución inicial $\pi^{(1)}$, así como se grafican los diagramas de transición de estados asociados a la matriz $P$.

Por último, se comprueban en distintos casos las caracterizaciones del teorema de convergencia para procesos de Markov unicadenales y aperiódicos. En particular, si $p(n_{steps}, n_{samples})$ es el vector de frecuencias relativas empíricas en el paso exactamente $n_{steps}$ en $n_{samples}$ simulaciones aleatorias de la misma MC; y $\pi$ es la única distribución estacionaria, entonces:
$$\lim_{n_{steps}, n_{samples} \rightarrow \infty} p(n_{steps}, n_{samples}) \rightarrow^P \pi.$$

También se comprueba el teorema ergódico para procesos de Markov unicadenales y aperiódicos. En particular, si $q(n_steps)$ es el vector de frecuencias relativas empíricas de una cadena de Markov hasta el paso $n_{steps}$, entonces
$$\lim_{n_{steps} \rightarrow \infty} q(n_{steps}) \rightarrow \pi.$$

