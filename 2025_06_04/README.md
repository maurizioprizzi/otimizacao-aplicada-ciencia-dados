# 📅 Aula 04/06/2025 - Programação com Restrições

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![OR-Tools](https://img.shields.io/badge/OR--Tools-9.8+-green.svg)](https://developers.google.com/optimization)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

Materiais práticos da aula de **Programação com Restrições** aplicada à **Ciência de Dados**, ministrada em **04 de Junho de 2025**.

## 🎯 Objetivo da Aula

Demonstrar a aplicação prática de **Programação com Restrições (CP)** usando **OR-Tools** do Google para resolver problemas reais de otimização em laboratórios e pipelines de dados.

## 📊 Projetos Desenvolvidos

### 🍷 **Projeto 1: Otimização de Alocação de Amostras** [`01.ipynb`]

**📋 Problema:**  
Um laboratório de análise enológica precisa alocar 5 amostras de vinho para 2 máquinas de teste, minimizando custos operacionais.

**🔧 Abordagem:**
- **Variáveis:** Alocação binária (amostra → máquina)
- **Restrições:** Cada amostra em exatamente uma máquina + capacidade máxima
- **Objetivo:** Minimizar custo total = Σ(custo_máquina × alocações)

**📈 Resultados:**
- ✅ **Custo Ótimo:** 600 unidades
- ✅ **Máquina 1:** Amostras A, B, C (3/3 utilizadas)
- ✅ **Máquina 2:** Amostras D, E (2/2 utilizadas)
- ✅ **Tempo de Solução:** < 1ms

**💡 Conceitos Demonstrados:**
- Modelagem com variáveis booleanas
- Restrições de cardinalidade
- Comparação implementação básica vs. modular

---

### 📊 **Projeto 2: Agendamento Inteligente de Tarefas** [`02.ipynb`]

**📋 Problema:**  
Agendar 6 tarefas de análise do dataset Iris em 2 máquinas, respeitando dependências de precedência e otimizando makespan.

**🔧 Abordagem:**
- **Variáveis:** Tripla (tarefa, slot_tempo, máquina)
- **Restrições:** Precedência temporal + uma tarefa por slot + capacidade
- **Objetivos:** Minimizar makespan OU balancear carga entre máquinas

**📈 Resultados:**
- ✅ **Makespan Ótimo:** 4 slots de tempo
- ✅ **Precedências Respeitadas:** 100% das dependências
- ✅ **Balanceamento:** Carga uniforme entre máquinas
- ✅ **Pipeline Completo:** Carregamento → Limpeza → Análise → Visualização

**💡 Conceitos Demonstrados:**
- Restrições de precedência temporal
- Otimização multi-objetivo
- Classe reutilizável `TaskScheduler`
- Visualização tipo Gantt Chart

## 🛠️ Configuração e Execução

### **Pré-requisitos**
```bash
# Instale as dependências
pip install -r requirements.txt

# Ou instale manualmente:
pip install ortools pandas matplotlib seaborn scikit-learn jupyter
```

### **Executando os Projetos**
```bash
# Inicie o Jupyter Notebook
jupyter notebook

# Execute na ordem recomendada:
# 1. 01.ipynb - Alocação de Amostras (30 min)
# 2. 02.ipynb - Agendamento de Tarefas (45 min)
```

### **Estrutura dos Arquivos**
```
📂 2025_06_04/
├── 📓 01.ipynb                                      # Projeto 1: Alocação
├── 📓 02.ipynb                                      # Projeto 2: Agendamento
├── 📚 Documento Científico - Otimização com OR-Tools.pdf  # Paper completo
├── 📋 requirements.txt                              # Dependências
└── 📖 README.md                                     # Este arquivo
```

## 🎮 Exercícios Práticos

### 🔰 **Iniciante (30 min)**
1. **Modifique o Projeto 1:**
   - Altere custos das máquinas para [80, 200]
   - Teste com 3 máquinas em vez de 2
   - Compare os resultados

2. **Explore o Projeto 2:**
   - Execute com 6 slots em vez de 4
   - Teste o objetivo de balanceamento
   - Observe as diferenças no cronograma

### 🎯 **Intermediário (1h)**
1. **Estenda o Projeto 1:**
   - Adicione tipos diferentes de amostras (tinto, branco, rosé)
   - Implemente restrições de compatibilidade
   - Crie custos dependentes do tipo de análise

2. **Melhore o Projeto 2:**
   - Adicione durações variáveis (1-3 slots por tarefa)
   - Implemente prioridades nas tarefas
   - Crie janelas de tempo obrigatórias

### 🚀 **Avançado (2h+)**
1. **Integração dos Projetos:**
   - Combine alocação + agendamento em um problema único
   - Use dados reais de um dataset maior (Wine Quality)
   - Implemente interface interativa com widgets

2. **Aplicação Real:**
   - Modele um problema do seu trabalho/estudo
   - Implemente otimização multi-objetivo com pesos
   - Desenvolva análise de sensibilidade automática

## 📚 Conceitos-Chave Abordados

### 🧠 **Teóricos**
- **Constraint Programming (CP)** vs. Linear Programming (LP)
- **Variáveis de Decisão** e domínios discretos
- **Restrições Hard** vs. objetivos de otimização
- **Satisfiabilidade** vs. otimalidade
- **Complexidade computacional** em problemas combinatórios

### 💻 **Práticos**
- **OR-Tools CP-SAT Solver**: API e modelagem
- **Variáveis Booleanas**: NewBoolVar() para decisões 0/1
- **Restrições de Soma**: Add(sum(...) == valor)
- **Precedência Temporal**: Add(var1 < var2)
- **Objetivos**: Minimize() e Maximize()

## 📊 Técnicas de Implementação

### **Projeto 1 - Padrões de Código:**
```python
# Variável de decisão binária
assignment = {}
for s in samples:
    for m in machines:
        assignment[(s, m)] = model.NewBoolVar(f'assign_{s}_{m}')

# Restrição: cada amostra em exatamente uma máquina
for s in samples:
    model.Add(sum(assignment[(s, m)] for m in machines) == 1)

# Objetivo: minimizar custos
model.Minimize(sum(assignment[(s, m)] * costs[m] 
                  for s in samples for m in machines))
```

### **Projeto 2 - Classe Reutilizável:**
```python
class TaskScheduler:
    def __init__(self, tasks, machines, max_slots):
        self.model = cp_model.CpModel()
        self.assignments = {}  # (task, slot, machine): BoolVar
        
    def add_precedence_constraint(self, task_before, task_after):
        # Implementa: task_before deve terminar antes de task_after começar
        
    def set_objective_minimize_makespan(self):
        # Minimiza o último slot usado
        
    def solve_and_display(self):
        # Resolve o modelo e exibe cronograma visual
```

## 🎨 Visualizações Geradas

### **Projeto 1 - Gráficos:**
- 📊 **Barras**: Distribuição de amostras por máquina
- 💰 **Custos**: Comparação de custos por configuração
- 📋 **Tabela**: Detalhamento da alocação ótima

### **Projeto 2 - Cronogramas:**
- 📅 **Gantt Chart**: Timeline visual das tarefas
- ⚖️ **Balanceamento**: Utilização das máquinas por slot
- 🎯 **Métricas**: Makespan, eficiência, tempo ocioso

## 📖 Material Complementar

### **Para Aprofundamento:**
- 📚 **Paper Científico:** `Documento Científico - Otimização com OR-Tools.pdf`
- 🌐 **OR-Tools Guide:** [developers.google.com/optimization](https://developers.google.com/optimization)
- 📘 **Livro:** "Handbook of Constraint Programming" - Rossi, van Beek, Walsh

### **Datasets Utilizados:**
- 🍷 **Wine Dataset:** Amostras sintéticas para demonstração
- 🌸 **Iris Dataset:** Sklearn.datasets para pipeline realista

## 🤔 FAQ - Dúvidas Frequentes

**❓ Por que OR-Tools em vez de outras bibliotecas?**  
OR-Tools é otimizado para problemas combinatórios, tem sintaxe clara e é mantido pelo Google. PuLP é bom para LP, mas CP-SAT é superior para problemas discretos.

**❓ Qual a diferença entre CP e programação linear?**  
CP trabalha com domínios discretos e restrições não-lineares. LP assume variáveis contínuas e restrições lineares. CP é melhor para scheduling, alocação, etc.

**❓ Como escolher entre minimizar makespan vs. balancear carga?**  
Makespan minimiza tempo total (urgência). Balanceamento distribui trabalho uniformemente (equidade). A escolha depende da prioridade do negócio.

**❓ OR-Tools sempre encontra a solução ótima?**  
Para problemas pequenos/médios, sim. Para problemas grandes, pode retornar boas soluções dentro do tempo limite configurado.

## 🏆 Resultados de Aprendizagem

Ao completar esta aula, você será capaz de:

### ✅ **Habilidades Técnicas**
- Modelar problemas de alocação usando programação com restrições
- Implementar algoritmos de scheduling com dependências
- Usar OR-Tools CP-SAT para resolver problemas combinatórios
- Comparar diferentes estratégias de otimização

### ✅ **Competências Analíticas**
- Identificar quando usar CP vs. outras técnicas
- Analisar trade-offs entre objetivos conflitantes
- Interpretar resultados de otimização em contexto de negócio
- Desenvolver soluções escaláveis e reutilizáveis

## 🔗 Próximos Passos

### **📅 Para a Próxima Aula:**
- **Tópico:** Programação Linear e Otimização de Portfólio
- **Preparação:** Revisar álgebra linear e conceitos de risco/retorno
- **Bibliografia:** Seções sobre simplex e programação linear

### **🎯 Para Casa:**
1. Complete todos os exercícios propostos
2. Leia o documento científico completo
3. Teste os códigos com seus próprios dados
4. Explore a documentação do OR-Tools

## 📞 Contato

**Prof. Maurizio Prizzi**
- 📧 **Email:** [maurizioprizzi@gmail.com](mailto:maurizioprizzi@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/maurizioprizzi](https://www.linkedin.com/in/maurizioprizzi/)
- 🐙 **GitHub:** [github.com/maurizioprizzi](https://github.com/maurizioprizzi)

---

⭐ **Gostou dos projetos? Deixe uma estrela no repositório!**  
🔄 **Compartilhe** com colegas interessados em otimização!  
💬 **Dúvidas?** Abra uma issue ou me envie um email!

🎓 **Bons estudos e excelentes otimizações!** 🚀