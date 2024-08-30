# comandos-git
Documento para me auxiliar e conhecer os principais comandos do GIT.

# Documentação de Comandos Git

## Configrações básicas

***Gravar o nome nas transações de commits***

    $ git config --global user.name "nome aqui"

***Gravar o e-mail nas transações de commits***

    $ git config --global user.email "email aqui"

***Gravar o e-mail nas transações de commits***

    $ git config --global color.ui auto

## 1. Iniciar um repositório Git na máquina

***Para inicializar um repositório Git no diretório atual, use o comando:***

    $ git init

## 2. Clonar um repositório existente

***Para clonar um repositório existente, use o comando:***
    
    $ git clone <URL do repositório>


## 3. Adicionar mudanças ao índice (staging area)

***Para adicionar mudanças ao índice, use:***

    $    git add "nome do arquivo"

ou

***Para adicionar todas as mudanças de uma só vez:***

    $ git add .


## 4. Confirmar mudanças (commit)

***Para confirmar as mudanças adicionadas ao índice, use:***

    $ git commit -m "Mensagem de commit"


## 5. Verificar o estado do repositório

***Para verificar o estado atual do repositório, incluindo arquivos modificados e não rastreados, use:***

    $ git status


## 6. Visualizar o histórico de commits

***Para visualizar o histórico de commits, utilize:***
    
    $ git log


## 7. Criar e mudar para uma nova branch***Para criar e mudar para uma nova branch, utilize:***

    $ git checkout -b <nome-da-branch>


## 8. Mudar para uma branch existente

***Para mudar para uma branch já existente, use:***

    $ git checkout <nome-da-branch>


## 9. Mesclar branches

***Para mesclar uma branch na branch atual, use:***

    $ git merge <nome-da-branch>


## 10. Enviar mudanças para o repositório remoto

***Para enviar commits locais para o repositório remoto, use:***

    $ git push origin <nome-da-branch>

## 11. Atualizar o repositório local com mudanças do repositório remoto

***Para obter mudanças do repositório remoto e mesclar com a branch local, use:***

    $ git pull


## 12. Remover um arquivo do índice (unstage)

***Para remover um arquivo do índice sem apagar o arquivo, utilize:***

    $ git reset <nome do arquivo>

## 13. Descartar mudanças em um arquivo

***Para descartar mudanças não confirmadas em um arquivo, use:***

    $ git checkout -- <nome do arquivo>


## 14. Remover branches locais

***Para remover uma branch local que não está em uso, utilize:***

    $ git branch -d <nome-da-branch>

## 15. Remover branches remotas
***Para remover uma branch no repositório remoto, use:***

    $ git push origin --delete <nome-da-branch>


## 16. Adicionar um repositório remoto

***Para adicionar um repositório remoto, utilize:***

    $ git remote add origin <URL do repositório remoto>


## 16.1 Trocar Remoto

***Se você quiser apenas alterar a URL do remote existente, pode usar o seguinte comando:***

    $ git remote set-url <nome-do-remote> <nova-URL>


***Por exemplo, para alterar a URL do remote chamado origin:***

    $ git remote set-url origin https://nova-url-do-repositorio.git


## 17. Visualizar repositórios remotos
***Para listar todos os repositórios remotos configurados, use:***

    $ git remote -v


## 18. Remover um repositório remoto
***Para remover um repositório remoto, utilize:***

    $ git remote remove <nome-do-remote>


## 19. Renomear um repositório remoto

***Para renomear um repositório remoto, use:***

    $ git remote rename <nome-antigo> <nome-novo>


## 20. Atualizar as referências de remotes

***Para atualizar as referências de branches remotas, utilize:***


## 21. Obter e mesclar mudanças de um repositório remoto

***Para obter mudanças do repositório remoto e mesclar com a branch local atual, use:***

    $ git pull <nome-do-remote> <nome-da-branch>


## 22. Enviar mudanças para um repositório remoto

***Para enviar commits locais para uma branch específica do repositório remoto, utilize:***

    $ git push <nome-do-remote> <nome-da-branch>


## 23. Definir o repositório remoto de uma branch

***Para definir ou alterar o repositório remoto associado a uma branch local, use:***

    $ git branch --set-upstream-to=<nome-do-remote>/<nome-da-branch>

## 24. Desfazer commits

***Desfaz todos os commits e mantém as mudanças locais***
    
    $ git reset "commit"

***Descartar todoo histórico e mudanças para o commit específicado***

    $ git reset --hard "commit"

## 25. Histórico de Commits

***Lista o histórico de versões para a branch atual***

    $ git log

***Lista o histórico de versões para um arquivo específico, incluindo mudanças e nomes***

    $ git log --follow

***Mostra diferença de conteúdo entre duas branchs***

    $ git diff "primeira branch"..."segunda branch"

***Retorna mudanças de Metadata e conteúdo para o commit específicado***

    $ git show "commit"
