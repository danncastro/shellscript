## Comandos TMUX

### Informações

**O asterisco informa em qual janela estou no momento**


~~~bash
tmux # Cria uma nova sessão que sera fechada ao sair
~~~

~~~bash
tmux new -s nome_sessão # Cria uma nova sessão mantendo-a ativa mesmo que seia da sessão
~~~

~~~bash
tmux ls # Lista as sessões que estão ativas no momento
~~~

~~~bash
tmux attach -t nome_sessão # Entra novamente na sessão que está em execução
~~~

~~~bash
tmuxinator new nome-sessão # Cria uma sessão que pode ser gerenciada
nome: nome-sessão
root: /caminho/do/projeto

windows:
    - VIM: vim .
    - DANGER ZONE:
        layout: main-horizontal
        panes:
            - git fetch --all
            - git status
~~~

~~~bash
tmuxinator nome-sessão # Abre a sessão criada pelo gerenciador
~~~

## Prefixo padrão

**CTRL + B** + (ação)

- Exemplos: 
**CTRL + B** + C                ## Cria uma nova janelas dentro da sessão
**CTRL + B** + N ou P           ## Alterna entre as janelas
**CTRL + B** + ,                ## Altera o nome da janela criada
**CTRL + B** + D                ## Saí da sessão, sem que ela seja encerrada
**CTRL + B** + %                ## Cria um painel de divisão vertical para a janela atual
**CTRL + B** + X                ## Fecha o painel de divisão aberto na janela
**CTRL + B** + "                ## Cria um painel de divisão horizontal para a janela
**CTRL + B** + Q                ## Mostra todos os indices dos paineis que foram criados
**CTRL + B** + &                ## Fecha a janela com todos os paineis abertos
**CTRL + B** + O                ## Alterna entre os paineis



#### Descontração
~~~bash
curl parrot.live
~~~