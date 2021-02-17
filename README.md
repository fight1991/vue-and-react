# vue-and-react
vue和react的相同点和不同点汇总
## 粗略对比
# vue优点
1. 模板和渲染函数的弹性选择
2. 简单的语法及项⽬创建
3. 更快的渲染速度和更⼩的体积
# react优点
1. 更适⽤于⼤型应⽤和更好的可测试性
2. 同时适⽤于 Web 端和原⽣ App
3. 更⼤的⽣态圈带来的更多⽀持和⼯具

# 相同点
1. 虚拟dom
2. 都是穿件UI的js库
3. 轻快便捷
4. 基于组件的架构
5. 都可以放入单个HTML文件中, 或者成为更复杂webpack设置中的模块;
6. 都有独立常用的路由器和状态管理库;

# 最大不同点
vue通常使用html模板文件; react则完全是javascript  vue有双向绑定的语法糖, 而react需要setState更新视图
# 不同点
1. vue组件可以注册为全局和局部, 而react都是通过import相应的组件
2. props可以动态变化,子组件也实时更新, 在react中官方建议props要向纯函数那样, 输入输出一致对应, 而且不太建议通过props来更改视图
3. ⼦组件⼀般要显示地调⽤ props 选项来声明它期待获得的数据。⽽在
react 中不必需，另两者都有 props 校验机制
4. 每个 Vue 实例都实现了事件接⼝，⽅便⽗⼦组件通信，⼩型项⽬中不
需要引⼊状态管理机制，⽽ react 必需⾃⼰实现
5. 使⽤插槽分发内容，使得可以混合⽗组件的内容与⼦组件⾃⼰的模板
6. 多了指令系统，让模版可以实现更丰富的功能，⽽ React 只能使⽤ JSX
语法
7. Vue 增加的语法糖 computed 和 watch，⽽在 React 中需要⾃⼰写⼀
套逻辑来实现
8. react 的思路是 all in js，通过 js 来⽣成 html，所以设计了 jsx，还有
通过 js 来操作 css，社区的 styled-component、jss 等；⽽ vue 是把
html，css，js 组合到⼀起，⽤各⾃的处理⽅式，vue 有单⽂件组件，
可以把 html、css、js 写到⼀个⽂件中，html 提供了模板引擎来处
理
9. react 做的事情很少，很多都交给社区去做，vue 很多东⻄都是内置的，写起来确实⽅便⼀些， ⽐如 redux 的 combineReducer 就对应vuex 的 modules， ⽐如 reselect 就对应 vuex 的 getter 和 vue 组件的 computed， vuex 的 mutation 是直接改变的原始数据，⽽ redux的 reducer 是返回⼀个全新的 state，所以 redux 结合 immutable 来
优化性能，vue 不需要。
10. react 是整体的思路的就是函数式，所以推崇纯组件，数据不可变，单
向数据流，当然需要双向的地⽅也可以做到，⽐如结合 redux-form，
组件的横向拆分⼀般是通过⾼阶组件。⽽ vue 是数据可变的，双向绑
定，声明式的写法，vue 组件的横向拆分很多情况下⽤ mixin
