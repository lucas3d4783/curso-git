Comandos Básicos para Manipulação de Commits
git init -> inicia o repositório git
git status -> veirifica os status do repositório
git add *, ou git add ., ou git add --all -> vai adicionar todos os arquivos a um "container de modificações" para posteriormente ser salvo no repositório local com o comando commit
git commit -m "comentário" -> salva o estado atual do "container de modificações" como uma versão do repositório
git commit -am "comentário" -> adiciona todos os arquivos e da um commit
git log -> mostra o log detalhado dos commits feitos no repositório
git log --oneline -> mostra os log dos commits em uma única linha
git log --oneline --graph -> mostra graficamente o log dos commits com a descrição dos commits em um única linha
git log --graph -> mostra graficamente os commits
git branch -> verificar a brench atual
git checkout <hash do commit para onde quer ir> -> vai voltar para como os arquivos estavam naquele commit
git checkout master -> voltar para a brench master em seu último commit
git diff ->  verifica as modificações que foram feitas nos arquivos antes de realizar um commit
git reset HEAD -> vai remover as alterações adicionadas ao container com o comando "git add", assim os arquivos continuam modificados, porém não estão mais no container
git reset --hard <hash do commit> -> retornando para um commit específico e removando os últimos

Manipulando Ramificações do Repositório
git checkout -b <nome do ramo> -> vai criar um novo ramo local e por padrão você será direcionado para ele
git merge <nome do ramo que vai ser unido ao ramo atual> -> unindo um ramo específico ao ramo atual, após isso os arquivos serão adicionados porém ainda vai faltar adicionar no container e dar o commit
git merge --abort -> para abortar um merge caso não queira resolver um conflito por exemplo


Manipulando Repositório remoto
git remote -> verifica se tem um repositório remoto configurado
git push <branch remota> <branch local> -> envia os commits para o repositório remoto
git pull -> busca as altarações realizadas no repositório remoto 

