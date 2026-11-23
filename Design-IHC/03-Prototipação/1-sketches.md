# Protótipos de Baixa Fidelidade (Sketches)

## 1. Introdução

Esta etapa apresenta os esboços de baixa fidelidade das telas do sistema de gerenciamento de materiais e agendamentos do Laboratório de Biologia da UFAM. Os esboços foram elaborados no Draw.io e representam telas reais do sistema, ainda **sem interação**: as setas indicam apenas o fluxo de navegação entre as telas.

As telas foram construídas a partir das [Personas](../02-ideacao/1-personas.md), da [Metamensagem](../02-ideacao/2-metamensagem.md), dos [Mapas de Objetivos](../02-ideacao/3-mapa-de-objetivos.md), dos [HTAs](../02-ideacao/4-htas.md) e dos diagramas [MoLIC](../02-ideacao/5-molic.md). Ao todo, são **17 telas**, organizadas em seis grupos.

> **Nota de terminologia:** nas telas, o professor realiza o **agendamento** do laboratório e a solicitação dos equipamentos na mesma ação, e o histórico é chamado de **requerimentos**. Nos HTAs e nos mapas, esse processo é descrito como **solicitação** ou **pedido**. Os termos se referem ao mesmo processo.

## 2. Visão geral do fluxo

![Visão geral do fluxo das telas](imagens/sketch-00-visao-geral.png)

O usuário entra pela tela de boas-vindas e faz login. Conforme o perfil, é direcionado a um dos dois hubs:

- **Professor(a):** hub do professor → agendar laboratório, acompanhar agendamentos, histórico de requerimentos.
- **Técnico(a) de laboratório:** hub da técnica → acompanhar agendamentos, cadastro de professores, controle de estoque (com saída de materiais, lançamento de perda e inventário).

Os dois perfis acessam o menu lateral e, a partir dele, as configurações de acessibilidade.

## 3. Telas

### 3.1 Entrada no sistema

| Tela | Descrição | Relação com o projeto |
|---|---|---|
| **Boas-vindas** | Saudação ao usuário, botão *Prosseguir* e botão *Ajuda* | Apresenta o sistema e oferece ajuda desde o início |
| **Login** | Campos de e-mail e senha, *Esqueci minha senha*, *Entrar* e opção de entrada alternativa (*Ou se preferir*) | Passo "Acessar o sistema", presente em todos os HTAs; cena de login do MoLIC |

![Boas-vindas](imagens/sketch-01-boas-vindas.png)
![Login](imagens/sketch-02-login.png)

### 3.2 Hubs e menus de navegação

| Tela | Descrição | Relação com o projeto |
|---|---|---|
| **Hub da técnica** | Saudação e três atalhos: *Acompanhar agendamentos*, *Cadastrar professor* e *Controle de estoque* | Ponto de partida da Persona 3 (Elisângela) |
| **Menu lateral da técnica** | Início, Acompanhar agendamentos, Cad. Professor, Controle de estoque, Configurações, Centro de Ajuda e Sair, com o perfil do usuário | Navegação consistente e ajuda sempre acessível |
| **Hub do professor** | Saudação e três atalhos: *Agendar Laboratório*, *Acompanhar agendamentos* e *Histórico de requerimentos* | Ponto de partida das Personas 1 (Camila) e 2 (Lucas) |
| **Menu lateral do professor** | Início, Acompanhar agendamentos, Histórico de requerimentos, Configurações, Centro de Ajuda e Sair, com o perfil do usuário | Mesma estrutura do menu da técnica, com as opções do professor |

![Hub da técnica](imagens/sketch-03-hub-tecnica.png)
![Menu lateral da técnica](imagens/sketch-04-menu-tecnica.png)
![Hub do professor](imagens/sketch-05-hub-professor.png)
![Menu lateral do professor](imagens/sketch-06-menu-professor.png)

### 3.3 Acessibilidade

| Tela | Descrição | Relação com o projeto |
|---|---|---|
| **Configurações > Acessibilidade** | *Zoom padrão* (100%) para aumentar ou diminuir o texto de toda a tela e opção *Texto em alto contraste* | **HTA 4** e Persona 1 (Camila): objetivos *Ampliar textos* e *Ajustar contraste e legibilidade* |

