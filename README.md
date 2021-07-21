<h3 align="center">
  <a href="https://git-scm.com/">Git</a> e <a href="https://github.com/">GitHub</a>: Controle e Compartilhe seu Código
</h3>

<table>
  
  <tr>
    <th>Comando:</th>
    <th>Descrição:</th>
  </tr>
 
  <tr>
    <td>git config --local user.name "Seu nome"</td>
    <td>Define o nome localmente.</td>
  </tr>
  
  <tr>
    <td>git config --local user.email "Seu e-mail"</td>
    <td>Define o endereço de e-mail localmente.</td>
  </tr>
  
  <tr>
    <td>git config --global user.name "Seu nome"</td>
    <td>Define o nome globalmente.</td>
  </tr>
  
  <tr>
    <td>git config --global user.email "Seu e-mail"</td>
    <td>Define o endereço de e-mail globalmente.</td>
  </tr>
  
  <tr>
    <td>git config --global --list</td>
    <td>Lista as configurações globais.</td>
  </tr>
  
  <tr>
    <td>git config --global core.editor "code --wait"</td>
    <td>Define o Visual Studio Code como editor padrão.</td>
  </tr>
  
  <tr>
    <td>git config --global core.editor "vim"</td>
    <td>Define o vim como editor padrão.</td>
  </tr>
  
  <tr>
    <td>git config --global --unset core.editor</td>
    <td>Volta para o editor padrão.</td>
  </tr>
  
  <tr>
    <td>git init</td>
    <td>Cria um repositório Git.</td>
  </tr>
  
  <tr>
    <td>git status</td>
    <td>Analisa o estado do repositório.</td>
  </tr>
  
  <tr>
    <td>git add nomeDoArquivo</td>
    <td>Marcar o arquivo para ser salvo (commitado).</td>
  </tr>
  
  <tr>
    <td>git add .</td>
    <td>Marcar todos os arquivos para serem salvos (commitados).</td>
  </tr>
  
  <tr>
    <td>git commit -m "Mensagem"</td>
    <td>Realiza o commit.</td>
  </tr>
  
  <tr>
    <td>git log --oneline</td>
    <td>Lista os logs em linhas de forma mais limpa.</td>
  </tr>
  
  <tr>
    <td>git log -p</td>
    <td>Lista os logs com mais detalhes, mostrando o que aconteceu no projeto.</td>
  </tr>
  
  <tr>
    <td>git log --graph --oneline --all</td>
    <td>Todos os logs super detalhados.</td>
  </tr>
   
  <tr>
    <td>git log --help</td>
    <td>Ver algumas opções disponíveis.</td>
  </tr>
  
  <tr>
    <td><a href="https://devhints.io/git-log">git log cheatsheet</a></td>
    <td>Comandos para personalizar a busca de logs.</td>
  </tr>
  
  <tr>
    <td>gitk</td>
    <td>Visualizador de histórico gráfico.</td>
  </tr>
  
  <tr>
    <td>git init --bare</td>
    <td>Cria um repositório que não terá a working tree, ou seja, não conterá uma cópia dos arquivos. Como o repositório servirá apenas como servidor, para que outros membros da equipe sincronizem seus trabalhos, poupa espaço de armazenamento desta forma.</td>
  </tr>
  
  <tr>
    <td>git remote add nome-repositorio caminho/para/o/repositorio</td>
    <td>Desta forma teremos um link do repositório local com o repositório remoto, que chamamos de nome-repositorio, que está armazenado em caminho/para/o/repositorio.</td>
  </tr>
  
  <tr>
    <td>git remote</td>
    <td>Lista os remotes.</td>
  </tr>
  
  <tr>
    <td>git remote -v</td>
    <td>Lista os nomes e endereços.</td>
  </tr>
  
  <tr>
    <td>git remote rename nome-atual novo-nome</td>
    <td>Renomea o remote.</td>
  </tr>
  
  <tr>
    <td>git clone url nome</td>
    <td>Baixa o repositório localmente. Nome é opcional caso queira definir um nome diferente do original.</td>
  </tr>
  
  <tr>
    <td>git push origin main</td>
    <td>Envia os dados para o repositório remoto. Se utilizar git push -u origin main ficará salvo e na próxima vez rodar somente: git push.</td>
  </tr>
  
  <tr>
    <td>git pull</td>
    <td>Atualiza as informações do repositório local.</td>
  </tr>
  
  <tr>
    <td>GitHub: git remote add origin https://github.com/lucasrmagalhaes/projeto.git</td>
    <td>Adiciona o repositório remoto no diretório local.</td>
  </tr>
  
  <tr>
    <td>git branch nome-branch</td>
    <td>Cria uma branch.</td>
  </tr>
  
  <tr>
    <td>git branch</td>
    <td>Lista as branches.</td>
  </tr>
  
  <tr>
    <td>git checkout nome-branch</td>
    <td>Muda de branch.</td>
  </tr>
  
  <tr>
    <td>git switch nome-branch</td>
    <td>Muda de branch.</td>
  </tr>
  
  <tr>
    <td>git checkout -b nome-branch</td>
    <td>Cria e entra na branch.</td>
  </tr>
  
  <tr>
    <td>git branch -m novo-nome</td>
    <td>Renomeia a branch, se estiver dentro dela.</td>
  </tr>
  
  <tr>
    <td>git branch -m nome-atual novo-nome</td>
    <td>Renomeia a branch, dentro de outra branch.</td>
  </tr>
  
  <tr>
    <td>git branch -d nome-branch</td>
    <td>Deleta a branch.</td>
  </tr>
  
  <tr>
    <td>git merge nome-branch-secundaria</td>
    <td>Caso tenha commits fora da branch principal e ocorreu um BUG na branch principal. Acessar a branch principal, corrigir o erro e rodar o comando.</td>
  </tr>
  
  <tr>
    <td>git rebase nome-branch-secundaria</td>
    <td>O merge junta os trabalhos e gera um merge commit. O rebase aplica os commits de outra branch na branch atual.</td>
  </tr>
  
  <tr>
    <td>git checkout -- nome-arquivo</td>
    <td>Descarta alterações de em arquivo.</td>
  </tr>

  <tr>
    <td>git reset HEAD index.html</td>
    <td>Desmarcar o arquivo para ser commitado.</td>
  </tr>
  
  <tr>
    <td>git reset HEAD~1</td>
    <td>Desfaz o último commit e não remove as alterações no arquivo.</td>
  </tr>
  
  <tr>
    <td>git revert nome-hash</td>
    <td>Remove as alterações no código do commit.</td>
  </tr>
  
  <tr>
    <td>git stash</td>
    <td>Salva os dados modificados para depois.</td>
  </tr>
  
  <tr>
    <td>git stash save "mensagem"</td>
    <td>Salva os dados modificados para depois com contexto.</td>
  </tr>
  
  <tr>
    <td>git stash list</td>
    <td>Lista os estados salvos.</td>
  </tr>
  
  <tr>
    <td>git stash clear</td>
    <td>Limpa os estados.</td>
  </tr>
  
  <tr>
    <td>git stash apply numero-array</td>
    <td>Aplica as modificações.</td>
  </tr>
  
  <tr>
    <td>git stash drop numero-array</td>
    <td>Remove as modificações.</td>
  </tr>
  
  <tr>
    <td>git stash pop numero-array</td>
    <td>Aplica e remove do stash.</td>
  </tr>

  <tr>
    <td>git checkout nome-hash</td>
    <td>Viajando no tempo. Não é possível editar e salvar, apenas se criar uma nova branch ou entrar dentro da master.</td>
  </tr>

  <tr>
    <td>git diff nome-commit..nome-commit</td>
    <td>Mostra as diferenças entre dois commits.</td>
  </tr>
  
  <tr>
    <td>git diff</td>
    <td>Mostra o que foi alterado e o que ainda não foi adicionado para ser commitado.</td>
  </tr>
  
  <tr>
    <td>git tag -a versao-0.1.0 -m "Lançando a primeira versão."</td>
    <td>Cria um ponto que não pode ser mais modificado.</td>
  </tr>
  
  <tr>
    <td>git tag</td>
    <td>Lista as versões.</td>
  </tr>
  
  <tr>
    <td>git push origin main versao-0.1.0</td>
    <td>Subindo a versão.</td>
  </tr>
  
   <tr>
    <td>git config --global init.defaultBranch main</td>
    <td>Configurando o git para iniciar sempre com a branch main ao invés da master (git init). A partir da versão 2.28.</td>
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
