[4-htas-organizado.md](https://github.com/user-attachments/files/35308026/4-htas-organizado.md)
# HTAs (Hierarchical Task Analysis)

<a name="sumario"></a>
## Sumário

- [1. Introdução](#secao-1)
- [2. Consistência entre o Mapa de Objetivos e os HTAs](#secao-2)
- [3. HTA 1 – Solicitar materiais e equipamentos](#secao-3)
- [4. HTA 2 – Acompanhar o andamento de um pedido](#secao-4)
- [5. HTA 3 – Consultar materiais e equipamentos disponíveis](#secao-5)
- [6. HTA 4 – Ajustar a apresentação para facilitar a leitura](#secao-6)
- [7. HTA 5 – Gerenciar solicitações recebidas](#secao-7)
- [8. HTA 6 – Identificar e solicitar reposição de materiais](#secao-8)
- [9. HTA 7 – Consultar informações dos responsáveis](#secao-9)
- [10. Considerações finais](#secao-10)

---

<a name="secao-1"></a>
## 1. Introdução

Os HTAs detalham **como** cada persona realiza os objetivos definidos no [Mapa de Objetivos](3-mapa-de-objetivos.md). Cada HTA representa uma tarefa principal do sistema de gerenciamento de materiais do Laboratório de Biologia da UFAM, decomposta em subtarefas e planos de execução.

### Notação utilizada

| Elemento | Significado |
|---|---|
| Caixa numerada (ex.: 3. / 3.1) | Tarefa ou subtarefa |
| Plano (ex.: 1 > 2 > 3) | Ordem de execução. `>` indica sequência e `/` indica escolha entre alternativas |
| Caixa tracejada | Tarefa opcional |
| Linha sob a caixa | Tarefa elementar (não é decomposta) |
| Verde (lado esquerdo) | Objetivo(s) do mapa que originam o HTA |

[Voltar ao sumário](#sumario)

---

<a name="secao-2"></a>
## 2. Consistência entre o Mapa de Objetivos e os HTAs

| HTA | Grupo do mapa | Objetivos cobertos | Persona principal |
|---|---|---|---|
| 1 – Solicitar materiais e labortório desejado | Solicitação de materiais e laboratório desejado | Solicitar materiais e laboratório; Planejar conforme a data da aula; Considerar o prazo de 48 horas | Lucas (também Camila) |
| 2 – Acompanhar o andamento de um pedido | Acompanhamento de pedidos | Acompanhar o andamento; Consultar confirmações; Receber lembretes e notificações | Lucas (também Camila) |
| 3 – Consultar materiais e equipamentos disponíveis | Consulta de materiais | Consultar materiais e equipamentos disponíveis | Camila (também Lucas e Elisângela) |
| 4 – Ajustar a apresentação para facilitar a leitura | Acessibilidade e autonomia | Ampliar textos; Ajustar contraste e legibilidade; Navegar pelo teclado | Camila |
| 5 – Gerenciar solicitações recebidas | Gerenciar solicitações | Acompanhar pedidos recebidos; Identificar pendentes; Registrar e consultar em um único sistema | Elisângela |
| 6 – Identificar e solicitar reposição de materiais | Controlar reposições | Identificar necessidades de reposição; Acompanhar materiais a repor; Solicitar novos pedidos ao almoxarifado | Elisângela |
| 7 – Consultar informações dos responsáveis | Consultar informações dos responsáveis | Localizar professores e regentes; Obter dados de contato e responsabilidades | Elisângela (também Camila e Lucas) |

[Voltar ao sumário](#sumario)

---

<a name="secao-3"></a>
## 3. HTA 1 – Solicitar materiais e equipamentos

<p align="center">
  <img height="797" alt="HTA 1 — Solicitação de materiais e laboratório" src="https://github.com/user-attachments/assets/88da1fd4-b1b1-44cb-9350-49ea1bb8865c" />
</p>
<p align="center"><em>Figura 1 – HTA 1: Solicitar materiais e equipamentos.</em></p>


### Propósito

permitir que o professor solicite os materiais e equipamentos de que precisa para uma aula prática, informando a data da aula e respeitando o prazo mínimo de 48 horas.

### Tarefas e subtarefas

> **Plano 0:** `1 > 2 > 3 > 4 > 5 > 6`

1. **Acessar o sistema:** entrada do usuário no sistema.
2. **Iniciar nova solicitação:** abre o formulário de solicitação.
3. **Selecionar materiais e equipamentos** (3.1 > 3.2 > 3.3): buscar e escolher o item (3.1), informar a quantidade (3.2) e, opcionalmente, adicionar outro item repetindo 3.1 e 3.2 (3.3).
4. **Informar a data da aula** (4.1 > 4.2): selecionar a data (4.1) e conferir o prazo mínimo de 48 horas (4.2).
5. **Revisar a solicitação:** conferência dos itens, quantidades e data antes do envio.
6. **Enviar a solicitação** (6.1 > 6.2): confirmar o envio (6.1) e visualizar a confirmação de recebimento (6.2).

### Decisões envolvidas

quantos itens adicionar (laço 3.3) e, em 4.2, o que fazer se a data estiver a menos de 48 horas (ajustar a data). A conferência do prazo vem antes do envio para evitar pedidos que serão recusados, problema relatado pela Elisângela (P2) e pelo Lucas (P1).

### Contribuição ao fluxo

é a tarefa central do sistema. Seu resultado (a solicitação enviada) alimenta o HTA 2 (acompanhar) e o HTA 5 (gerenciar solicitações recebidas).

[Voltar ao sumário](#sumario)

---

<a name="secao-4"></a>
## 4. HTA 2 – Acompanhar o andamento de um pedido

<p align="center">
  <img height="450" alt="hta-2-acompanhar-pedido" src="https://github.com/user-attachments/assets/29bc9668-271c-484d-8f3a-1a92c299d907" />
</p>
<p align="center"><em>Figura 2 – HTA 2: Acompanhar o andamento de um pedido.</em></p>


### Propósito

permitir que o professor veja a situação de seus pedidos sem precisar perguntar constantemente à equipe do laboratório.

### Tarefas e subtarefas

> **Plano 0:** `1 > 2 > 3 > 4 > 5`

1. **Acessar o sistema.**
2. **Abrir a lista de pedidos.**
3. **Localizar o pedido** (3.1 / 3.2): procurar na lista (3.1) ou filtrar por status ou data (3.2).
4. **Consultar o andamento** (4.1 > 4.2): ver o status atual (4.1) e ver confirmações e atualizações (4.2).
5. **Receber lembretes e notificações** (opcional; 5.1 > 5.2): ativar lembretes de prazo (5.1, opcional) e visualizar a notificação recebida (5.2).

### Decisões envolvidas

em 3, o usuário escolhe entre procurar na lista ou filtrar, conforme a quantidade de pedidos. A tarefa 5 é opcional porque o usuário pode consultar o status por conta própria ou aguardar a notificação.

### Contribuição ao fluxo

responde aos problemas P3 e P4 do Lucas, que quer acompanhar sem perguntar e receber lembretes e confirmações. Fecha o ciclo iniciado no HTA 1.

[Voltar ao sumário](#sumario)

---

<a name="secao-5"></a>
## 5. HTA 3 – Consultar materiais e equipamentos disponíveis

<p align="center">
  <img height="450" alt="hta-3-consultar-materiais" src="https://github.com/user-attachments/assets/e9c2cd09-4a8b-4e7f-a165-fababf5b1937" />
</p>
<p align="center"><em>Figura 3 – HTA 3: Consultar materiais e equipamentos disponíveis.</em></p>


### Propósito

permitir que qualquer usuário saiba quais materiais e equipamentos estão disponíveis antes de planejar ou solicitar.

### Tarefas e subtarefas

> **Plano 0:** `1 > 2 > 3 > 4 > 5`

1. **Acessar o sistema.**
2. **Abrir o catálogo de materiais.**
3. **Localizar o material** (3.1 / 3.2): buscar pelo nome (3.1) ou filtrar por categoria (3.2).
4. **Verificar a disponibilidade** (4.1 > 4.2): ver a quantidade disponível (4.1) e os detalhes do item (4.2).
5. **Solicitar o item** (opcional): se o item estiver disponível, o usuário pode seguir para o HTA 1.

### Decisões envolvidas

a busca (3.1) ou o filtro (3.2) são alternativas, conforme o usuário conheça ou não o nome do item. A decisão de solicitar o item é opcional.

### Contribuição ao fluxo

apoia o planejamento da aula, antes da solicitação. Para a Camila, o catálogo precisa ser legível e navegável por teclado (ver HTA 4).

[Voltar ao sumário](#sumario)

---

<a name="secao-6"></a>
## 6. HTA 4 – Ajustar a apresentação para facilitar a leitura

<p align="center">
  <img height="450" alt="hta-4-ajustar-apresentacao" src="https://github.com/user-attachments/assets/760066d9-307b-4b9f-bc4d-927318488694" />
</p>
<p align="center"><em>Figura 4 – HTA 4: Ajustar a apresentação para facilitar a leitura.</em></p>


### Propósito

permitir que a Camila, que tem baixa visão, adapte o sistema às suas necessidades (tamanho do texto e contraste) sem prejudicar a organização das informações.

### Tarefas e subtarefas

> **Plano 0:** `1 > 2 > 3 > 4 > 5`

1. **Acessar o sistema** (por teclado ou tecnologia assistiva).
2. **Abrir as opções de acessibilidade.**
3. **Ampliar o texto** (3.1 > 3.2): escolher o tamanho do texto (3.1) e conferir a organização do conteúdo (3.2). Se o resultado não ficar adequado, repete-se 3.1.
4. **Ajustar o contraste** (4.1 > 4.2): escolher o modo de contraste (4.1) e conferir a legibilidade (4.2).
5. **Salvar as preferências** (5.1 / 5.2): confirmar os ajustes (5.1) ou, opcionalmente, restaurar o padrão (5.2).

### Decisões envolvidas

em 3.2 e 4.2 o usuário decide se o resultado está adequado e, se não estiver, refaz a escolha. A opção de restaurar o padrão (5.2) evita que um ajuste ruim prenda o usuário em uma configuração ilegível.

### Contribuição ao fluxo

atende aos problemas P1, P2 e P4 da Camila. Todas as tarefas devem poder ser feitas pelo teclado e ser compatíveis com tecnologias assistivas, requisito que vale para todos os HTAs.

[Voltar ao sumário](#sumario)

---

<a name="secao-7"></a>
## 7. HTA 5 – Gerenciar solicitações recebidas

<p align="center">
  <img height="450" alt="hta-5-gerenciar-solicitacoes" src="https://github.com/user-attachments/assets/4cb55af1-b328-44e8-b7cc-b8a89e809391" />
</p>
<p align="center"><em>Figura 5 – HTA 5: Gerenciar solicitações recebidas.</em></p>


### Propósito

permitir que a técnica acompanhe, analise e atualize as solicitações dos professores em um único sistema, no lugar de planilhas, e-mail e WhatsApp.

### Tarefas e subtarefas

> **Plano 0:** `1 > 2 > 3 > 4 > 5`

1. **Acessar o sistema.**
2. **Abrir as solicitações recebidas.**
3. **Selecionar a solicitação** (3.1 > 3.2): filtrar as pendentes (3.1, opcional) e abrir a solicitação (3.2).
4. **Analisar a solicitação** (4.1 > 4.2): verificar itens e quantidades (4.1) e verificar a data da aula e o prazo (4.2).
5. **Atualizar o andamento** (5.1 > 5.2): atualizar o status (5.1) e registrar uma observação (5.2, opcional).

### Decisões envolvidas

filtrar apenas as pendentes ou ver todas; em 4.2, avaliar se o prazo de 48 horas foi respeitado; em 5.2, decidir se é necessário registrar uma observação para o professor.

### Contribuição ao fluxo

é o lado receptor do HTA 1. Ao atualizar o status (5.1), a técnica alimenta o que o professor vê no HTA 2. Responde aos problemas P2 e P4 da Elisângela.

[Voltar ao sumário](#sumario)

---

<a name="secao-8"></a>
## 8. HTA 6 – Identificar e solicitar reposição de materiais

<p align="center">
  <img height="450" alt="hta-6-solicitar-reposicao" src="https://github.com/user-attachments/assets/4b201238-fd38-4115-893e-41d5237dd972" />
</p>
<p align="center"><em>Figura 6 – HTA 6: Identificar e solicitar reposição de materiais.</em></p>


### Propósito

permitir que a técnica identifique materiais em falta ou com pouca quantidade e peça a reposição ao almoxarifado.

### Tarefas e subtarefas

> **Plano 0:** `1 > 2 > 3 > 4 > 5`

1. **Acessar o sistema.**
2. **Consultar o estoque do laboratório** (2.1 > 2.2): ver itens com pouca quantidade (2.1) e itens indisponíveis (2.2).
3. **Selecionar itens para reposição** (3.1 > 3.2): marcar os itens (3.1) e informar as quantidades (3.2).
4. **Enviar pedido ao almoxarifado** (4.1 > 4.2): revisar o pedido (4.1) e confirmar o envio (4.2).
5. **Acompanhar a reposição** (5.1 > 5.2): consultar a situação do pedido (5.1) e registrar o recebimento quando o material chegar (5.2).

### Decisões envolvidas

quais itens repor e em que quantidade, com base no estoque e nas solicitações previstas. O registro do recebimento (5.2) mantém o catálogo do HTA 3 atualizado.

### Contribuição ao fluxo

atende aos problemas P1 e P2 da Elisângela (escassez de itens e falhas nos pedidos) e mantém o estoque confiável para os professores.

[Voltar ao sumário](#sumario)

---

<a name="secao-9"></a>
## 9. HTA 7 – Consultar informações dos responsáveis

<p align="center">
  <img height="450" alt="hta-7-consultar-responsaveis" src="https://github.com/user-attachments/assets/32c7e390-1d6e-4d1b-b3a8-34078055f256" />
</p>
<p align="center"><em>Figura 7 – HTA 7: Consultar informações dos responsáveis.</em></p>


### Propósito

permitir que o usuário localize professores e regentes responsáveis pelo laboratório e obtenha seus dados de contato e responsabilidades.

### Tarefas e subtarefas

> **Plano 0:** `1 > 2 > 3 > 4 > 5`

1. **Acessar o sistema.**
2. **Abrir a lista de responsáveis.**
3. **Localizar o responsável** (3.1 / 3.2): buscar pelo nome (3.1) ou filtrar por disciplina ou laboratório (3.2).
4. **Consultar os dados** (4.1 > 4.2): ver o contato (4.1) e as responsabilidades (4.2).
5. **Entrar em contato** (opcional).

### Decisões envolvidas

buscar por nome ou filtrar, conforme o que o usuário já sabe sobre o responsável. Entrar em contato é opcional, pois o usuário pode só precisar da informação.

### Contribuição ao fluxo

responde ao problema P3 da Elisângela, que tem dificuldade para levantar informações sobre os regentes. O objetivo também aparece nos mapas da Camila e do Lucas.

[Voltar ao sumário](#sumario)

---

<a name="secao-10"></a>
## 10. Considerações finais

Os sete HTAs cobrem os grupos de objetivos dos três mapas: solicitação, acompanhamento, consulta de materiais, acessibilidade, gerenciamento de solicitações, reposição e consulta de responsáveis. Eles servirão de base para os diagramas [MoLIC](5-molic.md) e para os [sketches](../03-prototipacao/1-sketches.md), que devem ser coerentes com as tarefas aqui definidas.

[Voltar ao sumário](#sumario)