![Configurações de acessibilidade](imagens/sketch-07-acessibilidade.png)

### 3.4 Fluxo do professor

| Tela | Descrição | Relação com o projeto |
|---|---|---|
| **Agendar laboratório** | Seleção de data, turno e horário, escolha do laboratório, *Selecionar equipamentos*, campo de conteúdo da aula, aviso sobre o prazo de 48 horas e botão *Submeter agendamento* | **HTA 1**: solicitar materiais e equipamentos. Objetivos *Planejar conforme a data da aula* e *Considerar o prazo mínimo de 48 horas* |
| **Acompanhar agendamento (professor)** | Semana atual, lista de agendamentos com código, laboratório, data e hora, e aviso para ativar notificações | **HTA 2**: acompanhar o andamento de um pedido |
| **Histórico de requerimentos** | Alerta de proximidade da aula (*Faltam 4h*), filtros por disciplina e período e lista de requerimentos | **HTA 2**: consultar confirmações, atualizações e lembretes |

![Agendar laboratório](imagens/sketch-08-agendar-laboratorio.png)
![Acompanhar agendamento (professor)](imagens/sketch-09-acompanhar-professor.png)
![Histórico de requerimentos](imagens/sketch-10-historico.png)

### 3.5 Fluxo da técnica de laboratório

| Tela | Descrição | Relação com o projeto |
|---|---|---|
| **Acompanhar agendamento (técnica)** | Calendário do mês, busca, abas *Agendados*, *Próximos*, *Recentes* e *Concluídos*, e cards com código, laboratório, professor, data e hora | **HTA 5**: gerenciar solicitações recebidas |
| **Controle de estoque** | Busca, botão *Incluir*, lista de categorias (vidrarias, equipamentos, consumo e reagentes, EPIs, apoio) com ações *Edit* e *Del*, e abas *Saída de Materiais*, *Lançamento de Perda* e *Inventário do Estoque* | **HTA 6** e grupo *Controlar reposições* |
| **Inventário de estoque** | Total de itens, filtro por nome ou código, *Incluir inventário*, e cards com código, quantidade, contagem e motivo | **HTA 6**: identificar necessidades de reposição |
| **Lançamento de perda** | Data e local do inventário, itens com diferença de quantidade e motivo da perda | **HTA 6**: identificar itens indisponíveis |
| **Saída de materiais** | Data, patrimônio, botão *Incluir* e tabela com produto, estoque e quantidade | **HTA 6**: controle do estoque do laboratório |
| **Cadastro de professores** | Busca, *Incluir* e lista com nome, tipo de usuário e ações *Edit* e *Del* | Apoio ao objetivo *Consultar informações dos responsáveis* (**HTA 7**) |
| **Cadastro de professor (formulário)** | Data, matrícula, nome, e-mail, senha com regras de formação, confirmação de senha e botão *Salvar* | Complementa o cadastro de responsáveis |

![Acompanhar agendamento (técnica)](imagens/sketch-11-acompanhar-tecnica.png)
![Controle de estoque](imagens/sketch-12-controle-estoque.png)
![Inventário de estoque](imagens/sketch-13-inventario.png)
![Lançamento de perda](imagens/sketch-14-lancamento-perda.png)
![Saída de materiais](imagens/sketch-15-saida-materiais.png)
![Cadastro de professores](imagens/sketch-16-cadastro-professores.png)
![Cadastro de professor (formulário)](imagens/sketch-17-cadastro-formulario.png)

## 4. Versões alternativas das telas

O enunciado exige duas versões alternativas para algumas telas, para discutir e validar qual corresponde melhor ao modelo de interação. As telas abaixo foram escolhidas por terem papel central nos HTAs. A **Tela A** é a versão apresentada na seção 3; a **Tela B** é a alternativa.

### 4.1 Agendar laboratório (HTA 1)

