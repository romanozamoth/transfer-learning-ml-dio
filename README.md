# 🧠 Projeto de Transfer Learning - Gatos vs Cachorros

Este projeto faz parte do desafio proposto no bootcamp de Machine Learning da DIO.  
Aplicamos o conceito de **Transfer Learning** utilizando o modelo pré-treinado **MobileNetV2** para classificar imagens de **gatos** e **cachorros**.

## 📁 Dataset

Utilizamos o dataset público disponível no TensorFlow Datasets:

- [`cats_vs_dogs`](https://www.tensorflow.org/datasets/catalog/cats_vs_dogs)
- Classes: **0 = Gato**, **1 = Cachorro**

## 🧠 Técnica utilizada

Foi usada a técnica de **Transfer Learning** com as seguintes etapas:

- Carregamento do modelo MobileNetV2 com pesos do ImageNet
- Congelamento da base convolucional
- Adição de camadas de pooling e classificação
- Treinamento com imagens redimensionadas para `160x160`

## 🔍 Resultados

O modelo foi treinado por 5 épocas com bom desempenho inicial:

- Acurácia final (exemplo): **~90%** (varia a cada execução)
- Avaliação no conjunto de validação para generalização

## 📈 Visualizações

Trechos do notebook incluem gráficos e predições para exemplificar a performance do modelo.

## 🚀 Execução

O notebook foi desenvolvido no Google Colab.  
Acesse diretamente aqui:

👉 [`Transfer_Learning_Projeto.ipynb`](Transfer_Learning_Projeto.ipynb)

## 🧑‍💻 Tecnologias

- Python
- TensorFlow / Keras
- Google Colab
- TensorFlow Datasets
