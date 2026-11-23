# Protótipos de Baixa Fidelidade (Sketches)

## 1. Introdução

Esta etapa apresenta os protótipos de baixa fidelidade das telas do
sistema de gerenciamento de materiais e agendamentos do Laboratório de
Biologia da Universidade Federal do Amazonas (UFAM). Os esboços foram
elaborados no Draw.io e representam as principais telas previstas para a
solução. Nesta etapa, as telas ainda não possuem interação implementada:
as setas presentes no material representam somente o fluxo de navegação
entre as telas.

A construção dos protótipos foi orientada pelas Personas, pela
Metamensagem, pelos Mapas de Objetivos, pelas Análises Hierárquicas de
Tarefas (HTAs) e pelos diagramas MoLIC, desenvolvidos na etapa de
ideação. Dessa forma, as telas procuram transformar os objetivos e as
tarefas identificados em uma representação visual da solução.

O conjunto apresentado contempla **17 telas**, organizadas em seis
grupos: entrada no sistema, hubs e menus, acessibilidade, fluxo do
professor e fluxo da técnica de laboratório. Também são apresentadas
versões alternativas para três telas centrais, permitindo comparar
diferentes possibilidades de organização da interface.

> **Nota de terminologia:** neste protótipo, o professor realiza o
> agendamento do laboratório e a solicitação de equipamentos em um mesmo
> processo. O histórico desse processo é denominado "Histórico de
> requerimentos". Nos HTAs e nos mapas de objetivos, podem aparecer os
> termos "solicitação" ou "pedido"; neste documento, eles representam o
> mesmo processo de interação.

## 2. Visão geral do fluxo

<img width="2840" height="2620" alt="Lab Manager Sketch drawio (3)" src="https://github.com/user-attachments/assets/569d31fa-3625-4146-a704-40463cf3e177" />


O fluxo começa na tela de boas-vindas, pela qual o usuário acessa a tela
de login. Após a autenticação, o sistema direciona o usuário ao ambiente
correspondente ao seu perfil.

-   **Professor(a):** acessa o hub do professor e pode iniciar um
    agendamento, acompanhar seus agendamentos ou consultar o histórico
    de requerimentos.
-   **Técnico(a) de laboratório:** acessa o hub da técnica e pode
    acompanhar os agendamentos recebidos, cadastrar professores e
    controlar o estoque do laboratório. No controle de estoque, estão
    disponíveis as operações de saída de materiais, lançamento de perdas
    e inventário.

Os dois perfis também possuem acesso ao menu lateral, que reúne as
opções de navegação, configurações, centro de ajuda e saída do sistema.
A partir das configurações, o usuário pode acessar os recursos de
acessibilidade.

As setas do diagrama representam a sequência prevista de navegação. Elas
não indicam que as telas já possuam funcionalidades implementadas.

## 3. Descrição das telas

### 3.1 Entrada no sistema

  -----------------------------------------------------------------------
  Tela                    Descrição               Relação com o projeto
  ----------------------- ----------------------- -----------------------
  **Boas-vindas**         Apresenta uma saudação  Introduz o sistema e
                          inicial, o botão        disponibiliza
                          **Prosseguir** e a      orientação desde o
                          opção **Ajuda**.        primeiro contato.

  **Login**               Apresenta campos de     Corresponde à tarefa de
                          e-mail e senha, opção   acessar o sistema,
                          **Esqueci minha         presente nos HTAs, e à
                          senha**, botão          cena de autenticação do
                          **Entrar** e uma        MoLIC.
                          alternativa de acesso   
                          indicada por **Ou se    
                          preferir**.             
  -----------------------------------------------------------------------

<img width="393" height="736" alt="image" src="https://github.com/user-attachments/assets/be02009f-079b-4a17-851a-3ec6e01404d2" />


<img width="465" height="905" alt="{E7773382-7509-420B-A3D9-B572C7556BC4}" src="https://github.com/user-attachments/assets/170b5e84-eb8f-457d-b0d0-e4cc02e82e71" />

