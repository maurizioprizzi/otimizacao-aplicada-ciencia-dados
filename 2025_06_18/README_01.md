# Exemplo 1: Otimização de Hiperparâmetros para Detecção de Fraudes

Bem-vindo ao **Exemplo 1** do curso *Modelagem Matemática Aplicada à Otimização em Análise de Dados*! Este projeto, criado pelo Prof. Maurizio Prizzi (CEUB), demonstra como usar técnicas de Machine Learning para detectar fraudes financeiras, otimizando um modelo para equilibrar a detecção de fraudes e a experiência do usuário.

Este README explica o que o código faz, como ele funciona e como você pode executá-lo. É ideal para alunos que estão aprendendo sobre otimização, Machine Learning e análise de dados.

---

## 📖 O que este projeto faz?

O código implementa um pipeline completo para treinar e otimizar um modelo de Machine Learning que detecta fraudes financeiras em transações bancárias. Ele usa um dataset sintético que simula transações reais, com 96% de transações legítimas e 4% fraudulentas (um cenário comum em fintechs).

O objetivo é **maximizar a detecção de fraudes** (identificar o maior número possível de transações fraudulentas) enquanto **minimiza falsos positivos** (evita classificar transações legítimas como fraudes, para não incomodar os clientes). Para isso, o código:

1. Cria um dataset sintético com 15 mil transações e 18 características (como valor da transação, hora do dia, localização, etc.).
2. Define uma função objetivo personalizada que combina três métricas:
   - **Recall**: Percentual de fraudes detectadas.
   - **Precisão**: Percentual de alertas que são realmente fraudes.
   - **Experiência do usuário**: Minimizar falsos positivos.
3. Divide os dados em treino (75%) e teste (25%), com normalização das features numéricas.
4. Otimiza os hiperparâmetros de um modelo Random Forest usando busca em grade (`GridSearchCV`) ou busca aleatória (`RandomizedSearchCV`).
5. Avalia o modelo com métricas detalhadas (Recall, Precisão, F1-Score, AUC-ROC).
6. Gera visualizações (matriz de confusão, importância de features, curva ROC, convergência da otimização).
7. Calcula o impacto financeiro do modelo (benefícios de detectar fraudes versus custos de falsos positivos e fraudes não detectadas).
8. Apresenta insights práticos e conceitos matemáticos aplicados.

O código é inspirado em práticas reais de empresas que desenvolvem sistemas antifraude para fintechs.

---

## 🧠 Conceitos aprendidos

Este projeto ensina conceitos fundamentais de Machine Learning, otimização e análise de dados, com base em matemática aplicada:

- **Otimização multi-objetivo**: Como combinar diferentes objetivos (detecção, precisão, experiência do usuário) em uma única função.
- **Busca de hiperparâmetros**: Uso de `GridSearchCV` ou `RandomizedSearchCV` para encontrar a melhor configuração do modelo.
- **Validação cruzada estratificada**: Garante que o modelo seja avaliado de forma robusta, preservando a proporção de fraudes.
- **Desbalanceamento de classes**: Lida com datasets onde uma classe (fraudes) é muito menos frequente.
- **Análise de trade-offs**: Avalia o impacto financeiro das decisões do modelo (e.g., custo de falsos positivos versus fraudes não detectadas).
- **Métricas de avaliação**: Recall, Precisão, F1-Score, AUC-ROC e matriz de confusão.
- **Visualização de dados**: Gráficos para entender o desempenho e a importância das features.

**Conceitos matemáticos**:
- Otimização combinatorial discreta.
- Função objetivo ponderada.
- Impureza de Gini/Entropia em árvores de decisão.
- Trade-off entre viés e variância em modelos ensemble.

---

## 📁 Estrutura do código

O arquivo principal é `fraud_detection_optimized.py`, que está dividido em 9 seções comentadas:

1. **Geração do dataset**: Cria um dataset sintético com 15 mil transações e verifica a proporção de fraudes.
2. **Função objetivo**: Define uma métrica personalizada que combina recall, precisão e experiência do usuário.
3. **Preparação dos dados**: Divide os dados em treino/teste e normaliza as features numéricas.
4. **Espaço de busca**: Configura os hiperparâmetros a serem otimizados (e.g., número de árvores, profundidade).
5. **Otimização**: Executa a busca de hiperparâmetros com validação cruzada e mede o tempo de execução.
6. **Avaliação do modelo**: Calcula métricas de desempenho no conjunto de teste.
7. **Visualizações**: Gera gráficos para análise (matriz de confusão, importância de features, curva ROC, convergência).
8. **Trade-offs de negócio**: Estima o impacto financeiro do modelo (ROI, custos, benefícios).
9. **Insights e conclusões**: Resume os resultados e sugere aplicações práticas.

