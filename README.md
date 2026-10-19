# 🖥️ Modelagem Computacional - Segmentação com SAM

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)

Repositório dedicado aos projetos e implementações da disciplina de Modelagem Computacional (Bacharelado em Ciência da Computação / BCT da UNIFESP). O foco principal deste repositório é a aplicação de modelos fundacionais de Visão Computacional para deteção e segmentação precisa de imagens.

## 🎯 Objetivos do Projeto

O caso de estudo central envolve a **segmentação de plumas de fumo e fogo** em imagens utilizando o **Segment Anything Model (SAM)** da Meta. O pipeline desenvolvido permite isolar o elemento de interesse do fundo com alta precisão, viabilizando a análise quantitativa da área de dispersão.

## ✨ Funcionalidades Implementadas

* **Inicialização e Inferência SAM:** Configuração do `SamPredictor` (checkpoint ViT-B) com otimização automática de hardware (CUDA/GPU).
* **Prompts de Bounding Box:** Geração de máscaras de segmentação precisas guiadas por caixas delimitadoras (*bounding boxes*).
* **Análise Quantitativa:** Cálculo e extração da área percentual ocupada pela máscara gerada em relação à dimensão total da imagem.
* **Visualização Analítica Tripla:** Geração de saídas visuais comparativas contendo a imagem original (com a bounding box), a máscara binária isolada, e a máscara colorida sobreposta à imagem original.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Ambiente de Desenvolvimento:** Jupyter Notebook / Google Colab
* **Bibliotecas Principais:**
  * `segment-anything` (Meta)
  * `torch` e `torchvision` (Processamento e inferência)
  * `opencv-python` (Manipulação e leitura de imagens)
  * `matplotlib` (Geração de resultados visuais)

## 🚀 Como Executar

1. Clone este repositório para o seu ambiente local:
```bash
git clone [https://github.com/seu-usuario/modelagem-computacional.git](https://github.com/seu-usuario/modelagem-computacional.git)
cd modelagem-computacional