### 3.2 Hubs e menus de navegação

  -----------------------------------------------------------------------
  Tela                    Descrição               Relação com o projeto
  ----------------------- ----------------------- -----------------------
  **Hub da técnica**      Apresenta uma saudação  Funciona como ponto de
                          e três atalhos          partida das tarefas da
                          principais:             persona técnica de
                          **Acompanhar            laboratório.
                          agendamentos**,         
                          **Cadastrar professor** 
                          e **Controle de         
                          estoque**.              

  **Menu lateral da       Reúne as opções Início, Mantém as opções de
  técnica**               Acompanhar              navegação acessíveis e
                          agendamentos, Cadastro  organizadas para a
                          de professores,         técnica.
                          Controle de estoque,    
                          Configurações, Centro   
                          de Ajuda e Sair, além   
                          da identificação do     
                          perfil.                 

  **Hub do professor**    Apresenta uma saudação  Reúne as tarefas
                          e três atalhos:         centrais das personas
                          **Agendar               professoras.
                          laboratório**,          
                          **Acompanhar            
                          agendamentos** e        
                          **Histórico de          
                          requerimentos**.        

  **Menu lateral do       Apresenta Início,       Mantém um padrão de
  professor**             Acompanhar              navegação semelhante ao
                          agendamentos, Histórico menu da técnica,
                          de requerimentos,       respeitando as
                          Configurações, Centro   funcionalidades de cada
                          de Ajuda e Sair, além   perfil.
                          da identificação do     
                          perfil.                 
  -----------------------------------------------------------------------

![Hub da técnica](imagens/sketch-03-hub-tecnica.png)

![Menu lateral da técnica](imagens/sketch-04-menu-tecnica.png)

![Hub do professor](imagens/sketch-05-hub-professor.png)

![Menu lateral do professor](imagens/sketch-06-menu-professor.png)

### 3.3 Acessibilidade

  -----------------------------------------------------------------------
  Tela                    Descrição               Relação com o projeto
  ----------------------- ----------------------- -----------------------
  **Configurações \>      Disponibiliza o ajuste  Relaciona-se ao HTA 4 e
  Acessibilidade**        de zoom, inicialmente   às necessidades de
                          em 100%, para aumentar  ampliar textos e
                          ou diminuir o texto, e  ajustar contraste e
                          a opção **Texto em alto legibilidade
                          contraste**.            identificadas na
                                                  persona com necessidade
                                                  de acessibilidade.

  -----------------------------------------------------------------------

![Configurações de acessibilidade](imagens/sketch-07-acessibilidade.png)

### 3.4 Fluxo do professor

  -----------------------------------------------------------------------
  Tela                    Descrição               Relação com o projeto
  ----------------------- ----------------------- -----------------------
  **Agendar laboratório** Permite selecionar      Relaciona-se ao HTA 1,
                          data, turno, horário e  que trata da
                          laboratório, selecionar solicitação de
                          equipamentos, informar  materiais e
                          o conteúdo da aula e    equipamentos, e aos
                          submeter o agendamento. objetivos de planejar a
                          Apresenta também o      aula e respeitar o
                          aviso sobre o prazo     prazo de antecedência.
                          mínimo de 48 horas.     

  **Acompanhar            Apresenta a semana      Relaciona-se ao HTA 2,
  agendamento             atual e uma lista de    permitindo acompanhar o
  (professor)**           agendamentos com        andamento dos pedidos.
                          código, laboratório,    
                          data e horário. Também  
                          informa sobre a         
                          ativação das            
                          notificações.           

  **Histórico de          Apresenta um alerta de  Complementa o HTA 2,
  requerimentos**         proximidade da aula,    permitindo consultar
                          como **Faltam 4h**,     registros,
                          filtros por disciplina  confirmações,
                          e período e uma lista   atualizações e
                          dos requerimentos       lembretes.
                          realizados.             
  -----------------------------------------------------------------------

![Agendar laboratório](imagens/sketch-08-agendar-laboratorio.png)

![Acompanhar agendamento
(professor)](imagens/sketch-09-acompanhar-professor.png)

![Histórico de requerimentos](imagens/sketch-10-historico.png)

