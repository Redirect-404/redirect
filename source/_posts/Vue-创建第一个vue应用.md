---
title: Vue 创建第一个vue应用
date: 2021-04-28 17:57:08
tags:
	- VUE 
categories: 
	- 前端
comments: true	
---
* * *
每个 Vue 应用都是通过用 Vue 函数创建一个新的 Vue 实例开始的：
```
var vm = new Vue({
// 选项
})
```

<!-- more -->

虽然没有完全遵循 MVVM 模型，但是 Vue 的设计也受到了它的启发。因此在文档中经常会使用 vm(ViewModel 的缩写) 这个变量名表示 Vue 实例。
当创建一个 Vue 实例时，你可以传入一个选项对象。

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title></title>
        <!--  文件引入-->
        <script src="vue.js" type="text/jscript"></script>
        <!--CND引入 -->
        <!-- <scriptsrc="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script> -->
    </head>
    <body>
        <div id="app">
            {{ message }}---{{ one }}
        </div>
        <script type="text/jscript">
            var app = new Vue({
                el:'#app', //元素
                data: {    //赋值数据
                    message: 'hello world',
                    one: '123'
                }
            });
        </script>
    </body>
</html>
```