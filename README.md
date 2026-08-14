<h1 align="center">
  <a href="https://git-scm.com/">Git</a> e <a href="https://github.com/">GitHub</a>
</h1>

<p align="center">Controle e compartilhe seu código — guia de referência rápida dos comandos mais usados no dia a dia, organizado por tema.</p>

<p align="center">
  <a href="https://github.com/lucasrmagalhaes/git-gitHub/issues">
    <img src="https://img.shields.io/github/issues/lucasrmagalhaes/git-gitHub" alt="Issues" />
  </a>
  <a href="https://github.com/lucasrmagalhaes/git-gitHub/network/members">
    <img src="https://img.shields.io/github/forks/lucasrmagalhaes/git-gitHub" alt="Forks" />
  </a>
  <a href="https://github.com/lucasrmagalhaes/git-gitHub/stargazers">
    <img src="https://img.shields.io/github/stars/lucasrmagalhaes/git-gitHub" alt="Stars" />
  </a>
  <a href="https://github.com/lucasrmagalhaes/git-gitHub/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/lucasrmagalhaes/git-gitHub" alt="License" />
  </a>
</p>

## Sumário

- [Configuração](#configuração)
- [Criando e clonando repositórios](#criando-e-clonando-repositórios)
- [Staging e commits](#staging-e-commits)
- [Histórico e inspeção](#histórico-e-inspeção)
- [Repositórios remotos](#repositórios-remotos)
- [Branches](#branches)
- [Merge, rebase e cherry-pick](#merge-rebase-e-cherry-pick)
- [Desfazendo alterações](#desfazendo-alterações)
- [Stash](#stash)
- [Tags e versões](#tags-e-versões)
- [Comandos avançados](#comandos-avançados)
- [.gitignore](#gitignore)
- [Links úteis](#links-úteis)
- [Licença](#licença)

## Configuração

| Comando | Descrição |
| --- | --- |
| `git config --local user.name "Seu nome"` | Define o nome apenas para o repositório atual. |
| `git config --local user.email "Seu e-mail"` | Define o e-mail apenas para o repositório atual. |
| `git config --global user.name "Seu nome"` | Define o nome globalmente. |
| `git config --global user.email "Seu e-mail"` | Define o e-mail globalmente. |
| `git config --global --list` | Lista as configurações globais. |
| `git config --global core.editor "code --wait"` | Define o Visual Studio Code como editor padrão. |
| `git config --global core.editor "vim"` | Define o Vim como editor padrão. |
| `git config --global --unset core.editor` | Volta para o editor padrão do sistema. |
| `git config --global init.defaultBranch main` | Faz o `git init` criar a branch inicial como `main` em vez de `master` (a partir do Git 2.28). |
| `git config --global core.excludesfile ~/.gitignore_global` | Define um arquivo `.gitignore` global, válido para todos os repositórios da máquina. |

## Criando e clonando repositórios

| Comando | Descrição |
| --- | --- |
| `git init` | Inicializa um repositório Git local. |
| `git init --bare` | Cria um repositório sem working tree (sem cópia dos arquivos). Útil como repositório servidor, para que outros membros da equipe sincronizem seus trabalhos, economizando espaço de armazenamento. |
| `git clone url nome` | Baixa o repositório localmente. O nome é opcional, caso queira uma pasta com nome diferente do original. |
| `git clone -b nome-branch url` | Clona o repositório já em uma branch específica (forma longa: `--branch`). |

## Staging e commits

| Comando | Descrição |
| --- | --- |
| `git status` | Mostra o estado do repositório (arquivos modificados, staged e não rastreados). |
| `git add nome-arquivo` | Adiciona o arquivo ao stage para ser commitado. |
| `git add .` | Adiciona todos os arquivos (novos, modificados e removidos) ao stage, **a partir do diretório atual** e seus subdiretórios. |
| `git add --all` | Adiciona todos os arquivos ao stage **desde a raiz do repositório**, não importando em qual diretório você está. |
| `git mv nome-arquivo novo-nome` | Renomeia (ou move) o arquivo, já registrando a mudança no stage. |
| `git rm nome-arquivo` | Remove o arquivo e registra a remoção no stage. |
| `git commit -m "Mensagem"` | Realiza o commit com título. |
| `git commit -m "Mensagem" -m "Descrição"` | Realiza o commit com título e descrição. |
| `git commit -a -m "Mensagem"` | Adiciona todos os arquivos **já rastreados** que foram modificados e realiza o commit (não inclui arquivos novos). |
| `git commit --amend` | Adiciona as mudanças em stage ao último commit e permite editar a mensagem. |
| `git commit --amend --no-edit` | Adiciona as mudanças em stage ao último commit mantendo a mensagem original. |

## Histórico e inspeção

| Comando | Descrição |
| --- | --- |
| `git log --oneline` | Lista os commits em uma linha cada, de forma mais limpa. |
| `git log -p` | Lista os commits com as alterações (diff) de cada um. |
| `git log --graph --oneline --all` | Mostra o histórico de todas as branches em formato de grafo. |
| `git log --help` | Mostra as opções disponíveis do `git log`. |
| `git show nome-hash` | Mostra os detalhes e as alterações de um commit específico. |
| `git blame nome-arquivo` | Mostra quem alterou cada linha do arquivo e em qual commit. |
| `git diff` | Mostra o que foi alterado e ainda não foi adicionado ao stage. |
| `git diff commit..commit` | Mostra as diferenças entre dois commits. |
| `git reflog` | Lista todos os movimentos do HEAD — ótimo para recuperar commits "perdidos" após reset ou rebase. |
| `gitk` | Abre o visualizador gráfico de histórico. |

> 💡 Para personalizar a saída do log, veja o [git log cheatsheet](https://devhints.io/git-log).

## Repositórios remotos

| Comando | Descrição |
| --- | --- |
| `git remote` | Lista os remotes. |
| `git remote -v` | Lista os remotes com nome e endereço. |
| `git remote add origin https://github.com/usuario/projeto.git` | Adiciona um repositório remoto ao diretório local. |
| `git remote set-url origin https://github.com/usuario/projeto.git` | Altera a URL de um remote já existente. |
| `git remote rename nome-atual novo-nome` | Renomeia o remote. |
| `git remote remove nome-remote` | Remove o remote. |
| `git push nome-remote nome-branch` | Envia os commits para o repositório remoto. Usando `git push -u origin main` uma vez, o vínculo fica salvo e depois basta `git push`. |
| `git push --all` | Envia todas as branches para o repositório remoto. |
| `git fetch` | Baixa as informações do repositório remoto **sem** alterar nenhuma branch local. |
| `git pull` | Baixa e incorpora as alterações do remoto na branch local atual. |
| `git pull --rebase` | Baixa as alterações do remoto e reaplica seus commits locais por cima, sem criar merge commit. |

## Branches

| Comando | Descrição |
| --- | --- |
| `git branch` | Lista as branches locais. |
| `git branch -a` | Lista as branches locais e remotas. |
| `git branch nome-branch` | Cria uma branch. |
| `git checkout nome-branch` | Muda para a branch. |
| `git switch nome-branch` | Muda para a branch (comando mais novo, equivalente ao checkout). |
| `git checkout -b nome-branch` | Cria a branch e já muda para ela. |
| `git switch -c nome-branch` | Cria a branch e já muda para ela (equivalente moderno). |
| `git checkout -` | Volta para a branch anterior sem precisar digitar o nome. |
| `git branch -m novo-nome` | Renomeia a branch atual. |
| `git branch -m nome-atual novo-nome` | Renomeia outra branch, estando fora dela. |
| `git branch -d nome-branch` | Deleta a branch (somente se já foi mesclada). |
| `git branch -D nome-branch` | Força a exclusão da branch, mesmo sem merge. |
| `git push origin --delete nome-branch` | Deleta a branch no repositório remoto. |

## Merge, rebase e cherry-pick

| Comando | Descrição |
| --- | --- |
| `git merge nome-branch` | Incorpora os commits da branch informada na branch atual, gerando um merge commit quando necessário. |
| `git merge --abort` | Cancela um merge em andamento (com conflitos). |
| `git rebase nome-branch` | Reaplica os commits da branch atual por cima da branch informada. Diferente do merge, não gera merge commit — o histórico fica linear. |
| `git rebase -i` | Modo interativo: permite reordenar, combinar (squash) e editar commits. |
| `git rebase -i --root` | Modo interativo desde o primeiro commit do repositório. |
| `git cherry-pick nome-hash` | Traz um commit específico de outra branch para a branch atual. |

## Desfazendo alterações

| Comando | Descrição |
| --- | --- |
| `git restore nome-arquivo` | Descarta as alterações do arquivo (comando mais novo). |
| `git checkout -- nome-arquivo` | Descarta as alterações do arquivo (forma antiga). |
| `git restore .` | Descarta as alterações de todos os arquivos. |
| `git restore --staged nome-arquivo` | Tira o arquivo do stage, mantendo as alterações (comando mais novo). |
| `git reset HEAD nome-arquivo` | Tira o arquivo do stage, mantendo as alterações (forma antiga). |
| `git reset --soft HEAD^` | Desfaz o último commit e mantém as mudanças no stage. |
| `git reset --hard HEAD^` | Desfaz o último commit e **descarta** as mudanças. Use com cuidado. |
| `git revert nome-hash` | Cria um novo commit que desfaz as alterações do commit informado — seguro para histórico já publicado. |
| `git clean -n` | Lista os arquivos não rastreados que seriam removidos (simulação). |
| `git clean -dn` | Lista arquivos e diretórios não rastreados que seriam removidos. |
| `git clean -df` | Remove arquivos e diretórios não rastreados. |
| `git rm -r --cached nome-diretorio/` | Remove o arquivo/diretório do controle do Git sem apagá-lo do disco — útil após atualizar o `.gitignore`. |
| `git checkout nome-hash` | "Viaja no tempo" para um commit (detached HEAD). Para salvar alterações a partir dele, crie uma nova branch. |

## Stash

| Comando | Descrição |
| --- | --- |
| `git stash` | Guarda as modificações atuais para usar depois, limpando a working tree. |
| `git stash push -m "mensagem"` | Guarda as modificações com uma mensagem de contexto (substitui o antigo `git stash save`). |
| `git stash list` | Lista os stashes salvos. |
| `git stash apply stash@{n}` | Aplica as modificações do stash indicado, mantendo-o na lista. |
| `git stash pop` | Aplica o stash mais recente e o remove da lista. |
| `git stash drop stash@{n}` | Remove o stash indicado da lista. |
| `git stash clear` | Remove todos os stashes. |

## Tags e versões

| Comando | Descrição |
| --- | --- |
| `git tag -a v0.1.0 -m "Lançando a primeira versão."` | Cria uma tag anotada — um ponto fixo no histórico que não deve mais ser modificado. |
| `git tag` | Lista as tags. |
| `git push origin v0.1.0` | Envia a tag para o repositório remoto. |
| `git push origin --tags` | Envia todas as tags para o repositório remoto. |

## Comandos avançados

| Comando | Descrição |
| --- | --- |
| `git bisect start`<br>`git bisect good nome-hash`<br>`git bisect bad nome-hash`<br>`git bisect reset` | Encontra o commit que quebrou o projeto por busca binária: você indica um commit bom (`good`) e um ruim (`bad`), o Git faz checkouts intermediários e você vai classificando cada um até ele apontar o commit culpado. |
| `git gc --prune=now` | Otimiza o repositório removendo objetos soltos. Resolve erros como `unable to resolve reference` ou `unable to update local ref` no pull. |

## .gitignore

O arquivo `.gitignore`, criado na raiz do repositório, define arquivos e diretórios que o Git **não** deve monitorar (dependências, builds, arquivos de ambiente etc.).

```gitignore
node_modules/
dist/
.env
*.log
```

> Se o arquivo já estava sendo rastreado antes de entrar no `.gitignore`, use `git rm -r --cached nome-arquivo` para removê-lo do controle do Git.

## Links úteis

- [Visualizing Git](https://git-school.github.io/visualizing-git/) — simulador visual de comandos Git.
- [Pro Git Book](https://git-scm.com/book/en/v2) — livro oficial, gratuito e completo.
- [GitHub Skills](https://skills.github.com/) — cursos interativos oficiais do GitHub.
- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) — convenção para mensagens de commit.
- [GitHub Docs — Conectar-se ao GitHub com SSH](https://docs.github.com/pt/authentication/connecting-to-github-with-ssh)
- [git log cheatsheet](https://devhints.io/git-log) — personalização da busca de logs.

## Licença

Este projeto está sob a licença [MIT](LICENSE).
