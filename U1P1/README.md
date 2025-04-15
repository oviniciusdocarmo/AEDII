# **📊 Análise Temporal de Redes de Coautoria (PPgEEC - 2010 a 2025)**
*Estudo prático sobre redes complexas, centralidade e evolução colaborativa no programa de pós-graduação em Engenharia Elétrica e Computação (UFRN)*  

---

## **📋 Informações Acadêmicas**
| Campo               | Detalhe                                                      |
|---------------------|--------------------------------------------------------------|
| **Universidade**    | *Universidade Federal do Rio Grande do Norte - UFRN*         |
| **Departamento**    | *Departamento de Engenharia da Computação e Automação - DCA* |
| **Disciplina**      | *DCA3702 - ALGORITMOS E ESTRUTURAS DE DADOS II*              |
| **Aluno(a)**        | *Vinícius Silva do Carmo*                                    |

---

## **🛠️ Tecnologias Utilizadas**
- ![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
- ![NetworkX](https://img.shields.io/badge/NetworkX-2.6+-orange)  
- ![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5+-yellowgreen)  
- ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red)  
- ![Pandas](https://img.shields.io/badge/Pandas-1.3+-lightgrey)  
- ![Numpy](https://img.shields.io/badge/Numpy-1.21+-lightblue)

---

## **📈 O Projeto**

O projeto tem como objetivo aplicar **conceitos de grafos** por meio da biblioteca **NetworkX** em Python. A proposta central é construir e explorar uma **rede de coautoria** utilizando **dados reais do PPgEEC**, promovendo a análise de estruturas, padrões de colaboração e métricas de redes. 

### **Requisitos:**

- **Requisito 1:** Cálculo de métricas (nós, arestas, densidade, componentes) para redes por período.  
- **Requisito 2:** Visualização da rede em 4 períodos com destaque para os top 5 autores por grau, coloração especial para membros permanentes, e largura das arestas proporcional às citações.  
- **Requisito 3:** Criação de um subgrafo baseado em grau ≥ média + desvio padrão; comparação de densidade com a rede geral; visualização da rede ego de um autor central.

---

## **🚀 Como Executar?**
1. Clone o repositório:  
   ```bash
   git clone https://github.com/oviniciusdocarmo/AEDII.git
   ```
2. Instale as dependências:  
   ```bash
   pip install -r requirements.txt
   ```
3. Execute os notebooks com Jupyter:  
   ```bash
   jupyter notebook
   ```

---

## **🔍 Principais Resultados**  
- A rede cresceu significativamente entre os períodos analisados, tanto em número de colaborações quanto em conectividade.  
- Autores como *Marcelo Sampaio de Alencar* e *Luiz Marcos G. Gonçalves* foram centrais ao longo de quase todos os períodos.  
- O subgrafo com autores mais conectados mostrou uma densidade muito maior, revelando um núcleo coeso de colaboração.  
- A rede ego analisada mostrou forte interconectividade e influência do autor no centro.

---

## **🎥 Vídeo Explicativo**
- [Link](https://drive.google.com/file/d/1K6N52NYqHff2ugXrDKCOe0O_3MEJstzH/view?usp=sharing)

---

## **📌 Referências**  

- **Livro Completo**: [Coscia, Michele. The Atlas for the Aspiring Network Scientist](https://www.networkatlas.eu/)  


