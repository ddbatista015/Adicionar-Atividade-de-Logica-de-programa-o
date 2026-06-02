**Exercício 1 – Menu da Lanchonete (estrutura escolha)**



algoritmo "menu\_lanchonete"



var

&#x20;  codigo: inteiro



inicio



&#x20;  escreval("===== MENU DA LANCHONETE =====")

&#x20;  escreval("1 - Cachorro Quente")

&#x20;  escreval("2 - Hamburguer")

&#x20;  escreval("3 - Misto Quente")

&#x20;  escreval("4 - Refrigerante")

&#x20;  escreva("Digite o codigo do item desejado: ")

&#x20;  leia(codigo)



&#x20;  escolha codigo

&#x20;     caso 1

&#x20;        escreval("Cachorro Quente - R$ 8,00")

&#x20;     caso 2

&#x20;        escreval("Hamburguer - R$ 15,00")

&#x20;     caso 3

&#x20;        escreval("Misto Quente - R$ 10,00")

&#x20;     caso 4

&#x20;        escreval("Refrigerante - R$ 5,00")

&#x20;     outrocaso

&#x20;        escreval("Codigo invalido!")

&#x20;  fimescolha



fimalgoritmo







**Exercício 2 – Tela de Bloqueio (estrutura enquanto)**

algoritmo "tela\_bloqueio"



var

&#x20;  senhaCorreta, senhaDigitada: caractere



inicio



&#x20;  senhaCorreta <- "123456"



&#x20;  escreva("Digite a senha: ")

&#x20;  leia(senhaDigitada)



enquanto senhaDigitada <> senhaCorreta faca

limpatela

escreval("Senha incorreta, acesso negado. Tente novamente:")

leia(senhaDigitada)

&#x20;  fimenquanto



&#x20;  escreval("Acesso liberado!")



fimalgoritmo





**Exercício 3 – Caixa Eletrônico (integração enquanto + escolha)**

algoritmo "caixa\_eletronico"



var

&#x20;  opcao: inteiro

&#x20;  saldo, valor: real



inicio



&#x20;  saldo <- 1000

&#x20;  opcao <- -1



&#x20;  enquanto opcao <> 0 faca



&#x20;     escreval("===== CAIXA ELETRONICO =====")

&#x20;     escreval("1 - Consultar Saldo")

&#x20;     escreval("2 - Fazer Saque")

&#x20;     escreval("3 - Fazer Deposito")

&#x20;     escreval("0 - Sair")

&#x20;     escreva("Escolha uma opcao: ")

&#x20;     leia(opcao)



&#x20;     escolha opcao



&#x20;caso 1

escreval("Saldo atual: R$ ", saldo:0:2)



&#x20;caso 2

&#x20; escreva("Digite o valor do saque: ")

leia(valor)

saldo <- saldo - valor

escreval("Novo saldo: R$ ", saldo:0:2)



caso 3

escreva("Digite o valor do deposito: ")

leia(valor)

saldo <- saldo + valor

escreval("Novo saldo: R$ ", saldo:0:2)



caso 0

escreval("Sistema encerrado.")



outrocaso

escreval("Opcao invalida!")



fimescolha



fimenquanto



fimalgoritmo

