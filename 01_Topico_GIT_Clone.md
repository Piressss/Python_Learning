# Utilização do GIT para acesso local ao repositório

Apesar de ser possível utilizar o GitHub para implementação, não traz muitas facilidades para esta finalidade.

A ideia deste material é aprender a fazer o clone do repositório (Download), abrir os arquivos, adicionar um novo arquivo e fazer o push (upload) para
o repositório.

## Configuração Inicial do GIT

Vamos iniciar fazer a configuração do seu ususário para o GIT.

Abra um terminal (Ctrl+T no Linux).

Configura o nome de usuário através do comando abaixo, troque o a informação NOME_DO_USUARIO pelo nome do seu usuário, uma boa prática é utilizar o mesmo usuário do Linux.

<pre>
git config --global user.name "NOME_DO_USUARIO"
</pre>

Depois vamos configurar um email padrão para o usuário.

<pre>
git config --global user.email fulano@example.com
</pre>

## Primeiro Passo - Clone

Primeiro passo é fazer o clone do repositório, para que possar ser utilizado no seu pc.

No site do GitHub, dentro do repositório você encontra o link para o clone no botão "Clone or Download", que deve ser o link abaixo:

<pre>
https://github.com/Piressss/Python_Learning.git
</pre>

Antes de efetuar o clone vamos definir o local onde você deverá executar o comando.

Abra um novo terminal (CTRL+ALT+T), vá se acostumando com as teclas de atallho.

Neste terminal digite o seguinte comando:

<pre>
pwd
</pre>

O resultado deve ser algo parecido com isso:

<pre>
/home/USER
</pre>

No lugar de USER deve estar escrito o nome de seu usuário, esse comando mostra o 'path' ou caminho da onde você está, em outras palavras o caminho do
diretório que você está. Usualmente dizemos que esse caminho é o seu HOME.

Agora vamos criar uma nova pasta:

<pre>
mkdir GitHub
</pre>

Para verificar se a pasta foi criada, execute:

<pre>
ls
</pre>

Deve aparecer as pastas que você tem no seu HOME e mais a pasta criada 'GitHub'. Você acabou de aprender 2 novos comandos, 'mkdir' para criar
diretórios e 'ls' para listar tudo que tem dentro do diretório que estiver.

Agora vamos entrar na pasta com o comando 'cd' que serve para obviamente entrar na pasta através do terminal.

<pre>
cd GitHub
</pre>

Execute novamente o comando 'pwd', deve aparecer algo como assim:

<pre>
/home/USER/GitHub
</pre>

Se der um 'ls' vai ver que não tem nada dentro, ainda.

Se tudo deu certo, você deve estar no diretório para fazer o clone do seu repositório. Então execute:

<pre>
git clone https://github.com/Piressss/Python_Learning.git
</pre>

Algumas coisas vão aparecer na sua tela e ao terminar ocê deve executar o comando 'ls' novamente, deve aparecer o nome do diretório 'Python_Learning'. Entre no diretório utilizando o comando 'cd', como vimos anteriormente, agora você está dentro do repositório local.

## Segundo Passo - Criar um novo arquivo

Agora crie um arquivo através de qualquer editor, salve com o nome "Teste.txt" e escreva no arquivo a frase "Teste no GIT". Lembre-se você deve criar o arquivo dentro do diretório que fizemos o clone.

Você pode criar com o gedit:

<pre>
gedit Teste.txt
</pre>

Editar e salvar. Verifique com o 'ls' se o arquivo foi criado depois que fechá-lo.

Agora vamos aprender a fazer o PUSH, isto é upload do repositório com o novo arquivo, são 3 passos:

## Terceiro Passo - Atualizar o repositório do GitHub com suas modificações

Adicione o arquivo para o seu repositório local:

<pre>
git add Teste.txt
</pre>

Faça o commit do arquivo, isto é, sinaliza que você vai enviar o arquivo.

<pre>
git commit -m "Enviando arquivo"
</pre>

Agora execute o envio, será requisitado o seu usário e senha do GitHub:

<pre>
git push
</pre>

Pronto se tudo deu certo você já consegue visualizar o arquivo pelo browser no repositório do GitHub.

## Quarto Passo - Atualizar o repositório local

Agora você aprendeu a executar os principais comandos do Git, recomendo pesquisar no google melhor sobre estes comandos. Mas ainda falta um comando importante, o 'Pull'. O 'Pull' serve para atualizar o seu repositório local, imagine que outro usuário alterou o repositório do Git e você precisa antes de retomar o seu trabalho atualizar o seu repositório com estas modificações, então dentro do seu repositório você vai executar:

<pre>
git pull
</pre>

Todas as modificações serão copiadas para o seu repositório e você poderá ver localmente as modificações.

*Resumo*, leia o link abaixo, bom até para treinar o inglês:

https://git-scm.com/docs/gittutorial
