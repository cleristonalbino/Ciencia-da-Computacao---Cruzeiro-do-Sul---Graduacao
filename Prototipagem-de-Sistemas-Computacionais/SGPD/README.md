# 🏥 SGPD - Sistema de Gestão de Pacientes e Diagnósticos

![Status](https://img.shields.io/badge/Status-Concluído-success)
![Curso](https://img.shields.io/badge/Curso-Ciência_da_Computação-blue)
![Semestre](https://img.shields.io/badge/Semestre-1º_Semestre-brightgreen)

## 💻 Sobre o Projeto
Este repositório consolida as experiências práticas desenvolvidas durante o curso de **Ciência da Computação**. O objetivo do projeto foi arquitetar e prototipar um sistema eficiente para a recepção de clínicas médicas (SGPD), focando na mitigação de erros de cadastro, otimização do fluxo de atendimento e usabilidade.

O projeto foi dividido em duas grandes frentes: a **Modelagem do Sistema** (Back-end/Lógica) e a **Prototipagem de Interface** (Front-end/UX).

---

## ⚙️ 1. Arquitetura e Modelagem do Sistema (UML)
Antes de qualquer tela ser desenhada, a estrutura lógica e o comportamento do sistema foram mapeados utilizando a Linguagem de Modelagem Unificada (UML). Isso garantiu que a orientação a objetos e as regras de negócio fizessem sentido desde a base.

* **Diagrama de Classes:** Mapeamento das entidades principais do sistema (Paciente, Atendente, Exame, Convênio), seus atributos e os métodos necessários para a comunicação entre eles.
* **Diagrama de Atividades:** Representação do fluxo de controle passo a passo do ponto de vista do sistema, desde o momento em que o paciente chega até a geração da Ordem de Serviço.
* **Diagrama de Sequência:** Detalhamento cronológico da troca de mensagens entre os atores (Recepcionista) e os objetos do sistema (Validação de plano de saúde, Geração de OS).

>  **Nota:** Os diagramas completos estão disponíveis na pasta `/diagramas-uml` deste repositório.

---



##  2. Prototipagem e Interface (UX/UI)
Com a base lógica definida, o próximo passo foi tangibilizar o sistema através de um protótipo navegável de alta fidelidade, focado no usuário final (recepcionistas operando sob pressão).

* **Ferramenta Utilizada:** Figma
* **Foco da Interface:** Redução de carga cognitiva, contraste visual para botões de ação principal (Call to Action) e prevenção de erros sistêmicos.
* **Testes de Usabilidade:** O protótipo foi submetido a testes simulados utilizando o protocolo *Think Aloud*, o que resultou na implementação iterativa de melhorias, como:
  * Inclusão de máscaras de formatação em campos numéricos críticos.
  * Criação de "rotas de fuga" (botões de cancelamento) em modais de validação.

>  **Acesse o Protótipo Navegável:** (https://www.figma.com/proto/oPPwZgahxzyUHWLGotBibW/SGPD?node-id=1-2&p=f&t=lV18PNr8MtJpzxiF-1&scaling=scale-down&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=1%3A2&show-proto-sidebar=1)

---

##  Aprendizados em Ciência da Computação
A construção do SGPD me permitiu entender o ciclo completo de concepção de um software. Desenhar as classes e sequências me deu a base estrutural para entender *como* a máquina processa a informação. Já a prototipagem me ensinou *como* o ser humano interage com essa informação. Unir esses dois mundos provou que um bom cientista da computação precisa equilibrar lógica computacional rigorosa com empatia pelo usuário final.

---
*Projeto desenvolvido como parte das práticas de Ciência da Computação.*
