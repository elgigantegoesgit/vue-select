# Simple vue-select example in Vue3.

## Open questions:
How to get vue-select package in codesandbox/github combination? (Create in codesandbox alone via Dependencies and THEN transfer to github works, but how do add-on on a project that already uses sandbox+github editor? I can't find the "dependencies" button there and a "npm install vue-select" does not work)

## vue-select short guide:
(full see https://vue-select.org/)

### Install package:  
` npm install vue-select `

(...or In codesandbox, select Dependencies" > "vue-select 3.xbeta" or higher.)

### In main.js do:
`import Vue from 'vue'`

`import vSelect from 'vue-select'`

`Vue.component('v-select', vSelect)`

`import 'vue-select/dist/vue-select.css';`


### In main.js finally register the component by:

`createApp(App).component("v-select", vSelect).mount("#app");`




## Project setup

```
yarn install
```

### Compiles and hot-reloads for development

```
yarn serve
```

### Compiles and minifies for production

```
yarn build
```

### Lints and fixes files

```
yarn lint
```

### Customize configuration

See [Configuration Reference](https://cli.vuejs.org/config/).
