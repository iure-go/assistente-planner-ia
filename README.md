# Assistente-planner-ia

Assistente de planejamento no Notion e no ChatGPT para transformar objetivos de estudo, carreira ou negócio em planos executáveis, adaptados à rotina e revisados por evidências.

Este projeto usa somente dados fictícios.

## Problema e diferencial

Uma intenção ampla costuma falhar por falta de próximas ações, tempo reservado, alternativas para imprevistos e acompanhamento. O assistente conduz cinco etapas: esclarecer o objetivo; transformar em plano de ação; adaptar à rotina; antecipar obstáculos; e revisar o progresso.

O diferencial é relacionar estratégia, execução e aprendizagem. Objetivos se conectam a ações, sessões de rotina, obstáculos e revisões, preservando o histórico das decisões.

## Ferramentas escolhidas

- Notion: bases de dados, relações, rollups, templates e views para manter o Planner estruturado.
- Notion AI: executa as habilidades no contexto dos registros.
- ChatGPT: armazena instruções reutilizáveis, analisa o plano e conduz revisões.

## Instruções gerais

O assistente deve transformar qualquer objetivo em um plano claro, com ações pequenas, observáveis e com critério de conclusão. Deve respeitar disponibilidade, energia e restrições informadas; diferenciar objetivo, resultado, ação, sessão, obstáculo e revisão; declarar hipóteses; priorizar poucas ações de alto impacto; registrar responsável, status, prazo, critério e objetivo relacionado; propor prevenção, gatilho e alternativa para cada risco; e comparar planejado e realizado sem julgamento.

## Estrutura do Planner

O Planner possui cinco bases relacionadas:

| Base | Propriedades principais | Relações |
|---|---|---|
| Objetivos | nome, área, resultado esperado, prazo, status, prioridade, progresso | ações, obstáculos e revisões |
| Ações | ação, status, data/janela, esforço, critério de conclusão, dependência | objetivo e rotina |
| Rotina | sessão, dia/horário, duração, energia, Plano B, realizada? | objetivo e ações |
| Obstáculos | tipo, sinal de alerta, prevenção, alternativa, status | objetivo |
| Revisões | período, concluído, evidências, desvios, decisão, próxima revisão | objetivo |

Detalhes de relações e views: [planner-schema.md](planner-schema.md).

## Habilidades

1. **Esclarecer e registrar o objetivo:** converte uma intenção vaga em resultado observável, com prazo, evidência de sucesso e restrições.
2. **Transformar o objetivo em plano de ação:** divide o resultado em marcos, dependências e ações com critérios verificáveis.
3. **Adaptar o plano à rotina:** cria sessões ideais e mínimas conforme disponibilidade, duração e energia.
4. **Antecipar obstáculos e definir alternativas:** registra riscos, sinais de alerta, prevenção e Plano B.
5. **Revisar o progresso:** compara intenção e execução, explica desvios sem julgamento e define ajustes.

Contrato de saída e critérios: [habilidades.md](habilidades.md).

## Demonstração prática

Objetivo fictício: preparar e realizar uma certificação de análise de dados em 12 semanas, alcançando pelo menos 80% no simulado final.

| Marco | Ação | Critério de conclusão |
|---|---|---|
| Diagnóstico | Fazer simulado inicial de 40 questões | Temas classificados por desempenho |
| Fundamentos | Estudar estatística e SQL | Resumo e 20 questões corrigidas |
| Aplicação | Resolver dois estudos de caso | Dois notebooks revisados |
| Consolidação | Fazer um simulado semanal | Nota e erros registrados |
| Decisão | Agendar a prova ao superar 80% | Duas notas acima de 80% |

Rotina: terça, 60 minutos de teoria; quinta, 90 minutos de exercícios; sábado, 120 minutos de caso ou simulado. Planos B reduzem a sessão para 20 ou 30 minutos em semanas difíceis.

Na revisão da semana 3, foram concluídas 4 de 6 ações e a nota subiu de 58% para 68%. O ajuste é separar teoria e exercícios, reduzir a sessão de terça a um módulo e manter o simulado de sábado.

Demonstração completa: [demonstracao.md](demonstracao.md).

## Como testar

Use um objetivo fictício por habilidade e verifique se a resposta produz registros concretos, respeita restrições, mantém relações corretas, define critérios observáveis, oferece um próximo passo pequeno e explicita hipóteses.

## Checklist

- [x] Documento em Markdown.
- [x] Dados fictícios.
- [x] Planner com plano de ação, rotina, obstáculos e acompanhamento.
- [x] Cinco habilidades descritas e demonstradas.
- [x] Repositório público com nome em minúsculas e sem acento.
- [x] Adicionar prints reais do Planner de exemplo, caso disponíveis.
