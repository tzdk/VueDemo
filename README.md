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
- [v-for指令示例](https://tzdk.github.io/VueDemo/02.ConditionalRendering/v-for-demo.html),官方示例v-for="(item,index) in items",第二个参数为索引，经测试第一个参数为索引，所以正确的代码应该为：v-for="(index,item) in items"
- [v-for-props指令示例](https://tzdk.github.io/VueDemo/02.ConditionalRendering/v-for.html)

## 3.组件 Components
### 组件创建和使用
- [开始使用组件](https://tzdk.github.io/VueDemo/03.Components/simple-demo.html)

组件的创建和使用过程如下

1. Vue.extend()是Vue构造器的扩展，调用Vue.extend()创建的是一个组件构造器。 
2. Vue.extend()构造器有一个选项对象，选项对象的template属性用于定义组件要渲染的HTML。 
3. 使用Vue.component()注册组件时，需要提供2个参数，第1个参数时组件的标签，第2个参数是组件构造器。 
4. 组件应该挂载到某个Vue实例下，否则它不会生效。

- 组件[简写方式](https://tzdk.github.io/VueDemo/03.Components/simple-demo-another.html)，可以省略extend方法：
- [全局注册组件示例](https://tzdk.github.io/VueDemo/03.Components/global-registration.html)，调用Vue.component()注册组件时，组件的注册是全局的，这意味着该组件可以在任意Vue示例下使用。如果不需要全局注册，或者是让组件使用在其它组件内，可以用选项对象的components属性实现局部注册。
- [局部注册组件示例](https://tzdk.github.io/VueDemo/03.Components/local-registration.html)
- [父组件和子组件](https://tzdk.github.io/VueDemo/03.Components/parent-child-components.html)
- [Script标签](https://tzdk.github.io/VueDemo/03.Components/script-tag.html)
- [Template标签](https://tzdk.github.io/VueDemo/03.Components/template-tag.html),如果使用 template 标签，则不需要指定type属性。

### 组件props使用
- [props基础示例](https://tzdk.github.io/VueDemo/03.Components/props-simple-demo.html)
- [props单向绑定](https://tzdk.github.io/VueDemo/03.Components/single-bind-props.html)，默认是单向绑定。
- [props双向绑定](https://tzdk.github.io/VueDemo/03.Components/double-bind-props.html)
- [props单次绑定](https://tzdk.github.io/VueDemo/03.Components/once-bind-props.html)，单次绑定完成以后不会彼此同步双方的变化。

### 组件slot使用
- [单个slot示例](https://tzdk.github.io/VueDemo/03.Components/single-slot.html)
- [多个slot示例](https://tzdk.github.io/VueDemo/03.Components/dialog-slot.html)

### 父子组件实例访问
- [$children示例](https://tzdk.github.io/VueDemo/03.Components/children.html)
- [$refs示例](https://tzdk.github.io/VueDemo/03.Components/refs.html)
- [$parent示例](https://tzdk.github.io/VueDemo/03.Components/parent.html)

### 父子组件通信
- [$dispatch向上派发事件示例](https://tzdk.github.io/VueDemo/03.Components/dispatch.html)
- [$broadcast向下广播事件示例](https://tzdk.github.io/VueDemo/03.Components/broadcast.html)
