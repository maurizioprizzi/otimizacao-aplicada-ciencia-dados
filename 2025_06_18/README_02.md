# Exemplo 2: Otimização Contínua de Threshold com Busca Ternária

Bem-vindo ao **Exemplo 2** do curso de **Modelagem Matemática Aplicada à Otimização em Análise de Dados**, ministrado pelo Prof. **Maurizio Prizzi** no Centro de Educação UnB (CEUB). Este projeto demonstra como otimizar continuamente o **threshold de classificação** em um modelo de detecção de fraudes, adaptando-se a mudanças nos padrões de dados (conhecidas como *concept drift*), utilizando a técnica de **busca ternária**. O código é inspirado em sistemas reais de calibração automática*.

Este README explica o que o código faz, como ele funciona, como executá-lo e os conceitos matemáticos envolvidos, de forma clara e acessível para alunos.

---

## 📜 Objetivo do Projeto

O objetivo deste projeto é **encontrar o melhor ponto de corte (threshold)** para classificar transações como fraudulentas ou legítimas, maximizando a detecção de fraudes (*recall*), mantendo alta precisão (*precision*) e minimizando falsos alarmes (*false positive rate*). O código também simula mudanças nos dados ao longo do tempo (*concept drift*) e ajusta o threshold automaticamente para manter a performance do modelo.

### Por que isso é importante?
Em sistemas reais de detecção de fraudes (como em bancos ou e-commerce), os padrões de comportamento mudam constantemente. Um threshold fixo (e.g., 0.5) pode se tornar ineficaz. Este projeto mostra como adaptar o modelo dinamicamente, balanceando métricas de negócio e mantendo eficiência computacional.

---

## 🧠 Conceitos Matemáticos e Computacionais

O projeto aborda os seguintes conceitos, ideais para alunos de ciência de dados, estatística ou matemática aplicada:

1. **Busca Ternária**: Um algoritmo eficiente (complexidade O(log₃ n)) para otimizar funções unimodais, usado aqui para encontrar o threshold ideal.
2. **Otimização Contínua**: Ajuste dinâmico de parâmetros em tempo real, essencial para sistemas em produção.
3. **Concept Drift**: Mudanças graduais ou sazonais nos dados, simuladas com variações nas features e probabilidades.
4. **Métricas de Negócio**: Combinação de *recall*, *precision* e *especificidade* com pesos ajustáveis para refletir prioridades (e.g., detectar fraudes sem incomodar clientes legítimos).
5. **Análise de Complexidade**: Comparação entre busca ternária (logarítmica) e busca linear (linear) para demonstrar eficiência.
6. **Visualização de Dados**: Gráficos para análise de convergência, sensibilidade e performance, incluindo uma visualização interativa em ChartJS.

---

## 📂 Estrutura do Código

O arquivo principal é `otimizacao_threshold.py`, que está organizado em 10 seções comentadas:

1. **Geração de Dataset e Modelo Base**: Cria um dataset sintético com 12.000 transações (95% legítimas, 5% fraudulentas) e treina um modelo *Random Forest*.
2. **Função Objetivo**: Define uma função que combina *recall* (65%), *precision* (25%) e *especificidade* (10%) para otimizar o threshold.
3. **Busca Ternária**: Implementa o algoritmo de busca ternária para encontrar o threshold ótimo.
4. **Execução da Otimização**: Aplica a busca ternária ao dataset de teste.
5. **Comparação Padrão vs. Otimizado**: Compara métricas com threshold padrão (0.5) e otimizado.
6. **Visualizações**: Gera gráficos para convergência, sensibilidade, curvas de performance e distribuição de probabilidades. O gráfico de convergência usa ChartJS.
7. **Simulação de Concept Drift**: Simula 12 meses de mudanças nos dados, ajustando o threshold dinamicamente.
8. **Visualização Temporal**: Mostra como o threshold e a performance evoluem com o *concept drift*.
9. **Análise de Complexidade**: Compara a eficiência da busca ternária com a busca linear.
10. **Relatório Final**: Resume resultados, métricas e aplicações práticas.

