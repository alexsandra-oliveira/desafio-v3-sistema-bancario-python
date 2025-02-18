***Desafio Sistema Bancário em Python***

Criar um sistema bancário com as operações: sacar, depositar e visualizar extrato.

Fomos contratados por um grande banco para desenvolver o seu novo sistema. Esse banco deseja modernizar suas operações e para isso escolhe a linguagem Python.
Para a primeira versão do sistema devemos implementar apenas 3 operações: depósito, saque e extrato.

***Operação de Depósito***

Deve ser possível depositar valores positivos parra a minha conta bancária. A v1 do do projeto trabalha apenas com 1 usuário, dessa forma não precisamos nos
preocupar em idetificar qual devem ser armazenados em uma variável e exibidos na operação de extrato.

***Operação de Saque***

O sistema deve permitir realizar 3 saques diários com limite máximo de R$ 500,00 por saque. Caso o usuário não tenha saldo em conta, o sistema deve exibir uma mensagem informando que não será possívelf sacar o dinheiro por falta de saldo. Todos os saques devem ser armazenados em uma variável e exibidos na operação de extrato.

***Operação de Extrato*** 

Essa operação deve listar todos os depósitos e saques realizados na conta. No fim da listagem deve ser exibido o saldo atual da conta.

Os valores devem ser exibidos utilizando o formato R$ xxx.xx, exemplo:
1500.45 = R$ 1500.45.


***Desafio Sistema Bancário em Python versão 2***

***Objetivo Geral***

Separar as funções existentes de saque, depósito e extrato em funções: Cadastrar Usuário(cliente) e cadastrar Conta Bancária.

***O Desafio na Versão 2***

Precisamos deixar nosso código mais modularizado para isso vamos criar funções para as operações existentes: Sacar, Depositar e Visualizar Extrato. Além disso, para a versão 2 do nosso sistema precisamos criar duas novas funções: Criar Usuário(cliente do banco) e criar conta corrente(vincular com o usuário).

***Separação em Funções***

Devemos criar funções para todas as operções do sistema. Para exercitar tudo o que aprendemos neste módulo, cada função vai ter uma regra na passagem de argumentos. O retorno e a forma como ser chamadas, pode ser definida por você de forma que achar melhor.

***saque***

A função saque deve receber os argumentos apenas por nome(keyword only). Sugest de argumentos: saldo, valor, extrato, limite, numero_saques, limite_saques. Sugestão de retorno: saldo e extrato.


***Depósito***

A função depósito deve receber os argumentos apenas por posição (positional only). Sugest de argumentos: saldo, valor, extrato. Sugestão de retorno: saldo e extrato.

***Extrato***

A função extrato deve receber os argumentos por posição e nome(positional only e keyword only). Argumentos posicionais: saldo, argumentos nomeados: extrato.

***Novas Funções***

Precisamos criar duas novas funções: criar usuário e criar conta corrente. Fique a vontade para adicionar mais funções, exemplo: listar contas.

 
***Criar Usuário(cliente)***

O programa deve armazenar os usuários em uma lista, uma usuário é composto por: mome, data de nascimento, cpf e endereço. O endereço é uma string com o formato: logradouro, nro - bairro - cidade/sigla estado. Deve ser armazenado somente os números de CPF. Não podemos cadastrar 2 usuários com o mesmo CPF.


***Criar Conta Corrente***

O programa deve armazenar contas em uma lista, uma conta é composta por: agencia, número da conta e usuário. O número da conta é sequencial, iniciando em 1. O número da agencia é fixo: "0001". O usuário pode ter mais de uma conta, ma uma conta pertence a somente um usuário.

***Dica***

Para vincular um usuário a uma conta, filtre a lista de usuários buscando o número do CPF informado para cada usuário da lista. 


***Desafio Sistema Bancário em Python versão 3***

***Objetivo Geral***

Iniciar a modelagem do sistema bancário em POO. Adicionar classes para cliente e as operações bancárias: depósito e saque. 


***Desafio versão 3***

Atualizar a implementação do sistema bancário, para armazenar os dados de clientes e contas bancárias em objetos ao invés de dicionários. O código deve seguir o modelo de classes UML.

***Desafio Extra***

Após concluir a modelagem das classes e a criação dos métodos. Atualizar os métodos que tratam as opções do menu, para funcionarem com as classe modeladas.