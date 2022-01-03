
# Meu Token 
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


# PARA INICIAR UMA LINHA DO TEMPO OU SEJA UM REPOSITÓRIO
UTILIZAMOS => GIT INIT

SEGUNDO COMANDO => touch landingpage.html


# para criar um ponto na história onde foi iniciado o projeto
# landingpage.html

ultilizamos o comando => add landingpage.html (adiciona o repositorio)


utilizando o comando (( git commit -m "adde landing page" )) => ele vai levar a alteração ao meu repositório



# para ver um ponto na historia que foi criado

git log

# para verificar alterações nos projetos git utiliza-se o comando

git status

# para reatualizar, utiliza-se o 
 git add landingpage.html

 git commit -m "updated landing page"  ((# para reenviar o arquivo para o repositório))

 # para verivicar mudanças utiliza-se 
 git log

# ao criar pontos no projeto com git show eu consigo revisitalos e observar o que foi feito neles
# com o comando 

git show ea9484f98aeffcd9deb087b6fb128663c830889b

# para ver so o ultimo ponto, utilizamos só o 

git show

# master no git é a linha do tempo principal 

dentro da linha master são executados os recursos principais do projeto

# branch significa ramificação  ou seja a brench e uma linha do tempo alternativa

com a brench podemos criar uma nova extenção do projeto porem sem afetar o recurso principal

# criando um branch 
git branch feature/cart

# para mundar de linha e entra na branch ultilizamos o comando 

git checkout feature/cart
ao utilizar esse comando criamos uma branch branch feature/cart

# utilize "git add " para incluir o que será submetido

# e para conferir usamos o comando => git status

git status 

# ao fazer esse procedimento estaremos dentro da branch , então devemos criar um repositorio 
# para criar um novo repositório utilizo o comando => touch cart.html

touch cart.html

# ao fazer todos os processos temos duas linhas do tempo a linha master e a linha branch
# para voltar para linha master eu utilizo => git checkout master 
git checkout master

# nós tambem podemos olhar todas as nossas linhas do tempo utilizando => git branch
git branch

#  para dar prosegmento voutaremos a nossa branch cart com o comando 
git checkout feature/cart

# damos um git status e vimos que ela ainda não foi adicionada 
# para adiciona damos o seguinte comando => git add cart.html logo após o
# git commit -m "adde cart"

(( => git add cart.html   ))   logo após o
(( => git commit -m "adde cart" ))
# texte se foi execultado com
git log

ao executarmos esse comando esse é o resultado

# commit aee1f2e2f84cbb5b275dca79dcb2e27725dbddb2 (HEAD -> feature/cart)
# Author: sanuelcpr <samuel@prte.com.br>
# Date:   Sun Jan 2 11:11:39 2022 -0300

  #  adde cart

# commit ea9484f98aeffcd9deb087b6fb128663c830889b (master)
# Author: sanuelcpr <samuel@prte.com.br>
# Date:   Sun Jan 2 10:10:18 2022 -0300
# add landing page

proximo passo 

# O proximo passo para fazermos algumas analises e voltar para a linha master
# ultilizando o comando 

git checkout master

# ao voltar vamos utilizar os comandos ls -al para fazer uma analise das linha

ls -al 

#ao fazer isso notamos que a branch feature/cart não foi compactada com o projeto

# para adicionalo a linha master vc conclui as modificações e aplica os seguintes comandos

=> git checkout feature/cart # para retornar a branch
=> git add cart.html # ao modificar é necessario add de novo
=> git commit "cart ok" # esses comando serão utilizado para modificação e conclusão dos projetos

# após os procedimentos acima voltamos a linha master com o comando => git checkout master
# depois utilizamos o comando => ls --al e vemos que a => branch feature/cart ainda não foi adicionada

=> git checkout master

=> ls --al

# para adionarmos a branch feature/cart a linha master do projeto utilizamos 

git merge feature/cart

# ao fazer isso temos a branch cart no prjeto, para conferirmos damo um 

git status
# com o git status vemos que o repositório cart.html foi alocado pois não o consta mais na lista


# samuel@samuel-H55:~/Documentos/Curso_git_github$ git status
No ramo master
Arquivos não monitorados:
  (utilize "git add <arquivo>..." para incluir o que será submetido)
        README.md
        gitcomandos.md


git log  
# com o git log vemos que a branch feature/cart esta contida dentro da linha master


# samuel@samuel-H55:~/Documentos/Curso_git_github$ git log
commit aee1f2e2f84cbb5b275dca79dcb2e27725dbddb2 (HEAD -> master, feature/cart)
Author: sanuelcpr <samuel@prte.com.br>
Date:   Sun Jan 2 11:11:39 2022 -0300

    adde cart

commit ea9484f98aeffcd9deb087b6fb128663c830889b
Author: sanuelcpr <samuel@prte.com.br>
Date:   Sun Jan 2 10:10:18 2022 -0300

# para vermos o que foi mudado nos projetos utilizamos o comando 

git show

# para deletar uma branch utilizamos os seguintes comandos 

git branch -D feature/cart 

ao utilizar esse comando a branch que vc direcionou será deletada 

# O proximo passo é adionar o git na nuvem ou seja no github
# para fazer isso ultilizamos os seguintes comandos 

git remote add origin https://github.com/samuelcpr/Aula-git.git
git branch -M master
git push -u origin master

# utilizando o comando git push podemos enviar os arquivos para a nuvem github
=> git push 

# para configurar o git 








# RESUMO DOS COMANDOS

# git init // inicia a linha do tempo
# git add // adiciona ou atualiza mudanças para irem para a linha do tempoo
# git commit // adiciona um ponto na linha do tempo
# git log // visualiza os pontos na linha do tempo / commit
# git status // informa o estado das alterações do nosso projeto
# git show // apresenta determinado ponto na história 
# git branch // gerenciar novas linhas do tempo (TIPO branch feature/cart)
# git checkout // manipula as linhas do tempo (DEFINE SE BRANCH OU MASTER)
# git merge // unir linhas do tempo ( EXEMPLO MASTER, BRANCH)
# git push // envia alterações locais para o repositório remoto
# git clone // clonar um projeto / repositório
# git pull // puxa do repositório remoto