### 3.5 Fluxo da técnica de laboratório

  -----------------------------------------------------------------------
  Tela                    Descrição               Relação com o projeto
  ----------------------- ----------------------- -----------------------
  **Acompanhar            Apresenta calendário    Relaciona-se ao HTA 5,
  agendamento (técnica)** mensal, campo de busca, que descreve o
                          abas **Agendados**,     gerenciamento das
                          **Próximos**,           solicitações recebidas.
                          **Recentes** e          
                          **Concluídos**, além de 
                          cards com código,       
                          laboratório, professor, 
                          data e horário.         

  **Controle de estoque** Apresenta busca, opção  Funciona como ponto
                          **Incluir**, categorias central das tarefas de
                          de materiais e ações de controle de materiais
                          edição e exclusão.      previstas no HTA 6.
                          Também reúne as áreas   
                          **Saída de Materiais**, 
                          **Lançamento de Perda** 
                          e **Inventário do       
                          Estoque**.              

  **Inventário de         Apresenta o total de    Relaciona-se ao HTA 6,
  estoque**               itens, filtro por nome  permitindo comparar
                          ou código, opção        quantidades registradas
                          **Incluir inventário**  e contadas e
                          e registros com código, identificar diferenças.
                          quantidade, contagem e  
                          motivo.                 

  **Lançamento de perda** Apresenta os dados de   Relaciona-se ao HTA 6,
                          data e local do         permitindo registrar
                          inventário, itens com   perdas e atualizar o
                          diferença de quantidade controle dos materiais.
                          e campo para informar o 
                          motivo da perda.        

  **Saída de materiais**  Apresenta data,         Relaciona-se ao
                          identificação           controle de
                          patrimonial, opção      movimentação dos
                          **Incluir** e tabela    materiais do
                          com produto, estoque    laboratório.
                          disponível e quantidade 
                          retirada.               

  **Cadastro de           Apresenta busca, opção  Apoia a consulta e a
  professores**           **Incluir** e lista de  manutenção das
                          professores com nome,   informações dos
                          tipo de usuário e ações responsáveis,
                          de editar e excluir.    relacionada ao HTA 7.

  **Cadastro de professor Apresenta campos para   Complementa o cadastro
  (formulário)**          data, matrícula, nome,  e a manutenção dos
                          e-mail, senha e         responsáveis pelo uso
                          confirmação de senha,   do sistema.
                          além das regras de      
                          formação da senha e do  
                          botão **Salvar**.       
  -----------------------------------------------------------------------

![Acompanhar agendamento
(técnica)](imagens/sketch-11-acompanhar-tecnica.png)

![Controle de estoque](imagens/sketch-12-controle-estoque.png)

![Inventário de estoque](imagens/sketch-13-inventario.png)

![Lançamento de perda](imagens/sketch-14-lancamento-perda.png)

![Saída de materiais](imagens/sketch-15-saida-materiais.png)

![Cadastro de professores](imagens/sketch-16-cadastro-professores.png)

![Cadastro de professor
(formulário)](imagens/sketch-17-cadastro-formulario.png)

## 4. Versões alternativas das telas

O enunciado do TP2 solicita a elaboração de versões alternativas para
algumas telas, com o objetivo de discutir possibilidades de interface e
verificar qual delas apresenta melhor correspondência com o modelo de
interação. Nesta seção, a **Tela A** corresponde à versão principal
apresentada na seção 3, enquanto a **Tela B** representa uma alternativa
de organização.

### 4.1 Agendar laboratório (HTA 1)

  -----------------------------------------------------------------------
  Critério                Tela A                  Tela B
  ----------------------- ----------------------- -----------------------
  **Estrutura**           Formulário único com    Fluxo dividido em
                          data, horário,          etapas: data e horário,
                          laboratório,            laboratório,
                          equipamentos e conteúdo equipamentos, conteúdo
                          da aula na mesma tela.  e revisão.

  **Vantagem**            Permite visualizar as   Reduz a quantidade de
                          informações em um único informações
                          lugar e concluir o      apresentadas
                          preenchimento sem       simultaneamente e
                          avançar por várias      inclui uma etapa de
                          telas.                  revisão antes do envio.

  **Risco**               Pode resultar em uma    Exige mais etapas e
                          tela extensa,           navegação entre telas,
                          dificultando a leitura  podendo aumentar o
                          e o preenchimento,      tempo de conclusão.
                          especialmente com       
                          ampliação de texto.     
  -----------------------------------------------------------------------

![Agendar laboratório -- Tela
A](imagens/sketch-08a-agendar-laboratorio.png)

![Agendar laboratório -- Tela
B](imagens/sketch-08b-agendar-laboratorio.png)

**Proposta de decisão:** escolher a **Tela B**. A divisão por etapas
organiza o preenchimento e permite que o professor confira os dados
antes de submeter o agendamento. Essa estrutura também reduz a
sobrecarga visual em cada etapa, aspecto relevante para a
acessibilidade. Para evitar que a navegação adicional prejudique a
eficiência, recomenda-se indicar claramente a etapa atual e permitir
retornar às etapas anteriores sem perder os dados preenchidos.

