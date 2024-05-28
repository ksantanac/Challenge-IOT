# Sistema de Recomendação de Produtos Eletrônicos

Este projeto implementa um sistema de recomendação de produtos eletrônicos utilizando aprendizado de máquina, bibliotecas de ciência de dados e uma interface gráfica simples. O objetivo é recomendar produtos similares com base nas características de um produto comprado.

## Arquitetura do Projeto

1. **Criação da Base de Dados**: Uma base de dados fictícia contendo informações sobre produtos eletrônicos, suas categorias, marcas, preços e avaliações.
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

1. **Criação da Base de Dados**
2. **Normalização dos Dados**
3. **Função de Recomendação**
4. **Interface Gráfica**

## Frameworks, Bibliotecas e Ferramentas Utilizadas

- **Scikit-learn**: Utilizamos a biblioteca Scikit-learn para implementar o algoritmo KNN (K-Nearest Neighbors) para realizar a tarefa de recomendação de produtos.
- **Pandas e NumPy**: Utilizamos as bibliotecas Pandas e NumPy para o pré-processamento de dados, incluindo a normalização de variáveis e codificação de variáveis categóricas.
- **Tkinter**: Implementamos uma interface gráfica simples utilizando a biblioteca Tkinter para facilitar a interação dos usuários com o sistema de recomendação.

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
