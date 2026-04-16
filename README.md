# A Armadilha da Zona Cinzenta (Z3)
### Análise de Dados — Performance e Recuperação em Atletas Recreativos

## Problema
Por que atletas recreativos que treinam consistentemente acumulam fadiga 
sem perceber evolução? A hipótese é que treinar predominantemente na Zona 3 
(moderada) gera esforço suficiente para cansar, mas insuficiente para 
desenvolver condicionamento.

## Resultados Encontrados

| Indicador | Z1-Z2 (Baixa) | Z3 (Moderada) | Z4-Z5 (Alta) |
|-----------|--------------|--------------|--------------|
| Sono médio | 6.87h | 6.19h ⚠️ | 6.08h |
| Calorias médias | 2190 | 2361 | 2648 |
| FC média | 75.7 bpm | 80.1 bpm ⚠️ | 75.4 bpm |

**Z3 tem FC mais alta que Z4-Z5** — indica menor eficiência cardiovascular.  
**Z3 dorme menos que Z1-Z2** — pior recuperação sem o retorno do treino intenso.

## Dataset
- Fitbit Public Dataset (Kaggle) — 30 usuários, 2016
- Arquivos usados: `dailyActivity`, `minuteSleep`, `heartrate_seconds`

## Tecnologias
- Python 3.10
- Pandas
- Matplotlib
- Jupyter Notebook

## Estrutura

data/raw/          → dataset original
reports/graficos/  → gráficos gerados
analise.ipynb      → análise completa

## Como Rodar
```bash
pip install pandas matplotlib numpy
jupyter notebook analise.ipynb
```

## Autor
Guilherme — Projeto Trainee Eniac Academy — Abril/2026