**Arquivos gerados**:
- `modelo_fraudes_rf.pkl`: Modelo Random Forest otimizado.
- `scaler_fraudes.pkl`: Normalizador das features.
- `resultados_search_cv.csv`: Resultados detalhados da busca de hiperparâmetros.
- Gráficos exibidos na tela (não salvos como arquivos).

---

## 🚀 Como executar o projeto

Siga estas instruções para clonar e executar o código no seu computador.

### Pré-requisitos
- **Python 3.8+** instalado.
- Bibliotecas necessárias:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `matplotlib`
  - `seaborn`
  - `joblib`
- Um ambiente virtual (opcional, mas recomendado).

### Passo a passo

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/maurizioprizzi/otimizacao-aplicada-ciencia-dados.git
   cd otimizacao-aplicada-ciencia-dados
   ```

2. **Crie um ambiente virtual** (opcional):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. **Instale as dependências**:
   Crie um arquivo `requirements.txt` com o seguinte conteúdo:
   ```
   pandas
   numpy
   scikit-learn
   matplotlib
   seaborn
   joblib
   ```
   Em seguida, instale:
   ```bash
   pip install -r requirements.txt
   ```

4. **Execute o código**:
   Certifique-se de que o arquivo `fraud_detection_optimized.py` está na pasta. Execute:
   ```bash
   python fraud_detection_optimized.py
   ```

5. **Explore os resultados**:
   - O terminal mostrará informações sobre o dataset, métricas, hiperparâmetros e impacto financeiro.
   - Gráficos serão exibidos na tela (matriz de confusão, curva ROC, etc.).
   - Arquivos como `modelo_fraudes_rf.pkl` e `resultados_search_cv.csv` serão salvos na pasta.

---

## 🔧 Personalizando o código

Você pode experimentar modificações para aprender mais:

- **Mudar o dataset**:
  - Altere `n_transacoes` ou `weights` na função `criar_dataset_transacoes_financeiras` para criar datasets maiores ou com mais/menos fraudes.
- **Ajustar a função objetivo**:
  - Modifique os pesos (`peso_deteccao`, `peso_precisao`, `peso_experiencia`) na função `funcao_objetivo_fintech` para priorizar diferentes objetivos.
- **Testar outros algoritmos**:
  - Substitua `RandomForestClassifier` por `XGBClassifier` ou `LogisticRegression` na seção 4.
- **Usar Grid Search ou Randomized Search**:
  - Altere a variável `use_random_search` para `False` (seção 4) para usar `GridSearchCV` em vez de `RandomizedSearchCV`.
- **Explorar os resultados**:
  - Abra o arquivo `resultados_search_cv.csv` em uma planilha para analisar todas as combinações de hiperparâmetros testadas.

---

## ❓ Perguntas frequentes

**1. Por que o dataset é sintético?**
- Dados reais de fraudes são confidenciais. O dataset sintético simula um cenário realista, com desbalanceamento e features típicas (e.g., valor da transação, localização).

**2. O que significa "otimização de hiperparâmetros"?**
- Hiperparâmetros são configurações do modelo (e.g., número de árvores). A otimização testa várias combinações para encontrar a que maximiza o desempenho.

**3. Por que usar Random Forest?**
- É um modelo robusto, que lida bem com datasets desbalanceados e features variadas, comum em sistemas antifraude.

**4. O que é a função objetivo personalizada?**
- Ela combina recall, precisão e experiência do usuário em um único número, permitindo otimizar o modelo para objetivos de negócio.

**5. Por que os gráficos são importantes?**
- Eles ajudam a visualizar o desempenho (e.g., matriz de confusão mostra erros) e entender quais features são mais relevantes.

---

## 📚 Próximos passos

- **Exemplo 2**: Explore a otimização contínua do limiar de decisão para melhorar o trade-off entre precisão e recall.
- **Leitura complementar**:
  - Documentação do `scikit-learn`: [https://scikit-learn.org/stable/](https://scikit-learn.org/stable/)
- **Exercícios**:
  - Adicione uma nova feature ao dataset (e.g., razão entre valor da transação e saldo médio).
  - Teste o modelo com um dataset maior (e.g., 100 mil transações).
  - Implemente uma métrica adicional na função objetivo (e.g., F1-Score).

---

## 📞 Contato

Dúvidas? Entre em contato com o Prof. Maurizio Prizzi ou abra uma *issue* no repositório:
- Repositório: [https://github.com/maurizioprizzi/otimizacao-aplicada-ciencia-dados](https://github.com/maurizioprizzi/otimizacao-aplicada-ciencia-dados)

Boa aprendizagem e divirta-se explorando o código! 🚀