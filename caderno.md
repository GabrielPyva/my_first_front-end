# Git

## Ações Básicas

O git não é nada mais nada menos que um **Sistema de Controle de Versões (VCS)**. Ele é uma ferramenta para ajudar uma equipe de programadores que estão trablhaando juntos num projeto a se organizarem melhor para que haja mais produtividade.

**OBS**: Para utilizar o git você **não precisa estar conectado a internet**, mas um servidor (mesmo que seja local) ainda será preciso para o seu uso.

### Onde acessar o Git

O git é acessível no terminal do computador ou em qualquer emulador que o aceite.

### Iniciando um repositório Git

Caso você já possua a pasta/diretório do seu projeto no seu sistema e deseja torná-la um repositório git, basta realizar o seguinte comando: 

`git init`

Este comando faz com que o git passe a 'enxergar' seu projeto como um **repositório git**.

### Dando uma 'checada' no git

Se você precisar checar como que as coisas estão no seu repositório git ou até mesmo se você quiser **saber se um diretório/pasta é um repositório git**, é só você estar nele e digitar no terminal o seguinte comando:

`git status`

Esse comando vai te mostrar algumas informações como:

* Em que **branch/ramo** você está.
* **commits** ativos.
* Arquivos que não estão sendo rastreados.

### Adicionando arquivos para revisão

Quando um repositório git é iniciado, ele não começa a monitorar as alterações dos seus arquivos internos de imediato, pois isso quem controla é o usuário. E o comando para adicionar alterações de algum(s) arquivo(s) é:

`git add <arquivos...>`

ou se você quiser adicionar tudo:

`git add .`

**Nota:**É importante saber que ADD não está adicionando um arquivo novo ao repositório, mas sim dizendo que o arquivo (sendo novo ou não) está sendo preparado para entrar na próxima revisão do repositório. É o que se chama de colocar em estado de **staged**.

### Salvando as alterações

No git, o termo acima não é muito utilizado pois ele se resume a uma palavra só: __snapshot__. E quando se salva alguma alteração no git, é obrigatório deixar uma mensagem explicando o que foi alterado. O comando é o seguinte:

`git commit -m "mensagem"`

#### Estados de um arquivo

Um arquivo pode possuir 2 estados: rastreado e não rastreado. Rastreados são arquivos que foram incluídos no **último snapshot**. E os Não rastreados são todo o resto.

### Como ver o histórico de snapshots/commits

Às vezes, para detectar algum bug ou erro de versão, ou até mesmo para verificar algum commit usamos o comando:

`git log`

Esse comando vai mostrar **todos os commits** realizados até então com os seguintes dados:

* O **hash** do commit (que é o numero hexadecimal que o identifica).
* A **branch** do commit.
* O **autor** do commit.
* A **data** do commit.
* A **mensagem** de commit.

#### Maneiras de visualizar o histórico de commits

Eis as segintes opções que se pode colocar no comando para exibí-lo de maneira diferenciada:

* `git log --oneline`
* `git log -p`
* `git log --pretty="format:%h %s %a"...`

### Fazendo o Git ignorar arquivos

Por algum motivo, você poder querer que o Git não saiba nem que seu arquivo exista. E a melhor forma de fazer com que ele faça isso é **criando um arquivo** dentro do seu projeto chamado **.gitignore**.

**Nota**: É crucial que o nome do arquivo seja EXATAMENTE esse acima.

Dentro desse arquivo serão escritos, em cada linha, o nome dos arquivos a serem ignorados pelo Git.

