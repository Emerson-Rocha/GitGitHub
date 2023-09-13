## Branch

Os branches permitem que você desenvolva recursos, corrija erros ou experimente com segurança novas ideias em uma área contida do seu repositório.

Você sempre cria um branch a partir de um branch existente. 

Normalmente, você pode criar um novo branch a partir do branch-padrão do seu repositório. 

Você então poderá trabalhar nesse novo branch isolado das mudanças que outras pessoas estão fazendo no repositório. 

Um branch que você cria para produzir um recurso é comumente referido como um branch de recurso ou branch de tópico.

https://wac-cdn.atlassian.com/dam/jcr:389059a7-214c-46a3-bc52-7781b4730301/hero.svg?cdnVersion=1299
## 2.Criar uma branch

```css 
    $ git branch [nome-da-sua-branch]
```

## Acessar a  branch

```css 
   $ git checkout [nome-da-sua-branch] 
```

E assim que a branch for criada, você já será levado para ela.

```css
  $  git checkout -b [nome-da-sua-branch]

```

## Subir uma branch local para um repositório remoto
``` css
 $ git  remote add origin [none_branch];
```
``` css 
git add arquivos-alterados
```


## O que é um merge

Estamos entendendo como trabalhar com branchs, mas se quisermos trazer o trabalho que fizermos em uma branch para outra?

Possuo duas branchs em um repositório GIT, uma chamada "ciclo-de-vida-basico" e a outra "master", estou trabalhando na primeira e após a finalização quero trazer o meu trabalho para "master", pois ela é a principal branch e onde deve ser depositado todo o código que funciona.

Como fazer isso? Através do **merge**, que é quando pegamos um código de uma branch e adicionamos à outra branch, unificando assim as alterações. É importante para manter sua branch atualizada ou para levar seu código para a branch principal.

Para unificar duas branchs, ou seja, fazer com que o conteúdo da primeira seja adicionado à segunda, utilizamos o comando `git merge nome-da-branch-a-ser-mergeada` na branch de destino. 

Abaixo um exemplo de **merge**:

1º Fazer checkout na branch de destino. Minha branch de destino é master, então farei: `git checkout master`.
	
	git checkout nome-da-branch-destino
	
2º Executar o merge para unificar sua branch na de destino. Como o nome da minha branch é ciclo-de-vida-basico, farei: `git merge ciclo-de-vida-basico`.

	git merge nome-da-branch-a-ser-mergeada 
    
Esse comando fará que o GIT automaticamente crie um commit com o branch atual e todo o conteúdo da branch origem.

### Exemplo de um merge local:

Após fazer commit das alterações na minha branch de trabalho, estou apta para fazer merge:

![printsceen de um merge local](../images/hands-on-merge.png)