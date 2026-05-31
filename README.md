# Controle de Níveis de Água

Este projeto simula o monitoramento de um reservatório de água utilizando Python e a biblioteca Colorama.

## Funcionalidades

* Utiliza uma lista para armazenar os níveis do reservatório.
* Utiliza a biblioteca Colorama para exibir mensagens coloridas no terminal.
* Possui uma função responsável por definir a cor de cada mensagem conforme o nível informado.
* Exibe os cinco níveis do reservatório com suas respectivas cores.
* Restaura o estilo padrão do terminal após a exibição das mensagens.

## Tecnologias Utilizadas

* Python
* Colorama

## Correspondência dos Níveis

| Nível | Situação              | Cor      |
| ----- | --------------------- | -------- |
| 1     | Muito baixo (crítico) | Vermelho |
| 2     | Baixo                 | Amarelo  |
| 3     | Médio                 | Verde    |
| 4     | Alto                  | Ciano    |
| 5     | Muito alto (alerta)   | Azul     |

## Estrutura do Código

A função `definir_cor()` recebe um nível e retorna a cor correspondente.

Os níveis são armazenados em uma lista e exibidos por meio de um laço de repetição, simulando o monitoramento do reservatório.
