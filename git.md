------------------------------------------------------------
- Configuração do Git

git config --global user.name "Seu Nome" \\ Configura o nome de usuário global.
git config --global user.email "seu-email@example.com" \\ Configura o e-mail do usuário global.
git config --list \\ Lista todas as configurações.

------------------------------------------------------------
- Iniciar um Repositório

git init \\ Inicia um novo repositório.

---------------------------git ----------------------------------
- Básico de Commits

git add <arquivo> \\ Adiciona um arquivo ao próximo commit.
git commit -m "Mensagem do commit" \\ Realiza um commit com uma mensagem descritiva.

------------------------------------------------------------
- Visualização e Status

git status \\ Mostra o status do repositório.
git log \\ Mostra o histórico de commits.
git log -p\\ Mostra os arquivos que estão com diferenças
git diff \\ Mostra as diferenças entre os arquivos modificados e os commits.
git show <hash-do-commit>\\ Mostra dados da alteração feita no commit

------------------------------------------------------------
- Visualizar Diferenças de Arquivo entre Branches 

git diff <branch-origem>..<branch-destino> -- <arquivo> \\ Mostra as diferenças de um arquivo entre duas branches.

------------------------------------------------------------
- Branches 

git branch \\ Lista todas as branches no repositório.
git checkout <nome-da-branch> \\ Muda para uma branch específica.
git merge <nome-da-branch> \\ Faz o merge de uma branch na branch atual.

------------------------------------------------------------
- Atualizações Remotas

git remote add origin URL-DO-REPOSITORIO
git pull origin <branch> \\ Puxa as alterações do repositório remoto para a branch local.
git push origin <branch> \\ Empurra as alterações da branch local para o repositório remoto.
git push origin <branch> --force \\ Força o push para uma branch remota, substituindo o histórico remoto.
git fetch --all \\ Atualiza as referências para todas as branches remotas.

------------------------------------------------------------
- Desfazendo Alterações

git reset --soft HEAD~<n> \\ Desfaz os últimos n commits mantendo as alterações no staged.
git revert <hash-do-commit> \\ Desfaz um commit específico.

------------------------------------------------------------
- Stash

git stash \\ Salva as alterações locais temporariamente.
git stash apply \\ Aplica a última stash.

------------------------------------------------------------
- Gitignore 

Crie um arquivo chamado .gitignore para listar os arquivos e diretórios que você deseja ignorar.

------------------------------------------------------------
- Rebase

git rebase <branch> \\ Reorganiza os commits para que a branch atual tenha os últimos commits da branch especificada.

------------------------------------------------------------
- Git Cherry 

git cherry -v <upstream-branch> \\ Mostra os commits que estão na branch local, mas não na branch upstream.

------------------------------------------------------------
- Cherry Pick 

git cherry-pick <hash-do-commit> \\ Aplica um commit específico em sua branch atual.

------------------------------------------------------------
- Restaurar Arquivo Deletado

git checkout <hash-do-commit> -- <caminho-do-arquivo> \\ Restaura um arquivo deletado de um commit específico.

------------------------------------------------------------
- Reescrever Histórico (Interativamente) 

git rebase -i <commit> \\ Permite reescrever o histórico interativamente.

------------------------------------------------------------
- Limpar Histórico Local (Squash)

git reset --soft HEAD~<n> \\ Desfaz os últimos n commits mantendo as alterações no staged.

------------------------------------------------------------
- Ignorar Alterações Locais

git checkout -- <arquivo> \\ Descarta as alterações locais em um arquivo específico.

------------------------------------------------------------
- Desfazer o último Commit sem Perder Alterações 

git reset HEAD~1 \\ Desfaz o último commit, mantendo as alterações no working directory.