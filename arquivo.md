# Comandos básicos no Git:
**Para criar um arquivo de texto dentro do repositório**

touch nomedoarquivo.md ou nomedoarquivo.txt;
Para salvar esse arquivo:
esc + :w

**Para salvar e sair:**

esc + :wq
Somente sair:
esc +:q



### Para configurações como nome e e-mail:

**Para listar configurações:**

git config --global --list

> **limpando as configurações anteriores:**
> git config --global --unset user.email"meuemail@gmail.com"
> git config --global --unset user.name"Meu Nome"
> git config --global --unset user.nickname"meu-apelido"

> **Configurando:**
> git config --global --user.email"meuemail@gmail.com"
> git config --global --user.name "Meu Nome"
> git config --global --user.nickname"meu-apelido"

**Configurando a cores de interação:**
git config --global color.ui.true





**Criando um diretório:**
mkdir nomedapasta

**Para acessar o diretório:**
cd nomedapasta/

**Para criar um novo repositório:**

git init (cria o diretório .git)

## Estágios do Git:

**mostra a situação do meu arquivo**

git status 

se estiver como untracked (primeiro estágio)

**para preparar para commitar**

git add nomedoarquivo.txt

aparece  **Changes to be committed** (segundo estágio e pronto para ser comitado quando ele **entra para o controle de versão e recebe um *hash* **)

se quiser voltar para unstage, ou seja, para o primeiro estágio untracked:

 git rm --cached nomedoarquivo.txt

**Para commitar de fato o arquivo ou diretório:**

git commit -m "Escreva aqui a mensagem inicial do seu commit"
e agora ele está comitado e no **stage** (já faz parte do controle de versão)










