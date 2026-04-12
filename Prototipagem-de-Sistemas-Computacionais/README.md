# Prototipagem de Sistemas Computacionais - Unidade 1

**Instituição:** Cruzeiro do Sul Virtual (CSED)
**Curso:** Bacharelado em Ciência da Computação
**Disciplina:** Prototipagem de Sistemas Computacionais
**Foco da Atividade:** Análise de Processos, Levantamento de Requisitos e Modelagem BPMN.

---

##  1. Definição do Problema e Contexto
**Cenário Escolhido:** Laboratório de Análises Clínicas
**Processo:** Triagem, Coleta e Rastreabilidade de Exames Laboratoriais.

**O Problema Atual:** Atualmente, a organização gerencia o fluxo de forma altamente manual. A recepção utiliza planilhas isoladas, pedidos médicos em papel e não há comunicação integrada em tempo real com a área técnica. 

**Impactos Negativos:**
* **Retrabalho e Falhas:** Redigitação constante de dados, gerando risco de troca de amostras.
* **Atrasos:** Falta de gestão de fila e prioridade em tempo real.
* **Custos:** Perda de receita (glosas) devido ao extravio de guias físicas de convênios.

---

## 2. Mapeamento de Stakeholders

| Stakeholder | Papel no Processo | Nível de Influência |
| :--- | :--- | :--- |
| **Recepcionista** | Cadastrar paciente, validar convênio e gerar ordem de serviço. | Média |
| **Biomédico / Técnico** | Processar exames na bancada e liberar laudos. | Alta |
| **Diretoria / Gerência** | Tomadores de decisão focados em reduzir custos e aumentar produtividade. | Muito Alta |
| **Paciente** | Usuário final do serviço laboratorial, aguardando diagnóstico. | Baixa (no projeto) / Alta (no negócio) |



## 3. Modelagem do Processo Atual (As-Is)

O diagrama abaixo, modelado em notação BPMN, ilustra o fluxo atual de atendimento e destaca os três principais gargalos operacionais: digitação manual (recepção), dependência de papel (coleta) e redigitação de resultados (área técnica).

![Diagrama BPMN do Processo Atual](./Imagens/BPMN%20Laboratório.drawio%20(3).png)

##  4. Documentação de Requisitos

### Requisitos Funcionais (RF)
| ID | Descrição | Prioridade |
| :--- | :--- | :--- |
| **RF-01** | Permitir o cadastro de pacientes e a validação eletrônica de planos de saúde, centralizando informações. | Alta |
| **RF-02** | Gerar Ordem de Serviço digital e emitir etiquetas com código de barras para os tubos de amostra. | Alta |
| **RF-03** | Exibir painel de fila digital para a coleta, ordenando por chegada e prioridade clínica. | Média |
| **RF-04** | Integrar com equipamentos de análise (interfaceamento) para envio e recebimento automático de dados. | Alta |
| **RF-05** | Gerar laudos em PDF automaticamente a partir dos resultados integrados. | Alta |

### Requisitos Não Funcionais (RNF)
| ID | Categoria | Descrição |
| :--- | :--- | :--- |
| **RNF-01** | Segurança (LGPD) | Criptografar dados de saúde e manter log de auditoria de acessos e edições. |
| **RNF-02** | Desempenho | Tempo de resposta inferior a 2 segundos ao salvar cadastros ou buscar laudos. |
| **RNF-03** | Usabilidade | Interface fluida com atalhos de teclado para agilizar o atendimento na recepção. |

---

##  5. Síntese e Reflexão Técnica
O levantamento estruturado de requisitos e a modelagem visual do cenário atual (AS-IS) foram fundamentais para diagnosticar com precisão as falhas da operação. O mapeamento BPMN tirou as ineficiências da invisibilidade, enquanto a documentação de RFs e RNFs estabeleceu um contrato técnico claro. Essa ponte entre a análise de negócios e a engenharia de requisitos garante que a futura solução tecnológica não seja apenas código, mas uma ferramenta robusta e alinhada às regras de negócio e de segurança (LGPD), preparando terreno para automações e futuras integrações com modelos de dados preditivos.
