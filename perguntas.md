# Perguntas para Reunião dia 25/09/2026

### Seção 2.4

1. O texto menciona "We say that $\preccurlyeq$ is a total order on $A$ if for any $a$, $b$ $\in$ $A$ we have $a \preccurlyeq b$ or $b \preccurlyeq a$". Esse ou deve ser exclusivo para a relação ser antisimétrica, certo?

2. O texto menciona "the set of the maximal elements of $(\~{A}, \preccurlyeq)$ is denoted by $\nabla^{\preccurlyeq}\~{A}$". Esse conjunto de elementos maximais deve ser maximal a que propriedade? Isso depende do caso de uso?

3.  O texto menciona "the set of the minimal elements of $(\~{A}, \preccurlyeq)$ is denoted by $\nabla^{\preccurlyeq}\~{A}$". Esse conjunto de elementos minimais deve ser minimal a que propriedade? Isso depende do caso de uso?

4. "When $(A, \preccurlyeq)$ is a totally ordered set and $a, b \in A$ with $a$ $b$ we denote by" $\llbracket a, b \rrbracket = \{ c \in A \mid a \preccurlyeq c \preccurlyeq b \}$. Sempre existe esse $c$?

### Seção 2.5

1. Sobre a notação $\preccurlyeq(a)$ no trecho "for any $a \in A$, the set $(\preccurlyeq(a), \preccurlyeq)$ is totally ordered". Acho que o artigo não chega a definir o que é a função de uma relação binária, mas imagino que signifique que a definição seja "Conjunto de valores em $A$ tal que $a \preccurlyeq b$, onde $b \in A$", certo?

### Seção 3.2 Threshold Sets and Connected Components

1. O texto menciona "the set of all the connected components for all the threshold sets $\Lambda_v (v \in \mathbb{V})$ (Fig 2b)". Mas o certo seria Fig 2a né?

### Seção 5

1. $\varGamma_v^- = \varGamma^- \cap \varTheta_v^-$ isso significa os nós de uma altura $v$ que estão conectados a $C$ no intervalo $\llbracket a, b \rrbracket$?

2. Em $C_v^+ = c \cup \bigcup \varGamma_v^- \in \varTheta_v^+$, quem percente a $\varTheta_v^+$ é a expressão toda, certo? Não somente $\varGamma_v^-$. Além disso, quais são os índice dessa união? Ela começa em $a$ e termina em $b$? 

3. Em $\varGamma^+ = \{ C_v^+ \}_{v \in \llbracket a, b \rrbracket}$, essa notação é para um valor de $v$ ou para um conjunto de valores no intervalo $\llbracket a, b \rrbracket$?

4. Em "In particular, Eq. (32) refines the definition initially given in Eq. (27).", refina em que sentido a definição?

5. Não entendi como fica distribuição das próprias partes dos novos nós na seguinte equação $\rho^+(C_v^+) = 
\begin{cases} 
\bigcup \rho^-(\varGamma_{\rho, b}^-) \cup C & \text{if } v = b \\ 
\bigcup \rho^-(\varGamma_{\rho, v}^-) \setminus C & \text{if } v \neq b 
\end{cases}$

6. $\varGamma_{\eta, \llbracket a, b \rrbracket}^- = \bigcup_{v \in \llbracket a, b \rrbracket} \varGamma_{\eta, v}^-$ esse é o conjunto de nós que serão mergeados?

7. $\varGamma_{\eta, \llbracket b+1, \top-1 \rrbracket}^- = \bigcup_{v \in \llbracket b+1, \top-1 \rrbracket} \varGamma_{\eta, v}^-$ esse é o conjunto de nós que não serão mergeados mesmo estando conectados a C?

### Seção 5.2

1. A remoção de uma subárvore é definida como a redução de nível de cinza de uma região da imagem?

### Seção 6
1. O que significa ser uma monoide?

2. Na equação $\kappa(X) = \alpha(\rho(X)) \oplus \bigoplus_{Y \triangleleft X} \kappa(Y)$, o símbolo $Y \triangleleft X$ significa que o atributo está sofrendo update das folhas $Y$ até o nó $X$?