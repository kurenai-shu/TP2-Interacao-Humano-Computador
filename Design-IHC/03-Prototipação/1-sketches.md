# Protótipos de Baixa Fidelidade (Sketches)

## 1. Introdução

Esta etapa apresenta os protótipos de baixa fidelidade das telas do sistema de gerenciamento de materiais e agendamentos do Laboratório de Biologia da Universidade Federal do Amazonas (UFAM). Os esboços foram elaborados no Draw.io e representam as principais telas previstas para a solução. Nesta etapa, as telas ainda não possuem interação implementada: as setas presentes no material representam somente o fluxo de navegação entre as telas.

A construção dos protótipos foi orientada pelas Personas, pela Metamensagem, pelos Mapas de Objetivos, pelas Análises Hierárquicas de Tarefas (HTAs) e pelos diagramas MoLIC, desenvolvidos na etapa de ideação. Dessa forma, as telas procuram transformar os objetivos e as tarefas identificados em uma representação visual da solução.

O conjunto apresentado contempla **17 telas**, organizadas em seis grupos: entrada no sistema, hubs e menus, acessibilidade, fluxo do professor e fluxo da técnica de laboratório. Também são apresentadas versões alternativas para três telas centrais, permitindo comparar diferentes possibilidades de organização da interface.

> **Nota de terminologia:** neste protótipo, o professor realiza o agendamento do laboratório e a solicitação de equipamentos em um mesmo processo. O histórico desse processo é denominado *"Histórico de requerimentos"*. Nos HTAs e nos mapas de objetivos, podem aparecer os termos *"solicitação"* ou *"pedido"*; neste documento, eles representam o mesmo processo de interação.

---

## 2. Visão geral do fluxo

<img width="2840" height="2620" alt="Lab Manager Sketch drawio (3)" src="https://github.com/user-attachments/assets/569d31fa-3625-4146-a704-40463cf3e177" />

O fluxo começa na tela de boas-vindas, pela qual o usuário acessa a tela de login. Após a autenticação, o sistema direciona o usuário ao ambiente correspondente ao seu perfil.

* **Professor(a):** acessa o hub do professor e pode iniciar um agendamento, acompanhar seus agendamentos ou consultar o histórico de requerimentos.
* **Técnico(a) de laboratório:** acessa o hub da técnica e pode acompanhar os agendamentos recebidos, cadastrar professores e controlar o estoque do laboratório. No controle de estoque, estão disponíveis as operações de saída de materiais, lançamento de perdas e inventário.

Os dois perfis também possuem acesso ao menu lateral, que reúne as opções de navegação, configurações, centro de ajuda e saída do sistema. A partir das configurações, o usuário pode acessar os recursos de acessibilidade.

As setas do diagrama representam a sequência prevista de navegação. Elas não indicam que as telas já possuam funcionalidades implementadas.

---

## 3. Descrição das telas

### 3.1 Entrada no sistema

| Tela | Descrição | Relação com o projeto |
| :--- | :--- | :--- |
| **Boas-vindas** | Apresenta uma saudação inicial, o botão **Prosseguir** e a opção **Ajuda**. | Introduz o sistema e disponibiliza orientação desde o primeiro contato. |
| **Login** | Apresenta campos de e-mail e senha, opção **Esqueci minha senha**, botão **Entrar** e uma alternativa de acesso indicada por **Ou se preferir**. | Corresponde à tarefa de acessar o sistema, presente nos HTAs, e à cena de autenticação do MoLIC. |

<img height="730" alt="image" src="https://github.com/user-attachments/assets/be02009f-079b-4a17-851a-3ec6e01404d2" />

<img height="730" alt="{E7773382-7509-420B-A3D9-B572C7556BC4}" src="https://github.com/user-attachments/assets/170b5e84-eb8f-457d-b0d0-e4cc02e82e71" />

### 3.2 Hubs e menus de navegação

