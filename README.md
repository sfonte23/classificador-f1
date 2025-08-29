# Classificador de Imagens de Fórmula 1 🏎️

Este projeto implementa um **classificador de imagens** utilizando **Visão Computacional e Aprendizado de Máquina**, com o objetivo de identificar **equipes e pilotos de Fórmula 1** a partir de imagens.  

O notebook `classificador_imagens_f1_v1_0_0.ipynb` contém todas as etapas necessárias para **pré-processamento, treinamento, avaliação e organização das imagens classificadas**.

## 📂 Estrutura
- `classificador_imagens_f1_v1_0_0.ipynb` → Notebook principal com todo o pipeline de classificação de imagens.  
- Diretório de imagens → Organizado em pastas por equipe e separado em **Train** e **Val**.  

```text
dataset/
├── Train/
│   ├── Mercedes/
│   ├── Ferrari/
│   ├── RedBull/
│   └── ...
├── Val/
│   ├── Mercedes/
│   ├── Ferrari/
│   ├── RedBull/
│   └── ...

```

## 🧑‍💻 Metodologia

O notebook segue as seguintes etapas:

1. **Carregamento do Dataset** – imagens organizadas por equipe.  
2. **Pré-processamento** – redimensionamento, normalização e augmentação.  
3. **Divisão de Dados** – separação em treino e validação.  
4. **Construção do Modelo** – utilizando redes neurais convolucionais (CNN) ou transfer learning.  
5. **Treinamento** – ajuste dos pesos da rede.  
6. **Avaliação** – métricas como acurácia, matriz de confusão e relatórios de classificação.  
7. **Classificação Final** – organização automática das novas imagens nas pastas correspondentes à equipe/piloto.  


## ⚙️ Requisitos

Para executar o notebook, é necessário ter instalado:

- Python 3.8+  
- [Jupyter Notebook](https://jupyter.org/) ou [Google Colab](https://colab.research.google.com/)  
- Bibliotecas principais:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow keras opencv-python
````


## ▶️ Como Executar

1. Clone este repositório ou faça o download dos arquivos.
2. Certifique-se de ter o dataset organizado na estrutura indicada.
3. Instale os requisitos listados acima.
4. Abra o notebook:

   ```bash
   jupyter notebook classificador_imagens_f1_v1_0_0.ipynb
   ```

   ou, se preferir, execute no **Google Colab**.
5. Execute as células na ordem para treinar e validar o modelo.

## 📊 Resultados e Avaliação

O modelo é avaliado por meio de:

* **Acurácia no conjunto de validação**
* **Matriz de Confusão** para verificar erros entre equipes/pilotos
* **Relatório de Classificação (Precision, Recall, F1-Score)**
* **Curvas de perda e acurácia durante o treinamento**

## 🚀 Próximos Passos

* Ampliar o dataset com mais imagens por piloto.
* Ajustar hiperparâmetros para melhorar a performance.
* Testar arquiteturas de redes mais avançadas (ResNet, EfficientNet, MobileNet).
* Implementar uma interface para classificação em tempo real.

## 📚 Referências

* [TensorFlow Documentation](https://www.tensorflow.org/)
* [Keras Documentation](https://keras.io/)
* Bishop, C. M. *Pattern Recognition and Machine Learning*.
* Goodfellow, I.; Bengio, Y.; Courville, A. *Deep Learning*.

