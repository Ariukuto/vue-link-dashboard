# vue-link-dashboard
vue-link-dashboard is my private Vue3 project to compare vue3 with React and Angular. The purpose of link-dashboard is that important links are grouped in card elments or in navbar. For example: In the Navbar there are links that appear only once on the page. In the grouped card elements there are, can be several same links that lead to different servers destinations. For example, servers, etc. 

**I'm use following concepts for better reading and understanding code:**
1. "Single File Components" instead of the app.component(), method. <br />
2. Composition API <br>
In React, but also in Vue etc. we often define methods, functions that TECHNICALLY match the component. But this has the following disadvantages: <br />
-Functionality can't be reused independently from components (components are not there to collect methods RIGHT, but to represent UI).
this components become much too big and cluttered very quickly. (I've never been a fan of data and methods syntax in Vue. That's why I liked React better afterwards) <br />
-Through the Composition API, auxiliary functions can now be better used and shared.
If you want to know exactly, this video opened my eyes: https://www.youtube.com/watch?v=6HUjDKVn0e0



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