| | Tela A | Tela B |
|---|---|---|
| **Estrutura** | Formulário único, com data, horário, laboratório, equipamentos e conteúdo da aula na mesma tela | Fluxo em etapas (data e horário → laboratório → equipamentos → conteúdo → revisão), uma etapa por tela |
| **Vantagem** | Visão completa e poucos passos | Menos informação por tela e etapa de revisão antes do envio (passo 5 do HTA 1) |
| **Risco** | Tela longa, difícil para quem usa ampliação de texto | Mais telas e cliques |

![Agendar laboratório – Tela A](imagens/sketch-08a-agendar-laboratorio.png)
![Agendar laboratório – Tela B](imagens/sketch-08b-agendar-laboratorio.png)

### 4.2 Acompanhar agendamento (HTA 2 e HTA 5)

| | Tela A | Tela B |
|---|---|---|
| **Estrutura** | Calendário no topo e lista de cards abaixo | Lista de cards em destaque, com filtros por status e data, sem calendário |
| **Vantagem** | Visão do período e dos dias com agendamentos | Menos elementos na tela e leitura mais direta |
| **Risco** | Calendário pequeno é difícil de ler com baixa visão | Perde a visão do mês |

![Acompanhar agendamento – Tela A](imagens/sketch-09a-acompanhar.png)
![Acompanhar agendamento – Tela B](imagens/sketch-09b-acompanhar.png)

### 4.3 Hub da técnica

| | Tela A | Tela B |
|---|---|---|
| **Estrutura** | Três atalhos em cartões | Lista de atalhos em largura total, com um resumo dos agendamentos do dia |
| **Vantagem** | Poucos elementos e leitura rápida | Mostra informação útil já na entrada |
| **Risco** | Não antecipa nenhuma informação | Tela mais carregada |

![Hub da técnica – Tela A](imagens/sketch-03a-hub-tecnica.png)
![Hub da técnica – Tela B](imagens/sketch-03b-hub-tecnica.png)

**Decisão da equipe:** [registrar aqui qual versão foi escolhida para cada tela e a justificativa].

## 5. Usabilidade, comunicabilidade e UX

| Princípio | Como aparece nas telas |
|---|---|
| **Usabilidade** (facilidade e eficiência) | Menu lateral com a mesma estrutura nos dois perfis; hubs com poucos atalhos; busca e filtros nas listas; abas de status nos agendamentos; ações de editar e excluir visíveis nas listas |
| **Comunicabilidade** (clareza da mensagem do designer) | Saudação com nome e perfil, botão de ajuda e *Centro de Ajuda* no menu, aviso sobre o prazo de 48 horas, aviso para ativar notificações, regras de senha informadas antes do preenchimento, rótulos explícitos nos botões |
| **Experiência do usuário (UX)** | Alerta de proximidade da aula (*Faltam 4h*), que reduz a ansiedade de quem planeja; acompanhamento sem precisar perguntar à equipe; opções de acessibilidade (zoom e alto contraste) que dão autonomia à persona com baixa visão |

## 6. Coerência com os HTAs e o MoLIC

| HTA | Telas relacionadas |
|---|---|
| HTA 1 – Solicitar materiais e equipamentos | Agendar laboratório (data, horário, equipamentos, conteúdo e envio) |
| HTA 2 – Acompanhar o andamento de um pedido | Acompanhar agendamento (professor) e Histórico de requerimentos |
| HTA 3 – Consultar materiais e equipamentos disponíveis | Parcial: *Selecionar equipamentos* na tela de agendamento e Controle de estoque (técnica) |
| HTA 4 – Ajustar a apresentação para facilitar a leitura | Configurações > Acessibilidade |
| HTA 5 – Gerenciar solicitações recebidas | Acompanhar agendamento (técnica) |
| HTA 6 – Identificar e solicitar reposição de materiais | Controle de estoque, Inventário, Lançamento de perda e Saída de materiais |
| HTA 7 – Consultar informações dos responsáveis | Parcial: Cadastro de professores |

As cenas do [MoLIC](../02-ideacao/5-molic.md) correspondem às telas pelo mesmo fluxo da seção 2: login, hub, e uma cena por funcionalidade.

## 7. Considerações finais

Os esboços materializam as tarefas definidas nos HTAs em telas para os dois perfis de usuário. As versões alternativas e a validação das decisões de interface orientam a próxima etapa do projeto.
