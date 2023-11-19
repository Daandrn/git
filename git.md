-------------------------------------------------------------
- Configuração do Git

git config --global user.name "Seu Nome" \\ Configura o nome de usuário global.
git config --global user.email "seu-email@example.com" \\ Configura o e-mail do usuário global.
git config --list \\ Lista todas as configurações.

-------------------------------------------------------------
- Iniciar um Repositório

git init \\ Inicia um novo repositório.

-------------------------------------------------------------
- Clonar um Repositório Existente

git clone <URL> \\ Clona um repositório existente.

-------------------------------------------------------------
- Básico de Commits

git add <arquivo> \\ Adiciona um arquivo ao próximo commit.
git add . ou git add --all \\ Adiciona todos os arquivos ao próximo commit.
git commit -m "Mensagem do commit" \\ Realiza um commit com uma mensagem descritiva.

-------------------------------------------------------------
- Visualização e Status

git status \\ Mostra o status do repositório.
git log \\ Mostra o histórico de commits.
git diff \\ Mostra as diferenças entre os arquivos modificados e os commits.

-------------------------------------------------------------
- Branches 

git branch \\ Lista todas as branches no repositório.
git branch <nome-da-branch> \\ Cria uma nova branch.
git checkout <nome-da-branch> \\ Muda para uma branch específica.
git merge <nome-da-branch> \\ Faz o merge de uma branch na branch atual.
git branch -d <nome-da-branch> \\ Deleta uma branch.

-------------------------------------------------------------
- Atualizações Remotas

git remote -v \\ Mostra os repositórios remotos configurados.
git pull origin <branch> \\ Puxa as alterações do repositório remoto para a branch local.
git push origin <branch> \\ Empurra as alterações da branch local para o repositório remoto.

-------------------------------------------------------------
- Resolução de Conflitos

git merge \\ Realiza o merge de branches.
git mergetool \\ Abre uma ferramenta para ajudar na resolução de conflitos.

-------------------------------------------------------------
- Desfazendo Alterações

git reset <arquivo> \\ Remove um arquivo da área de stage.
git reset --hard HEAD \\ Desfaz todas as alterações locais.
git revert <hash-do-commit> \\ Desfaz um commit específico.

-------------------------------------------------------------
- Tags

git tag -a <tag> -m "Mensagem" \\ Cria uma tag anotada.

-------------------------------------------------------------
- Stash

git stash \\ Salva as alterações locais temporariamente.
git stash list \\ Lista todas as stashes.
git stash apply \\ Aplica a última stash.
git stash drop \\ Remove a última stash.

-------------------------------------------------------------
- Gitignore 

Crie um arquivo chamado .gitignore para listar os arquivos e diretórios que você deseja ignorar.

-------------------------------------------------------------
- Submódulos 

git submodule add <URL> \\ Adiciona um submódulo ao seu repositório.
git submodule update --init --recursive \\ Inicializa e atualiza os submódulos.

-------------------------------------------------------------
- Rebase

git rebase <branch> \\ Reorganiza os commits para que a branch atual tenha os últimos commits da branch especificada.

-------------------------------------------------------------
- Cherry Pick 

git cherry-pick <hash-do-commit> \\ Aplica um commit específico em sua branch atual.

-------------------------------------------------------------
- Reflog 

git reflog \\ Mostra um registro de todas as ações realizadas no repositório.

-------------------------------------------------------------
- Git Bisect \\ Ajuda a encontrar um commit específico que introduziu um problema.

git bisect start
git bisect bad          # Indica o commit atual como ruim
git bisect good <hash>  # Indica um commit conhecido como bom
git bisect reset        # Completa o processo

-------------------------------------------------------------
- Trabalhando com Refs 

git show-ref \\ Exibe referências (refs), como branches e tags.
git update-ref \\ Atualiza referências diretamente.

-------------------------------------------------------------
- Bisect Automático

git bisect start <ruim> <bom> \\ Inicia automaticamente o processo bisect.
git bisect run <script> \\ Automatiza a busca usando um script para determinar se um commit é bom ou ruim.

-------------------------------------------------------------
- Bundler (para Projetos Ruby) 

bundle exec <comando> \\ Executa um comando usando as gemas (dependências) do projeto.

-------------------------------------------------------------
- Git LFS (Large File Storage)

Extensão do Git para lidar com arquivos grandes.
git lfs track "*.ext" \\ Configura arquivos específicos para serem tratados pelo Git LFS.

-------------------------------------------------------------
- Git Worktree

