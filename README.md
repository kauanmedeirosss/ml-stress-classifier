# 🧠 Projeto de Machine Learning - Detecção de Estresse

Este repositório contém um projeto de **Machine Learning** focado na **análise e classificação de estresse** a partir de dados de estilo de vida e hábitos.  

O objetivo é explorar técnicas de aprendizado de máquina para prever se um indivíduo está sob **alto, médio ou baixo nível de estresse**, utilizando o dataset [`Stress_Dataset.csv`](./Stress_Dataset.csv).

---

## 📂 Estrutura do Repositório

- `Inteligencia_Artificial.ipynb` → Notebook principal com análise exploratória, pré-processamento e modelos de machine learning.  
- `Stress_Dataset.csv` → Dataset utilizado para treinar e avaliar os modelos.  
- `README.md` → Este arquivo com a documentação do projeto.  

---

## 🚀 Tecnologias Utilizadas

- Python 3.x  
- Pandas & NumPy (manipulação e análise de dados)  
- Matplotlib & Seaborn (visualização de dados)  
- Scikit-learn (modelagem e avaliação de algoritmos de ML)  

---

## 🔍 Metodologia

1. **Análise exploratória de dados (EDA)**  
   - Estatísticas descritivas  
   - Distribuição das variáveis  
   - Correlações entre atributos  

2. **Pré-processamento**  
   - Limpeza de dados  
   - Codificação de variáveis categóricas  
   - Normalização/padronização  

3. **Modelagem (Supervisionada)**  
   - Teste de diferentes algoritmos de Machine Learning  
   - Comparação de métricas de desempenho (accuracy, precision, recall, f1-score)  

4. **Modelagem (Não Supervisionada)**  
   - Aplicação de algoritmos de **clustering**:  
     - **K-Means**  
     - **DBSCAN**  
     - **Agglomerative Clustering**  
   - Determinação do número de clusters com:  
     - Método do Cotovelo  
     - Coeficiente de Silhueta  
   - Avaliação com métricas internas:  
     - **Silhouette Score**  
     - **Davies-Bouldin Index**  
     - **Calinski-Harabasz Index**  
   - Redução de dimensionalidade com **PCA (2D)** para facilitar a visualização.  

5. **Conclusões e próximos passos**  
   - Melhorias possíveis  
   - Sugestões para trabalhos futuros  

---

## 📊 Dataset

O dataset utilizado é o **Stress_Dataset.csv**, que contém informações sobre hábitos, rotinas e fatores que podem influenciar o nível de estresse.  

🔹 *Exemplo de atributos (features):*  
  - Gender → gênero do participante  
  - Age → idade  
  - Have you recently experienced stress in your life?  
  - Have you noticed a rapid heartbeat or palpitations?  
  - Have you been dealing with anxiety or tension recently?  
  - Do you face any sleep problems or difficulties falling asleep?  
  - Have you been getting headaches more often than usual?  
  - Do you get irritated easily?  
  - Do you have trouble concentrating on your academic tasks?  
  - Do you feel overwhelmed with your academic workload?  
  - Do you find that your relationship often causes you stress?  
  - Is your working environment unpleasant or stressful?  
  - Do you lack confidence in your academic performance?  
  - Academic and extracurricular activities conflicting for you?  
  - Do you attend classes regularly?  
  - Have you gained/lost weight?  

🔹 *Variável alvo (target):*  
  - Which type of stress do you primarily experience?  

---

## 📊 Resultados

### Supervisionado
- Bons resultados de classificação foram obtidos em diferentes algoritmos.  
- Modelos baseados em árvores e ensembles tiveram desempenho superior nas métricas de predição.  

### Não Supervisionado
- **K-Means** foi o algoritmo mais eficaz, com clusters bem definidos e consistentes.  
- **Agglomerative Clustering** apresentou desempenho próximo, mas sem benefícios claros sobre o K-Means.  
- **DBSCAN** foi útil para detectar outliers, mas gerou clusters menos definidos.  
- A aplicação de **PCA** mostrou que a maior parte da variabilidade pode ser representada em 2 dimensões, facilitando a visualização dos agrupamentos.  

---

## 🤝 Contribuições

Este projeto foi desenvolvido para fins acadêmicos, mas contribuições são bem-vindas!  
Para sugerir melhorias, abra uma **issue** ou faça um **pull request**.  
