# todolist Purpose :smiley:
:wave: hey There!

This is a simple TodoList App I build to play around and familiarize myself with Vue's syntax and templating. 

This app utilizes the [jsonplaceholder API](https://jsonplaceholder.typicode.com/) to mimic simple /GET /POST /DELETE requests and get some experience using these requests in the vue framework. 

Noteable new syntax terms used in the project are: 
 - v-bind:class   -> Conditional style rendering: applies the text-decoration: line-through rule on condition
 - v-on:change    -> Vue's event handler for an onChange event
 - v-on:click     -> Vue's event handler for an onClick event
 - v-on:submit    -> Vue's event handler for an onSubmit event
 
 - this.$emit()   -> To pass a function up to a parent / grand-parent component.

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
