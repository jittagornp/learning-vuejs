# การใช้งาน Vue Router

# Install

### 1. Install
```sh
$ npm install vue-router  
```

### 2. ใช้ Router

ที่ไฟล์ main.js ให้ 
```js
...
import VueRouter from 'vue-router'
Vue.use(VueRouter)
...
```
  
![](vue_router_1.png)

### 3. Config Route

ที่ไฟล์ main.js ให้ 
```js
...
const routes = [
  {
    path : '/', 
    component : <YOUR_COMPONENT>
  },
  {
    path : '/change-password', 
    component : <YOUR_COMPONENT>
  }
];

const router = new VueRouter({
  routes: routes
});
...
new Vue({
  render: h => h(App),
  router : router /* add router */
}).$mount('#app');
```

![](vue_router_2.png)

### 4. Config HTML

ที่ไฟล์ App.vue 
```vue
<template>
    ...
    <router-view></router-view> 
    ...
</template>
...
```
![](vue_router_3.png)
