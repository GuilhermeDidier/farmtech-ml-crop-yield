# 📓 Notebooks do Projeto

Este diretório contém todos os notebooks Jupyter do projeto, organizados em ordem de execução.

## 📋 Ordem de Execução

Execute os notebooks na seguinte ordem:

### 1️⃣ Análise Exploratória de Dados (EDA)
**Arquivo:** `analise_exploratoria_crop_yield.ipynb`

**Conteúdo:**
- Carregamento e inspeção do dataset
- Análise de qualidade dos dados (nulos, duplicatas)
- Estatísticas descritivas completas
- Visualizações (histogramas, boxplots, correlação)
- Análise por tipo de cultura
- Detecção de outliers (IQR, Z-Score, Isolation Forest)

**Tempo estimado:** 5-10 minutos

---

### 2️⃣ Análise de Clusterização
**Arquivo:** `clusterizacao_crop_yield.ipynb`

**Conteúdo:**
- K-Means clustering com Elbow Method
- Determinação do número ótimo de clusters
- DBSCAN para detecção de outliers por densidade
- Hierarchical Clustering (Agglomerative)
- Comparação dos métodos
- Visualização com PCA (redução dimensional)
- Análise dos clusters formados

**Tempo estimado:** 10-15 minutos

---

### 3️⃣ Modelos Preditivos de Regressão
**Arquivo:** `modelos_preditivos_crop_yield.ipynb`

**Conteúdo:**
- Preparação dos dados (encoding, normalização)
- Treinamento de 5 modelos:
  1. Regressão Linear
  2. Random Forest Regressor
  3. Gradient Boosting Regressor
  4. Support Vector Regression (SVR)
  5. Multi-Layer Perceptron (MLP)
- Comparação de métricas (R², RMSE, MAE, MAPE)
- Análise de importância das features
- Validação cruzada
- Salvamento do melhor modelo

**Tempo estimado:** 15-20 minutos

---

## 🚀 Como Executar

### Método 1: Jupyter Notebook
```bash
# Navegar até a pasta do projeto
cd Documents/farmtech_ml_project

# Abrir Jupyter
jupyter notebook

# Executar os notebooks em ordem
```

### Método 2: Jupyter Lab
```bash
# Abrir Jupyter Lab
jupyter lab

# Navegar até a pasta notebooks e executar
```

### Método 3: VS Code
```bash
# Abrir VS Code na pasta do projeto
code .

# Abrir os notebooks e executar célula por célula
```

---

## 📊 Resultados Esperados

### Análise Exploratória
- ✅ Dataset limpo (sem nulos ou duplicatas)
- ✅ 4 tipos de culturas identificadas
- ✅ ~10% de outliers detectados

### Clusterização
- ✅ 8 clusters ótimos (K-Means)
- ✅ Silhouette Score: ~0.39
- ✅ Identificação de padrões de rendimento

### Modelos Preditivos
- ✅ Random Forest: R² > 0.99 (melhor modelo)
- ✅ Gradient Boosting: R² > 0.99
- ✅ MAPE < 10% (excelente precisão)

---

## 📝 Notas Importantes

- Certifique-se de ter instalado todas as dependências: `pip install -r requirements.txt`
- O dataset `crop_yield.csv` deve estar na pasta `data/`
- Os notebooks geram visualizações que podem demorar alguns segundos
- O treinamento dos modelos pode levar alguns minutos dependendo do hardware
