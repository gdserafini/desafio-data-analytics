# 📊 Desafio Técnico – Time de Dados  
**Manchester Investimentos**

## 🎯 Objetivo do Desafio

Este desafio tem como objetivo avaliar suas habilidades técnicas e analíticas em **dados**, além da sua capacidade de **transformar dados em insights de negócio** e comunicá-los com clareza.

Você irá trabalhar com um conjunto de dados de vendas de uma empresa fictícia (XYZ), simulando um cenário real de análise exploratória, preparação de dados, consultas SQL e visualização.

---

## 🏢 Contexto do Negócio

A **empresa XYZ** é uma rede de lojas de varejo especializada em produtos para **casa e jardim**, com atuação em diversas regiões do país. A empresa possui dados históricos de vendas contendo informações sobre:

- Clientes  
- Produtos e categorias  
- Datas de compra  
- Regiões geográficas  
- Valores e quantidades vendidas  

A liderança quer usar dados para **entender clientes**, **detectar sazonalidade**, **avaliar desempenho por categoria e região** e apoiar decisões estratégicas.

---

## 📂 Base de Dados

Você receberá um arquivo **EXCEL** contendo **duas abas**:

1. **Base de Vendas**  
   - Informações de clientes, vendas, datas, valores, regiões, produtos etc.

2. **Dicionário / Categorias de Produtos**  
   - Mapeamento e descrição correta das categorias  
   - Esta aba **deve ser utilizada obrigatoriamente** para enriquecer as análises (ex.: corrigir nomes, agrupar categorias, criar hierarquias).

> ⚠️ Importante: Considere que a aba de dicionário é a “fonte da verdade” para nomes e descrições de categorias.

---

## 📌 Perguntas de Negócio (Análises Esperadas)

Você deverá responder, com **análise + visualizações**, às perguntas abaixo:

### 1) Perfil demográfico dos clientes
- Distribuição de idade (média, mediana, faixas)
- Distribuição por região (e/ou outras colunas demográficas disponíveis)
- Identificação de perfis predominantes

### 2) Performance por categoria de produto
- Categorias mais vendidas e menos vendidas (por **volume** e por **faturamento**)
- Ticket médio por categoria
- Pareto (80/20) de categorias por faturamento (se aplicável)

### 3) Sazonalidade
- Existe relação entre vendas e época do ano?
- Meses com maior e menor faturamento
- Comparação trimestre a trimestre (ou mês a mês)

### 4) Tendência de vendas por região
- Evolução das vendas por região ao longo do tempo
- Identificação de regiões em crescimento/queda
- Comparação entre regiões (faturamento, volume, ticket médio)

### 5) Relação entre idade e categorias compradas
- Existe correlação/associação entre faixa etária e categorias?
- Quais categorias são mais comuns em cada faixa etária?
- Recomendações práticas (ex.: segmentação, campanhas, mix de produtos)

---

## 🛠️ Requisitos Técnicos (Obrigatórios)

### 🐍 Python (Análise de Dados)
Você deve utilizar **Python** para:
- Carregar o Excel
- Tratar e preparar dados
- Realizar as análises
- Gerar visualizações

Bibliotecas esperadas:
- `pandas`
- `numpy`
- visualização: `matplotlib` e/ou `seaborn` (ou equivalente)

### 🧾 SQL (Apenas consultas)
Você deve entregar um arquivo com **consultas SQL** que responderiam às análises principais.

Regras:
- **Não é necessário** criar banco de dados, tabelas físicas ou rodar em um SGBD.
- As consultas podem ser **teóricas**, mas devem ser **corretas e completas**, assumindo que existem tabelas como:
  - `vendas`
  - `categorias_produtos` (dicionário)

O que será avaliado:
- Joins
- Aggregations (`SUM`, `COUNT`, `AVG`)
- `GROUP BY`, `ORDER BY`
- Filtros e condições (`WHERE`, `CASE WHEN`)
- Janelas (`OVER(PARTITION BY ...)`) como diferencial

### 📊 Power BI (Modelagem + Dashboard)
Construir um dashboard no **Power BI** com:
- KPIs principais (ex.: faturamento total, volume total, ticket médio)
- Gráficos por **tempo**, **região** e **categoria**
- Segmentações (slicers) úteis
- Modelagem básica (relacionamento entre vendas e dicionário)
- Uso de **DAX simples** (ex.: medidas de total, média, variação temporal)

### 🌱 Git (Versionamento)
- Projeto deve estar em um repositório no **GitHub**
- Commits com mensagens claras
- Estrutura organizada de pastas

---

## 📦 Entregáveis

Seu repositório deve conter:

### 1) Notebook(s) Python
- `notebooks/`
  - Carregamento e tratamento
  - Análise exploratória
  - Respostas às perguntas com visualizações
  - Comentários explicando o raciocínio

### 2) Consultas SQL
- `sql/`
  - Um arquivo `analises.sql` com:
    - consultas para perfil demográfico
    - ranking de categorias
    - sazonalidade
    - tendência por região
    - relação idade x categoria

> Dica: comente cada bloco de query indicando qual pergunta está respondendo.

### 3) Power BI
- `powerbi/`
  - Arquivo `.pbix`
  - Se desejar, inclua prints do dashboard em `assets/`

### 4) README.md (Obrigatório)
Deve conter:
- Resumo do problema e abordagem
- Como executar os notebooks
- Principais insights e recomendações
- Limitações da base e da análise
- Próximos passos sugeridos (ex.: dados que faltam, melhorias)

---

## 🧠 Critérios de Avaliação

- Qualidade e consistência das análises
- Organização e legibilidade do código
- Clareza da comunicação (README + storytelling no dashboard)
- Capacidade de transformar dados em decisões
- Qualidade e correção das consultas SQL
- Boa prática de versionamento (Git)

---

## ⭐ Diferenciais (Opcional)

- Medidas no Power BI de variação (MoM/YoY), crescimento acumulado, ranking dinâmico
- Segmentação avançada por faixa etária
- Pareto (80/20) e análise de concentração por categoria/região
- Tratamento robusto de dados faltantes/erros e validações

---

## 📤 Instruções de Entrega

1. Faça um **fork** deste projeto no GitHub  
2. Desenvolva a solução no seu repositório  
3. Envie o **link do repositório** por e-mail ao seu contato na Manchester Investimentos  
4. Enviar com cópia para: `rh@manchesterinvest.com.br`

---

Boa sorte!
