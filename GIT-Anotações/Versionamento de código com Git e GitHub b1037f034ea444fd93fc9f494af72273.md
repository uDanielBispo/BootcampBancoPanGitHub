[link do curso](https://web.dio.me/course/versionamento-de-codigo-com-git-e-github/learning/b2ceffed-9d18-4369-a038-e72be0953455)

# Versionamento de código com Git e GitHub

Basicamente versionamento é quando se tem um arquivo onde varias pessoas podem mexer e as atualizações de cada não serão perdidas

## Tipos de Sistemas de controle de versão:

[VCS Centralizado (CVCS)](https://github.com/uDanielBispo/BootcampBancoPanGitHub/blob/main/GIT-Anota%C3%A7%C3%B5es/Versionamento%20de%20co%CC%81digo%20com%20Git%20e%20GitHub%20b1037f034ea444fd93fc9f494af72273/VCS%20Distribui%CC%81do%20(DVCS)%205d22a8e3f7c54c2da0cd0daea9b5c753.md)

[VCS Distribuído (DVCS)](https://github.com/uDanielBispo/BootcampBancoPanGitHub/blob/main/GIT-Anota%C3%A7%C3%B5es/Versionamento%20de%20co%CC%81digo%20com%20Git%20e%20GitHub%20b1037f034ea444fd93fc9f494af72273/VCS%20Centralizado%20(CVCS)%2063fe0a25a5e04f7b97d758b8046529f3.md)

## O ******Git****** é um sistema de controle de vesão distribuido

[Fluxo básico no Git](https://github.com/uDanielBispo/BootcampBancoPanGitHub/blob/main/GIT-Anota%C3%A7%C3%B5es/Versionamento%20de%20co%CC%81digo%20com%20Git%20e%20GitHub%20b1037f034ea444fd93fc9f494af72273/Fluxo%20ba%CC%81sico%20no%20Git%20c0a9b85e59794d37b7b3b1b32db40e02.md)

O ********GitHub******** é uma plataforma de hospedagem de códiogo para controle de versão com ********Git********, e colaboração.

## Autenticação de opearções Git:

**Token de acesso pessoal** - É uma senha aleatória gerada para que você possa colaborar no seu repositório, evita que você utilize sua senha pessoal do git

[**SSH** ](https://github.com/uDanielBispo/BootcampBancoPanGitHub/blob/main/GIT-Anota%C3%A7%C3%B5es/Versionamento%20de%20co%CC%81digo%20com%20Git%20e%20GitHub%20b1037f034ea444fd93fc9f494af72273/SSH%20a4385154207f42bd824adbd7c846838a.md)

### Recuperando versão

```bash
GIT RESTORE nomearquivo.ext
```

Esse código recupera a ultima versão e descarta as alterações antes feitas.

### Corrigindo a última mensagem de commit

```bash
GIT COMMIT --AMEND -M "Corrige commit"
```

### Restaurando commit anterior

```bash
git reset --soft hash do commit
```

### Forma diferente de criar repositório

Você pode anexar um repositório remoto a um repositório local sem precisar fazer o comando ********************git clone******************** 

Exemplo:

Abra o terminal em um diretório

```bash
mkdir diretorio
cd diretorio
git init
git add origin URL
```

Após isso você poderá realizar o **git push**

## **Trabalhando com Branches - Criando, Mesclando, Deletando e Tratando Conflitos**

Criando uma branch:

```bash
git checkout -b nomeBranch
```

A partir desse momento, ao commitar novamente, a **branch** tomará seu próprio rumo e apontará sozinha para os outros commits, enquanto a **main** ficará apontando para o ultimo commit

```bash
git checkout main **// para voltar basta realizar**
git branch -v **// mostra os ultimos commits de cada branch**
git branch **//** ******************************************************************************para descobrir todas as branchs criadas******************************************************************************
git merge branchName **// para mesclar as branchs faça**
git branch -d branchName ******************// para excluir branch******************
git pull = git feth + git merge
git diff branch1 branch2 
git stash ******// arquiva sua alteração que voce não deseja levar para a main******
```

Recomendação de leitura 3.branching

[Git - Book](https://git-scm.com/book/en/v2)

[https://github.com/elidianaandrade/dio-curso-git-github](https://github.com/elidianaandrade/dio-curso-git-github)