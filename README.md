# 📊 Base de Dados - Análise de Performance Comercial

Este repositório reúne os dados utilizados para a construção do painel interativo de performance comercial publicado pela **Potion Solutions - Data Analysis**.

---

## 🧱 Estrutura da Modelagem

O modelo segue uma estrutura de data warehouse do tipo **estrela**, com a tabela de fatos `fVendas` no centro, relacionada a diversas dimensões analíticas.

![Modelo Relacional](https://github.com/FelipeBNogueira/database_comercial/raw/main/modelo_relacional.png)

### 📌 Tabela Fato
- **`fVendas`**: Registra todas as transações comerciais com métricas e chaves para as dimensões.

### 🔗 Tabelas de Dimensão
- `dProdutos`: Produtos, categorias e marcas
- `dVendedores`: Nome, gerente e foto
- `dClientes`: Nome, cidade e UF
- `dCidade`: Localização geográfica
- `dUnidades`: Filiais ou unidades comerciais
- `dStatus`: Situação da venda
- `dPagamento`: Forma de pagamento
- `fMetas`: Metas por vendedor e período

---

## 📁 Organização dos Arquivos

### `/Extrações/`

📄 `Vendas.xlsx`  
Contém a base de fatos com os seguintes campos:

| Campo               | Descrição                                     |
|---------------------|-----------------------------------------------|
| Data, Data Envio    | Datas da venda e do envio/faturamento         |
| Id Produto, Cliente, Vendedor | Chaves que conectam às dimensões    |
| Qtde, Valor Unit    | Quantidade e valor unitário da venda          |
| Custo, Despesa, Impostos, Comissão | Indicadores de custo           |
| Faturamento Total, Custo Total | Indicadores consolidados           |

> ⏳ **Período coberto: 01/01/2018 a 30/04/2021**

---

### `/Dimensões/`

📄 `Dimensões.xlsx`  
Planilha com múltiplas abas, cada uma representando uma dimensão do modelo:

- `dProdutos`  
- `dVendedores`  
- `dClientes`  
- `dCidade`  
- `dUnidades`  
- `dStatus`  
- `dPagamento`

---

## 📊 Painel Interativo

Os dados alimentam um painel interativo publicado no Power BI:

👉 [Acessar o Dashboard](https://app.powerbi.com/view?r=eyJrIjoiOTFkMDBkZjMtN2E2Ny00MGRhLWI5NzctNWM1ODE2ODczNWEzIiwidCI6IjUxYTQ3M2E0LTI5MDAtNGEyNC05MjgzLTI5Mzg5NjY5ZjNkYyJ9)

---

## 🔐 Observações

- Todos os dados são fictícios ou anonimizados.
- Utilizados exclusivamente para fins educacionais e demonstrativos.

---

## 👨‍💻 Autor

Desenvolvido por [Felipe Nogueira](https://www.linkedin.com/in/cfbn-adm/)  
📧 [felipe@potionsolution.com](mailto:felipe@potionsolution.com)

---

© 2025 Potion Solutions - Data Analysis
