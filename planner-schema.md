# Esquema do Planner

Este arquivo resume a implementação das cinco bases descritas no README.

## Relações principais

```text
Objetivos 1 ─── N Ações
Objetivos 1 ─── N Rotina
Objetivos 1 ─── N Obstáculos
Objetivos 1 ─── N Revisões
Ações N ─────── N Rotina
```

## Views recomendadas

- **Objetivos ativos:** filtro `Status = ativo`.
- **Próximas ações:** filtro `Status = próxima ou em andamento`, ordenado por data.
- **Semana:** calendário da base `Rotina`, filtrado para os próximos sete dias.
- **Riscos ativos:** filtro `Status = monitorar ou ativo`.
- **Revisões:** tabela ordenada da mais recente para a mais antiga.

## Template de novo objetivo

1. Criar o registro em `Objetivos`.
2. Registrar o resultado esperado e o critério de sucesso.
3. Criar pelo menos uma revisão futura.
4. Executar a habilidade de plano de ação.
5. Distribuir as primeiras ações na base `Rotina`.
6. Registrar os riscos previsíveis em `Obstáculos`.