| Tela | Descrição | Relação com o projeto |
| :--- | :--- | :--- |
| **Hub da técnica** | Apresenta uma saudação e três atalhos principais: **Acompanhar agendamentos**, **Cadastrar professor** e **Controle de estoque**. | Funciona como ponto de partida das tarefas da persona técnica de laboratório. |
| **Menu lateral da técnica** | Reúne as opções **Início**, **Acompanhar agendamentos**, **Cadastro de professores**, **Controle de estoque**, **Configurações**, **Centro de Ajuda** e **Sair**, além da identificação do perfil. | Mantém as opções de navegação acessíveis e organizadas para a técnica. |
| **Hub do professor** | Apresenta uma saudação e três atalhos: **Agendar laboratório**, **Acompanhar agendamentos** e **Histórico de requerimentos**. | Reúne as tarefas centrais das personas professoras. |
| **Menu lateral do professor** | Apresenta **Início**, **Acompanhar agendamentos**, **Histórico de requerimentos**, **Configurações**, **Centro de Ajuda** e **Sair**, além da identificação do perfil. | Mantém um padrão de navegação semelhante ao menu da técnica, respeitando as funcionalidades de cada perfil. |

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/ccb9d620-8091-4329-a3b5-3142c68dc011" alt="Hub da técnica" width="250" /><br>
      <sub><b>Hub da técnica</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/d2c7e75f-406e-4661-be7a-8c1d8b6452d5" alt="Menu lateral da técnica" width="250" /><br>
      <sub><b>Menu lateral da técnica</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/74905b35-a9e2-4e5f-ad7a-f9ce300bbe52" alt="Hub do professor" width="250" /><br>
      <sub><b>Hub do professor</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/faaefacc-6137-4d88-abee-dba24054954e" alt="Menu lateral do professor" width="250" /><br>
      <sub><b>Menu lateral do professor</b></sub>
    </td>
  </tr>
</table>

### 3.3 Acessibilidade

| Tela | Descrição | Relação com o projeto |
| :--- | :--- | :--- |
| **Configurações > Acessibilidade** | Disponibiliza o ajuste de zoom, inicialmente em **100%**, para aumentar ou diminuir o texto, e a opção **Texto em alto contraste**. | Relaciona-se ao HTA 4 e às necessidades de ampliar textos e ajustar contraste e legibilidade identificadas na persona com necessidade de acessibilidade. |

![Configurações de acessibilidade](imagens/sketch-07-acessibilidade.png)

<img width="831" height="1600" alt="WhatsApp Image 2026-11-23 at 6 50 25 PM (2)" src="https://github.com/user-attachments/assets/aaab482d-519e-4efc-bda8-442612e5c175" />

### 3.4 Fluxo do professor

| Tela | Descrição | Relação com o projeto |
| :--- | :--- | :--- |
| **Agendar laboratório** | Permite selecionar data, turno, horário e laboratório, selecionar equipamentos, informar o conteúdo da aula e submeter o agendamento. Apresenta também o aviso sobre o prazo mínimo de **48 horas**. | Relaciona-se ao HTA 1, que trata da solicitação de materiais e equipamentos, e aos objetivos de planejar a aula e respeitar o prazo de antecedência. |
| **Acompanhar agendamento (professor)** | Apresenta a semana atual e uma lista de agendamentos com código, laboratório, data e horário. Também informa sobre a ativação das notificações. | Relaciona-se ao HTA 2, permitindo acompanhar o andamento dos pedidos. |
| **Histórico de requerimentos** | Apresenta um alerta de proximidade da aula, como **Faltam 4h**, filtros por disciplina e período e uma lista dos requerimentos realizados. | Complementa o HTA 2, permitindo consultar registros, confirmações, atualizações e lembretes. |

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/8cc6ccc7-07a9-463e-b405-4f599c9e9de1" alt="Agendar laboratório" width="250" /><br>
      <sub><b>Agendar laboratório</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/d6461ea8-1bea-4458-9257-12081ae3fe93" alt="Acompanhar agendamento (professor)" width="250" /><br>
      <sub><b>Acompanhar agendamento (professor)</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/cd34c779-f0cb-4e4b-a51d-e3ffb3e40d62" alt="Histórico de requerimentos" width="250" /><br>
      <sub><b>Histórico de requerimentos</b></sub>
    </td>
  </tr>
</table>


### 3.5 Fluxo da técnica de laboratório