### 4.2 Acompanhar agendamento (HTA 2 e HTA 5)

  -----------------------------------------------------------------------
  Critério                Tela A                  Tela B
  ----------------------- ----------------------- -----------------------
  **Estrutura**           Calendário na parte     Lista de cards em
                          superior e lista de     destaque, com filtros
                          cards abaixo.           por status e data, sem
                                                  calendário.

  **Vantagem**            Permite visualizar o    Dá maior destaque às
                          período e identificar   informações dos
                          os dias que possuem     agendamentos e oferece
                          agendamentos.           leitura mais direta.

  **Risco**               Um calendário pequeno   Não apresenta a visão
                          pode dificultar a       mensal dos
                          leitura e a seleção de  agendamentos, exigindo
                          datas por pessoas com   o uso dos filtros para
                          baixa visão.            localizar períodos.
  -----------------------------------------------------------------------

![Acompanhar agendamento -- Tela A](imagens/sketch-09a-acompanhar.png)

![Acompanhar agendamento -- Tela B](imagens/sketch-09b-acompanhar.png)

**Proposta de decisão:** escolher a **Tela B**. A lista de cards com
filtros prioriza as informações mais relevantes para acompanhar cada
solicitação, como status, laboratório, professor, data e horário. A
ausência do calendário reduz a quantidade de elementos simultâneos e
favorece a leitura. Os filtros por data preservam a possibilidade de
localizar agendamentos de períodos específicos.

### 4.3 Hub da técnica

  -----------------------------------------------------------------------
  Critério                Tela A                  Tela B
  ----------------------- ----------------------- -----------------------
  **Estrutura**           Apresenta três atalhos  Apresenta os atalhos em
                          em cartões.             uma lista de largura
                                                  maior e inclui um
                                                  resumo dos agendamentos
                                                  do dia.

  **Vantagem**            Possui poucos elementos Antecipadamente,
                          e permite identificar   oferece informações
                          rapidamente as três     sobre os agendamentos
                          funcionalidades         do dia, além dos
                          principais.             atalhos de navegação.

  **Risco**               Não apresenta           Pode concentrar
                          informações             informações demais na
                          operacionais antes de o tela inicial e aumentar
                          usuário acessar a área  a carga visual.
                          de agendamentos.        
  -----------------------------------------------------------------------

![Hub da técnica -- Tela A](imagens/sketch-03a-hub-tecnica.png)

![Hub da técnica -- Tela B](imagens/sketch-03b-hub-tecnica.png)

**Proposta de decisão:** escolher a **Tela A**. O hub funciona como
ponto inicial de navegação e deve facilitar o acesso às três tarefas
principais da técnica. Os cartões mantêm a interface objetiva, com menor
quantidade de informações simultâneas. Os detalhes dos agendamentos
podem ser consultados na tela específica de acompanhamento.

### 4.4 Síntese das decisões propostas

  -----------------------------------------------------------------------
  Tela analisada          Versão recomendada      Justificativa principal
  ----------------------- ----------------------- -----------------------
  Agendar laboratório     **Tela B**              Organização por etapas,
                                                  revisão antes do envio
                                                  e menor sobrecarga
                                                  visual por tela.

  Acompanhar agendamento  **Tela B**              Maior destaque às
                                                  informações e filtros
                                                  que facilitam a
                                                  localização dos
                                                  registros.

  Hub da técnica          **Tela A**              Navegação direta e
                                                  apresentação objetiva
                                                  das tarefas principais.
  -----------------------------------------------------------------------

> **Atenção:** as escolhas acima são recomendações fundamentadas na
> análise das alternativas e nos objetivos documentados. Antes da
> entrega, a equipe deve confirmar se essas decisões correspondem ao que
> foi efetivamente discutido e validado pelos integrantes. Não se deve
> apresentar uma validação com usuários como realizada caso ela não
> tenha acontecido.

## 5. Usabilidade, comunicabilidade e experiência do usuário

Os protótipos consideram os princípios de usabilidade, comunicabilidade
e experiência do usuário solicitados no enunciado do TP2.

  -----------------------------------------------------------------------
  Princípio                           Aplicação nos protótipos
  ----------------------------------- -----------------------------------
  **Usabilidade**                     Os hubs apresentam atalhos para as
                                      tarefas mais frequentes; os menus
                                      mantêm uma estrutura consistente
                                      entre os perfis; as listas utilizam
                                      busca e filtros; e as abas
                                      organizam os agendamentos por
                                      situação.

  **Comunicabilidade**                Os rótulos dos botões indicam suas
                                      ações; as telas identificam o
                                      perfil do usuário; os avisos
                                      explicam o prazo de antecedência e
                                      a importância das notificações; e o
                                      formulário de cadastro apresenta as
                                      regras de senha antes do
                                      preenchimento.

  **Experiência do usuário (UX)**     O acompanhamento dos agendamentos
                                      reduz a necessidade de procurar
                                      informações diretamente com a
                                      equipe; os alertas de proximidade
                                      da aula ajudam o professor a se
                                      preparar; e os recursos de zoom e
                                      alto contraste oferecem maior
                                      autonomia a pessoas com
                                      necessidades de acessibilidade.
  -----------------------------------------------------------------------

