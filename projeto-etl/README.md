# 🧠 Projeto ETL — Análise Automatizada de Feedbacks Internos
Versão adaptada e expandida por **Karin**

---

## 📘 Sobre o Projeto

Este projeto é uma **reimaginação completa** do pipeline ETL estudado no Santander Dev Week 2023.  
Enquanto o material original utiliza APIs externas para processamento, esta nova versão explora um domínio totalmente diferente e **remove qualquer dependência de serviços externos**, garantindo reprodutibilidade total.

O objetivo é demonstrar como dados textuais brutos podem ser convertidos em insights valiosos utilizando apenas Python e bibliotecas locais.

---

## 🎯 Objetivo Geral

Construir um pipeline **ETL (Extração, Transformação e Carregamento)** totalmente funcional que:

✔ Extrai arquivos `.txt` com feedbacks internos  
✔ Processa e limpa o texto  
✔ Remove stopwords  
✔ Classifica sentimento simples (positivo, negativo ou neutro)  
✔ Calcula métricas úteis (ex.: contagem de palavras)  
✔ Gera arquivos finais em **CSV** e **JSON**

Tudo isso sem uso de APIs externas ou dependência de internet.

---

## 🧱 Arquitetura do ETL

### **1. Extração**
Os dados são carregados a partir de uma pasta local (`/content/dados_feedbacks/`).  
Cada arquivo `.txt` representa um feedback individual.

### **2. Transformação**
São aplicadas diversas etapas:

- Limpeza de caracteres especiais  
- Normalização e padronização  
- Remoção de stopwords (NLTK)  
- Tokenização  
- Análise de sentimento baseada em palavras-chave  
- Contagem de palavras indexadas  

O resultado transforma texto não estruturado em um DataFrame totalmente limpo e analisável.

### **3. Carregamento**

O dataset final é exportado em dois formatos:

- `feedbacks_processados.csv`
- `feedbacks_processados.json`

Isso permite integração com dashboards, BI, bibliotecas analíticas ou sistemas internos.

---

## 🚀 Tecnologias Utilizadas

- Python 3.x  
- Pandas  
- NLTK  
- Regex  
- Google Colab ou VS Code com Jupyter  

---

## 📄 Código Completo do Projeto

O notebook contém:

- Geração de dados fictícios  
- Implementação da etapa E (extração)  
- Implementação da etapa T (transformação)  
- Implementação da etapa L (carregamento)  
- Visualização tabular dos dados  

---
