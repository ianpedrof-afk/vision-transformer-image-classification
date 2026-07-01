# Classificação de Imagens com Vision Transformer (ViT)

## 📖 Sobre o projeto

Este projeto foi desenvolvido como parte de um trabalho acadêmico da disciplina de Inteligência Artificial/Visão Computacional, com o objetivo de comparar o desempenho de duas arquiteturas da família **Vision Transformer (ViT)**:

- ViT-Base (`google/vit-base-patch16-224`)
- ViT-Large (`google/vit-large-patch16-224`)

Ambos os modelos foram utilizados para realizar a classificação de imagens contendo diferentes espécies de animais, permitindo comparar a precisão das classificações, a probabilidade das predições e o tempo de inferência de cada arquitetura.

---

## 🎯 Objetivos

- Implementar modelos Vision Transformer utilizando a biblioteca Hugging Face Transformers.
- Classificar imagens de animais utilizando modelos pré-treinados.
- Comparar os resultados obtidos entre as versões ViT-Base e ViT-Large.
- Avaliar o tempo de processamento e o nível de confiança das classificações.

---

## 🛠 Tecnologias utilizadas

- Python 3
- Google Colab
- PyTorch
- Hugging Face Transformers
- Pillow (PIL)
- Requests

---

## 📂 Estrutura do projeto

```
vision-transformer-image-classification/

├── Classificacao_Imagens_ViT.ipynb
├── README.md
├── requirements.txt
└── relatorio/
    └── Relatorio.pdf
```

---

## 📥 Instalação

Instale as dependências executando:

```bash
pip install -r requirements.txt
```

Ou diretamente no Google Colab:

```python
!pip install transformers torchvision pillow
```

---

## ▶️ Como executar

1. Abra o notebook `Classificacao_Imagens_ViT.ipynb` no Google Colab.
2. Execute todas as células.
3. O notebook irá:
   - Baixar a imagem utilizada no teste;
   - Carregar o modelo Vision Transformer;
   - Realizar a classificação da imagem;
   - Exibir a classe prevista;
   - Mostrar as 10 classes com maior probabilidade;
   - Informar o tempo de inferência.

---

## 📊 Resultados

Os testes foram realizados utilizando as versões **ViT-Base** e **ViT-Large** sobre o mesmo conjunto de imagens.

Durante a comparação foram analisados:

- Classe predita;
- Probabilidade da classificação;
- Tempo de inferência.

Os resultados mostraram que ambos os modelos apresentaram elevado desempenho na classificação da maioria das imagens. Entretanto, observou-se um erro comum na imagem da capivara, que foi classificada como "beaver" (castor), evidenciando uma limitação dos modelos pré-treinados.

Além disso, verificou-se que o modelo **ViT-Base** apresentou tempos de inferência significativamente menores, enquanto o **ViT-Large** apresentou maior confiança em algumas classificações específicas.

---

## 📚 Referências

- DOSOVITSKIY, A. et al. *An Image Is Worth 16×16 Words: Transformers for Image Recognition at Scale*. ICLR, 2021.
- VASWANI, A. et al. *Attention Is All You Need*. NeurIPS, 2017.
- GOODFELLOW, I.; BENGIO, Y.; COURVILLE, A. *Deep Learning*. MIT Press, 2016.
- DENG, J. et al. *ImageNet: A Large-Scale Hierarchical Image Database*. CVPR, 2009.

---

## 👨‍💻 Autor

**Ian Pedro Ferreira de Paula**

Graduando em Engenharia da Computação – Universidade Veiga de Almeida (UVA)

---

## 📄 Licença

Este projeto foi desenvolvido exclusivamente para fins acadêmicos.
