# Desafio Modelagem e Transformação de dados com DAX

O desafio proposto consiste em modelar a sample financial do Power BI em um modelo Star Schema e criar a tabela dimensão de tempo usando as funções DAX.

---
## Processo de construção do diagrama

- Foram criadas as tabelas de dimensão d_produtos, d_detalhes, d_descontos e d_produtos_detalhes duplicando a tabela de financial;
    - Na tabela de dimensão d_produtos os dados foram agrupados levando em consideração a coluna "Product", algumas colunas de agregação foram criadas, bem como a coluna de índice que foi nomeada de "ID_Produto";
    - Nas demais tabelas de dimensão (d_detalhes, d_descontos e d_produtos_detalhes) a coluna ID_Produto foi criada como uma coluna condicional levando em consideração o índice criado na d_produtos e a coluna "Product";
    - Em cada tabela de dimensão, colunas que não condiziam com a tabela, foram removidas;
    - A coluna ID_Produto foi criada para que conseguissemos criar a relação entre as tabelas dimensão e a fato.
- A tabela fato F_Vendas foi criada também duplicando-se a tabela financial;
- A tabela "Tabela Data" e suas coluna foram criadas usando DAX;
- Os relacionamentos foram criados na aba de modelagem do Power BI.

---
## Funções DAX utilizadas para criação da Tabela Data

- CALENDARAUTO - para criação da tabela;
- YEAR, MONTH, DATE e FORMAT - para criação das colunas.

---
## Diagrama Star Schema

<p align="center" alt="Diagrama Entidade Relacionamento Universidade">
<img 
    src="https://github.com/talitachobits/power-bi/blob/main/Modelagem%20e%20Transforma%C3%A7%C3%A3o%20de%20dados%20com%20DAX/StarSchemaFinancial.png"
    width="800"  
/>
</p>