### Melhorias Implementadas
- Validação de entradas para evitar erros (e.g., probabilidades inválidas).
- Caching da função objetivo para maior eficiência.
- Simulação realista de *concept drift* com variação nas features.
- Logs estruturados com o módulo `logging`.
- Visualização interativa em ChartJS para convergência.
- Modularidade com funções menores e mais legíveis.

---

## 🛠️ Como Executar o Código

### Pré-requisitos
Você precisa de um ambiente Python 3.8+ com as seguintes bibliotecas:
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

### Passo a Passo

1. **Clone o Repositório**
   ```bash
   git clone https://github.com/maurizioprizzi/otimizacao-aplicada-ciencia-dados.git
   cd otimizacao-aplicada-ciencia-dados
   ```

2. **Crie um Ambiente Virtual (opcional, mas recomendado)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. **Instale as Dependências**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

4. **Execute o Código**
   ```bash
   python otimizacao_threshold.py
   ```

5. **Visualize os Resultados**
   - O código gera gráficos em Matplotlib (janelas pop-up).
   - Um JSON para ChartJS é gerado para o gráfico de convergência. Para visualizá-lo, crie uma página HTML simples (exemplo abaixo) e abra no navegador:
     ```html
     <!DOCTYPE html>
     <html>
     <head>
         <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
     </head>
     <body>
         <canvas id="myChart"></canvas>
         <script>
             const ctx = document.getElementById('myChart').getContext('2d');
             new Chart(ctx, /* Cole o JSON gerado pelo código aqui */);
         </script>
     </body>
     </html>
     ```

### Saídas Esperadas
- **Logs no console**: Informações sobre o treinamento do modelo, iterações da busca ternária, métricas e resultados.
- **Gráficos**: Visualizações de convergência, sensibilidade, performance e adaptação temporal.
- **Relatório Final**: Um resumo detalhado com métricas, melhorias e aplicações práticas.

---

## 📊 O que Você Verá ao Executar

1. **Modelo Base**: Um *Random Forest* é treinado em um dataset sintético com 12.000 transações.
2. **Otimização do Threshold**: A busca ternária encontra o threshold ótimo (geralmente próximo de 0.3–0.4, dependendo dos dados).
3. **Comparação**: O threshold otimizado melhora o *recall* e o *F1-score* em relação ao padrão (0.5).
4. **Simulação de Concept Drift**: Durante 12 meses simulados, o threshold se ajusta a mudanças nos dados, mantendo a performance.
5. **Gráficos**:
   - Convergência da busca ternária (ChartJS).
   - Redução do intervalo de busca.
   - Sensibilidade do threshold.
   - Comparação de métricas.
   - Curva Precision-Recall.
   - Distribuição de probabilidades.
   - Evolução do threshold e performance ao longo do tempo.
6. **Análise de Complexidade**: A busca ternária é significativamente mais rápida que a busca linear.
7. **Relatório Final**: Insights sobre a eficácia da abordagem e sua aplicabilidade em sistemas reais.

---

## 📚 Para Estudo Adicional

- **Busca Ternária**: Leia sobre otimização de funções unimodais em livros como *Numerical Optimization* de Nocedal e Wright.
- **Concept Drift**: Explore artigos sobre adaptação em machine learning, como "Learning under Concept Drift" de Gama et al.
- **Detecção de Fraudes**: Veja estudos de caso ou artigos sobre *anomaly detection* em finanças.
- **ChartJS**: Consulte a documentação oficial em [chartjs.org](https://www.chartjs.org/) para criar gráficos interativos.

---

## 🤝 Contribuições e Contato

Este código é um recurso educacional aberto. Sinta-se à vontade para:
- Clonar e experimentar.
- Sugerir melhorias via pull requests.
- Reportar problemas via issues no GitHub.

Para dúvidas ou feedback, entre em contato:
- **Prof. Maurizio Prizzi**: maurizio.prizzi@ceub.edu.br
- **Repositório**: [github.com/maurizioprizzi/otimizacao-aplicada-ciencia-dados](https://github.com/maurizioprizzi/otimizacao-aplicada-ciencia-dados)

---

**Aproveite o aprendizado e explore a otimização aplicada à ciência de dados!**