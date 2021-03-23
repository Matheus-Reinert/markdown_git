# Git e GitHub
### Controle de versão de código

O GitHub é uma plataforma web que serve como repositório de código, utilizando de recursos do GIT para que possamos centralizar nosso repositório na internet, sendo públicos ou privados. 

### Monitoramento e controle de estágios

![](Images/estagiosgit.png)

* Untracked apesar do arquivo fazer parte do projeto ele ainda não foi adicionado ao monitoramento do git.
* Tracked a partir de então o git passa a controlar as mudanças nesse arquivo, conhecido como **New file**.
* Staged neste ponto o arquivo está preparado para ser enviado ao repositório através de um commit.
* Committed é o processo de salvar as mudanças do projeto até o atual momento.
* Modified é quando ocorre uma modificação sobre um arquivo que está sendo rastreado.

### Comandos básicos

```sh
git init
```
* Inicializa o repositório .git.
----
```sh
git config user.name "Nome do usúario"
```
* Define o nome do usúario.
----
```sh
git config user.email "Email do usúario"
```
* Define o e-mail do usúario.
----
```sh
git status
```
* Verfica  o status do repositório.

![](Images/gitstatus-modified.png)

---
```sh
git add "Nome do arquivo"
git add .
```
* Adiciona o arquivo ou todos os arquivos ao repositório.

![](Images/gitadd-modified.png)

---

```sh
git commit -m "Informação sobre o que foi realizado"
```
* Salva as mudanças que ocorreram até o momento e as identifica através de uma mensagem.

![](Images/gitcommit-m.png)

---

```sh
git push
```
* Atualiza o repositório com o ultimo commit

---
# Comandos Intermediários

```sh
git log
git log --oneline
```

* Histórico de comitts

![](Images/gitlogoneline.png)

---

```sh
git checkout 
```

* Navegação por versões do projeto

----


```sh
git diff
```
* Compara alterações de arquivos

![](Images/diff.png)

---

```sh
git commit --amend -m "Texto para substituir"
```
* Substitui o ultimo commit caso escreveu algo errado

---
## Branch

Os branches permitem que você desenvolva recursos, corrija erros ou experimente com segurança novas ideias em uma área contida do seu repositório.

```sh
git branch testeBranch
git branch
git checkout testeBranch
```

![](Images/criandoeentrando.png)


* Branch
    * Cria branch chamada **testeBranch**
    * Visualiza suas branchs criadas
    * Entra na branch criada

------
```sh
git branch -D testeBranch2
```
![](Images/deletandoBranch.png)

* Excluí  branch testeBranch2











