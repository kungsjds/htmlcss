<strong>Iniciando um git repository</strong>

1 - selecionar o caminho da pasta que deseja incluir no repositorio (cd "caminho")

2 - Executar o comando: git init

3 - Seguir a ordem de commit abaixo                                  

--------------------------------------------------------------------------------------------------

<strong>Ordem de commit:</strong>

1 - git status (para verificar alterações);

2 - git add -A (para inserir tudo no monitor do git);

3 - git commit -m "Descrição" (para dar commit no git).

Obs: git commit -am (para adicionar e dar commit, sem precisar fazer o passo 2 e depois o 3)



--------------------------------------------------------------------------------------------------

<strong>Revertendo Modificações:</strong>

git reset --?

Formas do reset:

--soft (mantém as alterações e arquivos preparados(já add) para dar commit e volta para o commit informado.)

--mixed (mantém as alterações e arquivos NÃO preparados(NÃO add) para dar commit, precisará ADD e depois dar o COMMIT, e volta para o commit informado.)

--hard (exclui todas alterações e arquivos adicionados e volta para o commit informado)

--------------------------------------------------------------------------------------------------


<strong>Trabalhando com diferentes Branchs:</strong>


<strong>Comando para criar um novo branch:</strong>

git branch (nome do novo branch)


<strong>Comando para alterar o branch atual:</strong>

git checkout (nome do branch)


--------------------------------------------------------------------------------------------------

<strong>Diferença entre arquivos</strong>


<strong>Ver o que foi alterado em todos arquivos:</strong>

git diff

<strong>Ver o nome dos arquivos que foram alterados:</strong>

git diff --name-only

<strong>Ver arquivos especificos que foram alterados:</strong>

git diff (nome do arquivo)


<strong>Voltar as alterações feitas no arquivo para uma versão anterior</strong>

git checkout (nome do branch)ou(ex."HEAD" vai voltar para uma versão dentro do branch em que está no momento) --(nome do arquivo)

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<strong>Passo para conectar ao repositório no github</strong>

1 - Gerar chaves SSH (https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent) 

    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

2 - Pegar o arquivo gerado da chave pública e arrastar para o editor de código(Ex.: VSCode) e copiar a chave;

3 - Ir em Settings no GitHub e selecionar o menu SSH and GPG Keys;

4 - Clicar em New SSH Key;

5 - Definir um título (Ex.: Jonathan Home/Work, nome do computador, etc);

6 - Ir até o repositório criado no GitHub e seguir os passos que estão lá. Resumido abaixo:

<strong>Caso já tenha o repositório criado localmente, se não, consultar no link do repositório remoto do GitHub:</strong>

git remote add origin (https gerado pelo git ao criar o repositório).


<strong>Enviando e recebendo alterações para o repositório remoto:</strong>

fetch, puxar o conteúdo que está no repositório remoto para o repositório local(no meu computador).

push, enviar os conteúdos locais para o repositório remoto, o inverso do Fetch.

Como utilizar:

git push -u origin(Destino) master(branch)  [Enviando o branch master para o repositório origin, do GitHub]

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<strong>Ignorando arquivos/pastas:</strong>

Criar na pasta onde está o repositório, um arquivo chamado .gitignore. Nele escrever os nomes dos arquivos com a extensão ou nome da pasta, que não são para aparecer no repositório. Exemplo:

nomeDoArquivo.txt

*.txt (todos arquivos .txt)

nomeDaPasta/*


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<strong>Observação:</strong>

Se no terminal, dando git log por exemplo, ou em algum momento chegar em "END" e não conseguir digitar mais, pressionar a tecla "Q". 

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
<strong>Como utilizar o revert:</strong>

Diferença entre git RESET e git REVERT

reset - irá perder tudo que foi alterado do commit que resetar.

revert - irá voltar para um commit anterior mas manterá o commit revertido disponível para voltar novamente.

Observação:

Quando faz um revert ele abre o editor que foi cadastrado na configuração do git, na instalação, com as alterações pra se quiser alterar algo ou salvar novamente. Caso não queria alterar nada, somente reverter, que é o que acontece na maioria das vezes, é só executar comc o --no-edit, como no exemplo abaixo.

git revert --no-edit


Como fazer o revert:

1 - Executar: o git log e copia o código do commit que está com problema e irá reverter;

2 - Executar o: git revert (código do commit que foi copiado) ou git revert --no-edit (código do commit que foi copiado)

O commit revertido continua no log para consulta e para retornar novamente a ele.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<strong>Comando para deletar um branch remoto:</strong>

git push origin :teste (É o mesmo formato do push normal, só incluir um ":" no começo do nome do branch, que irá deletar)

<strong>Comando para deletar um branch local:</strong>

git branch -D [nome do branch aqui]

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<strong>Puxando alterações de outras pessoas (pull)</strong>

git pull - Pegar as atualizações do repositório remoto e atualizar no repositório local

<strong>Comando para fazer o pull:</strong>

git pull origin(repositorio remoto) master(nome do branch)

<strong>Sempre fazer o pull antes do push.</strong>

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<strong>Clonando repositórios remotos</strong>

<strong>Comando para clonar um repositório remoto:</strong>

git clone [https do repositório]

Em um repositório clonado, não conseguirá fazer push pro repositório remoto. Só poderá fazer uma contribuição. O commit só é feito no repositório local.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

<strong>Contribuindo com outros repositórios (fork / pull request)</strong>

<strong>Passo para realizar o Fork de contribuição:</strong>

1 - Estando dentro do repositório no GitHub, clicar no botão "Fork", no canto superior da tela;

2 - Será criado uma copia do repositório no seu GitHub. Informando que é um fork do repositório? "...";

3 - Ir no git local e executar o comando git clone [https do seu repositório criado pelo Fork];

4 - Fazer a alteração que precisar. Executar a ordem de commit e push normalmente, verificando o nome do branch;

5 - Voltar no GitHub, no seu repositório clonado e clicar em "New pull request";

6 - Verificar se o base fork está com o nome do repositório original e o head fork com o nome do seu repositório clonado, se não, colocar nessa ordem;

7 - Clicar em "Create pull request";

8 - Colocar o comentário sobre a alteração, o que foi feito, etc. Depois é só clicar em "Create pull request".

Será enviado para o repositório original a solicitação e poderá ser aceita ou não pelo criadores do repositório.
