# Projeto de Visão Computacional – Comparação de Modelos

## Resumo Executivo

Este projeto tem como objetivo avaliar e comparar diferentes abordagens de visão computacional aplicadas à identificação de objetos (*mouse* e *apontador*), utilizando um dataset reduzido.

Foram analisados três modelos distintos:

- YOLO customizado (com fine-tuning)  
- YOLO pré-treinado (sem adaptação)  
- CNN treinada do zero  

A proposta central foi entender como cada abordagem se comporta em termos de precisão, capacidade de generalização e dependência de dados.

---

## Principais Resultados

- O **YOLO customizado** apresentou o melhor desempenho, com alta precisão e excelente capacidade de generalização, mesmo com poucas imagens.

- O **YOLO pré-treinado**, sem ajuste, não conseguiu reconhecer corretamente os objetos, evidenciando a limitação de modelos genéricos em problemas específicos.

- A **CNN treinada do zero** apresentou bons resultados no treino e validação, porém falhou no teste, com acurácia de 50%, indicando overfitting e baixa capacidade de generalização.

---

## Principais Insights

- O **tamanho reduzido do dataset** impacta diretamente o desempenho dos modelos, especialmente aqueles treinados do zero.

- Resultados de validação podem ser **enganosos em datasets pequenos**, não refletindo a performance real.

- A **transferência de aprendizado** se mostrou essencial para alcançar bons resultados em cenários com limitação de dados.

---

##  Conclusão

A abordagem baseada em YOLO customizado se destacou como a mais eficiente para o problema proposto, combinando precisão, robustez e capacidade de generalização.

Modelos sem adaptação ou treinados do zero apresentaram limitações significativas, reforçando a importância do uso de técnicas modernas como transfer learning em aplicações reais.

---

## Estrutura do Projeto

- `Fase_06_Rede_Neural.ipynb`: treinamento do YOLO customizado  
- Notebook atual: YOLO pré-treinado, CNN e análise comparativa  

---

## Execução

1. Abrir o notebook no Google Colab  
2. Conectar ao Google Drive  
3. Ajustar os caminhos do dataset  
4. Executar as células sequencialmente  
