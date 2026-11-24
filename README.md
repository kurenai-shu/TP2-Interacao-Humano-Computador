# TP2 – Interação Humano-Computador (IHC)

<p align="center"><strong>Lab Manager</strong></p>
<p align="center">Sistema de gerenciamento de materiais e agendamentos do Laboratório de Biologia</p>

**Instituição:** Universidade Federal do Amazonas (UFAM) – Instituto de Ciências Exatas e Tecnologia (ICET)  
**Disciplina:** Interação Humano-Computador (IHC)  
**Trabalho:** Trabalho Prático 2 (TP2)  
**Ano:** 2026

## Integrantes

- Bruno Gomes
- Davi Marques
- Emanuel Queiroz
- Guilherme Alencar
- Kairlly Magalhães
- Sergio Roberto

---

## 1. Apresentação do sistema

O **Lab Manager** é uma proposta de sistema para centralizar a solicitação de materiais e equipamentos, o agendamento de aulas práticas e o acompanhamento de pedidos no Laboratório de Biologia da UFAM.

O projeto busca facilitar a rotina dos professores e da equipe técnica, reduzindo a dispersão de informações entre planilhas, e-mails e WhatsApp. A proposta considera a consulta de disponibilidade de materiais, o prazo mínimo de 48 horas para solicitações, as notificações, o controle de reposições e a consulta de informações dos responsáveis pelo laboratório.

Também são considerados recursos de acessibilidade, como ampliação de textos, ajustes de contraste e navegação por teclado, visando à autonomia dos usuários.

> [!NOTE]
> O sistema encontra-se na etapa de design e prototipação de baixa fidelidade. As funcionalidades descritas representam propostas de interação, e não funcionalidades já implementadas.

---

<a id="sumario"></a>
## 2. Sumário

### 📁 Imersão

| Documento | Descrição |
|---|---|
| 📁 [1 – Briefing com o cliente](Design-IHC/01-Imersão/1-briefing.md) | Entrevista inicial com a técnica do laboratório e registro das necessidades identificadas. |
| 📁 [2 – Matriz CSD](Design-IHC/01-Imersão/2-matriz-csd.md) | Organização das certezas, suposições e dúvidas levantadas no briefing. |
| 📁 [3 – Pesquisa com o usuário](Design-IHC/01-Imersão/3-pesquisa-com-o-usuário.md) | Questionários complementares, síntese dos resultados e evidências da coleta. |

### 📁 Ideação

| Documento | Descrição |
|---|---|
| 📁 [1 – Personas](Design-IHC/02-Ideação/1-Personas.md) | Representação de três perfis de usuários por meio da técnica PATHY. |
| 📁 [2 – Metamensagem](Design-IHC/02-Ideação/2-metamensagem.md) | Comunicação da proposta do sistema, das necessidades dos usuários e das formas de interação. |
| 📁 [3 – Mapa de objetivos](Design-IHC/02-Ideação/3-mapa-de-objetivos.md) | Representação dos objetivos individuais e compartilhados das personas. |
| 📁 [4 – HTAs](Design-IHC/02-Ideação/4-htas.md) | Decomposição hierárquica das tarefas e seus planos de execução. |
| 📁 [5 – MoLIC](Design-IHC/02-Ideação/5-molic.md) | Modelagem dos fluxos de interação entre o usuário e o sistema. |

### 📁 Prototipação

| Documento | Descrição |
|---|---|
| 📁 [1 – Sketches](Design-IHC/03-Prototipação/1-sketches.md) | Protótipos de baixa fidelidade, alternativas de interface e justificativas das decisões de design. |

### Informações complementares

