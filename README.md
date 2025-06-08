# 📊 Otimização Matemática Aplicada à Análise de Dados

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![OR-Tools](https://img.shields.io/badge/OR--Tools-9.8+-green.svg)](https://developers.google.com/optimization)
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

## 📚 Estrutura do Curso

### 📅 **Cronograma de Aulas Disponíveis**

| Data | Tópico | Tecnologias | Status |
|------|--------|-------------|--------|
| [**2025-06-04**](./2025_06_04/) | 🎮 **Programação com Restrições** | OR-Tools, CP-SAT | ✅ Disponível |

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
- 📊 **Pandas/NumPy:** Manipulação e análise de dados
- 📈 **Matplotlib/Seaborn:** Visualização de resultados
- 🧠 **Scikit-learn:** Machine learning e datasets
- 📓 **Jupyter:** Notebooks interativos

### **Áreas de Aplicação:**
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
cd 2025_06_04

# 4. Instale dependências
pip install -r requirements.txt

# 5. Inicie Jupyter
jupyter notebook

# 6. Execute os notebooks na ordem recomendada!
```

### **Estrutura de Pastas:**
```
📦 otimizacao-aplicada-ciencia-dados/
├── 📖 README.md                     # Este arquivo
├── 🙈 .gitignore                   # Controle de versionamento
├── 📅 2025_06_04/                  # Aula: Programação com Restrições
│   ├── 📓 01.ipynb                 # Alocação de Amostras
│   ├── 📓 02.ipynb                 # Agendamento de Tarefas
│   ├── 📚 Documento Científico.pdf # Paper completo
│   ├── 📋 requirements.txt         # Dependências
│   └── 📖 README.md                # Detalhes da aula
├── 📅 2025_06_11/                  # [Em breve] Programação Linear
├── 📅 2025_06_18/                  # [Em breve] Algoritmos Genéticos
└── 📅 ...                          # Outras aulas do semestre
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

### 🧠 **Competências Desenvolvidas**
- **Pensamento analítico** para modelagem de problemas
- **Programação** em Python com foco científico
- **Visualização** de dados e comunicação de resultados
- **Otimização** matemática aplicada

### 🎯 **Aplicações Imediatas**
- **Estágios** em empresas de tecnologia e consultoria
- **Iniciação científica** em projetos de pesquisa
- **Trabalho de conclusão** de curso (TCC)
- **Pós-graduação** em áreas quantitativas

## 🤝 Agradecimentos

### 🎓 **À Comunidade CEUB:**
- **Coordenação** do curso de Modelagem Matemática
- **Colegas professores** pelas discussões interdisciplinares
- **Alunos** pelo feedback constante e contribuições

### 🌍 **À Comunidade Open Source:**
- **Google OR-Tools** pela ferramenta excepcional
- **Jupyter Project** pelo ambiente interativo
- **Python Community** pelo ecossistema científico robusto

## 📈 Roadmap Futuro

### **Próximas Aulas (Confirmar Cronograma):**
- 🔢 **Programação Linear:** Simplex, dualidade, análise de sensibilidade
- 🧬 **Metaheurísticas:** Algoritmos genéticos, simulated annealing
- 🎯 **Otimização Multi-Objetivo:** Pareto, NSGA-II, trade-offs
- 📊 **Otimização Estocástica:** Problemas com incerteza
- 🚀 **Projeto Integrador:** Problema real de grande escala

### **Melhorias Planejadas:**
- 🎮 **Widgets interativos** para experimentos em tempo real
- 📱 **Interface web** para visualização de resultados
- 🎥 **Vídeos explicativos** dos conceitos principais
- 📚 **Exercícios autograding** para prática individual

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