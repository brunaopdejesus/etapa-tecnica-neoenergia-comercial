# Desafio Técnico: Analista Data Science Júnior (Comercial) - Neoenergia

Este repositório contém a resolução do desafio técnico para a vaga de **Analista Data Science Júnior** na Neoenergia. O objetivo do projeto é realizar uma análise exploratória de dados públicos da ANEEL (Base BDGD - UCMT_PJ), focando em geração de valor para a área comercial e escalabilidade técnica.

## 🏗️ Arquitetura de Dados (Padrão Medallion)

O pipeline foi estruturado em camadas para garantir a governança e a integridade das informações:

*   **Bronze (Raw):** Ingestão dos dados brutos armazenados em ambiente de staging para garantir a reprodutibilidade.
*   **Silver (Clean):** Processamento, limpeza, tratamento de tipagem e filtragem de registros ativos.
*   **Gold (Business):** Aplicação de regras de negócio, agregações anuais e criação de métricas de risco.

## 💡 Principais Insights Comerciais

A análise focou em três pilares fundamentais para a estratégia da companhia:

1.  **Concentração de Mercado:** Identificação dos polos geográficos de maior consumo nacional (Benchmark).
2.  **Gestão de Risco e Churn:** Criação de uma matriz de risco cruzando faturamento (Consumo) vs. Qualidade do Serviço (DIC). Foram mapeados clientes prioritários para retenção.
3.  **Sazonalidade de Demanda:** Mapeamento de picos de consumo ao longo do ano para suporte ao planejamento de carga e campanhas de eficiência.

## 🛠️ Tecnologias Utilizadas

*   **Python:** Processamento de dados (Pandas, NumPy).
*   **Matplotlib / Seaborn / Squarify:** Visualização de dados e gráficos executivos.
*   **Jupyter Notebook (Google Colab):** Ambiente de desenvolvimento.
*   **Git:** Versionamento de código.

## 🚀 Como Executar

O projeto foi desenvolvido no Google Colab. Para reproduzir a análise:
1. Clone este repositório.
2. Faça o upload do arquivo `.ipynb` no ambiente Colab.
3. Certifique-se de que a base de dados `UCMT_PJ` está acessível conforme documentado no código.

---
**Candidata:** Bruna Oliveira Pedroso de Jesus
[https://www.linkedin.com/in/brunaopdejesus/] | [bruna.opdejesus@gmail.com]
