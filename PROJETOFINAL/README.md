# Análise de Estruturas Complexas com Gephi e NetworkX

## **📋 Informações Acadêmicas**  
| Campo               | Detalhe                                                                |
|---------------------|------------------------------------------------------------------------|
| **Universidade**    | *Universidade Federal do Rio Grande do Norte - UFRN*                   |
| **Departamento**    | *Departamento de Engenharia da Computação e Automação - DCA*           |
| **Disciplina**      | *DCA4013 - Grafos e Estruturas Complexas*                              |
| **Aluno**           | *Vinícius Silva do Carmo*                                              |

---

## **🛠️ Tecnologias Utilizadas**
- ![Gephi](https://img.shields.io/badge/Gephi-0.10-blueviolet)
- ![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow)
- ![HTML](https://img.shields.io/badge/HTML-5-orange)
- ![CSS](https://img.shields.io/badge/CSS-3-blue)

---

## **📁 Organização do Projeto**

| Pasta/Arquivo            | Descrição                                                       |
|--------------------------|-----------------------------------------------------------------|
| `imagens/`               | Contém as visualizações geradas no Gephi.                       |
| `network/`               | Rede exportada com Plugin SigmaExporter.                        |
| `final_netwokr.gexf`     | Rede exportada para análise no Gephi.                           |

---

## **📊 Requisitos Atendidos**

### ✅ Requisito 1 – Centralidade e Visualização
- **Tamanho do nó:** proporcional ao grau.
- **Cor do nó:** baseada na **Betweenness Centrality**.
- **Layout:** ForceAtlas2.

### ✅ Requisito 2 – K-Core e K-Shell
- **Visualização com cores por k-core** (azul: k=1, amarelo: k=2, verde: k=3).
- **Tamanho do nó:** proporcional ao grau.

### ✅ Requisito 3 – Comunidades e Métrica Livre
- **Cores dos nós:** por detecção de comunidades (modularity class).
- **Tamanho dos nós:** baseado em grau.
- **Layout:** ForceAtlas2.

