# projeto-curso-git

# Curso Introdução ao Git e Controle de Versões

Curso promovido pela Digital Innovation One com o propósito de ensinar sobre a importância de adotar o controle de versão em seus projetos e como trabalhar com versionamento utilizando o Git e seus principais comandos. 

Complementei com alguns outros comandos que aprendi realizando um estudo pessoal.

 
## Principais comandos:


### - git help

Exibe informações de ajuda sobre o Git.


#
### - git help <comando_git> ou git <comando_git> --help

Exibe informações de um comando Git específico.


#
### - git config --global user.name "Nome do Usuário"

Define o nome do usuário.


#
### - git config --global user.email "email@email.com"

Define o email do usuário.


#
### - git config --global core.editor vscode

Define o editor que será utilizado.


#
### - git config --list

Lista as configurações.


#
### - git init

Cria um repositório Git vazio ou reinicializa um existente.


#
### - git status

Verifica em que estado estão os arquivos.


#
### - git log

Exibe o histórico de commits em ordem cronológica inversa, com informações tais como o autor, a data e o identificador de cada commit.


#
### - git add .

Adiciona todos os arquivos ao índice (também conhecido como Index, Stage ou Staging Area) para serem commitados, indicando ao Git que esses arquivos serão monitorados, rastreados.


#
### - git add <nome_arquivo.extensao>

Uma forma de adicionar um arquivo específico para ser commitado.


#
### - git add <nome_diretorio>

Uma forma de adicionar um diretório específico que contém arquivos que serão commitados.


#
### - git commit -m "Mensagem referente a alteração."

Commita as alterações realizadas nos arquivos com uma mensagem. De fato, as mudanças são salvas no repositório local adicionando uma mensagem.


#
### - git rm --cached <nome_arquivo.extensao>

Remove o arquivo especificado da staging area, deixando de ser monitorado pelo Git. E, logo em seguida, já pode commitar a alteração com uma mensagem referente a esta alteração.


#
### - git rm -f <nome_arquivo.extensao>

Além de remover o arquivo especificado da staging area, deixando de ser monitorado pelo Git. O arquivo também é removido da máquina. Da mesma forma, logo em seguida, já pode commitar a alteração com uma mensagem referente a esta alteração.


#
### - git rm -r --cached <nome_diretorio>

Remove o diretório (pasta) especificado da staging area, onde os arquivos contidos neste diretório deixam de ser monitorados pelo Git. Da mesma forma, logo em seguida, já pode commitar a alteração com uma mensagem referente a esta alteração.


#
### - git rm -r -f <nome_diretorio>

Além de remover o diretório (pasta) especificado da staging area, onde os arquivos contidos neste diretório deixam de ser monitorados pelo Git. O diretório (pasta) também é removido da máquina.  Da mesma forma, logo em seguida, já pode commitar a alteração com uma mensagem referente a esta alteração.


#
### - git reset HEAD <nome_arquivo.extensao>

Comando utilizado quando o arquivo já foi adicionado a staging area, porém, não é para remover o arquivo, para ele deixar de ser monitorado. Com este comando a alteração é desfeita e o arquivo sai da staging area.


#
### - git checkout <nome_arquivo.extensao>

Retorna o arquivo ao estado do último commit. Todas as alterações feitas após o último commit são descartadas.


#
### - git reset --soft HEAD~1

Reverte o commit, retornando exatamente para a etapa anterior ao commit, ou seja, as alterações continuam feitas e continuam na staging area. 
O número 1 após o HEAD é para indicar a quantidade de commits que desejamos reverter.


#
### - git reset --mixed HEAD~1 ou 
### - git reset HEAD~1

Reverte o commit, removendo as alterações da staging area.


#
### - git reset --hard HEAD~1

Reverte o commit, removendo as alterações da staging area e removendo as alterações realizadas no arquivo.


#
### - git revert HEAD~1 ou git revert <inicial_da_hash_do_commit>
 
Reverte o commit sem alterar o histórico. O histórico é mantido.


#
### - git diff

Visualiza as modificações feitas nos arquivos, exibindo linhas exatas que foram adicionadas ou removidas.


#
### - git diff <nome_arquivo.extensao>

Visualiza as modificações feitas no arquivo especificado, exibindo linhas exatas que foram adicionadas ou removidas.


#
### - Criando o arquivo .gitignore

Faz com que o Git ignore arquivos, pastas ou arquivos com determinadas extensões listados dentro deste arquivo .gitignore. 


#
### - git remote add origin <endereco_do_seu_repositorio_remoto>

Vincula um repostório local a um repositório remoto. O repositório que era apenas local agora passa a ter uma cópia num repositório remoto.


#
### - git push -u origin master

Envia as alterações, os commits feitos localmente para a branch do repositório remoto. O comando acima é utilizado no primeiro push ao repositório remoto. Nos demais pushes, pode utilizar apenas o git push.


#
### - git pull

Atualiza o repositório local de acordo com o repositório remoto. Baixa as alterações de uma branch que está no repostório remoto para o repositório local.


#
### - git clone

Clona um repositório existente. Cria uma cópia de um repositório.


#
### - git remote -v

Verifica o novo repositório remoto clonado. Exibe o repositório remoto.


#
### - git branch

Lista as branchs (ramificações) existentes no projeto atualmente.


#
### - git branch <nome_branch>

Cria uma nova branch, cópia do projeto independente, onde podemos alterar os arquivos do projeto sem interferir nos originais.


#
### - git branch -D <nome_branch>

Deleta a branch. E, para conseguir deletar, não pode estar na branch que deseja deletar. 


#
### - git branch -d <nome_branch>

Deleta a branch se ela estiver sincronizada com o repositório remoto, ou se, tiver usado o git merge. Da mesma forma, para conseguir deletar, não pode estar na branch que deseja deletar. 


#
### - git checkout <nome_branch>

Muda de uma branch para outra branch.


#
### - git checkout -b <nome_branch>

Cria uma nova branch e automaticamente muda para ela.


#
### - git branch -m <novo_nome_branch>

Renomeia a branch.


#
### - git merge <nome_branch>

Une uma branch com uma outra branch. Para realizar o merge, é necessário estar na branch que deverá receber as alterações.


#
### - git fetch

Baixa as mudanças encontradas no repositório remoto que não estão no repositório local. 
