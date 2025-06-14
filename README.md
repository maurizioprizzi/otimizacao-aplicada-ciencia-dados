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

### 🌟 **Aula NOVA: 2025-06-11**

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

#### 🔬 **Conceitos Avançados Introduzidos:**
- **🎯 Otimização Não-Convexa:** Problemas com múltiplos mínimos locais
- **⚡ Relaxação Convexa:** Estratégia de duas etapas para problemas difíceis
- **🧹 Seleção de Características:** Técnicas L0, L1 e quadráticas
- **🔗 Interações Complexas:** Captura de relações não-lineares entre variáveis
- **🎮 Thresholding Inteligente:** Soft e hard thresholding para esparsidade

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

### **Áreas de Aplicação:**
- 🏥 **Medicina:** Diagnóstico inteligente e seleção de biomarcadores
- 🛍️ **Marketing:** Segmentação de clientes e análise comportamental
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
cd 2025_06_11  # Para a aula mais recente

# 4. Instale dependências
pip install -r requirements.txt

# 5. Inicie Jupyter
jupyter notebook

# 6. Execute os notebooks na ordem recomendada!
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
│   ├── 📓 01.ipynb  # Seleção de Características Médicas
│   ├── 📓 02.ipynb     # Clustering Esparso de Clientes
│   ├── 🐍 scop_classificacao_comentado.py  # Código comentado completo
│   ├── 🐍 scop_clustering_comentado.py     # Código comentado completo
│   └── 📖 README.md                    # Detalhes da aula
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
- **Próximas:** Complexidade crescente e aplicações interdisciplinares

## 🌟 Destaques da Nova Aula (2025-06-11)

### 🎯 **Por que SCOP é Revolucionário?**

#### **Problemas Tradicionais:**
- Métodos convencionais tratam **seleção de características** e **otimização do modelo** separadamente
- Características irrelevantes "poluem" os modelos
- Interpretabilidade limitada em modelos complexos

#### **Solução SCOP:**
- **Integração total:** Seleciona características E otimiza simultaneamente
- **Não-convexidade:** Captura relações complexas que métodos lineares perdem
- **Esparsidade inteligente:** Elimina automaticamente variáveis irrelevantes
- **Aplicabilidade universal:** Funciona para classificação E clustering

### 🔬 **Inovações Técnicas Introduzidas:**

#### **1. Regularização Híbrida:**
```
Função Objetivo = Fidelidade + λ₁||w||₁ + λ₂w^T Q w - λ₃||w||₀
                     ↑           ↑          ↑           ↑
                 Precisão   Esparsidade  Interações  Combinatorial
```

#### **2. Estratégia de Duas Etapas:**
- **Etapa 1:** Relaxação convexa (rápida e garantida)
- **Etapa 2:** Refinamento não-convexo (qualidade superior)

#### **3. Thresholding Adaptativo:**
- **Soft-thresholding:** Para regularização suave
- **Hard-thresholding:** Para eliminação definitiva
- **Critérios automáticos:** Sem necessidade de ajuste manual

### 💡 **Aplicações Demonstradas:**

#### **🏥 Medicina: "Menos Exames, Mesma Precisão"**
- **Entrada:** 30 características médicas complexas
- **SCOP:** Identifica automaticamente as 8 mais importantes
- **Resultado:** 95.8% de precisão (vs 96.5% com todas)
- **Impacto:** Diagnósticos mais rápidos e baratos

#### **🛍️ Marketing: "Segmentação Inteligente"**
- **Entrada:** 20 características de clientes (incluindo ruído)
- **SCOP:** Descobre 4 grupos naturais + elimina ruído
- **Resultado:** Clusters mais puros e interpretáveis
- **Impacto:** Campanhas mais efetivas e insights claros

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

### 🧠 **Competências Desenvolvidas**
- **Pensamento analítico** para modelagem de problemas complexos
- **Programação científica** em Python com bibliotecas avançadas
- **Visualização** de dados e comunicação de resultados
- **Otimização não-convexa** (competência rara no mercado)
- **Integração teoria-prática** em problemas multidisciplinares

### 🎯 **Aplicações Imediatas**
- **Estágios** em empresas de tecnologia, consultoria e healthcare
- **Iniciação científica** em projetos de pesquisa aplicada
- **Trabalho de conclusão** de curso (TCC) com diferencial técnico
- **Pós-graduação** em áreas quantitativas e interdisciplinares
- **Freelancing** em projetos de análise de dados avançada

## 🤝 Agradecimentos

### 🎓 **À Comunidade CEUB:**
- **Coordenação** do curso de Modelagem Matemática
- **Colegas professores** pelas discussões interdisciplinares
- **Alunos** pelo feedback constante e contribuições valiosas

### 🌍 **À Comunidade Open Source:**
- **Google OR-Tools** pela ferramenta excepcional de otimização
- **CVXPY Team** pela biblioteca elegante de otimização convexa
- **Jupyter Project** pelo ambiente interativo incomparável
- **Scikit-learn** pelo ecossistema de machine learning
- **Python Community** pelo ecossistema científico robusto

## 📈 Roadmap Futuro

### **Próximas Aulas (Cronograma 2025):**
- 🧬 **2025-06-18: Metaheurísticas Avançadas**
  - Algoritmos genéticos para otimização global
  - Simulated annealing e busca tabu
  - Aplicação em problemas de scheduling complexo

- 🎯 **2025-06-25: Otimização Multi-Objetivo**
  - Fronteira de Pareto e trade-offs
  - NSGA-II e algoritmos evolutivos
  - Aplicação em design de produtos

- 📊 **2025-07-02: Otimização Estocástica**
  - Problemas com incerteza e ruído
  - Programação estocástica
  - Aplicação em finanças e logística

- 🚀 **2025-07-09: Projeto Integrador Final**
  - Problema real de grande escala
  - Integração de todas as técnicas aprendidas
  - Apresentações e avaliação final

### **Melhorias Planejadas:**
- 🎮 **Widgets interativos** para experimentos em tempo real
- 📱 **Interface web** para visualização de resultados
- 🎥 **Vídeos explicativos** dos conceitos principais
- 📚 **Exercícios autograding** para prática individual
- 🤖 **Chatbot educacional** para dúvidas frequentes
- 📊 **Dashboard** de progresso personalizado

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

### 🔥 **NOVIDADE: Já conferiu a aula de SCOP + Programação Quadrática Não-Convexa?**
👉 [**Clique aqui para acessar: 2025-06-11**](./2025_06_11/)

**O que você vai aprender:**
- 🎯 Seleção automática de características para diagnóstico médico
- 🛍️ Segmentação inteligente de clientes com eliminação de ruído  
- 🔬 Técnicas não-convexas que vão além dos métodos tradicionais
- 💡 Estratégias de duas etapas para problemas complexos

**Não perca esta oportunidade de dominar técnicas de otimização de ponta!** 🚀