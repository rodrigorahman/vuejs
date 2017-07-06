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


For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
