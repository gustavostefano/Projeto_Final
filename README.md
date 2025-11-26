# Projeto_Final
Projeto final de Deep Learning e Laboratório de Inovação

# 🚗 Uber NYC 2014 — Analytics & Interactive Dashboard

Projeto final da disciplina **Laboratório de Inovação IV (FAC SENAC DF)** — análise da mobilidade urbana com dados da Uber em Nova York (abril–setembro/2014).  
Inclui **coleta via Kaggle API**, **limpeza e análise com Pandas**, e **dashboard interativo** construído no **Lovable** (e versão alternativa em Flask + Plotly).

## 📁 Estrutura do Projeto

```text
uber-nyc-2014-analytics/
├─ data/                # CSVs originais (abril a setembro/2014)
├─ processed/           # Arquivos de cache (parquet)
├─ notebooks/           # Notebooks do Google Colab (.ipynb)
├─ app_flask/           # Versão Flask interativa com Plotly
├─ lovable/             # Prompt e assets do dashboard Lovable
├─ reports/             # Relatórios semanais (.docx / .pdf)
├─ README.md
├─ .gitignore
└─ .gitattributes


---

## 🧩 1. Fonte dos Dados

Dataset público utilizado:

🔗 **FiveThirtyEight / Uber Pickups in New York City – Kaggle**  
https://www.kaggle.com/datasets/fivethirtyeight/uber-pickups-in-new-york-city

Período coberto: **Abril a Setembro de 2014**  
Colunas originais:  
- `Date/Time`  
- `Lat`  
- `Lon`  
- `Base`  

---

## 🧱 2. Como Reproduzir o Projeto

### ▶ 2.1 Google Colab

Execute o notebook:

notebooks/uber_semana2_kagglehub_do_zero_v2.ipynb


Ele inclui:
- Autenticação com o Kaggle usando `kagglehub`
- Download automático dos CSVs
- Limpeza e padronização das colunas
- Geração das colunas derivadas: `hour`, `weekday`, `month`
- EDA e insights iniciais com IA

---


▶ 2.2 Dashboard no Lovable

O dashboard final do projeto será criado no Lovable usando o prompt:
lovable/prompt.txt

🤖 3. IA e Engenharia de Prompt

O projeto incorpora práticas de Engenharia de Prompt para:

Criar descrições automáticas de gráficos

Gerar relatórios narrativos semanais

Elaborar perguntas exploratórias

Auxiliar na interpretação dos dados

Os prompts estão documentados no notebook e na pasta lovable/.

🎯 4. Objetivo do Dashboard Interativo

O dashboard interativo visa:

Identificar padrões de demanda da Uber em NYC

Explorar frequência por hora, dia da semana e base

Analisar a distribuição geográfica via mapa interativo

Utilizar filtros globais para permitir análise dinâmica

Gerar relatórios automáticos com IA

Funcionalidades incluídas:

KPIs gerais

Gráficos reativos

Heatmap weekday × hour

Scattermapbox com amostragem

Exportação de dados filtrados e gráficos

Filtros globais com cross-filtering

🧭 5. Autoria

Aluno: Gustavo Stefano Thomazinho
Professor: Alexsander Barreto
Curso: Ciência de Dados — FAC SENAC DF
Disciplina: Laboratório de Inovação IV – 2025/2

⚖️ 6. Licença

Projeto distribuído sob a Licença MIT, de uso livre para fins educacionais e acadêmicos.
