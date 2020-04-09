---
title: es6
date: 2020-03-30 14:37:05
tags:
---

## 项目中应该区分哪些是同步函数哪些是异步函数

# promise

promise 是


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

# Iterator 的概念

# 区分同步函数和异步函数 

# 功能行函数拆分

