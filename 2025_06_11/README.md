# Dentro da pasta 2025_06_11/
cat > README.md << 'EOF'
# 🎯 SCOP + Programação Quadrática Não-Convexa

## 📚 Aula do dia 11 de junho de 2025

### 🏥 Projeto 1: Seleção de Características para Diagnóstico Médico
- **Arquivo:** `scop_classificacao_comentado.py`
- **Dataset:** Câncer de mama (30 → 8 características)
- **Resultado:** 95.8% precisão com modelo 73% mais simples

### 🛍️ Projeto 2: Clustering Esparso para Segmentação de Clientes  
- **Arquivo:** `scop_clustering_comentado.py`
- **Dataset:** 300 clientes com ruído simulado
- **Resultado:** 4 clusters bem definidos + eliminação automática de ruído

## 🚀 Como executar:

```bash
pip install -r requirements.txt
python scop_classificacao_comentado.py
python scop_clustering_comentado.py