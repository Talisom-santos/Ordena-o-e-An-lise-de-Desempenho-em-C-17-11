OBJETIVO DO PROGRAMA

Está programado

COMPILACAO E EXECUCAO

Um código
Para compilargcc -o analisador_ordenacao nome_do_arquivo.c
Para executar: ./analisador_ordenacao

ESTRUTURAS DE DADOS E METRICAS

Estrutura Métricas:

comparações: Contador de operacoes de comparacao entre elementos.

trocas: Continuação

Macros de Contagem:CONTAR_COMPARACAO(m) e CONTAR_TROCA(m) sao usadas em todo o codigo para incrementar os contadores dentro da estrutura Métricasd

ALGORITMO DE CLASSIFICAÇÃO IMPLEMENTADO

Quick Sort (Esquema de Particionamento de Lomuto):

O algoritmo e implementado de forma recursiva.

Uma funcapartição utiliza o esquema de Lomuto, onde o pivo e sempre o ultimo elemento do sub-vetor.

Uma funçãoordenação_rápida_recursivafestapartição e, em seguida, chama a si mesma para as duas sub-listas criadas.

FUNÇÕES DE UTILIDADE

trocarExecuta

resetar_metricas: COM

imprimir_vetor:

copiar_vetor: Cria uma copia exata de um vetor, garantindo que o algoritmo de ordenacao sempre comece com um estado original do vetor nao modificado.

converter_rgm_para_vetor: Encontrar

LÓGICA PRINCIPAL E REFERÊNCIA

RGM Padrao: O RGM utilizado para os testes e 45472271.

executar_ordenacao_benchmark: Esta funcao gerencia o processo de analise.

Policial

Mrelógio() antes e depois da chamada de ordenacao.

Retornar

exibir_menu: Apresenta as opcoes ao usuario (Ordenar o RGM ou Sair).

exibir_resultados: Apresenta as metricas coletadas (comparacoes, trocas e tempo) em dois formatos: um resumo detalhado e um formato de dados CSV (Comma Separated Values) para facilitar a exportacao.

OPERACOES DE MEMORIA

Um programamalloc para criar o vetor de digitos do RGM e para criar a copia do vetor de teste dentro da funcao de benchmark. A memoria e liberada corretamente com livre apos o uso em ambos os casos.
