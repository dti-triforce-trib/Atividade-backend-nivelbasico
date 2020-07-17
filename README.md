# Atividade back-end nivel básico

Olá ficamos felizes com sua participação em nosso processo seletivo e desde já lhe desejamos uma boa sorte!

### Contexto
Você será responsável por gerenciar as transações entre usuários de um banco. Cada usuário possui um código único (vide dados.txt).
Sua implementação deve ler o arquivo dados.txt localizado no diretorio base deste repositório. Cada dado do arquivo é separado por um conjunto de caracteres especiais "-%p". Neste arquivo temos uma chave única UUID que representa o código único do usuário (1º dado), o saldo em conta do usuário (2º dado), o nome do usuário (3º dado), a data da transação (4º dado) no formato yyyy-MM-DD, o valor a ser transferido (5º dado) e o código único do usuário de destino (6º dado). Cada linha do arquivo representa uma transação.
Você deve implementar um programa que lê o arquivo, processa cada transação linha por linha e retorna no final uma mensagem na tela exibindo cada transação realizada e logo após o saldo final de cada usuário.

### Exemplo:
Suponha o arquivo com as seguintes linhas:

        0e3a864c-c867-11ea-87d0-0242ac130003-%p1500.52-%pMaria de Souza-%p2020-01-01-%p100.00-%p0e3a96be-c867-11ea-87d0-0242ac130003
        0e3a96be-c867-11ea-87d0-0242ac130003-%p1000.10-%pJuca Marcos-%p2020-05-03-%p50.00-%p0e3a864c-c867-11ea-87d0-0242ac130003

O resultado esperado seria um resultado devolvido do tipo:

        Maria de Souza transferiu R$ 100.00 para Juca Marcos no dia 01/01/2020
        Juca Marcos transferiu R$ 50.00 para Maria de Souza no dia 03/05/2020
        Saldos:
        Maria de Souza - R$ 1450.52
        Juca Marcos - R$ 950.10

Supondo que o saldo de Juca Marcos fosse de R$ 40.00 e a transferencia de Maria de Souza fosse R$ 5.00:

        Maria de Souza transferiu R$ 5.00 para Juca Marcos no dia 01/01/2020
        Juca Marcos não pode transferir R$ 50.00 para Maria de Souza no dia 03/01/2020 por possuir saldo insuficiente (R$ 45.00)
        Saldos:
        Maria de Souza - R$ 1495.52
        Juca Marcos - R$ 45.00
        
### Regras
  - Você deve conter um arquivo README com as instruções para executar sua aplicação.
  - Sua aplicação deve seguir os conceitos de Orientação a Objetos
  - O uso do git sera considerado na avaliação.
  - Poderá utilizar qualquer linguagem que aceite Orientação a Objetos.
  - Você terá 3 dias para enviar o link do seu repositório do git contendo seu desenvolvimento para o e-mail que lhe solicitou a atividade.

#BOA SORTE!