- [Organização do repositório](#3-organização-do-repositório)
- [Resumo das atividades e avaliações](#4-resumo-das-atividades-e-avaliações)
- [Ferramentas utilizadas](#5-ferramentas-utilizadas)
- [Termo de uso de inteligência artificial](#6-termo-de-uso-de-inteligência-artificial)
- [Observações gerais](#7-observações-gerais)

---

## 3. Organização do repositório

```text
📁 TP2-Interacao-Humano-Computador/
├── README.md
└── 📁 Design-IHC/
    ├── 📁 01-Imersão/
    │   ├── 1-briefing.md
    │   ├── 2-matriz-csd.md
    │   └── 3-pesquisa-com-o-usuário.md
    ├── 📁 02-Ideação/
    │   ├── 1-Personas.md
    │   ├── 2-metamensagem.md
    │   ├── 3-mapa-de-objetivos.md
    │   ├── 4-htas.md
    │   └── 5-molic.md
    └── 📁 03-Prototipação/
        └── 1-sketches.md
```

A documentação está organizada conforme as etapas do processo de design de interação: imersão, ideação e prototipação. Cada arquivo apresenta os resultados e registros de sua respectiva atividade.

[↑ Voltar ao sumário](#sumario)

---

## 4. Resumo das atividades e avaliações

### 4.1. Imersão

Foi realizado um briefing por videochamada com uma técnica do Laboratório de Biologia, seguido da elaboração da Matriz CSD, composta por 14 certezas, 9 suposições e 17 dúvidas. A pesquisa complementar foi conduzida com dois formulários eletrônicos: o direcionado aos professores recebeu duas respostas, enquanto o destinado aos técnicos não recebeu respostas.

As respostas dos professores apontaram a importância da consulta de disponibilidade de equipamentos e do acompanhamento das solicitações, além da preferência pelo acesso por computador e celular.

### 4.2. Ideação

Foram elaboradas três personas utilizando a técnica PATHY, incluindo uma persona com necessidade de acessibilidade. A metamensagem, os mapas de objetivos, os sete HTAs e os diagramas MoLIC orientaram a definição das tarefas e dos fluxos de interação do sistema.

### 4.3. Prototipação e análise das interfaces

Foram produzidos sketches de baixa fidelidade para representar as principais telas do Lab Manager. A equipe documentou comparações entre alternativas de interface para o agendamento de laboratório, o acompanhamento de agendamentos e o hub da técnica, considerando critérios de organização, usabilidade, comunicabilidade e experiência do usuário.

> [!IMPORTANT]
> As comparações dos sketches constituem uma análise preliminar de design. Não há registros, nos documentos disponibilizados, de testes formais de usabilidade com usuários ou de avaliações da interação implementada. As decisões propostas ainda precisam ser validadas em etapas posteriores.

[↑ Voltar ao sumário](#sumario)

---

## 5. Ferramentas utilizadas

| Ferramenta | Finalidade no projeto |
|---|---|
| [Draw.io](https://www.drawio.com/) | Elaboração de diagramas e sketches. |
| [Google Forms](https://forms.google.com/) | Criação e aplicação dos questionários complementares. |
| [Canva](https://www.canva.com/) | Apoio à organização e apresentação visual dos materiais do projeto. |
| [ChatGPT](https://chatgpt.com/) | Apoio à organização da documentação, revisão textual e desenvolvimento dos materiais. |
| [Gemini](https://gemini.google.com/) | Apoio de inteligência artificial nas atividades do projeto. |
| [GitHub](https://github.com/) | Armazenamento e organização da documentação do repositório. |
| [Google Meet](https://meet.google.com/) | Realização da videochamada do briefing com o cliente. |

[↑ Voltar ao sumário](#sumario)

---

## 6. Termo de uso de inteligência artificial

A equipe utilizou ferramentas de inteligência artificial, como ChatGPT e Gemini, para apoiar a organização do repositório, a elaboração dos questionários de acordo com o perfil dos entrevistados e usuários, a criação das personas, a revisão da metamensagem e a otimização do desenvolvimento dos HTAs e dos diagramas MoLIC.

Os materiais produzidos com esse apoio passaram por revisões dos integrantes da equipe, com o objetivo de assegurar a coerência, a relevância e a adequação das informações ao contexto do trabalho.

[↑ Voltar ao sumário](#sumario)

---

## 7. Observações gerais

- Os dados pessoais presentes nas evidências da pesquisa foram ocultados para preservar a identidade dos participantes.
- Os resultados da pesquisa complementar devem ser interpretados considerando o número reduzido de respostas.
- As personas e os demais artefatos de design orientam a proposta do sistema, mas não substituem a validação com usuários.
- Os protótipos de baixa fidelidade representam a proposta de navegação e interação, sem funcionalidades implementadas nesta etapa.

[↑ Voltar ao sumário](#sumario)

---

<p align="center"><strong>Lab Manager | TP2 – Interação Humano-Computador | ICET/UFAM – 2026</strong></p>

