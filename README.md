### Projeto da disciplina Introdução à Ciência de Dados

# 🌎 Qualidade do Ar na América Latina

## 📘 Objetivo

O projeto **Qualidade do Ar na América Latina** tem como objetivo realizar a **coleta, tratamento e análise de dados** sobre as condições climáticas e a qualidade do ar nas principais **capitais latino-americanas**, permitindo uma visão abrangente do cenário ambiental atual do continente.

---

## 🌱 Contexto

Entre os dias **10 e 21 de novembro de 2025**, será realizada a **COP30 (Conferência das Partes)** na cidade de **Belém (PA), Brasil**.

Nesse contexto de debate internacional sobre **mudanças climáticas**, torna-se essencial compreender:

- Em que posição o Brasil se encontra no panorama ambiental global;  
- Quais aspectos demandam **ações governamentais urgentes**;  
- E em quais pontos o país **serve de exemplo** para o restante do mundo.

Para isso, busca-se responder algumas perguntas focadas:

- Como a qualidade do ar em Brasília se compara com a das capitais de outros países como Chile, Colômbia ou Argentina?
- Quais variáveis meteorológicas (temperatura, velocidade do vento, pressão atmosférica) são os preditores mais importantes para a qualidade do ar, e essa importância varia entre as diferentes regiões ?
- É possível desenvolver um modelo de regressão que preveja os níveis de PM2.5 para cidades da América Latina, usando dados meteorológicos e históricos como entrada?
- A média dos níveis de poluição em Brasília difere de forma estatisticamente significativa da média das outras capitais da América Latina?

O projeto busca, portanto, **trazer uma visão baseada em dados** sobre o tema, reforçando a importância de políticas públicas sustentáveis e do monitoramento constante da qualidade do ar.

---

## 📊 Fontes dos Dados

Os dados utilizados foram obtidos a partir do dataset **Latin America Weather and Air Quality Data**, disponível no **Kaggle** (dados gerados a partir da API Open-Meteo).

Essa base contém **dois arquivos CSV** com informações referentes a diversos países da América Latina, incluindo:

- Nome do país e da capital;  
- Dados meteorológicos recentes;  
- Indicadores de qualidade do ar.

### Estrutura dos dados

- `weather_data.csv` — informações de temperatura, umidade, vento etc.;  
- `air_quality_data.csv` — indicadores como PM2.5, PM10, CO, NO₂, SO₂ e O₃.

> **Nota:** Nem todas as cidades latino-americanas possuem dados disponíveis em todas as métricas, devido a limitações de monitoramento local.

---

## 🧠 Tecnologias Utilizadas

- **Python 3**  
- **Pandas** — manipulação e limpeza de dados  
- **NumPy** — cálculos numéricos e vetorização  
- **Matplotlib / Seaborn / Plotly** — visualizações gráficas  
- **Geopy** — geocodificação e mapeamento geográfico  
- **Ipywidgets** — criação de interatividade no notebook  
- **Google Colab / Jupyter Notebook** — ambiente de execução e análise

---

## 🗂 Estrutura do Projeto

```text
PROJETO-ICD/
│
├── datasets/                         # Conjunto de dados brutos e tratados
│   ├── LA_daily_air_quality.csv
│   ├── LA_daily_air_quality_clean.csv
│   ├── LA_daily_climate.csv
│   └── LA_daily_climate_clean.csv
│
├── imagens/                          # Logos, figuras e recursos visuais
│   ├── COP30_logo.jpeg
│   ├── Nominatim_logo.png
│   ├── img_teste_2.jpg
│   └── (outros arquivos de imagem)
│
├── notebooks/                        # Notebooks Jupyter usados nas análises
│   ├── Analise_Exploratoria.ipynb
│   ├── Correlacao_e_Regressao.ipynb
│   ├── Dados_e_Tratamento.ipynb
│   ├── Graficos_interativos.ipynb
│   ├── Testes_de_Hipóteses_e_ICs.ipynb
│   └── icd.ipynb
│
├── relatorio/                        # Relatórios ou saídas textuais
│   └── Teste.txt
│
├── resultados/                       # Resultados gerados (imagens, gráficos, etc.)
│   └── img_teste.jpg
│
├── requirements.txt                  # Dependências do projeto
├── LICENSE                           # Licença do projeto (MIT)
└── README.md                         # Descrição e instruções do projeto
```

---

## ⚙️ Instalação e Execução

### 1️⃣ Clonar o repositório

```bash
git clone https://github.com/marcelohpos/PROJETO-ICD.git
cd PROJETO-ICD
```

### 2️⃣ Criar ambiente virtual (opcional)

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

### 3️⃣ Instalar dependências

```bash
pip install -r requirements.txt
```

> **Colab:** se for usar o Google Colab, não é necessário ambiente virtual. Instale as bibliotecas (se faltar) com:
>
> ```python
> !pip install pandas numpy matplotlib seaborn plotly geopy ipywidgets
> ```

### 4️⃣ Executar o notebook

Abra o arquivo:

```bash
notebooks/Analise_Exploratoria.ipynb
```

Ou acesse via navegador:  
https://colab.research.google.com/

---

## 📈 Etapas do Projeto

1. **Coleta de Dados** — obtenção via API e dataset do Kaggle.  
2. **Limpeza e Tratamento** — padronização, remoção de valores nulos e outliers.  
3. **Análise Exploratória (EDA)** — descrição estatística e visualização dos padrões.  
4. **Integração Climática x Poluição** — análise da correlação entre variáveis meteorológicas e poluentes.  
5. **Discussão e Insights** — interpretação dos resultados no contexto da COP30.

---

## 🧾 Arquivo de Requisitos

Disponível como `requirements.txt`.

---

## 📜 Licença

Este projeto está licenciado sob a **MIT License**.

---

## 👥 Contribuintes
 
- [Carolina Penido Barcellos](https://github.com/carolinabarcellos)
- [Gabrielly Xavier dos Santos](https://github.com/gabyxsantos)
- [Marcelo Henrique Pereira Oliveira e Silva](https://github.com/marcelohpos) 
- [Matheus Soares dos Santos de Freitas](https://github.com/Doctor-Math)  

**Data de início:** Outubro de 2025  
**Última atualização:** Dezembro de 2025
