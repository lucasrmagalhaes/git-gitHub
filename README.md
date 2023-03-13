<h3 align="center">
  <a href="https://git-scm.com/">Git</a> e <a href="https://github.com/">GitHub</a>: Controle e Compartilhe seu Código
</h3>

<p align="center">
  <a href="https://github.com/lucasrmagalhaes/git-gitHub/issues">
    <img src="https://img.shields.io/github/issues/lucasrmagalhaes/git-gitHub" /> 
  </a>
    
  <a href="https://github.com/lucasrmagalhaes/git-gitHub/network/members">
    <img src="https://img.shields.io/github/forks/lucasrmagalhaes/git-gitHub" /> 
  </a>
    
  <a href="https://github.com/lucasrmagalhaes/git-gitHub/stargazers">
    <img src="https://img.shields.io/github/stars/lucasrmagalhaes/git-gitHub" /> 
  </a>
  
   <a href="https://github.com/lucasrmagalhaes/git-gitHub/blob/master/LICENSE">
    <img src="https://img.shields.io/github/license/lucasrmagalhaes/git-gitHub" /> 
  </a>
</p>

<table>
  
  <tr>
    <th>Comando:</th>
    <th>Descrição:</th>
  </tr>
 
  <tr>
    <td><code>git config --local user.name "Seu nome"</code></td>
    <td>Define o nome localmente.</td>
  </tr>
  
  <tr>
    <td><code>git config --local user.email "Seu e-mail"</code></td>
    <td>Define o endereço de e-mail localmente.</td>
  </tr>
  
  <tr>
    <td><code>git config --global user.name "Seu nome"</code></td>
    <td>Define o nome globalmente.</td>
  </tr>
  
  <tr>
    <td><code>git config --global user.email "Seu e-mail"</code></td>
    <td>Define o endereço de e-mail globalmente.</td>
  </tr>
  
  <tr>
    <td><code>git config --global --list</code></td>
    <td>Lista as configurações globais.</td>
  </tr>
  
  <tr>
    <td><code>git config --global core.editor "code --wait"</code></td>
    <td>Define o Visual Studio Code como editor padrão.</td>
  </tr>
  
  <tr>
    <td><code>git config --global core.editor "vim"</code></td>
    <td>Define o vim como editor padrão.</td>
  </tr>
  
  <tr>
    <td><code>git config --global --unset core.editor</code></td>
    <td>Volta para o editor padrão.</td>
  </tr>
  
  <tr>
    <td><code>git config --global init.defaultBranch main</code></td>
    <td>Configurando o git para iniciar sempre com a branch main ao invés da master (git init). A partir da versão 2.28.</td>
  </tr>

   <tr>
    <td><code>git config --global core.excludesfile nome-arquivo</code></td>
    <td>Arquivo global ignorado.</td>
  </tr>
  
  <tr>
    <td><code>git init</code></td>
    <td>Inicializa um repositório Git local.</td>
  </tr>
  
  <tr>
    <td><code>git init --bare</code></td>
    <td>Cria um repositório que não terá a working tree, ou seja, não conterá uma cópia dos arquivos. Como o repositório servirá apenas como servidor, para que outros membros da equipe sincronizem seus trabalhos, poupa espaço de armazenamento desta forma.</td>
  </tr>
  
  <tr>
    <td><code>git status</code></td>
    <td>Analisa o estado do repositório.</td>
  </tr>
  
  <tr>
    <td><code>git add nomeDoArquivo<code></td>
    <td>Marcar o arquivo para ser salvo (commitado).</td>
  </tr>
  
  <tr>
    <td><code>git add .</code></td>
    <td>Coloca todos arquivos (novos, modificados e removidos) no index/stage. Usando o ponto, será adicionado ao stagging somente os arquivos a partir do diretório que você está, e os sub-diretórios deste.</td>
  </tr>
  
  <tr>
    <td><code>git add --all</code></td>
    <td>Coloca todos arquivos (novos, modificados e removidos) no index/stage. Adiciona ao staging arquivos desde a raiz do repositório passando por todos os subdiretórios, e aqui está a diferença, não importa se você está na raiz ou no sub-diretório.</td>
  </tr>

  <tr>
    <td><code>git mv nome-arquivo novo-nome-arquivo</code></td>
    <td>Renomeia o arquivo.</td>
  </tr>
  
  <tr>
    <td><code>git rm nome-arquivo</code></td>
    <td>Deleta o arquivo.</td>
  </tr>

  <tr>
    <td><code>git commit -m "Mensagem"</code></td>
    <td>Realiza o commit com o título.</td>
  </tr>
  
  <tr>
    <td><code>git commit -m "Mensagem" -m "Descrição"</code></td>
    <td>Realiza o commit com o título e descrição.</td>
  </tr>
  
  <tr>
    <td><code>git commit -a -m "Mensagem"</code></td>
    <td>Adiciona todos os arquivos e realiza o commit.</td>
  </tr>
  
  <tr>
    <td><code>git log --oneline</code></td>
    <td>Lista os logs em linhas de forma mais limpa.</td>
  </tr>
  
  <tr>
    <td><code>git log -p</code></td>
    <td>Lista os logs com mais detalhes, mostrando o que aconteceu no projeto.</td>
  </tr>
  
  <tr>
    <td><code>git log --graph --oneline --all</code></td>
    <td>Todos os logs super detalhados.</td>
  </tr>
   
  <tr>
    <td><code>git log --help</code></td>
    <td>Ver algumas opções disponíveis.</td>
  </tr>
  
  <tr>
    <td><a href="https://devhints.io/git-log"><code>git log cheatsheet</code></a></td>
    <td>Comandos para personalizar a busca de logs.</td>
  </tr>
  
  <tr>
    <td><code>gitk</code></td>
    <td>Visualizador de histórico gráfico.</td>
  </tr>
  
  <tr>
    <td><code>git remote</code></td>
    <td>Lista os remotes.</td>
  </tr>
  
  <tr>
    <td><code>git remote -v</code></td>
    <td>Lista os nomes e endereços.</td>
  </tr>

  <tr>
    <td><code>git remote add origin https://github.com/usuario/projeto.git</code></td>
    <td>Adiciona o repositório remoto no diretório local.</td>
  </tr>
  
  <tr>
    <td><code>git remote set-url origin https://github.com/usuario/projeto.git</code></td>
    <td>Outra maneira de adicionar o repositório remoto no diretório local.</td>
  </tr>
  
  <tr>
    <td><code>git remote remove nome-remote</code></td>
    <td>Remove o remote.</td>
  </tr>
  
  <tr>
    <td><code>git remote rename nome-atual novo-nome</code></td>
    <td>Renomeia o remote.</td>
  </tr>
  
  <tr>
    <td><code>git clone url nome</code></td>
    <td>Baixa o repositório localmente. Nome é opcional caso queira definir um nome diferente do original.</td>
  </tr>
  
  <tr>
    <td><code>git clone -b nome-branch repositorio-remoto-url</code></td>
    <td>Baixa o repositório localmente em um branch específico.</td>
  </tr>
  
  <tr>
    <td><code>git clone --branch nome-branch repositorio-remoto-url</code></td>
    <td>Outra maneira de baixar o repositório localmente em um branch específico.</td>
  </tr>
  
  <tr>
    <td><code>git push nome-remote nome-branch</code></td>
    <td>Envia os dados para o repositório remoto. Se utilizar git push -u origin main ficará salvo e na próxima vez rodar somente: git push.</td>
  </tr>
  
  <tr>
    <td><code>git push --all</code></td>
    <td>Envia os dados de todas as branches para o repositório remoto.</td>
  </tr>
  
  <tr>
    <td><code>git fetch</code></td>
    <td>Para obter informações sobre um repositório remoto, mas não alterar nenhuma branch.</td>
  </tr>
  
  <tr>
    <td><code>git pull</code></td>
    <td>Atualiza as informações do repositório local.</td>
  </tr>
  
  <tr>
    <td><code>git branch</code></td>
    <td>Lista as branches locais.</td>
  </tr>
  
  <tr>
    <td><code>git branch -a</code></td>
    <td>Lista as branches locais e remotas.</td>
  </tr>
  
  <tr>
    <td><code>git branch nome-branch</code></td>
    <td>Cria uma branch.</td>
  </tr>
  
  <tr>
    <td><code>git checkout nome-branch</code></td>
    <td>Muda de branch.</td>
  </tr>
  
  <tr>
    <td><code>git switch nome-branch</code></td>
    <td>Muda de branch.</td>
  </tr>
  
  <tr>
    <td><code>git checkout -b nome-branch</code></td>
    <td>Copia e entra na branch.</td>
  </tr>
  
  <tr>
    <td><code>git switch -c nome-branch</code></td>
    <td>Copia e entra na branch.</td>
  </tr>
  
  <tr>
    <td><code>git checkout -</code></td>
    <td>Volta para a branch anterior sem escrever o nome.</td>
  </tr>
  
  <tr>
    <td><code>git branch -m novo-nome</code></td>
    <td>Renomeia a branch, se estiver dentro dela.</td>
  </tr>
  
  <tr>
    <td><code>git branch -m nome-atual novo-nome</code></td>
    <td>Renomeia a branch, dentro de outra branch.</td>
  </tr>
  
  <tr>
    <td><code>git branch -d nome-branch</code></td>
    <td>Deleta a branch somente sem conflitos.</td>
  </tr>

  <tr>
    <td><code>git branch -D nome-branch</code></td>
    <td>Deleta a branch com ou sem conflitos.</td>
  </tr>
  
  <tr>
    <td><code>git merge nome-branch-secundaria</code></td>
    <td>Caso tenha commits fora da branch principal e ocorreu um BUG na branch principal. Acessar a branch principal, corrigir o erro e rodar o comando.</td>
  </tr>
  
  <tr>
    <td><code>git merge --abort</code></td>
    <td>Cancelar um merge.</td>
  </tr>
  
  <tr>
    <td><code>git rebase -i --root</code></td>
    <td>Edita no terminal todos os commits. Possível alterar a ordem, combinar e etc.</td>
  </tr>
  
  <tr>
    <td><code>git rebase nome-branch-secundaria</code></td>
    <td>O merge junta os trabalhos e gera um merge commit. O rebase aplica os commits de outra branch na branch atual.</td>
  </tr>
  
  <tr>
    <td><code>git rebase -i</code></td>
    <td>Deixa o usuário editar a lista de commits para liberar.</td>
  </tr>
  
   <tr>
    <td><code>git clean -n</code></td>
    <td>Lista arquivos a serem removidos.</td>
  </tr>
  
   <tr>
    <td><code>git clean -dn</code></td>
    <td>Lista arquivos e diretórios a serem removidos.</td>
  </tr>
  
   <tr>
    <td><code>git clean -df</code></td>
    <td>Remove arquivos e diretórios.</td>
  </tr>
  
  <tr>
    <td><code>git checkout -- nome-arquivo</code></td>
    <td>Descarta alterações do arquivo.</td>
  </tr>
  
  <tr>
    <td><code>git restore nome-arquivo</code></td>
    <td>Descarta alterações do arquivo.</td>
  </tr>
  
  <tr>
    <td><code>git checkout .</code></td>
    <td>Descarta alterações de todos os arquivos.</td>
  </tr>

  <tr>
    <td><code>git restore .</code></td>
    <td>Descarta alterações de todos os arquivos.</td>
  </tr>

  <tr>
    <td><code>git reset HEAD nome-arquivo</code></td>
    <td>Desmarcar o arquivo para ser commitado.</td>
  </tr>
  
  <tr>
    <td><code>git reset --soft HEAD^</code></td>
    <td>Configura HEAD para o commit anterior e deixa as mudanças do commit desfeito no stage/index.</td>
  </tr>
  
  <tr>
    <td><code>git reset --hard HEAD^</code></td>
    <td>Configura HEAD para o commit anterior e remove as mudanças do commit desfeito.</td>
  </tr>
  
  <tr>
    <td><code>git revert nome-hash</code></td>
    <td>Remove as alterações no código do commit.</td>
  </tr>
  
  <tr>
    <td><code>git stash</code></td>
    <td>Salva os dados modificados para depois.</td>
  </tr>
  
  <tr>
    <td><code>git stash save "mensagem"</code></td>
    <td>Salva os dados modificados para depois com contexto.</td>
  </tr>
  
  <tr>
    <td><code>git stash list</code></td>
    <td>Lista os estados salvos.</td>
  </tr>
  
  <tr>
    <td><code>git stash clear</code></td>
    <td>Limpa os estados.</td>
  </tr>
  
  <tr>
    <td><code>git stash apply numero-array</code></td>
    <td>Aplica as modificações.</td>
  </tr>
  
  <tr>
    <td><code>git stash drop numero-array</code></td>
    <td>Remove as modificações.</td>
  </tr>
  
  <tr>
    <td><code>git stash pop numero-array</code></td>
    <td>Aplica e remove do stash.</td>
  </tr>

  <tr>
    <td><code>git checkout nome-hash</code></td>
    <td>Viajando no tempo. Não é possível editar e salvar, apenas se criar uma nova branch ou entrar dentro da master.</td>
  </tr>

  <tr>
    <td><code>git diff nome-commit..nome-commit</code></td>
    <td>Mostra as diferenças entre dois commits.</td>
  </tr> 
  
  <tr>
    <td><code>git rm -rf --cached nome-diretorio/</code></td>
    <td>Remove o arquivo/diretório dos arquivos monitorados.</td>
  </tr>
  
  <tr>
    <td><code>git diff</code></td>
    <td>Mostra o que foi alterado e o que ainda não foi adicionado para ser commitado.</td>
  </tr>
  
  <tr>
    <td><code>git tag -a versao-0.1.0 -m "Lançando a primeira versão."</code></td>
    <td>Cria um ponto que não pode ser mais modificado.</td>
  </tr>
  
  <tr>
    <td><code>git tag</code></td>
    <td>Lista as versões.</td>
  </tr>
  
  <tr>
    <td><code>git push origin main versao-0.1.0</code></td>
    <td>Subindo a versão.</td>
  </tr>
  
  <tr>
    <td><code>git cherry-pick id-commit</code></td>
    <td>Selecionar commit específico para trazer ao branch desejado.</td>
  </tr>
  
  <tr>
    <td>
      <code>git bisect start</code><br>
      <code>git bisect good commit</code><br>
      <code>git bisect bad commit</code><br>
      <code>git bisect reset</code>
    </td>
    <td>
      Achar um commit que quebra o build do projeto. <br>Indica um commit que contém um estado bom do seu repositório (good) e um commit que contém um estado ruim do seu repositório (bad). Com isso o git vai realizando checkouts, seguindo uma busca binária, e você pode indicar se o estado é bom ou ruim. Ao final, o git lhe diz qual commit danificou o repositório.
    </td>
  </tr>

   <tr>
    <td><code>git rm -r --cached</code></td>
    <td>Limpando o cache.</td>
  </tr>

   <tr>
    <td><code>git commit --amend</code></td>
    <td>Altera e adiciona as novas modificações no último commit com a mensagem alterada.</td>
  </tr>

   <tr>
    <td><code>git commit -am "Nova messagem de commit"</code></td>
    <td>Altera e adiciona as novas modificações no último commit com a mensagem alterada.</td>
  </tr>
  
   <tr>
    <td><code>git commit -amend --no-edit</code></td>
    <td>Altera e adiciona as novas modificações no último commit sem alterar a mensagem.</td>
  </tr>
  
   <tr>
    <td><code>git gc --prune=now</code></td>
    <td>Git pull fails "unable to resolve reference" or "unable to update local ref".</td>
  </tr>
</table>

<details>
    <summary>.gitignore</summary>
      <br />
      <p align="left">
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>Arquivo</strong>: .gitignore <br />
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Funciona para não monitorar arquivo(s) ou diretórios. <br />
      </p>
</details>

<details>
    <summary>Links</summary>
      <br />
      <ul>
        <li><a href="https://git-school.github.io/visualizing-git/">Visualizing GIT</a></li>
        <li><a href="http://git-scm.com/book/en/v2">Git Book</a></li>
        <li><a href="https://lab.github.com/">GitHub Learning Lab</a></li>
        <li><a href="https://www.conventionalcommits.org/en/v1.0.0/">Convetional Commits</a></li>
        <li><a href="https://docs.github.com/pt/github/authenticating-to-github/connecting-to-github-with-ssh">GitHub Docs - Conectar-se ao GitHub com SSH.</li>
      </ul>
</details>
