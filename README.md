===============================================================================

Alunos: Guilherme de Oliveira Aredes - 2025.1.08.026
        Pedro Ferreira Prado - 2025.1.08.028
Projeto: Sistema de Manipulação de Imagens PGM

Objetivo: Adquirir conhecimentos de manipulação de matrizes (imagens) com
ponteiros, implementando funcionalidades que geram novas matrizes
(imagens) a partir de valores carregados de arquivos-texto em
formato PGM de representação de imagens.

Descrição do projeto:
Este aplicativo foi desenvolvido para manipular imagens em formato PGM
(Portable Graymap). Ele permite ao usuário carregar uma imagem de entrada,
realizar diversas operações sobre ela e salvar o resultado de cada
operação em um novo arquivo PGM. O programa gerencia a imagem como uma
matriz de pixels, utilizando ponteiros para manipulação eficiente dos dados.
===============================================================================
Formato do arquivo de Imagem PGM (Portable Graymap):

O programa espera arquivos de imagem no formato PGM (P2), seguindo a
estrutura abaixo:

1ª linha: string "P2" (identificador do formato).
2ª linha: quantidade de colunas (largura) em inteiro, seguida de um espaço,
          e seguida de quantidade de linhas (altura) em inteiro.
3ª linha: o valor máximo de tons de cinza em inteiros (ex: 255).
Da 4ª linha em diante: valores inteiros de todos os pixels da imagem,
                       variando entre zero e o valor máximo de tons de
                       cinza da 3ª linha, separados por espaços.

Observação: O programa ignorará todas as linhas que começam com '#'.

===============================================================================
Requisitos e Funcionalidades:

O aplicativo deverá:
- Ler uma imagem de entrada criada pelos autores em formato PGM.
- Apresentar um menu de operações que serão realizadas sobre a imagem
  de entrada indicada.
- Cada operação deve ser implementada em uma função C/C++ separada.
- Os comandos `cin` e `cout` (entrada e saída padrão) só podem ser
  utilizados na função `main`.
- Escrever um arquivo-texto de saída para cada operação realizada,
  mantendo o formato PGM.
- Para todas as operações, os valores de tons de cinza dos pixels
  resultantes devem estar entre zero e o valor máximo especificado na
  imagem original.
===============================================================================
Operações Implementadas:
1.  **Escurecer ou Clarear Imagem:** Ajusta os tons de cinza da imagem
    por um fator informado pelo usuário.
2.  **Rotacionar Imagem:** Permite rotacionar a imagem para a esquerda,
    para a direita, em torno da linha horizontal e em torno da linha
    vertical.
3.  **Imagem Negativa:** Inverte os tons de cinza da imagem, criando um
    efeito de negativo fotográfico.
4.  **Binarizar Imagem:** Converte a imagem em preto e branco com base
    em um limiar informado pelo usuário. Pixels com valores menores que
    o limiar se tornam zero (preto), e valores maiores se tornam o valor
    máximo (branco).
5.  **Iconizar Imagem:** Reduz a imagem de entrada para uma nova imagem
    de 64 x 64 pixels.
===============================================================================
Instruções de Uso:

- Execute o programa e utilize o menu de opções para selecionar a operação
  desejada.
- A primeira opção do menu será para carregar a imagem de entrada em
  formato PGM.
- Para cada operação realizada, um novo arquivo-texto PGM será gerado
  com o resultado, em um nome diferente do arquivo de entrada.

===============================================================================
