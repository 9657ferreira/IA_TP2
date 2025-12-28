IA25\_P02\_G02
Trabalho Prático 2 — IA Project 02 (2025/26)
Grupo: G02
Repositório GitHub: https://github.com/9657ferreira/IA\_TP2.git

1. Estrutura do projeto

* /data

  * WorldCupMatches.csv
  * WorldCups.csv
  * fifa\_ranking-2024-06-20.csv

* Notebook\_1\_Classification.ipynb
* Notebook\_2\_Clustering.ipynb
* Notebook\_3\_Association.ipynb
* readme.txt
* requirements.txt (opcional, mas recomendado)

Nota:

* As regras de associação (Apriori) são obtidas a partir de “transações” construídas com base em métricas discretizadas
  (ex.: tiers de ranking/pontos/vitórias) por (team, year), não sendo necessário um dataset de “market basket”.

2. Notebooks

Notebook 1 — Classificação

* Objetivo: treinar e comparar modelos de classificação (2–3 algoritmos) com base em features do Mundial e do ranking FIFA.
* Inclui: preparação de dados, split, métricas (accuracy, f1-macro, etc.), e otimização de hiperparâmetros (GridSearchCV).

Notebook 2 — Clustering (K-Means)

* Objetivo: agrupar seleções (team, year) por “perfil” de ranking FIFA + performance no Mundial.
* Inclui: escolha de K (Elbow + Silhouette), treino do K-Means e caracterização dos clusters (tamanho e estatísticas).

Notebook 3 — Regras de Associação (Apriori)

* Objetivo: extrair regras de associação (Apriori) a partir de itens gerados por discretização (tiers) por (team, year).
* Inclui: ajuste de parâmetros (min\_support, min\_confidence/metric) e análise das regras (lift/confidence).

3. Como correr
   Requisitos:

* Python 3.x
* Bibliotecas: numpy, pandas, scikit-learn, matplotlib, mlxtend, joblib

Instalação (exemplo):
pip install numpy pandas scikit-learn matplotlib mlxtend joblib

Execução:

1. Abrir os notebooks em Jupyter/VSCode
2. Garantir que os ficheiros CSV estão dentro da pasta /data
3. Correr os notebooks por ordem:

   * Notebook\_1\_Classification.ipynb
   * Notebook\_2\_Clustering.ipynb
   * Notebook\_3\_Association.ipynb

4. Outputs gerados (podem variar conforme as células executadas)

* best\_worldcup\_model.joblib
* clusters\_team\_year.csv
* apriori\_frequent\_itemsets.csv
* apriori\_rules\_all.csv
* apriori\_rules\_top.csv

5. Autores

* António Ferreira — Nº 9657
* Mafalda Barão — Nº 20446
* Ruben Dias — Nº 23033
* Gonçalo Gomes — Nº 23039
* João Morais — Nº 23041
