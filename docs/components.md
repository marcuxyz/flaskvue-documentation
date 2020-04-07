# Components

When the command `flask vue init` is executed, it create the **frontend** folder in root directory. That's great!
Because, inside, it create `frontend/components/HelloWorld.vue`.

Let's take a look at the HelloWorld Component:

```vue
<template>
  <div id="presentation">
    <h1>Apresentation</h1>
    Hello {{ name }}
  </div>
</template>

<script>
import Axios from "axios";
export default {
  name: "HelloWorld",
  props: ["name"],
};
</script>
```

It has the `name props`, because, in [templates section](/templates#creating-your-base-template), we managed to use `<hello-world :name='Pacotei'></hello-world>`.

## Creating Component

You can create your own components... And, let's say you have created `Product.vue` component. 
But, after create you should register it in `frontend/index.js`, see:

```javascript
import Vue from "vue";
import HelloWorld from "./components/HelloWorld";
import Product from "./components/Product";
import store from "./store";

new Vue({
  store,
  components: {
    HelloWorld,
    Product
  },
}).$mount("#app");
```

After registered, you can use in your `.jinja or .html templates` as in [templates section](/templates#creating-your-base-template).