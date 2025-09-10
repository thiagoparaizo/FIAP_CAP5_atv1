# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="https://avatars.githubusercontent.com/u/70102670?s=200&v=4" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# EasyAgro - FarmTechSolutions

## Nome do grupo

## 👨‍🎓 Integrantes: 
- <a href="https://www.linkedin.com/in/thiagoparaizo/?originalSubdomain=br">Thiago Paraizo</a>

## 👩‍🏫 Professores:
### Tutor(a) 
- <a href="https://www.linkedin.com/company/inova-fusca">Leonardo Ruiz Orabona</a>
### Coordenador(a)
- <a href="https://www.linkedin.com/company/inova-fusca">Andre Godoy Chiovato</a>

## 📜 Descrição

# 🌾 FarmTech Solutions - Análise de Rendimento Agrícola

## Projeto de Machine Learning para Predição de Safras

Este projeto desenvolve modelos de Machine Learning para predição de rendimento agrícola baseado em condições climáticas. Desenvolvido para a FarmTech Solutions, analisa dados de uma fazenda de médio porte (200 hectares) com quatro culturas diferentes: cacau, dendê, arroz e borracha natural.

## 🎯 Objetivos Principais

- **Análise Exploratória:** Compreender relações entre variáveis climáticas e produtividade
- **Clustering:** Descobrir padrões ocultos nas condições de cultivo  
- **Modelagem Preditiva:** Criar modelos específicos por cultura
- **Avaliação:** Comparar performance de cinco algoritmos diferentes

## 📊 Dataset

- **156 registros** de condições climáticas e rendimento
- **4 culturas:** Cocoa beans, Oil palm fruit, Rice paddy, Rubber natural
- **5 variáveis climáticas:** Precipitação, umidade específica, umidade relativa, temperatura
- **Target:** Rendimento da safra (yield)

## 🔬 Metodologia

O projeto segue rigor científico com **correção metodológica importante**: eliminamos data leakage criando modelos separados por cultura usando apenas variáveis climáticas, tornando os modelos praticamente úteis.

**Algoritmos testados:**
- Linear Regression
- Ridge Regression  
- Random Forest
- Gradient Boosting
- Support Vector Regression

## 📈 Principais Resultados

| Cultura | Melhor Modelo | R² Score | Status |
|---------|---------------|----------|---------|
| Rice, paddy | Ridge Regression | 0.341 | ✅ Utilizável |
| Cocoa, beans | Gradient Boosting | 0.214 | ⚠️ Limitado |
| Oil palm fruit | Linear Regression | -0.052 | ❌ Inadequado |
| Rubber, natural | Ridge Regression | -0.247 | ❌ Inadequado |

**Feature mais importante:** Umidade específica (33.3% de influência)

## 🚀 Como Executar

### Pré-requisitos
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### Execução
1. Clone este repositório
2. Abra o Jupyter Notebook: `ThiagoParaizo_rm566159_pbl_fase5.ipynb`
3. Execute as células sequencialmente
4. O notebook contém análise completa com explicações detalhadas

## 🔍 Destaques Técnicos

- **Correção de Data Leakage:** Identificação e correção de vazamento de informação
- **Clustering K-means:** 4 padrões distintos descobertos via método do cotovelo
- **PCA Validation:** 74.76% da variância preservada na visualização 2D
- **Feature Importance:** Umidade específica identificada como fator-chave

## 💡 Insights Principais

1. **Variáveis climáticas alone são insuficientes** para culturas complexas
2. **Rice e Cocoa são mais previsíveis** que Oil palm e Rubber
3. **Umidade específica > Temperatura > Precipitação** em ordem de importância
4. **22% de outliers** sugerem necessidade de variáveis adicionais

## ⚠️ Limitações Reconhecidas

- Dataset pequeno (39 registros por cultura)
- Ausência de variáveis de solo, manejo e genética
- Modelos falham para Oil palm e Rubber natural
- Necessidade de validação temporal

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
