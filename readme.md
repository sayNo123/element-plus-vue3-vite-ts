## ELEMENT-PLUS-VUE3  

*！！！此项目为 `element-plus` + `vue3` + `vite` + `typescript`的学习，仅基础！！！*  

### `yarn` 安装 vite  

```
yarn global add vite
```

### 使用 `vite` + `vue` 搭建项目  

``` 
yarn create @vitejs/app
```  

```
yarn create @vitejs/app element-plus-vue3 --template vue
```

__支持的模板预设选择的是 `vue-ts`__  

### 进入 element-plus-vue3 目录  

`yarn` 安装一下依赖  

```
yarn dev
```

浏览器里能看到 vue logo 即成功。

## 安装 element-plus  

参考官网安装 [`element-plus`](https://element-plus.org/#/zh-CN/component/installation#npm-an-zhuang)，然后将 main.ts 文件中的代码改成如下：  

```
import { createApp } from 'vue'
import ElementPlus from 'element-plus'
import 'element-plus/lib/theme-chalk/index.css'
import App from './App.vue'

const app = createApp(App)
app.use(ElementPlus)
app.mount('#app')
```

### 在 components 目录下创建一个 demo.vue 的文件  

将 element-plus 代码写进去，再在 main.ts 文件中导入 demo.vue，`yarn dev` 运行看看是否正常。