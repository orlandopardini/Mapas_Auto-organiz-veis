# Análise Não Supervisionada com Mapas Auto-organizáveis (SOM)

Os **Mapas Auto-organizáveis** (Self-Organizing Maps, ou SOMs) são um tipo de rede neural não supervisionada projetada para **redução de dimensionalidade** e **agrupamento de dados complexos**, preservando a topologia original dos dados.

Esses mapas organizam padrões similares em regiões próximas de um grid bidimensional, sendo úteis para **detecção de padrões, clusters e anomalias**, mesmo sem rótulos conhecidos.

### Por que SOMs são eficientes?

- Reduzem a dimensionalidade de dados de forma visual
- Agrupam dados com base em similaridade
- Preservam a estrutura topológica dos dados
- São altamente interpretáveis por meio de mapas de calor

### Exemplo intuitivo

Imagine analisar a renda e a idade de milhares de pessoas. O SOM organiza esses dados de forma que pessoas com **características semelhantes fiquem próximas no mapa**, revelando **grupos e padrões ocultos**, como possíveis classes sociais ou segmentos de mercado.

---

## 📂 Estrutura dos Notebooks

### 1. `SOM1_Credito_Orlando.ipynb`
**📌 Tarefa:** Análise de clientes com base em características de crédito  
**📚 Dataset:** Informações financeiras e cadastrais de clientes  
**🔍 Destaques:**
- Normalização de dados financeiros
- Aplicação de SOM para segmentação de risco
- Visualização de anomalias em clusters

### 2. `SOM2_idade_salario_Orlando.ipynb`
**📌 Tarefa:** Agrupamento de dados simples com idade e salário  
**📚 Dataset:** Informações sintéticas ou reais sobre perfil populacional  
**🔍 Destaques:**
- Aplicação didática para entender o funcionamento do SOM
- Clusterização visível por cor e coordenadas
- Análise bidimensional com fácil interpretação

### 3. `SOM3_Vinhos_Orlando.ipynb`
**📌 Tarefa:** Agrupamento de vinhos por características químicas  
**📚 Dataset:** [Wine Dataset - UCI](https://archive.ics.uci.edu/ml/datasets/wine)  
**🔍 Destaques:**
- Clusterização não supervisionada por atributos químicos
- Visualização de regiões com vinhos similares
- Interpretação de grupos de qualidade

---

## 📈 Métricas e Visualizações

Como técnica não supervisionada, os SOMs são avaliados com base em:

- **Mapas de distância (U-Matrix)**
- **Mapas de ativação de neurônios**
- **Clusters formados visualmente**
- **Identificação de padrões emergentes**

---

## 💡 Observação

Todos os notebooks utilizam a biblioteca `MiniSom`, uma implementação simples e eficiente para SOMs em Python.
"""

# Caminho para salvar o README do SOM
readme_path_som = Path("/mnt/data/README_SOM.md")
readme_path_som.write_text(readme_som, encoding="utf-8")

readme_path_som
