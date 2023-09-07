# Git tips

## 1.0

Usando o comando "git commit", sem o argumento "-m", o git abrirá um arquivo de commit no seu editor de código que você escolheu no seu arquivo "git.config". Dentro desse editor, ficará mais fácil de explicar o que o seu commit faz. A primeira linha é o nome do commit, tudo que vem após  a quebra de linha se torna a sua descrição. 

### 1.1
Há várias ferramentas que tentam padronizar a mensagem do commit. Por exemplo: Conventional Commits Pattern.

### 1.2
Sempre use a mensagem em inglês e no tempo verbal imperativo. 

## 2
Commits Atômicos: Faça commits pequenos e atômicos, que contenham apenas uma funcionalidade ou correção de cada vez. Isso torna mais fácil rastrear as mudanças e entender o histórico.

## 3
Criar alias no Git é uma maneira conveniente de encurtar comandos frequentemente usados ou até mesmo personalizar comandos para se adequar ao seu fluxo de trabalho.

### 3.1
Por exemplo, para criar um alias global chamado co para checkout, você pode usar o seguinte comando:

```sh
git config --global alias.co checkout
```

3.2

Para criar um alias global chamado `cmp` para add, commitar e fazer push para o repositório remoto. 

```sh
git config --global alias.cmp '!f() { git add -A && git commit && git push; }; f'
```