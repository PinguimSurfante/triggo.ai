# Análise de Dados Olist – Projeto de Engenharia de Dados e Data Science

## Sobre o projeto

Este projeto analisa o dataset público do e-commerce brasileiro Olist (disponível no Kaggle) para extrair insights sobre comportamento dos clientes, desempenho dos vendedores, satisfação, logística e vendas.

O trabalho está dividido em quatro etapas principais:

1. **Tratamento e modelagem dos dados**  
   Limpeza e organização dos dados para facilitar as análises.

2. **Análise exploratória de dados**  
   Investigação do volume de pedidos, tempo de entrega, relação entre frete e distância, categorias mais lucrativas e comportamento por estado.

3. **Resolução de problemas de negócio**  
   - Taxa de clientes recorrentes.  
   - Modelo simples para prever atrasos nas entregas.  
   - Segmentação de clientes via clustering.  
   - Análise da satisfação dos clientes.

4. **Visualizações e dashboards**  
   Gráficos interativos para analisar vendas por estado e categoria, mapas de calor regionais, análise de satisfação e desempenho dos vendedores.

## Como executar

### Pré-requisitos

- Python 3.8+  
- Jupyter Notebook ou Google Colab  
- Bibliotecas: pandas, numpy, matplotlib, seaborn, scikit-learn, plotly

### Passos para rodar

1. Clone ou baixe este repositório.  
2. Baixe o dataset Olist no Kaggle:  
   [https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)  
3. Coloque os arquivos CSV na pasta `data/` (ou ajuste os caminhos no notebook).  
4. Abra o notebook no Jupyter ou Google Colab.  
5. Execute as células na ordem.

## Principais resultados

### Etapa 2 – Análise exploratória

- Crescimento no volume de pedidos ao longo do tempo, com picos sazonais (Black Friday, Natal).  
- Tempo médio de entrega entre 5 e 15 dias, com alguns casos extremos.  
- Valor do frete pouco correlacionado com distância estimada.  
- Categorias mais lucrativas: health_beauty, watches_gifts, bed_bath_table.  
- Ticket médio mais alto em alguns estados do Nordeste.

### Etapa 3 – Solução de problemas

- Apenas 3% dos clientes compram mais de uma vez, apontando oportunidades para fidelização.  
- Modelo Random Forest básico identifica bem entregas pontuais, mas precisa de ajustes para detectar atrasos.  
- Clientes segmentados em três grupos: pontuais, intermediários e VIPs.  
- Satisfação vinculada a tempo de entrega, custo do frete e categoria do produto.

### Etapa 4 – Visualizações e dashboards

- Dashboard interativo com vendas ao longo do tempo, por estado e categoria.  
- Mapa de calor com concentração de faturamento em SP, RJ e MG.  
- Gráficos relacionando avaliação do cliente e tempo de entrega.  
- Análise dos top 20 vendedores mostrando volume, satisfação e tempo médio de entrega.
