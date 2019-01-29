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
