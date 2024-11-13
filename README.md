# Dashboard de Vendas com Grafana e PostgreSQL

Este projeto é um dashboard interativo criado no Grafana para análise de vendas. Os dados foram armazenados em um banco de dados PostgreSQL e contêm informações fictícias relacionadas a clientes, funil de vendas, produtos e lojas. O objetivo é demonstrar como utilizar consultas SQL para construir painéis gráficos com dados complexos e insights comerciais.

## Descrição do Projeto

O dashboard foi criado para fornecer uma visão detalhada dos seguintes pontos:

- **Estados com mais vendas** e **volume total de vendas**
- **Marcas mais vendidas**
- **Dias com maior número de visitas ao site**
- **Top 10 lojas que mais venderam**
- **Indicadores de Leads, Vendas, Receita, Conversão e Ticket Médio**

Cada análise foi construída a partir de consultas SQL, usando o campo de código SQL (`code`) diretamente no Grafana.

## Estrutura do Banco de Dados

As informações fictícias foram organizadas em quatro tabelas principais:

1. **Customers**: Dados dos clientes.
   - Campos: `customer_id`, `city`, `state`, etc.

2. **Funnel**: Dados de visitas à página e informações de desconto para cada cliente.
   - Campos: `funnel_id`, `customer_id`, `visit_page_date`, `discount`, etc.

3. **Products**: Dados dos produtos à venda, incluindo marca, modelo e preço.
   - Campos: `product_id`, `brand`, `model`, `price`, etc.

4. **Stores**: Dados das lojas que vendem os produtos.
   - Campos: `store_id`, `store_name`, etc.

Essas tabelas foram relacionadas por meio de `joins` para realizar análises mais avançadas, como vendas por estado, marcas mais vendidas, dias com mais visitas ao site e lojas com maior volume de vendas.

![dashboard-sales](https://github.com/user-attachments/assets/46d37579-3dc5-4aae-b56c-829519addbdb)

