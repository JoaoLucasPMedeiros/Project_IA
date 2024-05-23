# Técnicas 

## Normalização e Padronização

Objetivo: Ajustar os valores de pixel das imagens para um intervalo comum (geralmente [0, 1] ou [-1, 1]) para facilitar a aprendizagem do modelo.

Aplicação:

Normalizar os valores dos pixels dividindo pelo valor máximo (por exemplo, 255 para imagens de 8 bits).

Padronizar subtraindo a média e dividindo pelo desvio padrão dos valores dos pixels.

## Redimensionamento

Objetivo: Ajustar as dimensões das imagens para um tamanho uniforme que é suportado pelo modelo.

Aplicação:

Redimensionar todas as imagens para uma resolução específica (ex.: 224x224 pixels).

## Ajuste de Contraste e Brilho

Objetivo: Melhorar a qualidade visual das imagens, facilitando a detecção de características importantes.

Aplicação:
Utilizar técnicas como equalização de histograma para ajustar o contraste.

Ajustar o brilho conforme necessário.

## Remoção de Ruído

Objetivo: Eliminar ruídos que podem interferir na análise da imagem.

Aplicação:

Aplicar filtros de suavização como Gaussian Blur para reduzir o ruído.

## Segmentação

Objetivo: Identificar e isolar regiões de interesse nas imagens.

Aplicação:

Utilizar algoritmos de segmentação (ex.: Watershed, Segmentação por Limiar) para isolar áreas específicas como tumores ou órgãos.

## Augmentação de Dados

Objetivo: Aumentar a diversidade do conjunto de dados de treinamento e reduzir o overfitting.

Aplicação:

Aplicar técnicas como rotação, translação, espelhamento, zoom e adição de ruído.

Garantir que a augmentação mantenha a relevância médica da imagem.

## Anotação de Dados

Objetivo: Marcar regiões de interesse e fornecer rótulos para treinamento supervisionado.

Aplicação:

Utilizar ferramentas de anotação para marcar manualmente regiões ou utilizar anotações já fornecidas nos datasets.

## Divisão do Dataset

Objetivo: Dividir os dados em conjuntos de treinamento, validação e teste.

Aplicação:

Realizar uma divisão estratificada para garantir a representatividade de classes em todas as divisões (ex.: 70% treino, 15% validação, 15% teste).

## Correção de Artefatos

Objetivo: Remover ou minimizar artefatos de imagem que possam distorcer a análise.

Aplicação:

Aplicar técnicas de correção de artefatos específicos da modalidade de imagem (ex.: correção de movimento em ressonância magnética).

## Transformação de Dados

Objetivo: Aplicar transformações específicas necessárias para o modelo.

Aplicação:

Aplicar transformações como PCA (Principal Component Analysis) se necessário para redução de dimensionalidade.

Converter imagens para o formato de tensor se estiver utilizando frameworks de deep learning (ex.: PyTorch, TensorFlow).
