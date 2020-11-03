# Git

O git não é nada mais nada menos que um **Sistema de Controle de Versões (VCS)**. Ele é uma ferramenta para ajudar uma equipe de programadores que estão trablhaando juntos num projeto a se organizarem melhor para que haja mais produtividade.

**OBS**: Para utilizar o git você **não precisa estar conectado a internet**, mas um servidor (mesmo que seja local) ainda será preciso para o seu uso.

## Onde acessar o Git

O git é acessível no terminal do computador ou em qualquer emulador que o aceite

## Iniciando um repositório Git

Caso você já possua a pasta/diretório do seu projeto no seu sistema e deseja torná-la um repositório git, basta realizar o seguinte comando: 

`git init`

Este comando faz com que o git passe a 'enxergar' seu projeto como um **repositório git**.

## Dando uma 'checada' no git

Se você precisar checar como que as coisas estão no seu repositório git ou até mesmo se você quiser **saber se um diretório/pasta é um repositório git**, é só você estar nele e digitar no terminal o seguinte comando:

`git status`

Esse comando vai te mostrar algumas informações como:

* Em que **branch/ramo** você está.
* **commits** ativos.
* Arquivos que não estão sendo monitorados.

## Fazendo o Git fazer o trabalho dele

Quando um repositório git é iniciado, ele não começa a monitorar as alterações dos seus arquivos internos de imediato, pois isso quem controla é o usuário. E o comando para adicionar alterações é:

`git add <arquivos...>`

ou se você quiser adicionar tudo:

`git add .`

**Nota: É importante saber que ADD não está adicionando um arquivo novo ao repositório, mas sim dizendo que o arquivo (sendo novo ou não) está sendo preparado para entrar na próxima revisão do repositório.**

    