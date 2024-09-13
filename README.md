# Backpropagation - Neural Network with Training

Este projeto implementa uma rede neural simples utilizando o algoritmo de **backpropagation** para treinar os pesos. O objetivo é ajustar os pesos da rede neural através de um processo de propagação direta e retropropagação do erro, ajustando os pesos conforme a diferença entre a saída prevista e a saída desejada.

## Funcionalidades

- **Função Sigmoide**: Utiliza a função sigmoide como função de ativação para calcular as saídas dos neurônios.
- **Propagação Direta (Feedforward)**: Os dados de entrada passam pelas camadas da rede neural até a camada de saída, onde são feitas as predições.
- **Backpropagation**: O erro entre a predição e o valor alvo é calculado, e os pesos da rede são atualizados de forma iterativa para reduzir o erro.
- **Atualização dos Pesos**: Os pesos são ajustados a cada iteração do treinamento, utilizando uma taxa de aprendizado e considerando o erro derivado da retropropagação.

## Estrutura do Código

1. **Função `sigmoid`**: Calcula a função de ativação sigmoide, usada para definir a saída dos neurônios.
2. **Inicialização**: Vetores e matrizes são inicializados para armazenar entradas, saídas e pesos, além de armazenar os valores intermediários para o processo de backpropagation.
3. **Treinamento**: O código realiza várias iterações de treinamento (1000 épocas), ajustando os pesos em cada iteração com base no erro calculado pela retropropagação.
4. **Exibição dos Pesos**: Após o treinamento, os pesos finais da rede neural são exibidos.

## Como Usar

1. O código define os vetores de entrada (`E1`, `E2`) e os alvos (`t`), que representam a saída esperada para cada conjunto de entradas.
2. Durante o treinamento, os pesos são ajustados usando o algoritmo de retropropagação e gradiente descendente.
3. Ao final do treinamento, os pesos finais da rede são exibidos, juntamente com a evolução do erro ao longo das iterações.

### Exemplo de Saída

Após 1000 iterações de treinamento, o erro acumulado é exibido, seguido pelos pesos finais da rede:

```bash
1000 0.0023
1.2354 -0.6343 0.4582
-0.8932 1.0257 0.3254
