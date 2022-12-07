# 这是学习arrify的笔记心得

> 首先介绍一下`arrify` 是干嘛用的。`arrify`用于把一个值转换为一个数组，转化规则在`readme.md`中。

## 学习知识

1. Symbol.iterator

在index.js中有如下代码，判断是否可迭代

```
if (typeof value[Symbol.iterator] === 'function') {
	return [...value];
}
```

*不了解迭代器与生成器的可参考这篇文章：[javascript迭代器与生成器](https://blog.csdn.net/m0_62336865/article/details/125585842)*


2. 如何测试
在`package.json`中有如下代码
```
"scripts": {
	"test": "xo && ava && tsd"
}
```
所以我们执行 `npm test`时其实执行了三个任务
其中ava表示使用的是ava测试框架


*参考文章:[调试源码](https://jishuin.proginn.com/p/763bfbd6e43c)   [package.json命令解析](package.json文件scripts命令解析)*

3. 一些文件用途
