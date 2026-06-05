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

## 👥 Identificação do Grupo & Repositório

| Integrante | RA |
| :--- | :--- |
| **Lucas Ricieri Siquinelli Pereira** | 1858025 |

* **Repositório Git para acompanhamento:** [lucas-ricieri/data-science](https://github.com/lucas-ricieri/data-science)

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
   git clone https://github.com/lucas-ricieri/data-science.git
   cd data-science
   ```
2. Instale as bibliotecas necessárias para manipulação de dados e modelagem:
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn openpyxl jupyter

### Execução do Projeto
Toda a esteira de análise exploratória, processamento e modelagem está concentrada no notebook principal:
1. Abra o Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
2. Navegue até a pasta `final` e abra o arquivo:
   * **[main.ipynb](file:///c:/UTFPR/data-science/final/main.ipynb)**
3. Execute as células sequencialmente para visualizar o carregamento dos dados das pastas `data/commodity`, `data/weather` e `data/economic`, a análise estatística e os resultados do modelo preditivo.
