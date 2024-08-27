Validador de CPF em JavaScript

Este repositório contém uma implementação de um validador de CPF em JavaScript.

Funcionamento

A classe validarCpf é responsável por realizar a validação do CPF. Ela remove qualquer caractere não numérico do CPF enviado, calcula os dígitos verificadores, e compara com o CPF original para verificar sua validade.

Documentação do Código ->

Função Construtora: validarCpf(cpfEnviado)

Parâmetro: cpfEnviado - O CPF que será validado.
Descrição: A função construtora define uma propriedade cpfLimpo, que remove todos os caracteres não numéricos do CPF enviado.

Método: valida()

Descrição: Este método valida o CPF com base em três verificações principais:
Verifica se cpfLimpo foi definido corretamente.
Checa se o comprimento do cpfLimpo é igual a 11.
Verifica se o CPF não é uma sequência de números repetidos.
Retorno: true se o CPF for válido, false caso contrário.

Método: criaDigito(cpfParcial)

Parâmetro: cpfParcial - Parte inicial do CPF, sem os dois últimos dígitos verificadores.
Descrição: Este método calcula os dígitos verificadores do CPF usando um algoritmo de multiplicação e soma.
Retorno: O dígito verificador calculado.

Método: sequencia()

Descrição: Este método verifica se o CPF é uma sequência de números repetidos, como 111.111.111-11.
Retorno: true se o CPF for uma sequência, false caso contrário.