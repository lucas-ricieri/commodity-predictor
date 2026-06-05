> **Etapa 1:** Escolha do Dataset e Definição do Problema  

## Descrição do Dataset

O projeto visa predizer o output da produção agrícola nacional cruzando três pilares fontes de dados oficiais:

1. **Produção Agrícola (IBGE):** Histórico de produção de diferentes culturas agrícolas brasileiras (área plantada, área colhida, quantidade produzida, rendimento médio).
   * **Retirado de:** `https://sidra.ibge.gov.br/tabela/5457`(várias culturas desde 2010)
2. **Dados Climáticos (INMET):** Histórico detalhado de medições climáticas organizadas por ano.
   * **Retirado de:** `https://portal.inmet.gov.br/dadoshistoricos` (pastas de 2010 a 2026)
3. **Dados Econômicos (Banco Central):** Série histórica com indicadores econômicos e financeiros.
   * **Retirado de:** `https://www3.bcb.gov.br/sgspub/localizarseries/localizarSeries.do?method=prepararTelaLocalizarSeries`

### Estrutura e Formato dos Dados
Os dados consistem em uma integração multimodal de fontes de dados tabulares (arquivos CSV e planilhas Excel) e séries temporais meteorológicas:



### Tamanho Estimado
* **Período Histórico:** de 2010 a 2026.
* **Dados Meteorológicos:** Milhares de registros diários estruturados em pastas anuais contendo dados de sensores meteorológicos nacionais.
* **Culturas Analisadas:** Diferentes culturas agrícolas temporárias e permanentes (como soja, milho, arroz, feijão, algodão, cana-de-açúcar, café, laranja e banana).  


### Justificativa
---

Explorar a correlação e a capacidade preditiva do output agrícola nacional com base em informações metereologicas e econômicas permite antever riscos setoriais cruciais, como quebra de safras e flutuações no preço de commodities. 

## Hipóteses de Pesquisa

* **H1:** A precipitação acumulada e a temperatura média estiveram relacionadas ao rendimento médio das principais culturas agrícolas entre 2010 e 2025.
* **H2:** De que forma a flutuação cambial e as taxas de juros influenciam a área plantada e a quantidade produzida de commodities de exportação em comparação com culturas destinadas ao mercado interno?
* **H3:** É possível predizer o output da colheita agrícola unindo valores climáticos de curto prazo e dinâmicas econômicas de longo prazo?

