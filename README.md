# ZelaBairro – Automação RPA (GS 2026.2)

Parte de RPA da Global Solution 2026.2 (CitizenTech), disciplina Robotic Process Automation, Prof.ª Cibele Lopes Ribeiro.

O robô, feito no UiPath Studio, encaminha as ocorrências registradas no ZelaBairro para o Portal SP156 da Prefeitura. Ele lê a planilha de ocorrências pendentes, valida os campos, verifica se a ocorrência é duplicada, preenche o formulário de zeladoria e grava o número de protocolo de volta na planilha.

Vídeo da solução: https://youtu.be/vb518GqLTto

## Estrutura

- `Relatorio_RPA_ZelaBairro.pdf` – relatório da entrega
- `Automacao/ZelaBairro_Encaminhamento_SP156/` – projeto do UiPath (`Main.xaml`, planilha de entrada e portal de demonstração)
- `Diagramas/` – AS-IS e TO-BE no Bizagi (`.bpm`) e em BPMN
- `Analise_e_Business_Case/` – Process Assessment Tool, Score Card, ROI e OnePager
- `Prints/` – prints do fluxo, dos diagramas, do log e da planilha

## Como rodar

1. Abrir o `project.json` no UiPath Studio (usamos a versão 26.10 Community).
2. Ter a extensão UiPath Browser Automation instalada no Chrome, com acesso a URLs de arquivo liberado.
3. Executar o `Main.xaml`. O robô abre o portal de demonstração (`Ambiente_Demonstracao/portal_zeladoria.html`), que é uma cópia local do formulário, para não abrir pedidos reais no SP156.
4. No final, a planilha `Data/Ocorrencias_ZelaBairro.xlsx` fica com as colunas `rpa_protocolo` e `rpa_status` preenchidas.

## Integrantes

- Gabriel Leão da Silva – RM552642
- Matheus Farias – RM554254
- Miguel Mauricio Parrado Patarroyo – RM554007
- Pedro Chaves – RM553988
- Vitor Pinheiro Nascimento – RM553693