| Tela | Descrição | Relação com o projeto |
| :--- | :--- | :--- |
| **Acompanhar agendamento (técnica)** | Apresenta calendário mensal, campo de busca, abas **Agendados**, **Próximos**, **Recentes** e **Concluídos**, além de cards com código, laboratório, professor, data e horário. | Relaciona-se ao HTA 5, que descreve o gerenciamento das solicitações recebidas. |
| **Controle de estoque** | Apresenta busca, opção **Incluir**, categorias de materiais e ações de edição e exclusão. Também reúne as áreas **Saída de Materiais**, **Lançamento de Perda** e **Inventário do Estoque**. | Funciona como ponto central das tarefas de controle de materiais previstas no HTA 6. |
| **Inventário de estoque** | Apresenta o total de itens, filtro por nome ou código, opção **Incluir inventário** e registros com código, quantidade, contagem e motivo. | Relaciona-se ao HTA 6, permitindo comparar quantidades registradas e contadas e identificar diferenças. |
| **Lançamento de perda** | Apresenta os dados de data e local do inventário, itens com diferença de quantidade e campo para informar o motivo da perda. | Relaciona-se ao HTA 6, permitindo registrar perdas e atualizar o controle dos materiais. |
| **Saída de materiais** | Apresenta data, identificação patrimonial, opção **Incluir** e tabela com produto, estoque disponível e quantidade retirada. | Relaciona-se ao controle de movimentação dos materiais do laboratório. |
| **Cadastro de professores** | Apresenta busca, opção **Incluir** e lista de professores com nome, tipo de usuário e ações de editar e excluir. | Apoia a consulta e a manutenção das informações dos responsáveis, relacionada ao HTA 7. |
| **Cadastro de professor (formulário)** | Apresenta campos para data, matrícula, nome, e-mail, senha e confirmação de senha, além das regras de formação da senha e do botão **Salvar**. | Complementa o cadastro e a manutenção dos responsáveis pelo uso do sistema. |

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/ecc0e454-87ed-465d-9a3e-e7410e7bb6aa" alt="Acompanhar agendamento (técnica)" width="250" /><br>
      <sub><b>Acompanhar agendamento (técnica)</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/cb090386-1770-4c49-bfdf-1950e13227d4" alt="Controle de estoque" width="250" /><br>
      <sub><b>Controle de estoque</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/b44711d9-b397-48f2-beaa-a2d0e020c6f5" alt="Inventário de estoque" width="250" /><br>
      <sub><b>Inventário de estoque</b></sub>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/3b749845-3f88-4c40-a0e0-aa7f2670d6fa" alt="Lançamento de perda" width="250" /><br>
      <sub><b>Lançamento de perda</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/0f5930a5-449c-4d34-ada1-dd1ee937e425" alt="Saída de materiais" width="250" /><br>
      <sub><b>Saída de materiais</b></sub>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/04323a17-6397-4a54-9b73-eb5d0ded3689" alt="Cadastro de professores" width="250" /><br>
      <sub><b>Cadastro de professores</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/30b523a1-6db0-499d-876f-e9b241e705f8" alt="Cadastro de professor (formulário)" width="250" /><br>
      <sub><b>Cadastro de professor (formulário)</b></sub>
    </td>
  </tr>
</table>

---

## 4. Versões alternativas das telas

O enunciado do TP2 solicita a elaboração de versões alternativas para algumas telas, com o objetivo de discutir possibilidades de interface e verificar qual delas apresenta melhor correspondência com o modelo de interação. Nesta seção, a **Tela A** corresponde à versão principal apresentada na seção 3, enquanto a **Tela B** representa uma alternativa de organização.

### 4.1 Agendar laboratório (HTA 1)

| Critério | Tela A | Tela B |
| :--- | :--- | :--- |
| **Estrutura** | Formulário único com data, horário, laboratório, equipamentos e conteúdo da aula na mesma tela. | Fluxo dividido em etapas: data e horário, laboratório, equipamentos, conteúdo e revisão. |
| **Vantagem** | Permite visualizar as informações em um único lugar e concluir o preenchimento sem avançar por várias telas. | Reduz a quantidade de informações apresentadas simultaneamente e inclui uma etapa de revisão antes do envio. |
| **Risco** | Pode resultar em uma tela extensa, dificultando a leitura e o preenchimento, especialmente com ampliação de texto. | Exige mais etapas e navegação entre telas, podendo aumentar o tempo de conclusão. |

<table>
  <tr>
    <td align="center">
      <img width="280" alt="Agendar laboratório -- Tela A" src="https://github.com/user-attachments/assets/55b89112-5ee6-4f27-a1ab-553df54981c4" /><br>
      <sub><b>Agendar laboratório -- Tela A</b></sub>
    </td>
    <td align="center">
      <img width="300" alt="Agendar laboratório -- Tela B" src="https://github.com/user-attachments/assets/8fd61b53-562e-484a-b825-0deb2d9eba0d" /><br>
      <sub><b>Agendar laboratório -- Tela B</b></sub>
    </td>
  </tr>
</table>

