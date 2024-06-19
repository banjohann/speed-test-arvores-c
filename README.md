O objetivo deste trabalho consiste em analisar a complexidade algorítmica das operações de adição e remoção de nós (considerando o balanceamento) em árvores AVL, rubro-negra e B. No caso da árvore B, devem ser consideradas o parâmetro de ordem da árvore igual a 1, 5 e 10. A análise deve ser realizada considerando a geração de um conjunto de dados (chaves) com tamanho variando entre 1 e 10000. As chaves devem ser geradas reproduzindo um caso médio, isto é, utilizando chaves aleatórias. Para geração das chaves aleatórias, sugere-se o uso da função rand em C considerando uma quantidade de amostra de pelo menos 10 conjuntos para validade estatística, calculando a média dos resultados obtidos.

O resultado final do experimento deve ser apresentado em um relatório contendo dois gráficos de linha (um para a operação de adição e outro para a operação de remoção), onde o eixo X representa o tamanho dos conjuntos de dados (1 a 10000) e o eixo Y representa o esforço computacional das operações considerando eventuais balanceamentos. Cada gráfico deve apresentar 5 linhas, as quais representam as respectivas operações para cada estrutura de dados avaliada (árvore AVL, rubro-negra e as três variações da árvore B). O relatório também deve conter uma discussão final sobre os resultados obtidos. Além do relatório, os códigos-fonte utilizados nos experimentos devem ser entregues também.

## Dependências:
- Docker
- Makefile

## Para rodar:
Execute os scripts:
- make build
&&
- make run

## Thought Process:
- Usamos o Docker para isolar ao máximo variáveis de Sistema Operacional, com o Docker ainda podemos limitar a quantidade de CPUs em 1 e a memória ram em 500mb
- Decidimos que para um teste mais justo com as versões da árvore, todos as árvores vão rodar com o mesmo dataset para cada iteração

## Dúvidas:
- Qual a melhor forma de medir esforço computacional? (tempo, ram)
- Qual a melhor forma do python gerar os dados e o C ler? (arquivo? várias entradas?)