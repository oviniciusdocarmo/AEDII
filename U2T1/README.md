# Comparação de Algoritmos de Caminho Mínimo para Serviços de Emergência

## **📋 Informações Acadêmicas**  
| Campo               | Detalhe                              |
|---------------------|--------------------------------------------------------------|
| **Universidade**    | *Universidade Federal do Rio Grande do Norte - UFRN*         |
| **Departamento**    | *Departamento de Engenharia da Computação e Automação - DCA* |
| **Disciplina**      | *DCA3702 - ALGORITMOS E ESTRUTURAS DE DADOS II*              |
| **Aluno(a)**        | *Vinícius Silva do Carmo*                                    |

---

## **🛠️ Tecnologias Utilizadas**  
- ![Python](https://img.shields.io/badge/Python-3.8%2B-blue)  
- ![NetworkX](https://img.shields.io/badge/NetworkX-2.6%2B-orange)  
- ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-red)  
- ![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5%2B-yellowgreen)  
- ![OSMnx](https://img.shields.io/badge/OSMnx-2.0.3%2B-brightgreen)

---

## **🚀 Como Executar?**  
1. Clone o repositório:  
   ```bash
   git clone https://github.com/oviniciusdocarmo/AEDII
   ```
2. Instale as dependências:  
   ```bash
   pip install -r requirements.txt
   ```
3. Abra os notebooks no Jupyter:  
   ```bash
   jupyter notebook
   ```

---

## Cenário

O presente estudo foi desenvolvido com o objetivo de comparar três algoritmos de caminho mínimo no contexto de deslocamentos de serviços de emergência, como ambulâncias, partindo do Hospital Walfredo Gurgel em Natal/RN para bairros populosos da cidade. A análise leva em consideração não apenas a precisão dos caminhos gerados, mas também a eficiência computacional e o impacto ambiental em termos de consumo de energia e emissões de carbono.

## Algoritmos Comparados

1. **Dijkstra Tradicional**: implementação básica utilizando listas.
2. **Dijkstra com MinHeap**: otimização usando uma fila de prioridade baseada em heap.
3. **Dijkstra via NetworkX (OSMnx)**: utilização de bibliotecas consolidadas de grafos com suporte a dados geográficos.

## Metodologia

- Os algoritmos foram aplicados a uma malha viária extraída via [OSMnx](https://osmnx.readthedocs.io/), considerando pesos baseados na distância (metros).
- O nó de origem foi fixado no Hospital Walfredo Gurgel.
- Os destinos foram definidos com base em bairros específicos.
- O tempo de execução e as emissões de carbono de cada algoritmo foram monitorados com a biblioteca [CodeCarbon](https://mlco2.github.io/codecarbon/).
- Os resultados de distância foram salvos em [distancias_por_algoritmo.csv](emissions/distancias_por_algoritmo.csv) e os dados de consumo energético em [emissions.csv](emissions/emissions.csv).

## Resultados

### Distâncias (em metros) entre o Hospital Walfredo Gurgel e os bairros analisados

| Bairro                  | Dijkstra Tradicional (m) | Dijkstra MinHeap (m) | Dijkstra via OSMnx (m) |
|-------------------------|---------------------------|------------------------|--------------------------|
| Hospital Walfredo Gurgel | 0.0                       | 0.0                    | 0.0                      |
| Felipe Camarão          | 7168.48                   | 7168.48                | 7168.48                  |
| Alecrim                 | 3084.26                   | 3084.26                | 3084.26                  |
| Quintas                 | 4174.86                   | 4174.86                | 4174.86                  |
| Cidade da Esperança     | 5617.46                   | 5617.46                | 5617.46                  |
| Lagoa Nova              | 2328.88                   | 2328.88                | 2328.88                  |
| Via Costeira            | 8940.13                   | 8940.13                | 8940.13                  |
| Ponta Negra             | 12192.17                  | 12192.17               | 12192.17                 |
| Capim Macio             | 6499.30                   | 6499.30                | 6499.30                  |
| Neópolis                | 6872.97                   | 6872.97                | 6872.97                  |

### Emissões de Carbono

| Algoritmo               | Energia Consumida (kWh)  | Tempo de Execussão (s) |
|-------------------------|--------------------------|------------------------|
| Dijkstra Tradicional    | 0.000768                 | 6.8775                 |
| Dijkstra com MinHeap    | 0.000009                 | 0.0840                 |
| Dijkstra via OSMnx      | 0.000005                 | 0.0455                 |

### Observações

- O algoritmo **tradicional** foi significativamente menos eficiente em termos de consumo energético, mesmo que os resultados de distância fossem os mesmos.
- O **MinHeap** e o **OSMnx** foram mais eficientes energeticamente, com desempenho similar entre si.
- O OSMnx tem a vantagem adicional de abstrair a malha urbana real, o que pode ser útil em implementações práticas para sistemas de emergência urbanos.

## Conclusões

- **Eficiência Computacional**: Algoritmos otimizados com estruturas de dados apropriadas (como MinHeap) são muito mais eficientes.
- **Sustentabilidade**: Reduzir o consumo computacional tem impacto direto na emissão de carbono, especialmente em execuções em larga escala ou tempo real.
- **Aplicabilidade**: Para aplicações práticas com dados reais (ex. sistemas de despacho de ambulância), o uso de bibliotecas como OSMnx é altamente recomendado.

## Próximos Passos

- Considerar pesos baseados em tempo (e não apenas distância).
- Incorporar dados em tempo real de trânsito.
- Avaliar impacto da escala (número de origens e destinos) no consumo.


---
📹 **Link para o vídeo de apresentação**: [Vídeo](https://youtu.be/V2bBloL8LUY)

