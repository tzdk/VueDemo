# VueDemo
## 1.Vue入门
[Hello World!双向绑定事例](https://tzdk.github.io/VueDemo/01.Start/index.html)
### 常用指令
- [v-bind指令示例](https://tzdk.github.io/VueDemo/01.Start/v-bind.html)
- [v-for指令示例](https://tzdk.github.io/VueDemo/01.Start/v-for.html)
- [v-for-grid指令示例](https://tzdk.github.io/VueDemo/01.Start/v-for-grid.html)，html文件单独引用js文件。
- [v-on指令示例](https://tzdk.github.io/VueDemo/01.Start/v-on.html)
- [综合示例](https://tzdk.github.io/VueDemo/01.Start/simple-demo.html)

## 2.条件渲染和列表渲染
### 条件渲染
- [v-if指令示例](https://tzdk.github.io/VueDemo/02.ConditionalRendering/v-if.html)
- [v-show指令示例](https://tzdk.github.io/VueDemo/02.ConditionalRendering/v-show.html).v-if和v-show在功能性上是一样的，不同点在于，在切换 v-if 块时， Vue.js 有一个局部编译/卸载过程，而v-show则不同，元素已经初始化会一直存在，判断条件不同时，本质上仅仅切换CSS属性display。因此，如果元素需要频繁切换 v-show 较好，如果在运行时条件不大可能改变 v-if 较好。

### 列表渲染