> **Proposta de decisão:** escolher a **Tela B**. A divisão por etapas organiza o preenchimento e permite que o professor confira os dados antes de submeter o agendamento. Essa estrutura também reduz a sobrecarga visual em cada etapa, aspecto relevante para a acessibilidade. Para evitar que a navegação adicional prejudique a eficiência, recomenda-se indicar claramente a etapa atual e permitir retornar às etapas anteriores sem perder os dados preenchidos.

### 4.2 Acompanhar agendamento (HTA 2 e HTA 5)

| Critério | Tela A | Tela B |
| :--- | :--- | :--- |
| **Estrutura** | Calendário na parte superior e lista de cards abaixo. | Lista de cards em destaque, com filtros por status e data, sem calendário. |
| **Vantagem** | Permite visualizar o período e identificar os dias que possuem agendamentos. | Dá maior destaque às informações dos agendamentos e oferece leitura mais direta. |
| **Risco** | Um calendário pequeno pode dificultar a leitura e a seleção de datas por pessoas com baixa visão. | Não apresenta a visão mensal dos agendamentos, exigindo o uso dos filtros para localizar períodos. |

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/114fa345-9d63-4bba-9d64-dcf0602b3a97" alt="Acompanhar agendamento -- Tela A" width="280" /><br>
      <sub><b>Acompanhar agendamento -- Tela A</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/4782a83f-913e-4989-883c-89c14b8c5e6f" alt="Acompanhar agendamento -- Tela B" width="300" /><br>
      <sub><b>Acompanhar agendamento -- Tela B</b></sub>
    </td>
  </tr>
</table>

> **Proposta de decisão:** escolher a **Tela B**. A lista de cards com filtros prioriza as informações mais relevantes para acompanhar cada solicitação, como status, laboratório, professor, data e horário. A ausência do calendário reduz a quantidade de elementos simultâneos e favorece a leitura. Os filtros por data preservam a possibilidade de localizar agendamentos de períodos específicos.

### 4.3 Hub da técnica

| Critério | Tela A | Tela B |
| :--- | :--- | :--- |
| **Estrutura** | Apresenta três atalhos em cartões. | Apresenta os atalhos em uma lista de largura maior e inclui um resumo dos agendamentos do dia. |
| **Vantagem** | Possui poucos elementos e permite identificar rapidamente as três funcionalidades principais. | Antecipadamente, oferece informações sobre os agendamentos do dia, além dos atalhos de navegação. |
| **Risco** | Não apresenta informações operacionais antes de o usuário acessar a área de agendamentos. | Pode concentrar informações demais na tela inicial e aumentar a carga visual. |

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/b9b75e4e-94b0-4671-9f49-e74aa23d48a0" alt="Hub da técnica -- Tela A" width="280" /><br>
      <sub><b>Hub da técnica -- Tela A</b></sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/5c05b5cf-15d1-4332-aaac-08365f4460c1" alt="Hub da técnica -- Tela B" width="280" /><br>
      <sub><b>Hub da técnica -- Tela B</b></sub>
    </td>
  </tr>
</table>

> **Proposta de decisão:** escolher a **Tela A**. O hub funciona como ponto inicial de navegação e deve facilitar o acesso às três tarefas principais da técnica. Os cartões mantêm a interface objetiva, com menor quantidade de informações simultâneas. Os detalhes dos agendamentos podem ser consultados na tela específica de acompanhamento.

### 4.4 Síntese das decisões propostas

| Tela analisada | Versão recomendada | Justificativa principal |
| :--- | :--- | :--- |
| **Agendar laboratório** | **Tela B** | Organização por etapas, revisão antes do envio e menor sobrecarga visual por tela. |
| **Acompanhar agendamento** | **Tela B** | Maior destaque às informações e filtros que facilitam a localização dos registros. |
| **Hub da técnica** | **Tela A** | Navegação direta e apresentação objetiva das tarefas principais. |

> **Atenção:** as escolhas acima são recomendações fundamentadas na análise das alternativas e nos objetivos documentados. Antes da entrega, a equipe deve confirmar se essas decisões correspondem ao que foi efetivamente discutido e validado pelos integrantes. Não se deve apresentar uma validação com usuários como realizada caso ela não tenha acontecido.

---

## 5. Usabilidade, comunicabilidade e experiência do usuário

Os protótipos consideram os princípios de usabilidade, comunicabilidade e experiência do usuário solicitados no enunciado do TP2.

