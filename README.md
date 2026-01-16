# Análise XYZ

Este projeto tem como objetivo explorar dados de vendas para responder a cinco problemáticas analíticas centrais, utilizando Python e Pandas em um Jupyter Notebook. O foco está em extrair insights de negócio e oportunidades de marketing direcionado a partir de dados demográficos, temporais e de performance de produtos.

## Problemas Analisados
1. Perfil demográfico dos clientes  
2. Performance por categoria de produto  
3. Sazonalidade das vendas  
4. Tendência de vendas por região  
5. Relação entre idade e categorias compradas

---

## Como configurar e rodar o notebook

### 1️ Pré-requisitos
- Python **3.11+

### 2 Criando o ambiente
```bash
python -m venv venv
```

Ativando o ambiente:
```bash
source venv/bin/activate
```

### 3 Instalando dependências
Instale as dependências:
```bash
pip install -r requirements.txt
```

---

## Principais Conclusões

### 1️ Perfil demográfico dos clientes
- A distribuição de idades apresenta maior concentração na faixa central, com menor presença nos extremos (18–24 e 60+).
- A análise utilizou histograma de idades reais, permitindo uma visão mais granular.
- Em relação à localização, São Paulo é o estado com maior número de clientes, evidenciado por gráfico de barras.

---

### 2️ Performance por categoria de produto
- Gráficos de barras foram utilizados para comparar faturamento entre categorias.
- Jardinagem lidera o faturamento, representando cerca de 30% do total.
- Utilidades Domésticas aparece logo em seguida, com ticket médio proporcionalmente elevado.
- O ticket médio acompanha o padrão de faturamento por categoria.

---

### 3️ Sazonalidade
- Foi analisada a variação mensal das vendas ao longo de 5 anos, usando gráficos de linhas sobrepostas.
- Observa-se concentração de vendas no início e no fim do ano.
- Há uma queda acentuada entre março e abril e crescimento gradual entre agosto e setembro.
- A comparação entre o último quadrimestre de 2024 e 2025 mostrou pouca variação significativa.

---

### 4️ Tendência de vendas por região
- A evolução mensal das vendas por estado foi analisada com gráficos de linha.
- O faturamento total por região foi comparado com tabelas resumo e gráficos de barras.
- SP se destaca tanto em volume quanto em faturamento e apresenta maior variação sazonal em comparação a outros estados.

---

### 5️ Relação entre idade e categorias compradas
- A análise foi feita com um mapa de calor, relacionando faixa etária e categorias.
- A categoria Mangueiras se destaca fortemente na faixa 35–44 anos.

---

## Insights para Campanhas de Marketing Direcionadas

- Segmentação etária: campanhas específicas para a faixa 35–44 anos focadas em produtos ex: Mangueiras.
- Aproveitamento da sazonalidade: antecipar campanhas promocionais antes dos picos de início e fim de ano.
- Foco regional: ações mais agressivas em SP, onde há maior volume, faturamento e resposta sazonal.
- Combinar produtos de alto ticket médio em categorias líderes para aumentar o faturamento por cliente.
- Campanhas de retenção em períodos de queda (março–abril), com cupons promocionais.

---

## Limitações da base e próximos passos
A base de dados possui apenas 7 colunas, o que limita análises mais profundas de comportamento do cliente (ex.: recorrência, fidelização ou jornada de compra).

Existência de valores ausentes em campos relevantes como CLIENTE, IDADE, ESTADO e PRODUTO. Apesar de serem poucos e tratados adequadamente, esse preenchimento pode introduzir viés estatístico, especialmente em análises demográficas.

Um próximo passo interessante seria o enriquecimentos dos dados visando análises mais aprofundadas das vendas tanto do ponto de vista do cliente como do ponto de vista do produtos, ainda podendo aplicar modelos de machine learning para a predições de vendas no próximo ano, por exemplo.