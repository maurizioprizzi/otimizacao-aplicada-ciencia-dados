# 📊 Otimização Matemática Aplicada à Análise de Dados

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![OR-Tools](https://img.shields.io/badge/OR--Tools-9.8+-green.svg)](https://developers.google.com/optimization)
[![CVXPY](https://img.shields.io/badge/CVXPY-1.4+-orange.svg)](https://www.cvxpy.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![CEUB](https://img.shields.io/badge/CEUB-Modelagem%20Matemática-red.svg)](https://www.ceub.edu.br/)

## 🎓 Sobre este Repositório

Este é o repositório **educacional** da disciplina **Otimização Matemática Aplicada à Análise de Dados**, do curso de **Modelagem Matemática** do [Centro Universitário de Brasília (CEUB)](https://www.ceub.edu.br/).

Aqui você encontrará **todos os projetos práticos**, notebooks interativos e materiais didáticos desenvolvidos ao longo do semestre, focados na aplicação de **técnicas de otimização** para resolver problemas reais de **ciência de dados**.

## 🎯 Objetivo Acadêmico

O objetivo deste repositório é fornecer aos estudantes uma **coleção completa** de exemplos práticos que demonstram como a **otimização matemática** pode ser aplicada para:

- 🔍 **Resolver problemas combinatórios** em análise de dados
- 📊 **Otimizar pipelines** de machine learning
- ⚖️ **Balancear recursos** em sistemas computacionais
- 🎯 **Maximizar eficiência** em processos analíticos
- 🧠 **Integrar teoria e prática** de forma aplicada
- 🎭 **Explorar técnicas não-convexas** para problemas complexos

## 📚 Estrutura do Curso

### 📅 **Cronograma de Aulas Disponíveis**

| Data | Tópico | Tecnologias | Status |
|------|--------|-------------|--------|
| [**2025-06-04**](./2025_06_04/) | 🎮 **Programação com Restrições** | OR-Tools, CP-SAT | ✅ Disponível |
| [**2025-06-11**](./2025_06_11/) | 🎯 **SCOP + Programação Quadrática Não-Convexa** | CVXPY, SciPy, Scikit-learn | ✅ Disponível |
| [**2025-06-18**](./2025_06_18/) | 🛡️ **Otimização Adaptativa para Detecção de Fraudes** | Scikit-learn, Busca Ternária, GridSearchCV | ✅ Disponível |

### 🔍 **Aula Destacada: 2025-06-04**

#### 🍷 **Projeto 1: Alocação Otimizada de Amostras**
- **Problema:** Laboratório enológico com 5 amostras de vinho → 2 máquinas de teste
- **Técnica:** Programação com Restrições (CP)
- **Objetivo:** Minimizar custos operacionais
- **Resultado:** Alocação ótima com custo 600 unidades

#### 📊 **Projeto 2: Agendamento Inteligente de Tarefas**
- **Problema:** 6 tarefas de análise do dataset Iris → 2 máquinas com precedências
- **Técnica:** Constraint Programming + Scheduling
- **Objetivo:** Minimizar makespan OU balancear carga
- **Resultado:** Pipeline completo em 4 slots temporais

### 🌟 **Aula Avançada: 2025-06-11**

#### 🏥 **Projeto 1: Seleção Esparsa de Características para Diagnóstico Médico**
- **Problema:** Dataset de câncer de mama com 30 características → identificar as mais importantes
- **Técnica:** SCOP (Sparse Constrained Optimization Problem) + Programação Quadrática Não-Convexa
- **Inovação:** Combina regularização L1, L0 e termos quadráticos não-convexos
- **Resultado:** Redução de 30 → 8 características mantendo 95.8% de precisão
- **Aplicação:** Diagnóstico médico mais eficiente e interpretável

#### 🛍️ **Projeto 2: Clustering Esparso para Segmentação de Clientes**
- **Problema:** 300 clientes com 20 características (15 relevantes + 5 ruído) → segmentação inteligente
- **Técnica:** SCOP + Clustering Não-Convexo com Seleção Automática de Características
- **Inovação:** Descobre grupos naturais E elimina características irrelevantes simultaneamente
- **Resultado:** 4 segmentos bem definidos usando apenas características relevantes
- **Aplicação:** Marketing direcionado com insights mais claros

### 🚀 **NOVA AULA: 2025-06-18**

#### 🛡️ **Projeto 1: Otimização de Hiperparâmetros para Detecção de Fraudes**
- **Problema:** Sistema antifraude para fintech com 15 mil transações (96% legítimas, 4% fraudes)
- **Técnica:** Otimização Multi-Objetivo + GridSearchCV/RandomizedSearchCV
- **Inovação:** Função objetivo personalizada combinando recall, precisão e experiência do usuário
- **Resultado:** Modelo Random Forest otimizado com trade-off ideal entre detecção e falsos positivos
- **Aplicação:** Sistemas bancários e e-commerce com impacto financeiro quantificado

#### 🎯 **Projeto 2: Otimização Contínua de Threshold com Busca Ternária**
- **Problema:** Adaptação automática do limiar de classificação para mudanças nos padrões de fraude (concept drift)
- **Técnica:** Busca Ternária + Otimização Contínua + Simulação de Concept Drift
- **Inovação:** Algoritmo O(log₃ n) para ajuste dinâmico em tempo real, 12 meses de simulação
- **Resultado:** Threshold adaptativo (0.3-0.4) superando o padrão fixo (0.5) em recall e F1-score
- **Aplicação:** Sistemas de produção que se adaptam automaticamente a novos padrões de fraude

#### 🔬 **Conceitos Revolucionários Introduzidos:**
- **🎯 Otimização Multi-Objetivo:** Balanceamento de métricas conflitantes (detecção vs. experiência do usuário)
- **⚡ Busca Ternária:** Algoritmo logarítmico para otimização de funções unimodais
- **🔄 Concept Drift:** Adaptação automática a mudanças temporais nos dados
- **📊 Métricas de Negócio:** ROI quantificado, custos de falsos positivos vs. fraudes não detectadas
- **🎮 Otimização Adaptativa:** Sistemas que aprendem e se ajustam continuamente
- **🔍 Trade-off Analysis:** Análise matemática de custos-benefícios em decisões de ML

## 👨‍🎓 Direitos e Permissões para Alunos CEUB

### ✅ **LIBERDADE TOTAL PARA ESTUDANTES**

**Caros alunos do curso de Modelagem Matemática do CEUB,**

Este repositório é **100% aberto** para vocês! Sintam-se **completamente livres** para:

- 📥 **Clonar** o repositório para seus computadores pessoais
- 🔧 **Modificar** códigos e experimentos conforme necessário
- 🚀 **Contribuir** com melhorias, correções ou novos exemplos
- 📤 **Fazer fork** e criar suas próprias versões
- 📚 **Usar como base** para projetos acadêmicos e trabalhos
- 🎓 **Estudar** todos os materiais sem qualquer restrição
- 💡 **Propor** novos problemas ou abordagens

### 🤝 **Como Contribuir**

1. **Fork** este repositório
2. **Crie** uma branch para sua feature: `git checkout -b minha-contribuicao`
3. **Commit** suas mudanças: `git commit -m 'Adiciona nova funcionalidade'`
4. **Push** para a branch: `git push origin minha-contribuicao`
5. **Abra** um Pull Request

### 🏆 **Reconhecimento Acadêmico**

Contribuições significativas de alunos serão:
- ⭐ **Creditadas** nos commits e documentação
- 🎯 **Consideradas** para bonificação na disciplina
- 📢 **Destacadas** como exemplos de excelência
- 🚀 **Recomendadas** para outros estudantes

## 🛠️ Tecnologias e Ferramentas

### **Bibliotecas Principais:**
- 🧮 **OR-Tools:** Otimização combinatória e linear
- 🎯 **CVXPY:** Otimização convexa e não-convexa
- 📊 **Pandas/NumPy:** Manipulação e análise de dados
- 📈 **Matplotlib/Seaborn:** Visualização de resultados
- 🧠 **Scikit-learn:** Machine learning e datasets
- 📓 **Jupyter:** Notebooks interativos
- ⚡ **SciPy:** Algoritmos de otimização avançados
- 🎮 **Joblib:** Paralelização e persistência de modelos

### **Áreas de Aplicação:**
- 🏥 **Medicina:** Diagnóstico inteligente e seleção de biomarcadores
- 🛍️ **Marketing:** Segmentação de clientes e análise comportamental
- 🛡️ **Fintech:** Detecção de fraudes e sistemas antifraude
- 🏭 **Otimização de Processos Industriais**
- 📦 **Logística e Supply Chain**
- 💰 **Otimização de Portfólios Financeiros**
- 🚀 **Scheduling de Recursos Computacionais**
- 🧬 **Bioinformática e Análise Genômica**

## 🚀 Quick Start

### **Pré-requisitos:**
```bash
# Python 3.8+ obrigatório
python --version

# Git para versionamento
git --version
```

### **Instalação:**
```bash
# 1. Clone o repositório
git clone https://github.com/maurizioprizzi/otimizacao-aplicada-ciencia-dados.git

# 2. Entre na pasta
cd otimizacao-aplicada-ciencia-dados

# 3. Navegue para uma aula específica
cd 2025_06_18  # Para a aula mais recente

# 4. Instale dependências
pip install -r requirements.txt

# 5. Execute os exemplos
python fraud_detection_optimized.py  # Exemplo 1
python otimizacao_threshold.py      # Exemplo 2

# 6. Para notebooks Jupyter (se disponível)
jupyter notebook
```

### **Estrutura de Pastas:**
```
📦 otimizacao-aplicada-ciencia-dados/
├── 📖 README.md                         # Este arquivo
├── 🙈 .gitignore                       # Controle de versionamento
├── 📅 2025_06_04/                      # Aula: Programação com Restrições
│   ├── 📓 01_alocacao_amostras.ipynb   # Alocação de Amostras
│   ├── 📓 02_agendamento_tarefas.ipynb # Agendamento de Tarefas
│   ├── 📚 documento_cientifico.pdf     # Paper completo
│   └── 📖 README.md                    # Detalhes da aula
├── 📅 2025_06_11/                      # Aula: SCOP + NonConvex QP
│   ├── 📓 01.ipynb                     # Seleção de Características Médicas
│   ├── 📓 02.ipynb                     # Clustering Esparso de Clientes
│   ├── 🐍 scop_classificacao_comentado.py  # Código comentado completo
│   ├── 🐍 scop_clustering_comentado.py     # Código comentado completo
│   └── 📖 README.md                    # Detalhes da aula
├── 📅 2025_06_18/                      # Aula: Otimização Adaptativa para Fraudes
│   ├── 🐍 fraud_detection_optimized.py # Exemplo 1: Otimização de Hiperparâmetros
│   ├── 🐍 otimizacao_threshold.py      # Exemplo 2: Busca Ternária + Concept Drift
│   ├── 📖 README_01.md                 # Detalhes do Exemplo 1
│   ├── 📖 README_02.md                 # Detalhes do Exemplo 2
│   └── 📖 README.md                    # Visão geral da aula
```

## 📖 Filosofia Educacional

### 🎓 **Aprendizado Baseado em Projetos**
Cada aula apresenta **problemas reais** que você poderia encontrar na **indústria** ou **pesquisa acadêmica**. Não são apenas exercícios teóricos!

### 🔬 **Teoria + Prática Integradas**
- 📚 **Fundamento teórico** sólido antes da implementação
- 💻 **Código comentado** e explicado linha por linha
- 🎯 **Resultados interpretados** no contexto do problema
- 🔄 **Iteração** entre conceitos e aplicação

### 🚀 **Mentalidade Open Source**
Este repositório segue os **princípios do software livre**:
- **Transparência:** Todo código é aberto e documentado
- **Colaboração:** Melhorias vêm da comunidade
- **Evolução:** Conteúdo se aprimora continuamente
- **Acessibilidade:** Conhecimento livre para todos

### 🧠 **Progressão Pedagógica**
- **Aula 1:** Conceitos básicos com problemas combinatórios
- **Aula 2:** Técnicas avançadas com otimização não-convexa
- **Aula 3:** Otimização adaptativa com aplicações em tempo real
- **Próximas:** Complexidade crescente e aplicações interdisciplinares

## 🌟 Destaques da Nova Aula (2025-06-18)

### 🛡️ **Por que Otimização Adaptativa para Fraudes é Crucial?**

#### **Problemas Tradicionais:**
- Sistemas de detecção com **thresholds fixos** se tornam ineficazes rapidamente
- **Concept drift** não é considerado: padrões de fraude mudam constantemente
- Trade-off entre **detecção** e **experiência do usuário** não é otimizado matematicamente
- Hiperparâmetros ajustados manualmente, sem garantia de otimalidade

#### **Solução com Otimização Adaptativa:**
- **Otimização multi-objetivo:** Combina recall, precisão e experiência do usuário
- **Busca ternária:** Algoritmo O(log₃ n) para encontrar threshold ótimo rapidamente
- **Adaptação automática:** Sistema se ajusta a mudanças nos dados (concept drift)
- **Quantificação de ROI:** Impacto financeiro medido e otimizado

### 🔬 **Inovações Técnicas da Aula 18/06:**

#### **1. Função Objetivo Multi-Criterio:**
```
Score = w₁ × Recall + w₂ × Precision + w₃ × (1 - FPR)
          ↑              ↑                   ↑
    Detectar fraudes  Evitar alarmes   Experiência positiva
```

#### **2. Busca Ternária para Threshold:**
- **Complexidade:** O(log₃ n) vs O(n) da busca linear
- **Convergência:** Garantida para funções unimodais
- **Eficiência:** 90% menos iterações que métodos tradicionais

#### **3. Simulação de Concept Drift:**
- **12 meses simulados** com mudanças graduais nos padrões
- **Adaptação automática** do threshold a cada período
- **Métricas de estabilidade** para avaliar robustez

#### **4. Análise de Impacto Financeiro:**
- **ROI calculado:** Benefícios de detectar fraudes vs custos de falsos positivos
- **Threshold economicamente ótimo:** Maximiza lucro real, não apenas métricas técnicas
- **Sensibilidade de custos:** Como variações nos custos afetam o threshold ideal

### 💡 **Aplicações Demonstradas:**

#### **🛡️ Fintech: "Sistema Antifraude Inteligente"**
- **Entrada:** 15 mil transações com 18 características
- **Otimização:** GridSearchCV + função objetivo personalizada
- **Resultado:** Modelo balanceado entre detecção (alta) e falsos positivos (baixos)
- **Impacto:** Sistema robusto para produção com ROI quantificado

#### **🎯 Adaptação Temporal: "Threshold que Evolui"**
- **Entrada:** Dados com concept drift simulado (12 meses)
- **Busca Ternária:** Threshold otimizado dinamicamente (0.3-0.4)
- **Resultado:** Performance superior ao threshold fixo (0.5)
- **Impacto:** Sistema que se mantém eficaz mesmo com mudanças nos padrões

### 📈 **Benefícios Mensuráveis:**
- **Recall:** +15% comparado ao threshold padrão
- **F1-Score:** +12% com otimização contínua
- **Tempo de otimização:** 90% redução com busca ternária
- **ROI:** Quantificado com base em custos reais de fraudes e falsos positivos

## 🏫 Integração com o CEUB

### 📧 **Suporte Acadêmico:**

**Para dúvidas relacionadas à disciplina, notas, ou conteúdo oficial:**
- 🎓 **Email Institucional:** [maurizio.prizzi@ceub.edu.br](mailto:maurizio.prizzi@ceub.edu.br)
- 🏢 **Horário de atendimento:** Conforme cronograma do CEUB
- 📍 **Localização:** Campus de acordo com a grade de horários

**Para discussões técnicas, colaborações no código, ou dúvidas sobre implementação:**
- 📧 **Email Pessoal:** [maurizioprizzi@gmail.com](mailto:maurizioprizzi@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/maurizioprizzi](https://www.linkedin.com/in/maurizioprizzi/)
- 🐙 **GitHub:** [github.com/maurizioprizzi](https://github.com/maurizioprizzi)

### 🎯 **Alinhamento Curricular:**
Os projetos deste repositório estão **alinhados** com:
- 📋 **Ementa oficial** da disciplina
- 🎓 **Objetivos de aprendizagem** do curso
- 📊 **Competências** exigidas pelo MEC
- 🔗 **Integração** com outras disciplinas do currículo

## 🌟 Benefícios para Sua Carreira

### 💼 **Portfólio Profissional**
- **Projetos reais** que você pode mostrar em entrevistas
- **Código limpo** e bem documentado no seu GitHub
- **Diversidade** de técnicas e tecnologias aplicadas
- **Experiência** com problemas não-convexos (diferencial competitivo!)
- **Sistemas adaptativos** (competência valorizada em fintech)

### 🧠 **Competências Desenvolvidas**
- **Pensamento analítico** para modelagem de problemas complexos
- **Programação científica** em Python com bibliotecas avançadas
- **Visualização** de dados e comunicação de resultados
- **Otimização não-convexa** (competência rara no mercado)
- **Integração teoria-prática** em problemas multidisciplinares
- **Sistemas antifraude** (área em alta demanda)

### 🎯 **Aplicações Imediatas**
- **Estágios** em empresas de tecnologia, consultoria e fintech
- **Iniciação científica** em projetos de pesquisa aplicada
- **Trabalho de conclusão** de curso (TCC) com diferencial técnico
- **Pós-graduação** em áreas quantitativas e interdisciplinares
- **Freelancing** em projetos de análise de dados avançada
- **Especialização** em segurança financeira e detecção de fraudes

## 🤝 Agradecimentos

### 🌍 **À Comunidade Open Source:**
- **Google OR-Tools** pela ferramenta excepcional de otimização
- **CVXPY Team** pela biblioteca elegante de otimização convexa
- **Jupyter Project** pelo ambiente interativo incomparável
- **Scikit-learn** pelo ecossistema de machine learning
- **Python Community** pelo ecossistema científico robusto

## 📄 Licença e Uso

Este repositório está sob licença **MIT**, garantindo:

### ✅ **Você PODE:**
- ✅ Usar comercialmente
- ✅ Modificar livremente
- ✅ Distribuir cópias
- ✅ Usar em trabalhos privados
- ✅ Sublicenciar

### ⚠️ **Você DEVE:**
- 📄 Incluir a licença original
- 📝 Incluir avisos de copyright
- 🎓 Dar crédito ao autor original (especialmente em contexto acadêmico)

### ❌ **Não há garantias:**
- ❌ Não há garantia de funcionamento
- ❌ Responsabilidade limitada pelo uso

## 🎊 Conclusão

Este repositório é mais que uma **simples coleção de códigos** - é um **ecossistema educacional** vivo e em constante evolução!

### 🎯 **Nossa Missão:**
Democratizar o acesso ao conhecimento de **otimização matemática** aplicada, criando uma ponte entre **teoria acadêmica** e **problemas reais** da indústria e pesquisa.

### 🚀 **Nosso Compromisso:**
- **Qualidade:** Conteúdo sempre atualizado e testado
- **Acessibilidade:** Explicações claras para todos os níveis
- **Relevância:** Problemas atuais e aplicáveis
- **Comunidade:** Espaço colaborativo e inclusivo
- **Inovação:** Técnicas de ponta explicadas didaticamente

### 🌟 **Diferenciais Únicos:**
- **Progressão natural:** De conceitos básicos a técnicas avançadas
- **Problemas reais:** Casos de uso autênticos da indústria
- **Código comentado:** Cada linha explicada pedagogicamente
- **Visualizações ricas:** Gráficos que facilitam o entendimento
- **Aplicabilidade imediata:** Conhecimento utilizável desde o primeiro dia
- **Sistemas adaptativos:** Técnicas que evoluem com os dados

---

## 📞 Contato e Suporte

### 👨‍🏫 **Prof. Maurizio Prizzi**

**🎓 Contato Acadêmico (CEUB):**
- 📧 **Email Institucional:** [maurizio.prizzi@ceub.edu.br](mailto:maurizio.prizzi@ceub.edu.br)
- 🏢 **Assuntos:** Notas, presenças, conteúdo oficial da disciplina

**🔬 Contato Técnico (Pessoal):**
- 📧 **Email:** [maurizioprizzi@gmail.com](mailto:maurizioprizzi@gmail.com)
- 💼 **LinkedIn:** [linkedin.com/in/maurizioprizzi](https://www.linkedin.com/in/maurizioprizzi/)
- 🐙 **GitHub:** [github.com/maurizioprizzi](https://github.com/maurizioprizzi)
- 💬 **Assuntos:** Dúvidas técnicas, contribuições, colaborações

---

⭐ **Gostou do repositório? Deixe uma estrela e compartilhe com outros estudantes!**  
🔄 **Contribua** com melhorias, correções ou novos exemplos!  
💬 **Tem dúvidas?** Abra uma issue ou me envie um email!

🎓 **Excelentes estudos e ótimas otimizações para todos!** 🚀✨

---

### 🔥 **NOVIDADES: Confira as últimas aulas!**

#### 👉 [**Aula SCOP + Programação Quadrática Não-Convexa: 2025-06-11**](./2025_06_11/)
**O que você vai aprender:**
- 🎯 Seleção automática de características para diagnóstico médico
- 🛍️ Segmentação inteligente de clientes com eliminação de ruído  
- 🔬 Técnicas não-convexas que vão além dos métodos tradicionais
- 💡 Estratégias de duas etapas para problemas complexos

#### 👉 [**NOVA: Otimização Adaptativa para Detecção de Fraudes: 2025-06-18**](./2025_06_18/)
**O que você vai aprender:**
- 🛡️ Sistemas antifraude adaptativos para fintech
- 🎯 Busca ternária para otimização de threshold em O(log₃ n)
- 🔄 Adaptação automática a concept drift (mudanças nos padrões)
- 📊 Quantificação de ROI e impacto financeiro real
- 🚀 Otimização multi-objetivo para balancear detecção e experiência do usuário

**Não perca estas oportunidades de dominar técnicas de otimização de ponta aplicadas a problemas reais!** 🚀