# Dados-Metereol-gicos
# 🌦️ Monitoramento & Coleta de Dados Meteorológicos

![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

Pipeline completo de coleta, tratamento e visualização de dados climáticos em tempo real. O projeto integra entradas de usuários via **Google Sheets**, consome a API meteorológica pública da **Open-Meteo** e apresenta os resultados tanto em ambiente de análise de dados (**Python/Colab**) quanto em uma interface web responsiva (**HTML/CSS/JS**).

---

## 🎯 Sobre o Projeto

O objetivo deste projeto é automatizar a consulta de temperaturas atuais a partir de coordenadas geográficas cadastradas colaborativamente em uma planilha. 

O fluxo de dados funciona em três etapas:
1. **Ingestão de Dados:** Leitura direta de uma planilha pública do Google Sheets exportada em formato `.csv`.
2. **Enriquecimento via API:** Extração de `Latitude` e `Longitude` de cada registro para consulta dinâmica à API da **Open-Meteo**.
3. **Visualização:** Exibição estruturada no notebook Python ou renderização em cards modernos e responsivos no navegador.

---

## 🛠️ Tecnologias & Ferramentas

* **Coleta & Análise (Notebook):**
  * **Python 3** (Google Colab)
  * **Pandas:** Leitura, estruturação e iteração sobre o dataset CSV.
  * **Requests:** Consumo da API REST da Open-Meteo.
* **Aplicação Web (Frontend):**
  * **HTML5 & CSS3:** Layout responsivo com CSS Grid, variáveis nativas e estilização em *Glassmorphism*.
  * **JavaScript (Vanilla):** Consumo assíncrono via `Fetch API`, requisições paralelas com `Promise.all` e parser customizado de CSV (com tratamento para separadores decimais locais).
* **Fontes de Dados:**
  * [Google Sheets](https://docs.google.com/spreadsheets/d/1vW4hmVmkvqXEQFC14FMRw_rmg8EUFvf4e-IxR0ZJ0oM/edit?usp=sharing) (Base de locais e coordenadas)
  * [Open-Meteo API](https://open-meteo.com/) (Dados meteorológicos gratuitos e sem necessidade de API Key)

---

## 📂 Estrutura do Repositório

```text
├── ColetaDadosMetereologicosipynb.ipynb   # Script original de coleta e análise em Python
├── index.html                            # Dashboard web completo (HTML + CSS + JS)
└── README.md                             # Documentação do projeto
