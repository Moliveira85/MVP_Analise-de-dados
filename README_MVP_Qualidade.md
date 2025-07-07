# 📊 MVP - Análise Exploratória de Dados em Controle de Qualidade Farmacêutico

Este projeto tem como objetivo aplicar as etapas de **análise exploratória e pré-processamento de dados**, conforme os princípios da disciplina de Ciência de Dados (PUC-Rio), utilizando um conjunto real de dados laboratoriais da indústria farmacêutica.

## 📁 Dataset

A base de dados contém atributos quantitativos de diferentes lotes de medicamentos, com foco nos seguintes parâmetros:

- `dissolution_av`: média de dissolução do princípio ativo (%)
- `batch_yield`: rendimento final do lote (%)
- `api_content`: teor do princípio ativo no produto final (%)

## 🧩 Definição do Problema

O projeto busca identificar **padrões, outliers e correlações** entre os atributos de qualidade, avaliando se existem **lotes críticos com múltiplas falhas** ou se os desvios são pontuais.

Este é um problema **não supervisionado**, com foco em análise descritiva, visualização e preparação de dados.

## ⚙️ Etapas Realizadas

- Leitura e seleção das variáveis de interesse
- Avaliação estatística descritiva
- Visualização da distribuição com boxplots
- Normalização dos dados com z-score
- Identificação de outliers estatísticos
- Análise de correlação entre as variáveis
- Verificação de quais lotes apresentaram os **valores mínimos e máximos**
- Conclusões específicas por atributo

## 📌 Resultados

- Os valores mínimos e máximos de `dissolution_av`, `batch_yield` e `api_content` **ocorreram em lotes distintos**, sugerindo que **as falhas são isoladas e não recorrentes**.
- A variável `api_content` se manteve, em sua maioria, **dentro da faixa regulamentar de 90% a 110%**, indicando **robustez no processo de dosagem** do princípio ativo.
- A normalização dos dados permitiu uma melhor detecção de outliers e compreensão das dispersões.

## ✅ Conclusão

O conjunto de dados se mostrou adequado para análises estatísticas e futuras aplicações preditivas. A ausência de correlação direta entre os atributos críticos e a distribuição dos desvios ao longo de diferentes lotes reforçam a **consistência do processo produtivo**.

## 🚀 Como executar

Este notebook pode ser executado diretamente no Google Colab com o link do dataset no formato `.raw` do GitHub:

```python
url = "https://raw.githubusercontent.com/Moliveira85/MVP_Analise-de-dados/main/Laboratory.csv"
```

---

🧠 Projeto acadêmico da Pós-Graduação em Ciência de Dados — PUC-Rio  
📅 Julho/2025 — Autor: Marcelo Albuquerque de Oliveira
