# Comandos básicos git (GitHub)

Segue uma lista de comandos git que podem ser utilizados na plataforma GitHub, isso é muito útil, pois existem comandos que utilizamos com pouca frequência que acabamos esquecendo sua sintaxe.

### Clonando um repositório remoto

```bash
git clone <URL do repositório> <nome repositório clonado>
```


### Vinculando um repositório local a um remoto

```bash
cd <repositório local>
```

```bash
git init .
```

```bash
git remote add origin <URL do repositório>
```

```bash
git pull origin main
```


### Mapeando alterações locais e enviando para o repositório remoto

+ Listando diferenças local/remoto

```bash
git status
```

+ Mapeando as diferenças locais

```bash
git add . 
```

+ Criando o commit com todas as alterações

```bash
git commit -am”Descrição das alterações mapeadas…”
```

+ Enviando as alterações para o repositório remoto

```bash
git push origin <branch-destino>
```


### Listando todos os commits já feitos no repositório.

```bash
git reflog
```

Ou

```bash
git log --pretty=oneline 
```


### Voltando um determinado commit (Remoto)

```bash
git revert <Id do commit>
```

```bash
git push origin <branch-destino>
```

> ***Observação***: Utilize o comando git reflog para pegar o ID do commit que deve ser revertido.


### Baixando atualizações remotas para repositório local

```bash
git pull origin <branch-origem>
```

### Criando branch para seu repositório local e remoto

+ Criando uma branch para seu repositório local e remoto

```bash
git branch <nova-branch> && git push -u origin <nova-branch>
```

+ Criando e já selecionando localmente uma branch para seu repositório

```bash
git checkout -b <nova-branch> && git push -u origin <nova-branch>
```

+ Alterando para nova branch

```bash
git checkout <nova-branch>
```

+ Selecionando a nova branch na sua criação

```bash
git checkout -b <nova-branch>
```

+ Listando as branches locais

```bash
git branch
```

+ Listando as branches remotas

```bash
git branch -r
```

+ Listando toda as branches locais/remotas

```bash
git branch -a
```

### Movendo atualizações de um branch para outra

+ Acesse a branch de destino

```bash
git checkout <branch-destino>
```

+ Faça a referência da branch de origem

```bash
git merge <branch-origem>
```

> ***Observação:*** Durante o merge, o Git identifica as diferenças entre as branches envolvidas e aplica essas alterações na branch de destino. Se houver conflitos, o Git solicitará que você resolva manualmente esses conflitos, combinando as alterações de forma apropriada.


# Referências

Git, ***Reference***. Disponível em: [\<https://git-scm.com/docs\>](https://git-scm.com/docs). Acesso em: 30 de jun. 2023.

GitHub, ***Introdução***. Disponível em: [\<https://docs.github.com/pt/pages/quickstart#introduction\>](https://docs.github.com/pt/pages/quickstart#introduction). Acesso em: 30 de jun. 2023.