git worktree add <diretório> <branch> \\ Cria uma nova cópia de trabalho ligada a uma branch existente.

-------------------------------------------------------------
- Aliases 

git config --global alias.<alias-name> "<git-command>" \\ Cria um alias para um comando Git.

-------------------------------------------------------------
- Git Cherry 

git cherry -v <upstream-branch> \\ Mostra os commits que estão na branch local, mas não na branch upstream.

-------------------------------------------------------------
- Git Archive 

git archive --format=<formato> --output=<arquivo> <branch> \\ Cria um arquivo a partir de uma branch.

-------------------------------------------------------------
- Git Bisect Skip 

git bisect skip \\ Pula o commit atual durante o processo bisect.

-------------------------------------------------------------
- Restaurar Arquivo Deletado

git checkout <hash-do-commit> -- <caminho-do-arquivo> \\ Restaura um arquivo deletado de um commit específico.

-------------------------------------------------------------
- Desabilitar o Git Pager (pager off) 

git --no-pager <comando> \\ Executa um comando Git sem usar o paginador.

-------------------------------------------------------------
- Analisar Dependências do Composer 

composer show --all \\ Lista todas as dependências do Composer instaladas no projeto.

-------------------------------------------------------------
- Reescrever Histórico (Interativamente) 

git rebase -i <commit> \\ Permite reescrever o histórico interativamente, como reorganizar, editar ou mesclar commits.

-------------------------------------------------------------
- Logs Decorados

git log --graph --oneline --decorate --all \\ Exibe um log decorado com informações visuais sobre as branches.

-------------------------------------------------------------
- Listar Tags Remotas 

git ls-remote --tags origin \\ Lista todas as tags remotas.

-------------------------------------------------------------
- Forçar Push

git push origin <branch> --force \\ Força o push para uma branch remota, substituindo o histórico remoto.

-------------------------------------------------------------
- Limpar Histórico Local (Squash)

git reset --soft HEAD~<n> \\ Desfaz os últimos n commits mantendo as alterações no staged.
git commit -m "Novo commit" \\ Cria um novo commit com as alterações agrupadas.

-------------------------------------------------------------
- Ignorar Alterações Locais

git checkout -- <arquivo> \\ Descarta as alterações locais em um arquivo específico.

-------------------------------------------------------------
- Git Bisect Reset

git bisect reset \\ Completa o processo bisect e retorna ao estado original.

-------------------------------------------------------------
- Hooks Personalizados 

Configure scripts personalizados nos diretórios .git/hooks/ para acionar em eventos específicos.

-------------------------------------------------------------
- Atualizar Todas as Branches Remotas

git fetch --all \\ Atualiza as referências para todas as branches remotas.

-------------------------------------------------------------
- Git Stash Pop

git stash pop \\ Aplica e remove a última stash automaticamente.

-------------------------------------------------------------
- Visualizar Diferenças de Arquivo entre Branches 

git diff <branch-origem>..<branch-destino> -- <arquivo> \\ Mostra as diferenças de um arquivo entre duas branches.

-------------------------------------------------------------
- Desabilitar Cores no Git

git config --global color.ui false \\ Desativa as cores nas saídas do Git.

-------------------------------------------------------------
- Log Gráfico com Datas Relativas 

git log --graph --oneline --decorate --all --relative-date \\ Exibe um log gráfico com datas relativas.

-------------------------------------------------------------
- Renomear um Branch Local e Remoto 

git branch -m <novo-nome> \\ Renomeia a branch local.
git push origin  \\<antigo-nome> \\ Deleta a branch remota antiga.
git push origin <novo-nome> \\ Empurra a nova branch remota.

-------------------------------------------------------------
- Ignorar Submódulos em Diferenças 

git diff --submodule=diff \\ Ignora diferenças em submódulos ao visualizar alterações.

-------------------------------------------------------------
- Ferramentas Gráficas 

Utilize ferramentas gráficas como gitk, git-gui ou outras de terceiros para visualização de histórico e manipulação.

-------------------------------------------------------------
- Trabalhar com Git LFS 

git lfs install \\ Instala o Git LFS no repositório.

-------------------------------------------------------------
- Git Show 

git show <hash-do-commit> \\ Exibe detalhes específicos de um commit.

-------------------------------------------------------------
- Desfazer o último Commit sem Perder Alterações 

git reset HEAD~1 \\ Desfaz o último commit, mantendo as alterações no working directory.

-------------------------------------------------------------
- Acessar o Histórico de um Arquivo 

git log --follow -- <arquivo> \\ Visualiza o histórico de um arquivo, mesmo após ser renomeado.