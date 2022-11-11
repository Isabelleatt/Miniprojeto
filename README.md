# MiniProjeto
### Miniprojeto de Matemática do Contínuo sobre otmização pelo vetor gradiente

Quando estudamos as funções de uma variável, vimo a importância da derivada nos processos de otmização (determinação dos pontos máximos e de mínimo de funções). O mesmo problema pode ser considerado no contexto das funções de duas ou mais variáveis. Por exemplo, de que forma as derivadas parciais podem ser usadas para determinar os pontos de máximo e de mínimo da função $f$ cujo gráfico é mostrado a seguir?
Neste miniprojeto, você vai estudar e implementar um método numérico para determinar pontos de máximo e de mínimos locais de funções de duas variáveis.

Na última aula, vimos que o vetor gradiente indica, em determinado ponto do domínio, a direção e o sentido em que a derivada direcional é máxima (e o oposto do vetor gradiente representa a direção e o sentido em que a derivada direcional é mínima). Dessa forma, se for possível, a partir de um ponto qualquer do domínio de uma função de várias variáveis, construir um caminho que aponte sempre para a direção e o sentido do vetor gradiente, esse caminho tenderá a nos conduzir ao ponto de máximo dessa função.

Partindo de um ponto $(x0, y0)$ do domínio de uma função $f$, e sendo $f(x0, y0) = (a,b)$, podemos realizar um deslocamento na direção e o sentido do vetor gradiente, chegando ao ponto $(x1, y1)$, fazendo, como ilustrador na figura,

$\left\{\begin{matrix}
 x1 = x0 + \alpha * a\\
 y1 = y0 + \alpha * b
\end{matrix}\right.$

A constante α é um fator que determina o tamanho do passo dado na direção e sentido de $▽f$.
Repetindo n vezes esse processo, poderemos nos aproximar cada vez mais de um ponto máximo da função $f$ (ou de um ponto mínimo, se o deslocamento for na direção e sentido de $-▽f$)
