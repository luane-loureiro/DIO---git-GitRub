# DIO | Resumos Git e GitHub

repositorio para armazenar resumo sobre git e gitHubdo curso de versionamento da [DIO](https://www.dio.me)

## 📑 documentação
- [documentação Git](https://git-scm.com/doc)
- [documentação GitHub](https://docs.github.com)

## 🖥️ Resumos das Aulas

| Aulas | Resumos |
|-------|---------|
| Aula 1 | [Resumo]() |
| Aula 2 | [Resumo]() |


## 📟 Codigos do Terminal

### Criando e Clonando Repositórios
Existem duas formas de obter um repositório Git na sua máquina:
1. Transformando um diretório local que não está sob controle de versão, num repositório Git;
2. Clonando um repositório Git existente.

#### Criando um Repositório Local
Acesse a pasta que deseja transformar em um repositório Git  pelo terminal ou clique no atalho em “Git Bash Here”:
1. Inicialize um repositório Git no diretório escolhido:
    ```bash
    $ git init
    ```
2. Conecte o repositório local com o repositório remoto:
    ```bash
    $ git remote add origin https://github.com/username/nome-do-repositorio.git
    ```

#### Clonando um repositorio do gitHub
1. Abra o repositorio q deseja clonar no gitHub, e copie o godigo http.
2. cesse a pasta que deseja que o arquivo clonado fique, pelo terminal ou clique no atalho em “Git Bash Here”:
    ```bash
    $ git clone https://github.com/username/nome-do-repositorio.git
    ```
### Verificando os Status de Seus Arquivos
A principal ferramenta que você vai usar para determinar quais arquivos estão em qual estado é o comando git status. Se você executar esse comando imediatamente após clonar um repositório, você vai ver algo assim:
```bash
$ git status
```

### Rastreando Arquivos Novos
Para começar a rastrear um novo arquivo, você deve usar o comando git add. 
Quando vc usa o comando git add você adiciona um arquivo no "stage", onde ele esta na "fila" para entar no proximo commit.
Para começar a rastrear o arquivo README, você deve executar o seguinte:
```
$ git add README
```
### Retirando um arquivo do Stage ( saindo da fila )
para retirar o arquivo do stage vamos usar o comando git reset HEAD + nome do aquivo que quer remover do stage, como por exemplo:
```bash
git reset HEAD README.md
```


### Fazendo Commit das Suas Alterações
Agora que sua área de stage está preparada do jeito que você quer, você pode fazer commit das suas alterações e junto com o comando -m coloca uma mensagem sobre a versão do commit.
```
$ git commit -m"mensagem de atualização do comit"
```

### Desfazendo Alterações no Repositório Local

#### Como alterar a mensagem do último commit
```bash
$ git commit --amend
```

Alterando a mensagem sem abrir o editor:  
```bash
$ git commit --amend –m"nova mensagem"
```

#### Como desfazer um commit
```bash
$ git reset
```
```bash
$ git reset --soft
```
```bash
$ git reset --mixed
```
```bash
$ git reset --hard
```
### Listando os comits Feitos
Por padrão, sem argumentos, git log lista os commits feitos neste repositório em ordem cronológica inversa; isto é, o commit mais recente aparece primeiro.
```bash
$ git log
```
### Trabalhando com repositórios remotos
#### enviando arquivos para seu repositório remoto
Quando você tem seu projeto em um ponto que deseja compartilhar, é necessário enviá-lo para o servidor remoto. O comando para isso é simples: git push
```bash
$ git push origin master
```
#### recebendo aqrquivow do reposit[orio remoto


## 🔎 Referências
- [DIO](www.dio.mr)
