# Sistema de Recomendação de Produtos Eletrônicos

Este projeto implementa um sistema de recomendação de produtos eletrônicos utilizando aprendizado de máquina, bibliotecas de ciência de dados e uma interface gráfica simples. O objetivo é recomendar produtos similares com base nas características de um produto comprado.

## Arquitetura do Projeto

1. **Importação da Base de Dados**: Uma base de dados em excel importada com pandas.
2. **Normalização dos Dados**: Utilização das bibliotecas Pandas e NumPy para normalizar os dados e prepará-los para o modelo de recomendação.
3. **Função de Recomendação**: Implementação do algoritmo KNN (K-Nearest Neighbors) utilizando a biblioteca Scikit-learn para encontrar produtos similares.
4. **Interface Gráfica**: Desenvolvimento de uma interface gráfica utilizando Tkinter para facilitar a interação do usuário com o sistema.

## Pré-requisitos e Instalação

### Bibliotecas Necessárias

Certifique-se de ter as seguintes bibliotecas instaladas no seu ambiente Python:

- `pandas`
- `numpy`
- `scikit-learn`
- `tkinter` (incluída na biblioteca padrão do Python)

Você pode instalar as bibliotecas necessárias utilizando o `pip`:

```bash
pip install pandas numpy scikit-learn
```
## Estrutura do Código

O código consiste nas seguintes partes principais:

1. **Importação da Base de Dados**
2. **Normalização dos Dados**
3. **Função de Recomendação**
4. **Interface Gráfica**

## Frameworks, Bibliotecas e Ferramentas Utilizadas

- **Scikit-learn**: Utilizamos a biblioteca Scikit-learn para implementar o algoritmo KNN (K-Nearest Neighbors) para realizar a tarefa de recomendação de produtos.
- **Pandas e NumPy**: Utilizamos as bibliotecas Pandas e NumPy para o pré-processamento de dados, incluindo a normalização de variáveis e codificação de variáveis categóricas.
- **Tkinter**: Implementamos uma interface gráfica simples utilizando a biblioteca Tkinter para facilitar a interação dos usuários com o sistema de recomendação.

## Arquitetura IA Utilizada
A arquitetura de IA usada neste código é baseada no algoritmo de K-Nearest Neighbors (KNN), que é um método de aprendizado supervisionado para encontrar itens similares com base em suas características. O KNN é aplicado para analisar múltiplas características de cada produto e recomendar os produtos mais parecidos com o produto escolhido.

- **Por que foi escolhido?** O KNN é um algoritmo simples e eficaz para problemas de recomendação. Ele funciona bem em contextos onde os produtos podem ser descritos por atributos numéricos ou categóricos, como no caso dos produtos eletrônicos. O algoritmo é não paramétrico, o que significa que não faz suposições sobre a distribuição dos dados, sendo flexível e fácil de implementar.

## Como foi implementado

### Preparação de dados
 - Os atributos numéricos como preço e avaliação são normalizados para que tenham a mesma escala. A normalização garante que essas características tenham a mesma influência no modelo.
 - O atributo categórico da categoria dos produtos é codificado usando One-Hot Encoding, convertendo as categorias em vetores binários.

### Construção do vetor de características
 - Após a codificação das categorias e a normalização dos atributos numéricos, é criado um vetor de características para cada produto, contendo informações sobre sua categoria, preço e avaliação.
 - A categoria do produto selecionado tem seu peso duplicado (peso 2) para enfatizar a importância de recomendar produtos da mesma categoria ou categorias relacionadas.

### Treinamento do modelo KNN
 - O algoritmo K-Nearest Neighbors é treinado com os vetores de características dos produtos usando a distância Manhattan, que mede a similaridade entre os produtos. A escolha da distância de Manhattan é apropriada quando se deseja medir diferenças absolutas entre múltiplas características.
 - O parâmetro n_neighbors foi definido como 4, o que significa que o KNN irá buscar até três produtos similares ao produto selecionado, além de considerar o próprio produto

### Recomendação de produtos:
 - Ao receber um produto como entrada, o modelo KNN encontra os produtos mais próximos no espaço de características, retornando uma lista dos produtos mais similares, excluindo o próprio produto.
 - A recomendação é baseada nas características ponderadas, garantindo que a categoria tenha mais peso, mas também levando em consideração o preço e a avaliação dos produtos.


## Conceitos de Machine Learning / IA Utilizados

- **Aprendizado Supervisionado**: Utilizamos o algoritmo KNN, um método de aprendizado supervisionado, para recomendar produtos com base nas características dos produtos.
- **Pré-processamento de Dados**: Aplicamos técnicas de pré-processamento de dados, como normalização de variáveis e codificação de variáveis categóricas, para preparar os dados antes do treinamento do modelo.
- **Implementação da IA em uma Interface Gráfica**: A IA treinada com o algoritmo KNN é integrada em uma interface gráfica, permitindo que o sistema de recomendação seja acessado e utilizado de forma interativa pelos usuários.

## Como Executar o Projeto

1. Certifique-se de ter todas as bibliotecas necessárias instaladas.
2. Clone o código (.ipynb).
3. Execute o arquivo Python para iniciar a interface gráfica.
4. Insira o nome de um produto no campo "Produto Comprado" e clique no botão "Recomendar" para ver os produtos recomendados.

Espero que este guia tenha sido útil! Se você tiver alguma dúvida ou precisar de mais assistência, sinta-se à vontade para perguntar.
