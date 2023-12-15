<strong>Principais comandos de Configuracao do Git </strong>

◯ git config --global user.name "[nome]"

    Configura o nome de exibicao atrelado aos commits.

◯ git config --global user.email "[endereco-de-email]"

    Configura o nome de exibicao atrelado aos commits.

---------------------------------------------------------

<strong>Criacao e Clonagem de Repositorios</strong>

◯ git init [nome-do-projeto]

    Cria e inicia um novo repositorio com base no destino aonde foi aberto. seja uma pasta terminal ou area de trabalho.

◯ git clone [url]

    Como o proprio nome ja diz. Faz um clone de um repositorio completo e pode ser feito tanto atraves da sua url quando de sua chave ssh apos configurada no disposito.

<strong>Fazendo Mudancas nos arquivos</strong>

◯ git status

    Lista todos os novos arquivos no repositorio local e as alteracoes feitas em todos os arquivos.

◯ git diff

    Mostra diferencas nos arquivos que nao foram realizadas.

◯ git add [arquivo] (arquivo singular por nome) ou [.] (todos os arquivos). obs: apenas modificados.

    Anexa o(s) arquivo na preparacao para o versionamento dos commits.

◯ git diff --staged

    Mostra a diferenca entre arquivos selecionados e a suas ultimas versoes.

◯ git reset [arquivo]

Remove os arquivos na preparacao para o versionamento dos commits, e mantem suas alteracoes.

◯ git commit -m "[mensagem descritiva]"

Salva o conteudo alterado nos arquivos em preparacao para o versionado ao historico de versao.

<strong>Alteracoes em Grupo e Diretorios</strong>

◯ git branch

Revela uma lista com todos os repositorios locais.

◯ git branch [nome-do-branch]

cria uma nova branch.

◯ git checkout [nome-do-branch]

Muda para a branch especificada e atualiza o diretorio de trabalho.

◯ git merge [branch]

Combina o trabalho feito em uma branch com a sua branch atual.

◯ git branch -d [nome-do-branch]

Exclui uma branch especifica.

<strong>Refatoramento de nomes dos arquivos</strong>

◯ git rm [arquivo]

    Remove o arquivo do diretorio de trabalho e o seleciona para remocao.

◯ git rm --cached [arquivo]

    Remove o arquivo do controle de versao, porem preserva o mesmo localmente no diretorio.

◯ git mv [arquivo-original] [arquivo-renomeado]

    Muda o nome do arquivo e o seleciona para o commit.

<strong>Supressao de Rastreamento</strong>

◯ *.log
   build/
    temp-*

    Um arquivo de texto chamado `.gitignore` suprime o versionamento acidental de arquivos e diretorios correspondentes aos padroes especificados ou seja, escondes arquivos listados.

◯ git ls-files --other --ignored --exclude-standard

    Lista todos os arquivos ignorados neste projeto.

<strong>Save de Fragmentos de Conteudo</strong>

◯ git stash

    Armazena temporariamento todos os arquivos modificados em uma especie de caixa de pandora.

◯ git stash pop

    Restaura os arquivos recentes em stash assim liberando essa caixa de pandora.

◯ git stash list

    Lista todos os conjuntos de alteracoes em stash ex: posso ter 3 caixas com conteudo dentro em stash. essa lista ira revelar.

◯ git stash drop

    Descarta a stash da mais recente para a mais antiga guardada.

<strong>Revisao de Historico</strong>

◯ git log

    Mostra o historico da branch atual.

◯ git log --follow [arquivo]

    Lista o historico de versoes (alteracoes) de um arquivo (incluso mudanca de nome).

◯ git diff [primerio-branch]...[segundo-branch]

    Mostra a diferenca de conteudo entre duas branchs.

◯ git show [commit]

    Retorna mudancas de metadata e conteudo para o commit especificado.

<strong>Desfazendo Commits</strong>

◯ git reset [commit]

    Desfaz todos os commits depois de [xxx] (nome do commit) e preserva as mudancas no arquivo local.

◯ git reset --hard [commit]

    Descarta completamente o commit e suas mudancas.

<strong>Sincronizacao de Mudancas</strong>

◯ git fetch [marcador]

    Baixa todo o historico de um marcador de repositorio.

◯ git merge [marcador]/[branch]

    Combina o marcador do branch no branch local.

◯ git push [alias] [branch]

    Realiza o envio de todos os commits versionados localmente para o GitHub.

◯ git pull

    Baixa o historico do projeto na nuvem do git hub e incorpora novas alteracoes do projeto.
