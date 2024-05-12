# Curso de Git e Github

## Anotações pessoais

### Comandos iniciais

### Configuração inicial do repositório local

* Definindo o nome do usuário: git config --global user.name "Hellano0209"
* Definindo e-mail do usuário:  git config --global user.email hellano.vda@gmail.com
* Definindo a Branch padrão: git config --global init.defaultBranch main
* Retornando as configurações globais: git config --global --list

### Criando um repositório local

* Inicializando repositório git: **git init**
* Conectando repositório local com remoto: **git remote add origin url_do_repositorio.git**
* Clonando um repositório: **git clone url_do_repositório.git**
* Verificando status da árvore de trabalho: **git status**

### Salvando alterações no repositório

* Adiciona o conteúdo na árvore de trabalho (para inserir no commit): **git add arquivo_para_adicionar**
* Criar um commit: **git commit -m "mensagem descritiva do commit"**
* Identificando o commit: **git log**

### Desfazendo alterações

* voltando para o último estado do um arquivo: **git restore**
* Desfazer a mensagem descritiva do commit: **git commit--amend -m "nova_mensagem"**
* Desfazer o commit anterior:  **git reset --soft id_commit**
* Desfazer o commit anterior e adiciona na árvore de trabalho: git reset --mixed id_commit**
* Desfazer e ignorar o commit anterior: **git reset --hard id_commit**

### Enviando e puxando alterações para repositório remoto

* git remote add origin url_do_repositorio.git
* Enviando do repositório local para remoto: **git push -u origin main**
* Puxando do repositório remoto para local: **git pull**