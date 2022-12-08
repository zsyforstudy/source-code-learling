# 这是学习arrify的笔记心得

> 首先介绍一下`arrify` 是干嘛用的。`arrify`用于把一个值转换为一个数组，转化规则在`readme.md`中。

## 学习知识

###### 1.Symbol.iterator

在index.js中有如下代码，判断是否可迭代

```javascript
if (typeof value[Symbol.iterator] === 'function') {
  return [...value];
}
```

*不了解迭代器与生成器的可参考这篇文章：[javascript迭代器与生成器](https://blog.csdn.net/m0_62336865/article/details/125585842)*

###### 2.如何测试
 在`package.json`中有如下代码

 ```json
 "scripts": {
      "test": "xo && ava && tsd"
 }
  ```
  
 所以我们执行 `npm test`时其实执行了三个任务
 其中ava表示使用的是ava测试框架

 **xo**
 > JavaScript/TypeScript linter (ESLint wrapper) with great defaults JavaScript/TypeScript linter（ESLint 包装器）具有很 的 默 认值

 **ava**
 > Node.js test runner that lets you develop with confidence

 **tsd**
 > Check TypeScript type definitions 检查 TypeScript 类型定义
  
 在ava测试中我们使用到了`is()` 和`deepEqual()`

 ```txt
 .is(value, expected, [message])                   断言 value 是否和 expected 相等
 .deepEqual(value, expected, [message])            断言 value 是否和 expected 深度相等
  ```

 *参考文章:[package.json命令解析](package.json文件scripts命令解析)&emsp;[关于ava测试框架](https://blog.csdn.net/weixin_34307464/article/details/89009363)*
