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

O projeto foi desenvolvido no Google Colab para facilitar o acesso e a visualização dos dados. Para reproduzir a análise:
1. Repositório: Faça o download ou clone este repositório.
2. Ambiente: Abra o arquivo .ipynb no Google Colab.
3. Dados (Importante):
* Devido ao volume de dados e instabilidades em servidores públicos, a camada Bronze está configurada para ler o arquivo ucmt_pj.csv a partir do Google Drive.
* Certifique-se de realizar o upload do dataset para a raiz do seu Google Drive ou ajustar o caminho na célula de "Camada Bronze" para o diretório local do Colab.
4. Execução: Execute as células sequencialmente para processar as camadas (Bronze, Silver e Gold) e gerar as visualizações.
  
---
**Candidata:** Bruna Oliveira Pedroso de Jesus
https://www.linkedin.com/in/brunaopdejesus/ | bruna.opdejesus@gmail.com
