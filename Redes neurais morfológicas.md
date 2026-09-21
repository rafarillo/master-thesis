* Redes neurais morfológicas
* Ler papers sobre dificuldade em redes neurais usando operadores morfológicos
* Oportunidade: qual a melhor maneira de inicializar a rede, qual o melhor metodo de treinar a rede
* Alguns tópicos ficaram por fora no paper CFP
    * Oportunidade: inicializar parametros
    * Qual a forma de treinar, como definir a função de custo
    * Dificuldade em acoplar essa camada de rede neural
https://miro.com/app/board/uXjVHrSkQI0=/?userEmail=rafaelgtvc%40usp.br&track=true&utm_source=notification&utm_medium=email&utm_campaign=add-to-team-and-board&utm_content=go-to-board&share_link_id=595964434712&lid=4oe19kzdo5cf

----------------------------------------------------
## 09/10/2026

Paper CPF
 - O problema de colocar a layer conexa no meio é o fato de ter que reconstruir a árvore
 - Problmea de normalização nos atributos
 - Problema de feature selection

- Sobre update rathern rebuild
    - O grande problema do paper é que é para algumas operações, não é genérico
    - 
- IFTs
    - Calculo de atributo

- Dada uma árvore:
    - Calcula-se o esqueleto dessa árvore

- Aprendizagem semi supervisionado
    - Exemplo da máscara
    - Esconde o nó (interpretabilidade)
    - Interpretabilidade

- Árvore de componente multiescala
- Até próxima semana realizar implementação do do upadte rather than rebuild

- Film masked (BERT)
- 

-------------------------
## 09/18/2026
- Primeiro passo caracterizar o problema
- Primeiro definir como a operação de split impacta na árvore
    - Realizar primeiro um estudo de caso (olhar como fica a árvore inicial e a final)
    - Realizar a comparação
- Depois realizar o algoritmo