# Análise e Tratamento de Dados Bancários

Este repositório contém um notebook Jupyter (`Exploração_Dados.ipynb`) que demonstra técnicas para análise e tratamento de dados utilizando um dataset de informações bancárias. O dataset possui as seguintes colunas:

- "Id"
- "Score"
- "Estado"
- "Genêro"
- "Idade"
- "Patrimonio"
- "Saldo"
- "Produtos"
- "CartãoDeCrédito"
- "Ativo"
- "Salário"
- "Saiu"

## Objetivo

O objetivo deste projeto é aprender técnicas para análise exploratória e tratamento de dados. Durante a exploração, foram realizadas as seguintes etapas:

1. **Importação e Visualização dos Dados:** Utilizando a biblioteca Pandas, os dados foram importados e visualizados para entender sua estrutura e conteúdo.

2. **Tratamento de Dados Faltantes:** Identificou-se valores faltantes (NAN) em algumas colunas, como "Salário" e "Genêro". Esses valores foram tratados substituindo-os pela mediana (para "Salário") e pela moda (para "Genêro").

3. **Tratamento de Outliers:** Outliers foram tratados em algumas colunas, como "Salário", onde valores superiores a 2 vezes o desvio padrão foram substituídos pela mediana da coluna.

4. **Tratamento de Valores Incoerentes:** Valores incoerentes com o domínio dos dados foram tratados, como idades muito altas ou muito baixas. Esses valores foram substituídos pela mediana das idades.

5. **Tratamento de Duplicatas:** Duplicatas de registros foram identificadas e removidas com base no identificador único "Id".

6. **Padronização de Dados:** Os dados foram padronizados, como a substituição de abreviações de gênero ("M" para "Masculino" e "F" para "Feminino").

7. **Tratamento de Estados:** Estados que não estavam de acordo com as regras de negócio foram ajustados, como substituir estados que não pertenciam à região Sul pelo estado "RS".

## Ferramentas Utilizadas

- **Pandas:** Utilizado para manipulação e análise dos dados.
- **Statistics:** Utilizado para cálculos estatísticos, como média e desvio padrão.
- **Seaborn:** Utilizado para visualização de dados, gerando gráficos para melhor compreensão dos dados.

Este projeto fornece uma visão geral das etapas comuns realizadas durante a análise e tratamento de dados, demonstrando o uso de diversas funcionalidades das bibliotecas Pandas, Statistics e Seaborn.
