>1 vue的组件传值

非父子组件传值：
**vuex**，
**总线机制**（bus/发布订阅模式/观察者模式）

`Vue.prototype.bus = new Vue(); 
this.bus.$emit()`

**不能改变父组件传递过来的数据 要拷贝之后再处理**

>2 组件校验和非props特性

 >3 作用域插槽
 
 <template>标签中加入 slot-scope 在slot中动态绑定数据v-bind 传递值，外层决定如何渲染，内层决定数据传递本身，跟组件其实意义差不多，但是比一半组件更灵活
>4 v-once 和动态组件

`<component>+ :is 可以给控制动态组件的显示`
> 5 little trick
`v-on:click="show = !show">` 可以省略函数