# AI Career Threat Analysis (Análise de Risco de IA nas Carreiras)

# Sobre o Projeto

Este projeto realiza uma análise exploratória de dados sobre o impacto e o risco de automação por Inteligência Artificial em diversas carreiras. O objetivo foi extrair insights sobre quais áreas estão mais vulneráveis, as tendências salariais e como a maturidade das ferramentas de IA afeta a adoção no mercado.

# Tecnologias Utilizadas

Python (Lógica principal e análise)

Pandas (Manipulação de DataFrames e cálculos estatísticos)

SQLite3 (Consultas SQL em banco de dados em memória)

Matplotlib (Visualização de dados)

Power BI (Criação de dashboard)

# Principais Insights e Resultados

Através de consultas SQL e cruzamentos no Pandas, os seguintes resultados foram obtidos:

## Cargos de Maior Risco (higher_risk_areas.csv):

Funções operacionais e repetitivas, como Data Entry Clerk com Score de 92 e Administrative Assistant com Score de 80, lideram o ranking de vulnerabilidade à automação.

| title                    | score |
|--------------------------|-------|
| Data Entry Clerk         | 92    |
| Administrative Assistant | 80    |
| Telemarketer             | 77    |
| Medical Transcriptionist | 75    |
| Call Center Agent        | 73    |
| Payroll Specialist       | 73    |
| Receptionist             | 72    |
| Content Writer           | 71    |
| Tax Preparer             | 69    |
| Contract Reviewer        | 69    |

## Cargos de Menor Risco (lower_risk_areas.csv):

Profissões que exigem presença física e habilidades manuais ou interpessoais Home Health Aide, Ironworker, Plumber possuem o menor índice de risco com Score 4.

## Tendência Salarial vs. Automação (declining_roles.csv):

Cargos com tendência salarial em declínio e com índice de automação de subtarefas superior a 66% foram categorizados como "Automatizáveis".

## Maturidade x Adoção:

Houve uma correlação fortíssima (0.93) entre a maturidade da ferramenta de IA e a adoção no mercado, indicando que ferramentas prontas são rapidamente absorvidas pelas empresas.

## Salário vs. Risco:

A correlação entre o salário médio e o score de risco é de -0.14, indicando uma tendência fraca de que cargos com menores salários sofrem um risco levemente maior.

# Estrutura do Repositório

main.ipynb: Notebook com todo o código (Python + SQL).

riscoXtempo.png: Gráfico gerado mostrando a evolução do risco da profissão mais ameaçada ao longo do tempo (2025 a 2026).

*.csv: Múltiplos arquivos contendo as bases tratadas e prontas para consumo em ferramentas de BI (ex: higher_risk_categories.csv, percentage_grow.csv, etc.).

# Como Executar

Clone o repositório.

Instale as bibliotecas necessárias: pip install pandas matplotlib

Execute o arquivo main.ipynb utilizando Jupyter Notebook, JupyterLab ou VS Code.

Projeto desenvolvido para fins de estudo em SQL, manipulação de dados com Pandas e visualização analítica.