| Princípio | Aplicação nos protótipos |
| :--- | :--- |
| **Usabilidade** | Os hubs apresentam atalhos para as tarefas mais frequentes; os menus mantêm uma estrutura consistente entre os perfis; as listas utilizam busca e filtros; e as abas organizam os agendamentos por situação. |
| **Comunicabilidade** | Os rótulos dos botões indicam suas ações; as telas identificam o perfil do usuário; os avisos explicam o prazo de antecedência e a importância das notificações; e o formulário de cadastro apresenta as regras de senha antes do preenchimento. |
| **Experiência do usuário (UX)** | O acompanhamento dos agendamentos reduz a necessidade de procurar informações diretamente com a equipe; os alertas de proximidade da aula ajudam o professor a se preparar; e os recursos de zoom e alto contraste oferecem maior autonomia a pessoas com necessidades de acessibilidade. |

Essas escolhas representam intenções de design presentes nos esboços. Como se trata de protótipos de baixa fidelidade e sem interação implementada, sua eficácia ainda deverá ser verificada em etapas posteriores de avaliação.

---

## 6. Coerência com os HTAs e o MoLIC

As telas foram organizadas para representar as tarefas identificadas nos HTAs e as cenas previstas nos diagramas MoLIC. A correspondência está resumida a seguir.

| HTA | Tarefa / objetivo | Telas relacionadas |
| :--- | :--- | :--- |
| **HTA 1 — Solicitar materiais e equipamentos** | Planejar o uso do laboratório e solicitar os materiais necessários. | **Agendar laboratório**, incluindo data, horário, laboratório, equipamentos, conteúdo da aula e envio. |
| **HTA 2 — Acompanhar o andamento de um pedido** | Consultar a situação e as informações de um requerimento. | **Acompanhar agendamento (professor)** e **Histórico de requerimentos**. |
| **HTA 3 — Consultar materiais e equipamentos disponíveis** | Verificar a disponibilidade antes de concluir a solicitação. | Seleção de equipamentos no fluxo de agendamento e informações de estoque. **Cobertura parcial nos esboços apresentados.** |
| **HTA 4 — Ajustar a apresentação para facilitar a leitura** | Modificar a apresentação visual conforme a necessidade de leitura. | **Configurações > Acessibilidade**. |
| **HTA 5 — Gerenciar solicitações recebidas** | Consultar e organizar os agendamentos recebidos pela equipe técnica. | **Acompanhar agendamento (técnica)**. |
| **HTA 6 — Identificar e solicitar reposição de materiais** | Controlar movimentações, registrar perdas e identificar diferenças no estoque. | **Controle de estoque**, **Inventário de estoque**, **Lançamento de perda** e **Saída de materiais**. |
| **HTA 7 — Consultar informações dos responsáveis** | Localizar e manter os dados dos professores responsáveis. | **Cadastro de professores** e **Cadastro de professor (formulário)**. **Cobertura parcial se o HTA exigir apenas consulta de dados.** |

As cenas do MoLIC devem corresponder às telas pelo fluxo de interação: entrada e login, direcionamento ao hub conforme o perfil e acesso às funcionalidades específicas. As transições entre cenas devem refletir as possibilidades de navegação representadas pelas setas do fluxo geral.

A correspondência entre os artefatos deve ser conferida em conjunto: cada tarefa detalhada no HTA precisa estar representada no fluxo de interação e possuir uma tela ou conjunto de telas que dê suporte à sua realização. Quando a cobertura for parcial, essa limitação deve permanecer explícita, sem afirmar que a funcionalidade está completamente representada.

---

## 7. Considerações finais

Os protótipos de baixa fidelidade materializam, em representações visuais, as principais tarefas identificadas durante as etapas de imersão e ideação. A separação das funcionalidades por perfil permite organizar o acesso às atividades do professor e da técnica de laboratório, enquanto os menus e os recursos de acessibilidade procuram oferecer uma navegação consistente e adaptável.

A apresentação de versões alternativas possibilita comparar diferentes estruturas de interface e justificar escolhas considerando a facilidade de uso, a clareza das informações e a experiência dos usuários. As recomendações apresentadas nesta documentação devem ser confirmadas pela equipe e, quando possível, submetidas à avaliação dos usuários.

Como continuidade do projeto, recomenda-se revisar a cobertura dos HTAs 3 e 7, conferir a correspondência entre todas as telas e as cenas do MoLIC e avançar para a etapa de prototipação com maior fidelidade e avaliação da interação.
