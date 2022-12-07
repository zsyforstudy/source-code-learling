# 这是学习arrify的笔记心得

> 首先介绍一下`arrify` 是干嘛用的。`arrify`用于把一个只转换为一个数组，转化规则在`readme.md`中

## 学习知识

* Symbol.iterator
```
	if (typeof value[Symbol.iterator] === 'function') {
		return [...value];
	}
```

* 如何测试

* 一些文件用途
