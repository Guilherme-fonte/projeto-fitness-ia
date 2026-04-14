{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "02bfec91",
   "metadata": {},
   "source": [
    "# A Armadilha da Zona Cinzenta (Z3)\n",
    "### Análise de Dados — Performance e Recuperação em Atletas Recreativos\n",
    "\n",
    "## Problema\n",
    "Por que atletas recreativos que treinam consistentemente acumulam fadiga \n",
    "sem perceber evolução? A hipótese é que treinar predominantemente na Zona 3 \n",
    "(moderada) gera esforço suficiente para cansar, mas insuficiente para \n",
    "desenvolver condicionamento.\n",
    "\n",
    "## Resultados Encontrados\n",
    "\n",
    "| Indicador | Z1-Z2 (Baixa) | Z3 (Moderada) | Z4-Z5 (Alta) |\n",
    "|-----------|--------------|--------------|--------------|\n",
    "| Sono médio | 6.87h | 6.19h ⚠️ | 6.08h |\n",
    "| Calorias médias | 2190 | 2361 | 2648 |\n",
    "| FC média | 75.7 bpm | 80.1 bpm ⚠️ | 75.4 bpm |\n",
    "\n",
    "**Z3 tem FC mais alta que Z4-Z5** — indica menor eficiência cardiovascular.  \n",
    "**Z3 dorme menos que Z1-Z2** — pior recuperação sem o retorno do treino intenso.\n",
    "\n",
    "## Dataset\n",
    "- Fitbit Public Dataset (Kaggle) — 30 usuários, 2016\n",
    "- Arquivos usados: `dailyActivity`, `minuteSleep`, `heartrate_seconds`\n",
    "\n",
    "## Tecnologias\n",
    "- Python 3.10\n",
    "- Pandas\n",
    "- Matplotlib\n",
    "- Jupyter Notebook\n",
    "\n",
    "## Estrutura\n",
    "\n",
    "data/raw/          → dataset original\n",
    "reports/graficos/  → gráficos gerados\n",
    "analise.ipynb      → análise completa\n",
    "\n",
    "## Como Rodar\n",
    "```bash\n",
    "pip install pandas matplotlib numpy\n",
    "jupyter notebook analise.ipynb\n",
    "```\n",
    "\n",
    "## Autor\n",
    "Guilherme — Projeto Trainee Eniac Academy — Abril/2026"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.10.11"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
