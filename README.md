README 


Sistema Bancário em Python


Visão Geral
Este script em Python implementa um sistema bancário básico que permite aos usuários criar contas, fazer depósitos, saques e visualizar extratos bancários. O sistema suporta múltiplos usuários e contas, rastreando as transações de cada conta.

Funcionalidades

Criar Contas de Usuários: Usuários podem ser criados com detalhes pessoais, como nome, CPF, data de nascimento e endereço.

Criar Contas Bancárias: Usuários podem abrir novas contas correntes associadas a uma agência e número de conta.

Depósitos e Saques: Os usuários podem depositar fundos ou sacar dinheiro de suas contas, sujeitos a certos limites.

Histórico de Transações: O sistema mantém um registro de cada transação (depósito ou saque) para cada conta e exibe o extrato quando solicitado.

Gerenciamento de Contas: Os usuários podem visualizar os detalhes de sua conta e o histórico de transações (ou seja, o extrato).

CLASSES

Cliente: Representa um cliente com endereço e uma lista de contas bancárias. Esta classe gerencia transações e a criação de contas para o cliente.

realizar_transacao(): Executa uma transação (depósito ou saque).
adicionar_conta(): Adiciona uma conta à lista de contas do cliente.
PessoaFisica (Cliente): Representa um cliente individual, herdando de Cliente com detalhes pessoais adicionais (nome, data de nascimento e CPF).

Conta: Representa uma conta bancária com atributos como saldo, número da conta, agência e cliente.

sacar(): Realiza saques da conta.
depositar(): Realiza depósitos na conta.
ContaCorrente (Conta): Uma conta corrente com recursos adicionais, como limites de saque e um limite no número de saques.

Historico: Gerencia o histórico de transações de cada conta, armazenando todos os depósitos e saques realizados.

Transacao (Abstrata): Uma classe abstrata para transações (tanto depósito quanto saque) com os métodos valor e registrar().

Saque (Transacao): Implementa a transação de saque.
Deposito (Transacao): Implementa a transação de depósito.

FUNÇÕES

menu(): Exibe o menu principal e permite que o usuário escolha diferentes operações (depositar, sacar, visualizar extrato, criar novo usuário, criar nova conta, listar contas ou sair).

filtrar_cliente(): Busca um cliente pelo CPF na lista de clientes.

recuperar_conta_cliente(): Recupera a conta do cliente, se ele possuir uma.

depositar(): Permite que um usuário deposite dinheiro em uma conta.

sacar(): Permite que um usuário saque dinheiro de uma conta.

exibir_extrato(): Exibe o extrato da conta, mostrando o histórico de transações e o saldo atual.

criar_cliente(): Cria um novo cliente coletando seus dados pessoais.

criar_conta(): Cria uma nova conta corrente para um cliente.

listar_contas(): Lista todas as contas bancárias no sistema.

Fluxo de Execução
Menu Principal: O usuário é solicitado a escolher opções para depositar, sacar, visualizar extratos, criar novos clientes, abrir novas contas ou sair do programa.

O sistema gerencia múltiplos clientes e contas e garante que apenas transações válidas sejam processadas.

Limites de saque e o número máximo de saques por dia são aplicados para contas correntes.
Uso
Execute o script e siga as instruções no menu para realizar as diversas operações bancárias.

Exemplo

1-Criar um novo usuário.

2-Abrir uma nova conta bancária para o usuário.

3-Depositar dinheiro na conta.

4-Sacar dinheiro.

5-Visualizar o extrato da conta, mostrando o histórico de transações e o saldo atual.





