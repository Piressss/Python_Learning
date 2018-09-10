# Python_Learning
Repositorio para aprendizado de Python

## Configurações necessárias

Partindo do princípio que iremos trabalhar com Ubuntu 14.04 ou Ubuntu 16.04 e Python 2.7.

As configurações iniciais são as seguintes e devem ser executadas em um Terminal do Linux.

Para abrir um terminal você pode procurar no Menu ou utilizar as teclas de acesso CTRL+ALT+T.

Com o terminal aberto vamos instalar os seguintes pacotes:

*GIT*
digite no terminal o comando:

<pre>
sudo apt-get install git
</pre>

Com este comando faremos a instalação do pacote GIT. O pacote GIT é um controle de versão muito útil que visa facilitar o desenvolvimento gerenciando as versões implementadas e o backup de forma adequada. 
Mais informaçes em: https://pt.wikipedia.org/wiki/Git

O comando acima utiliza o apt para instalar um novo pacote, para mais informaçes consulte: https://e-tinet.com/linux/comando-linux-apt/

A primeira parte do comando 'SUDO' fornece os mecanismos de previlégio para instalar no Ubuntu. Mais informações em: https://e-tinet.com/linux/comando-linux-apt/

Ao digitar o comando ser solicitada a confirmação e o pacote GIT será instalado.

*Editores*

Existem vários editores para implementação do código além de claro IDE, que são ferramentas mais complexas que não apenas permitem a edição mas fornecem alguns outros mecanismos.

Eu costumo utilizar o VIM, é editor mais bruto vamos dizer, um pouco mais complicado para se acostumar pois exige a memorização de várias teclas de acesso, mas em contrapartida depois dessa fase inicial o desenvolvimento fica bem acelerado.

<pre>
sudo apt-get install vim
</pre>

Caso não queira utilizar pode pesquisar no googles outros IDE/Editores, uma das recomendações é esta:
https://www.jetbrains.com/pycharm/download/#section=linux

*Terminator*

Essa aplicação é bastante útil pois permite dividir um terminal em vários telas, pelo menos para mim melhor do que ficar abrindo vários terminais e ter que ficar trocando de tela (ALT+TAB), ele também tem teclas de acesso rápido que facilitam a mudança entre os vários terminais abertos.

<pre>
sudo apt-get install terminator
</pre>

Finalizado estes pontos estaremos prontos para iniciar o desenvolvimento.
