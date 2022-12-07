# 这是学习arrify的笔记心得

> 首先介绍一下`arrify` 是干嘛用的。`arrify`用于把一个只转换为一个数组，转化规则在`readme.md`中。

## 学习知识

1. Symbol.iterator
在index.js中有如下代码
```
if (typeof value[Symbol.iterator] === 'function') {
	return [...value];
}
```
参考文档
 * [symbol对象的iterator属性:Symbol.iterator](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Symbol/iterator)
 * [JavaScript Symbol.iterator Property](https://www.geeksforgeeks.org/javascript-symbol-iterator-property/)
 * [解读 arrify 源码](https://blog.csdn.net/qq_19901795/article/details/126630698)

2. 如何测试

3. 一些文件用途
