# Comandos mais utilizados

## Ambientes de Preparação

Verifica o status/condição da branch em que você está trabalhando, arquivos modificados, criados e exluídos

```css
$ git status
```

Após criar um arquivo, adicione o arquivo no rastreamento do Git

```css
$ git add [nome_arquivo]
```

Depois de adicionar o arquivo a ser rastreado, confirme as alterações a serem rastreadas usando o Git. No Terminal, use git commit - m seguido por uma mensagem curta para confirmar as mudanças

```css
$ git commit -m "tipo mensagem"
```


Depois de confirmar as alterações, envie as alterações de sua máquina local para o repositório remoto. 

```css
$ git push origin master