# Executando um script python e trabalhando com números

Nesse tópico vamos aprender:

1. Criar um arquivo (script) python.
2. Como executar um script python.
3. Como trabalhar com números em python.

## Como criar um arquivo (script) python.

Primeiro passo consiste em criar um novo arquivo, no nosso exemplo vamos utilizar o VIM:

<pre>
vim primeiro_script.py
</pre>

No exemplo acima criamos um arquivo chamado "primeiro_script.py", note que a extensão do arquivo deve ser ".py".

É importante garantir que este arquivo tenha permissão de execução, isto é, que o sistema operacional seja capaz de executar arquivo,
não apenas ler ou escrever.

Para isso executamos o seguinte comando:

<pre>
chmod 755 primeiro_script.py
</pre>

Note que há outras formas de fazer o mesmo procedimento, verá isso se procurar na internet.

Após criar o arquivo é fundamental adicionar 2 linhas em todos os scripts python, no início dos arquivos:

<pre>
#!/usr/bin/python
# -*- coding: utf-8 -*-
</pre>

A primeira linha define onde o interpretador do python está instalado. A segunda linha define o padrão de codificação que
será utilizado, o UTF-8. Veja -> https://pt.wikipedia.org/wiki/UTF-8

Após essa duas linhas você pode começar a codificar o seu script python.

## Como executar um script python

A execução do script python é muito simples, uma vez que você já deu permissão de execução ao script basta executá-lo da seguinte
forma:

<pre>
./primeito_script.py
</pre>

## Como trabalhar com números em python.

Nesse ponto é importante lembrar que Python é uma linguagem não tipada, isto significa que as variáveis podem mudar de tipo após terem sido criadas, o que por um lado é bom pois facilita a codificação, mas que por outro lado pode gerar uma série de problemas se você esquecer desse detalhe.

Os principais tipos de variáveis númericas em python são o **int** e o **float**, mas além disso temos outros tipos, tais como **decimal**, **fraction**, **complex**. Mas nesse primeiro momento vamos focar nos dois principais visto que uma vez entendido o conceito desses tipos as demais ficam mais claras.

### As diferências entre int e float

Variáveis do tipo **int** representam números inteiros (lembra, 0, 1, 2 ...) e variáveis do tipo **float** representam números com casas decimais (lembra, 0.0, 0.5, 1.2 ...).

Abra o interpretador python, que você aprendeu a utilizar no exercício anterior e veja as diferenças através dos exemplos abaixo:

<pre>
>>> int(1)
1
>>> float(1)
1.0
>>> int(2.1)
2
>>> float(2.1)
2.1
</pre>

Note que o tipo **int** não representa inteiros, enquanto o tipo **float** consegue representar tanto inteiros quanto as casas decimais.

### Criando variáveis no script python

Agora vamos voltar a edição do primeiro_script.py.

Para criar uma nova variável basta escrecer da seguinte forma:

<pre>
nome_da_variavel = 1
</pre>

Como vimos, em python você não precisa dizer o tipo que a variável tem, o próprio interpretador já fiz por você, então você cria a variável e já atribui alguma informação ela e pronto. Se for criar um **float** fica assim:

<pre>
nome_da_variavel = 1.0
</pre>

#### Exercício 1:

Crie no seu script 2 variáveis, uma recebendo um valor inteiro e outra um valor com casa decimal, adicione a seguinte linha a seu script, depois de criar as variáveis:

<pre>
print nome_da_variavel1, nome_da_variavel2
</pre>

Salve o arquivo e tente executá-lo, você deverá ver os valores das variáveis sendo mostrados no terminal.

Depois faça o commit do arquivo para salvar uma versão no repositório.

### Operações númericas em python

As principais operações númericas em python são as seguintes:
* ** Exponenciação
* % Módulo
* \* Multiplicação
* / Divisão
* \+ Soma
* \- Subtração

Essa lista segue a ordem de precedência, isto é, qual operação é executada primeiro em caso de mais operações em conjunto, por exemplo:

<pre>
resultado = 2 * 2 + 3
7
</pre>

Primeiro é executado a multiplicaço, depois a soma.

Mas adquira o hábito de utilizar os () para deixar claro qual a precedência que você quer, por exemplo:

<pre>
resultado = 2 * (2 + 3)
10
</pre>

#### Exercício 2:

Edite o seu script e adiciona uma das operações acima para as suas variáveis. Use o 'print' para mostrar o resultado e verifique se está correto executando o script.

A ideia é que você crie uma terceira variável que vai receber diretamente a operação das duas variáveis criadas anteriormente, tipo assim:

<pre>
A = B + C
</pre>

Depois faça o commit do arquivo para salvar uma versão no repositório.

#### Exercício 3:

Edite novamente seu script, a ideia agora é acrescentar todas as operações que você viu e imprimir o resultado uma por vez.
É importante saber que você pode criar uma variável que já recebe uma operação sem necessidade de criar outras variáveis apenas para receber os números, como no exemplo abaixo:

<pre>
variavel_1 = 2
variavel_2 = 3
variavel_3 = variavel_1 + variavel_2

# Ou podemos fazer assim:

variavel_3 = 2 + 3
</pre>
