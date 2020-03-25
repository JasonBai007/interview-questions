# interview-questions

interview questions for senior front-end developers.

### 须知

1. 以下问题是最近**36 家大中型企业面试实战**的总结
2. 需要自己去[**掘金**](https://juejin.im/collection/5d81e875f265da06a19a05bc?utm_source=wechat)查询答案、理解、记忆
3. 建议面试前预留 1-2 周时间准备
4. 不准备就去面试会死的很惨
5. 如果大部分都搞明白了，那面试成功率会在 85%以上，**剩下的 15%是因为面试官眼瞎！**

### 语法基础【笔试】

1. 80%以上的面试会有笔试
2. 大部分笔试都可以使用手机查询答案（面试官不在场）
3. 笔试时可以只写关键点，不必完整作答
4. 笔试主要考察语法基础，包括：**作用域、THIS 指向、异步执行顺序、原型链**
5. 看这篇文章就够了：**[送你 43 道 JavaScript 面试题](https://juejin.im/post/5d0644976fb9a07ed064b0ca)**

### 浏览器里的事件循环

1. **宏任务**有哪些？
2. **微任务**有哪些？
3. 描述一下[**事件循环模型**](https://juejin.im/post/5b24b116e51d4558a65fdb70)

### VUE

1. VUE 框架原理：[**数据劫持 + 发布订阅模式**](https://www.cnblogs.com/canfoo/p/6891868.html)
2. 循环列表时为啥要绑定不同的 key？（[**diff 算法**](https://juejin.im/post/5affd01551882542c83301da)）（不一定要掌握）
3. VUEX 是如何实现单向数据流的？<br>
   ![vuex单向数据流](https://vuex.vuejs.org/vuex.png)
4. VUE 在哪些情况下监控不到数据的变化？[为什么？](https://www.cnblogs.com/youhong/p/12173354.html)<br>
   1）Vue 不能检测对象属性的添加或删除<br> 2）当你利用索引直接设置一个数组项时，例如：vm.items[indexOfItem] = newValue<br> 3）当你修改数组的长度时，例如：vm.items.length = newLength
5. 啥时候使用 nextTick？（可以在DOM更新完毕之后执行一个回调，确保我们操作的是更新后的DOM）
6. 手写弹框组件（控制弹框显示隐藏的变量，尽量使用 v-model 指令）
7. 手写递归组件（考到的概率很小，知道个大概就行）

### ES6

1. [箭头函数与普通函数的区别](https://juejin.im/post/5b14d0b4f265da6e60393680#heading-2)
2. 你使用过哪些 ES6 新特性？
3. Promise 中的 then 方法是同步的还是异步的？
4. Promise 的异常处理，then 的第二个回调函数可以处理异常，为啥还需要 catch 方法？<br>
catch可以捕获前面then方法执行中的错误,因此，建议总是使用catch方法，而不使用then方法的第二个参数。
5. let、const、var 的区别

### NODE JS

1. 是否用 Node.js 做过项目？
2. KOA 框架的洋葱模型有什么用？
3. Node.js 的全局对象是什么？是 global 对象，全局变量都是这个对象的属性

### HTTP 通信

1. 200 from cache 和 304 有什么区别？
2. 常见的 headers 有哪些？
3. 401 和 403 有什么区别？401 没权限、403 禁止访问
4. 跨域有哪几种解决方法？JSONP、CORS、nginx 反向代理、本地启动代理、PostMessage
5. 强缓存和协商缓存
6. CORS 解决跨域问题后，如何再解决携带 cookie 的问题？[参考这篇](https://www.cnblogs.com/sosohui/p/10273225.html)

### 服务器端

1. 是否配置过 Nginx 服务器？
2. Nginx 服务器如何配置反向代理？
3. 是否熟练掌握 Linux 命令？（不熟练掌握也没事）

### 样式布局

1. 垂直水平居中的方法有哪些？
2. 是否使用过 flex 布局？有哪些常用属性？

### 移动端布局

1. 如何实现响应式布局？

### 性能优化

1. 首屏优化的方法有哪些？
2. 提高网页加载速度的方法有哪些？
3. 手写代码实现节流和防抖

### 装逼算法

1. 冒泡排序
2. 快速排序
3. 数组去重的方法：[...new Set(arr)]
4. 斐波那契数列
5. 递归的两个必要条件：自己调用自己+结束条件
6. 实现深拷贝一个对象
