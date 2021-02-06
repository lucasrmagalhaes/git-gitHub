<h2 align="center">
  <a href="https://git-scm.com/">Git</a> e <a href="https://github.com/">GitHub</a>: Controle e Compartilhe seu Código
</h2>

<table>
  
  <tr>
    <th>Comando:</th>
    <th>Descrição:</th>
  </tr>
 
  <tr>
    <td>git config --local user.name "Nome da pessoa"</td>
    <td>Define o nome da pessoa.</td>
  </tr>
  
  <tr>
    <td>git config --local user.email "Nome do e-mail"</td>
    <td>Define o nome do e-mail.</td>
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
    <td>git log --help</td>
    <td>Ver algumas opções disponíveis.</td>
  </tr>
  
  <tr>
    <td><a href="https://devhints.io/git-log">git log cheatsheet</a></td>
    <td>Comandos para personalizar a busca de logs.</td>
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
    <td>git push origin master</td>
    <td>Envia os dados para o repositório remoto. Se utilizar git push -u origin master ficará salvo e na próxima vez rodar somente: git push.</td>
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
    <td>git revert hash</td>
    <td>Reverte a alteração.</td>
  </tr>
  
</table>

<p align="left">
  Arquivo: .gitignore<br />
  Funciona para não monitorar arquivo(s). 
</p>
