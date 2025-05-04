# JPR 2025 HandsOn IA: Classificação Binária de Radiografias de Tórax

Este projeto foi desenvolvido como parte do HandsOn IA da Jornada Paulista de Radiologia (JPR) 2025, focando na classificação binária de radiografias de tórax utilizando Deep Learning.

## 🎯 Objetivos

- Treinar uma Rede Neural Convolucional (CNN) didática para diferenciar radiografias de tórax Normais vs. com Opacidade
- Avaliar a performance do modelo no conjunto de teste (loss, acurácia, matriz de confusão, curvas ROC/PR, intervalos de confiança)
- Publicar e testar o modelo em produção através de uma interface web interativa (Gradio) para inferência em casos novos

## 🛠️ Requisitos

- Python 3.7+
- TensorFlow ≥ 2.x e Keras
- Bibliotecas principais:
  - numpy
  - scikit-learn
  - matplotlib
  - gradio
  - opencv-python
  - pillow
- Ambiente Colab ou máquina local com GPU (opcional, mas recomendado)

## 📂 Estrutura do Projeto

O projeto está organizado em um notebook Jupyter (`JPR2025_Handson_IA.ipynb`) com as seguintes seções:

1. **Preparação do Ambiente**
   - Instalação de dependências
   - Configuração de paths

2. **Ingestão e Pré-processamento**
   - Download do subset do Kaggle
   - Definição de train/val/test
   - Otimização de pipeline (cache, shuffle, prefetch)

3. **Construção e Treinamento do Modelo**
   - Data augmentation
   - Definição da arquitetura CNN
   - Callbacks
   - Cálculo de pesos de classe
   - Execução do treinamento

4. **Avaliação de Performance**
   - Classification report
   - Matriz de confusão
   - Curvas ROC e Precision-Recall
   - Intervalos de confiança via bootstrap

5. **Deploy e Inferência**
   - Carregamento do modelo salvo
   - Funções de pré-processamento
   - Interface Gradio com exemplos
   - CSS customizado

6. **Testes Interativos**
   - Interface web para upload de novas imagens
   - Predições em tempo real

## 🚀 Como Usar

1. Clone este repositório
2. Abra o notebook `JPR2025_Handson_IA.ipynb` no Google Colab ou em seu ambiente Jupyter local
3. Execute as células sequencialmente, seguindo as instruções em cada seção
4. Ao final, você terá um modelo treinado e uma interface web para testar novas imagens

## 👥 Autores

- **Julio Cesar Nather Junior, MD, MSc** - [LinkedIn](https://www.linkedin.com/in/julio-nather-049618181/)
- **Augusto Sarquis Serpa** - [LinkedIn](https://www.linkedin.com/in/augusto-sarquis-serpa-6aa8a3223/)
- **Eduardo Caminha Nunes** - [LinkedIn](https://www.linkedin.com/in/eduardocaminha/)
- **Eduardo Farina** - [LinkedIn](https://www.linkedin.com/in/eduardomjmfarina/)
- **Felipe Kitamura** - [LinkedIn](https://www.linkedin.com/in/felipekitamura/)

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

## 🔗 Links Úteis

- [Dataset no Kaggle](https://www.kaggle.com/datasets/jnather/jpr-2025-handson-ia)

## 📫 Contato

Para questões e sugestões, por favor abra uma issue no GitHub ou entre em contato com os autores através dos links fornecidos acima. 
