# 章节1

章节1介绍balabala....

## 开发语言
从事过网页编程的人知道，网页编程采用的是HTML + CSS + JS这样的组合，同样道理，chameleon中采用的是 CML + CMSS + JS。
[JS](./logic/lifecycle.html)语法用于处理页面的逻辑部分，与普通网页编程相比，本项目目标定义标准MVVM框架，拥有完整的生命周期，watch，computed，数据双向绑定等优秀的特性，能够快速提高开发速度、降低维护成本。 简单举例：
```javascript
<script>
class Index {
  // data
  data =  {
    message: 'Hello',
  }
  // 计算属性
  computed = {
    reversedMessage: function () {
      return this.message.split('').reverse().join('')
    }
  }
  // 观察数据变化
  watch: {
    message: function (newV, oldV) {
    }
  }
  // 各种生命周期
  mounted: function(res) {
  }
}
export new Index();
</script>
```

[CML](./view/cml.html)（Chameleon Markup Language）用于描述页面的结构，我们知道HTML是有一套标准的语义化标签，例如文本是`<span>` 按钮是`<button>`。CML同样具有一套标准的标签，我们将标签定义为`组件`，CML为用户提供了一系列[组件](./component/base/base.html)。同时CML中还支持<b>模板语法</b>，例如条件渲染、列表渲染，数据绑定等等。简单举例：

```html
<template>
  <view> 
     <!--数据绑定 message变量 -->
      <text>
        {{ message }}
      </text> 
  </view>
</template>

```
同时，CML支持使用[类VUE语法](./view/vue.html)，让你更快入手。


[CMSS](./view/cmss.html)(Chameleon Style Sheets)用于描述CML页面结构的样式语言，其具有大部分CSS的特性，并且还可以支持各种css的预处语言`less stylus`。 默认支持less处理，简单举例：
```html
<style>
@import './global.less';
@size: 10px;
.header {
  width: @size;
  height: @size;
}
</style>
```

<b>通过以上对于开发语言的介绍，相信你看到只要是有过网页编程知识的人都可以快速的上手chameleon的开发</b>。