Essas escolhas representam intenções de design presentes nos esboços.
Como se trata de protótipos de baixa fidelidade e sem interação
implementada, sua eficácia ainda deverá ser verificada em etapas
posteriores de avaliação.

## 6. Coerência com os HTAs e o MoLIC

As telas foram organizadas para representar as tarefas identificadas nos
HTAs e as cenas previstas nos diagramas MoLIC. A correspondência está
resumida a seguir.

  -----------------------------------------------------------------------
  HTA                     Tarefa/objetivo         Telas relacionadas
  ----------------------- ----------------------- -----------------------
  **HTA 1 -- Solicitar    Planejar o uso do       Agendar laboratório,
  materiais e             laboratório e solicitar incluindo data,
  equipamentos**          os materiais            horário, laboratório,
                          necessários.            equipamentos, conteúdo
                                                  da aula e envio.

  **HTA 2 -- Acompanhar o Consultar a situação e  Acompanhar agendamento
  andamento de um         as informações de um    (professor) e Histórico
  pedido**                requerimento.           de requerimentos.

  **HTA 3 -- Consultar    Verificar a             Seleção de equipamentos
  materiais e             disponibilidade antes   no fluxo de agendamento
  equipamentos            de concluir a           e informações de
  disponíveis**           solicitação.            estoque. **Cobertura
                                                  parcial nos esboços
                                                  apresentados.**

  **HTA 4 -- Ajustar a    Modificar a             Configurações \>
  apresentação para       apresentação visual     Acessibilidade.
  facilitar a leitura**   conforme a necessidade  
                          de leitura.             

  **HTA 5 -- Gerenciar    Consultar e organizar   Acompanhar agendamento
  solicitações            os agendamentos         (técnica).
  recebidas**             recebidos pela equipe   
                          técnica.                

  **HTA 6 -- Identificar  Controlar               Controle de estoque,
  e solicitar reposição   movimentações,          Inventário de estoque,
  de materiais**          registrar perdas e      Lançamento de perda e
                          identificar diferenças  Saída de materiais.
                          no estoque.             

  **HTA 7 -- Consultar    Localizar e manter os   Cadastro de professores
  informações dos         dados dos professores   e Cadastro de professor
  responsáveis**          responsáveis.           (formulário).
                                                  **Cobertura parcial se
                                                  o HTA exigir apenas
                                                  consulta de dados.**
  -----------------------------------------------------------------------

As cenas do MoLIC devem corresponder às telas pelo fluxo de interação:
entrada e login, direcionamento ao hub conforme o perfil e acesso às
funcionalidades específicas. As transições entre cenas devem refletir as
possibilidades de navegação representadas pelas setas do fluxo geral.

A correspondência entre os artefatos deve ser conferida em conjunto:
cada tarefa detalhada no HTA precisa estar representada no fluxo de
interação e possuir uma tela ou conjunto de telas que dê suporte à sua
realização. Quando a cobertura for parcial, essa limitação deve
permanecer explícita, sem afirmar que a funcionalidade está
completamente representada.

## 7. Considerações finais

Os protótipos de baixa fidelidade materializam, em representações
visuais, as principais tarefas identificadas durante as etapas de
imersão e ideação. A separação das funcionalidades por perfil permite
organizar o acesso às atividades do professor e da técnica de
laboratório, enquanto os menus e os recursos de acessibilidade procuram
oferecer uma navegação consistente e adaptável.

A apresentação de versões alternativas possibilita comparar diferentes
estruturas de interface e justificar escolhas considerando a facilidade
de uso, a clareza das informações e a experiência dos usuários. As
recomendações apresentadas nesta documentação devem ser confirmadas pela
equipe e, quando possível, submetidas à avaliação dos usuários.

Como continuidade do projeto, recomenda-se revisar a cobertura dos HTAs
3 e 7, conferir a correspondência entre todas as telas e as cenas do
MoLIC e avançar para a etapa de prototipação com maior fidelidade e
avaliação da interação.
