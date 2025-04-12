### Objetivo

Analisar o desempenho de vendas de uma rede de supermercados, identificando padrões de consumo e oportunidades de otimização com foco em produto, filial e sazonalidade.

**Perguntas a serem respondidas:**
- Quais são os produtos mais vendidos?
- Quais filiais têm maior faturamento?
- Qual o ticket médio por loja?
- Existe variação de vendas por mês?
- Quais produtos têm menor giro, e podem ser descontinuados?
- Quais categorias mais faturam?

---

### Pipeline e Etapas

#### 1. **Coleta de Dados**
Em repositório publico.

#### 2. **Ingestão e Tratamento**
- Upload de CSV no Databricks
- Inspeção do schema
- Leitura com PySpark e conversão para Delta Table

#### 3. **Modelagem Dimensional**
- Separação da base em:
  - `dim_produto`
  - `dim_filial`
  - `dim_tempo`
  - `fato_vendas`
- Aplicação do modelo estrela (Star Schema)
  ![image](https://github.com/user-attachments/assets/5fd2c2c0-2ba5-49bd-b2af-b39a0ddbf485)


#### 4. **Análises Realizadas**
- Top produtos por volume e faturamento
- Faturamento e ticket médio por filial
- Faturamento por categoria
- Giro de produto (baixo volume)
- Sazonalidade de vendas por mês

---

#### Autoavaliação

O projeto atingiu os objetivos principais propostos, permitindo análises úteis sobre desempenho de vendas. 

---

####  Foram utilizados:
- Databricks Community Edition
- PySpark e SQL
- Delta Lake
