# todo-list

> Lista de tarefas com Vue

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

# Adicionando funcao a diretiva #

Exemplo:

v-on:keyup ***.enter***=""

Isso irá dizer ao Vue que deve acionar a função somente quando o enter for clicado 
o Vue JS cria alguns atalhos para o keycode mais utilizado.

Para ver o keycode correto entre no site http://keycode.info/

```
<input class="new-todo"
           v-on:keyup="addTask"
           placeholder="O que precisa ser feito?">
```

##### Usando açúcar sintático #####

O vue.js nos da alguns atalhos interessantes para nao precisar ficar digitando muito código 

Para diretiva:

Inves de usar o ***v-on:*** utilize ***@***

Ex:

```
// De:
<input class="new-todo"
           v-on:keyup="addTask"
           placeholder="O que precisa ser feito?">

Para:
<input class="new-todo"
          @keyup="addTask"
          placeholder="O que precisa ser feito?">
```

### Alguns eventos ###

O .stop que evita que o evento seja propagado:

```
<a v-on:click.stop="doThis"></a>”
```

O modificador .prevent evita que a ação padrão do navegador aconteça, como em um envio de formulário que recarregaria a página.

``` 
<form v-on:submit.prevent="onSubmit"></form>
```

Temos também o .self que faz com que o evento seja disparado somente ao clicar no elemento, e não em seus filhos, como ocorre por padrão na maioria dos navegadores atuais.

```
<div v-on:click.self="doThat">...</div>
```
For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
