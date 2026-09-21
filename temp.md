**Protocolo de Avaliação de Usabilidade do Módulo Softbody (Unity C#)**

---

**1. Perfil do Desenvolvedor (Anamnese Técnica)**

* **Tempo de experiência com Unity:** [ ] < 3 anos  [ ] 3-5 anos  [ ] > 5 anos
* **Nível de senioridade em C# / Unity:** [ ] Pleno  [ ] Senior  [ ] Tech Lead / Specialist
* **Grau de familiaridade com motores de física customizados ou Softbody (XPBD/PBD):**
[ ] Nenhum  [ ] Básico  [ ] Avançado
* **Experiência prévia com arquiteturas de contexto/DI no Unity (ex: Service Locator, Zenject, VContainer):**
[ ] Sim  [ ] Não

---

**2. Guia de Execução de Tarefas (Tasks-Based Evaluation)**

> **Orientações para o facilitador:**
> * Aplique o protocolo *Think-Aloud*: peça para o desenvolvedor verbalizar todas as suas dúvidas, intenções e frustrações enquanto executa.
> 
> 
> * Anote o **Tempo de Conclusão** e a quantidade de **Erros/Exceções** para cada etapa.
> 
> 
> 
> 

* **Tarefa 1: Instalação e Inicialização do Contexto (Tempo limite: 10 min)**
* *Instrução:* Importe o pacote via `manifest.json`. Em uma cena limpa, instancie a infraestrutura do `SoftBodyContext` e vincule o arquivo de configuração de limites e parâmetros globais.


* *Métricas:*
* Tempo gasto: ____ min
* Concluiu sem ajuda? [ ] Sim  [ ] Não
* Erros / Dúvidas reportadas: _______________________________________




* **Tarefa 2: Conversão de Geometria e Presets no Inspector (Tempo limite: 15 min)**
* *Instrução:* Adicione o componente `SoftBody` em uma malha 3D de um órgão. Atribua um objeto de preset (`PresetValues`) ao componente e ajuste os parâmetros visuais/físicos como rigidez, massa e taxa de amortecimento direto na Unity GUI.


* *Métricas:*
* Tempo gasto: ____ min
* Concluiu sem ajuda? [ ] Sim  [ ] Não
* Erros / Dúvidas reportadas: _______________________________________




* **Tarefa 3: Programação e Manipulação de Eventos em C# (Tempo limite: 20 min)**
* *Instrução:* Crie um script C# customizado. Escreva o código para recuperar a instância do `Selector` ativo via `SoftBodyContext` e inscreva métodos aos eventos `OnSelect` e `OnRelease` para disparar um log ou uma alteração de estado ao agarrar o tecido.


* *Métricas:*
* Tempo gasto: ____ min
* Concluiu sem ajuda? [ ] Sim  [ ] Não
* Erros / Dúvidas reportadas: _______________________________________




* **Tarefa 4: Ferramentas Cinemáticas e Otimização (Tempo limite: 15 min)**
* *Instrução:* Configure um objeto de ferramenta rígida utilizando o componente `KinematicBody`. Em seguida, ative o `Physics Mesh Debugger` no Inspector para inspecionar os vértices/arestas físicas e avaliar o impacto de desempenho na cena.


* *Métricas:*
* Tempo gasto: ____ min
* Concluiu sem ajuda? [ ] Sim  [ ] Não
* Erros / Dúvidas reportadas: _______________________________________





---

**3. Avaliação Pós-Tarefa (Single Ease Question - SEQ)**
*Responda o nível de facilidade percebido logo após concluir cada etapa (1 = Extremamente Difícil, 7 = Extremamente Fácil):*

* **Tarefa 1 (Setup do Contexto):** [ 1 ] [ 2 ] [ 3 ] [ 4 ] [ 5 ] [ 6 ] [ 7 ]
* **Tarefa 2 (Softbody & Inspector):** [ 1 ] [ 2 ] [ 3 ] [ 4 ] [ 5 ] [ 6 ] [ 7 ]
* **Tarefa 3 (Código C# & Eventos):** [ 1 ] [ 2 ] [ 3 ] [ 4 ] [ 5 ] [ 6 ] [ 7 ]
* **Tarefa 4 (Kinematic & Debugger):** [ 1 ] [ 2 ] [ 3 ] [ 4 ] [ 5 ] [ 6 ] [ 7 ]

---

**4. Questionário Psicométrico (TAM e SUS)**

**Modelo de Aceitação de Tecnologia (TAM)**

* **Utilidade Percebida:**
> "O módulo fornece uma infraestrutura robusta para simular tecidos deformáveis sem que eu precise me preocupar com o motor de física subjacente?"
> 
> 


* [ ] 1 - Discordo Totalmente  [ ] 2  [ ] 3  [ ] 4  [ ] 5 - Concordo Totalmente


* **Facilidade de Uso Percebida:**
> "A curva de aprendizado para manipular interações físicas via C# (métodos e eventos de seleção/liberação) é baixa para meu nível de experiência?"
> 
> 


* [ ] 1 - Discordo Totalmente  [ ] 2  [ ] 3  [ ] 4  [ ] 5 - Concordo Totalmente



**System Usability Scale (SUS) — Adaptado para APIs**
*Marque de 1 (Discordo Totalmente) a 5 (Concordo Totalmente):*

1. Eu usaria este módulo com frequência caso precisasse de física de corpos macios em projetos Unity.


2. Achei a estrutura da API e os componentes no Inspector desnecessariamente complexos.


3. Achei o fluxo de inicialização via `SoftBodyContext` fácil de integrar ao ciclo de vida da Unity.


4. Acho que precisaria do suporte direto dos criadores para construir interações complexas com o módulo.
5. Achei que as diversas funcionalidades da API (presets, seletores, corpos cinemáticos) estão bem integradas.


6. Achei que havia muita inconsistência no comportamento dos componentes ou na documentação da API.
7. Imagino que a maioria dos desenvolvedores Unity sêniores aprenderia a usar este módulo rapidamente.
8. Achei o processo de configuração no Inspector pouco intuitivo ou propenso a erros.
9. Senti-me muito confiante ao manipular as propriedades físicas e eventos via código C#.


10. Precisei aprender muitas coisas novas sobre física antes de conseguir operar o módulo com sucesso.

---

**5. Entrevista Qualitativa & Dimensões Cognitivas (Pós-Teste)**

* **Viscosidade e Acoplamento (Viscosity & Coupling):**
* Ao ajustar o `PresetValues` ou alternar as propriedades físicas em tempo de execução, você sentiu a API flexível ou houve efeito colateral inesperado na simulação?




* **Invisibilidade e Abstração C#:**
* Como desenvolvedor Unity, a API em C# escondeu com sucesso a complexidade matemática do motor físico subjacente ou houve momentos em que você sentiu falta de controle de baixo nível?




* **Tratamento de Erros e Logs:**
* Ao cometer erros propositais ou esquecer dependências na cena (como o contexto global), os avisos no Console do Unity foram claros para solucionar o problema?




* **Pontos Fortes e Oportunidades de Melhoria:**
* Qual foi a melhor experiência no workflow de desenvolvimento? O que precisaria mudar na API antes deste pacote ser publicado para produção?