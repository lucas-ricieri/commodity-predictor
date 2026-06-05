# 🌾 Predição de Produção Agrícola
> **Universidade Tecnológica Federal do Paraná (UTFPR) — Campus Campo Mourão**  
> **Departamento de Computação (DACOM)**  
> **Disciplina:** OPT004 - Ciência de Dados  


---

## 📌 Sumário
- [👥 Identificação do Grupo & Repositório](#-identificação-do-grupo--repositório)
- [📊 Descrição do Dataset](#-descrição-do-dataset)
- [🛠️ Como Executar](#-como-executar)

---

## 👥 Identificação do Grupo

| Integrante | RA |
| :--- | :--- |
| **Lucas Ricieri Siquinelli Pereira** | 1858025 |



---
## 📊 Descrição do Dataset

O projeto visa explorar e predizer o output da produção agrícola nacional cruzando três pilares essenciais de dados obtidos de fontes oficiais:

1. **Produção Agrícola (IBGE):** Histórico de produção de diferentes culturas agrícolas brasileiras (área plantada, área colhida, quantidade produzida, rendimento médio).
   * **Localização:** `data/commodity/`
2. **Dados Climáticos (INMET):** Histórico detalhado de medições climáticas organizadas por ano.
   * **Localização:** `data/weather/` (pastas de 2000 a 2026)
3. **Dados Econômicos (Banco Central):** Série histórica com indicadores econômicos e financeiros.
   * **Localização:** `data/economic/`


## 🛠️ Como Executar

### Pré-requisitos
Certifique-se de possuir o Python (versão 3.8 ou superior) instalado em seu ambiente, acompanhado do Jupyter Notebook ou JupyterLab para rodar as análises.

### Instalação e Preparação
1. Clone o repositório:
   ```bash
   git clone https://github.com/lucas-ricieri/commodity-predictor.git
   cd commodity-predictor
   ```
2. Instale as bibliotecas necessárias para manipulação, análise e exportação dos dados:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn duckdb pyarrow openpyxl jupyter
   ```

### Execução do Projeto
Os notebooks finais devem ser executados em sequência, pois cada entrega utiliza artefatos gerados pela etapa anterior:

1. Abra o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Navegue até a pasta `final`.
3. Execute os notebooks nesta ordem:
   * `entrega_1.ipynb` - definição do problema, dataset e hipóteses.
   * `entrega_2.ipynb` - integração, limpeza e geração do dataset final em `data/processed/dataset_final.parquet`.
   * `entrega_3.ipynb` - consultas SQL, análise exploratória, janelas climáticas pré-colheita, testes preliminares das hipóteses H2/H3 e geração de `data/processed/dataset_entrega3_tidy.parquet`.

Também é possível executar a Entrega 3 diretamente pelo terminal, após a Entrega 2 já ter gerado os dados processados:
```bash
jupyter nbconvert --to notebook --execute final/entrega_3.ipynb --inplace
```

# commodity-predictor