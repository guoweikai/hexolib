---
title: es6
date: 2020-03-30 14:37:05
tags:
---
###  promise

```js
var p1 = new Promise(function (resolve) {
  setTimeout(function () {
    resolve(1);
  }, 1000);
})

p1.then(function (val) {
  var p3 = new Promise(function (resolve) {
    setTimeout(function () {
      resolve(val + 1);
    }, 1000);
  });

  return p3;
}).then(function (val) {
  console.log(val);
});
```
### Iterator

###  心得
* **项目中一定要区分哪些是异步函数哪些是功能函数**
* **功能函数的划分**
* **函数的返回值**
* **类和函数的区别**
