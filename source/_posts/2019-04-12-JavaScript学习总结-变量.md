---
title: JavaScript学习总结-变量
tags:
  - 前端
  - JavaScript
categories:
  - 前端
  - JavaScript
abbrlink: b062d643
date: 2019-04-12 18:02:49
---

## 一、命名

### 1、方法

#### a、匈牙利命名法（变量名=类型+对象描述）
- Int 整型   i
- float 浮点型   fi
- Bollean 布尔  b
- String 字符串   s
- Array 数组   a
- Obeject 对象  o
- Function 函数  fn
- Regular Expression 正则 re
  <!--more-->

#### b、驼峰命名法
- 全部小写
  - 单词与单词间用下划线分割
- 大小写混合
  - 大驼峰：每个单词首字母大写
  - 小驼峰：第一个单词首字母小写，其他首字母大写

### 2、规则
- 首字母：英文字母或者下划线
-  组成：英文字母，数字，下划线
- 禁忌：JavaScript关键词与保留字
  
## 二、声明

### 1、显示声明
- var变量名

### 2、陋习
- 没有类型
- 重复声明
- 隐式声明
- 不声明直接赋值

### 3、正解
- 先声明、后读写
- 先赋值、后运算

## 三、变量类型

### 1、值类型
- 占用空间固定，保存在栈中
- 保存与复制的是值本身
- 使用typeof检测数据的类型
- 基本类型数据是值类型

### 2、引用类型
- 占用空间不固定，保存在堆中
- 保存与复制的是指向对象的一个指针
- 使用instanceof检测数据的类型
- 使用new()方法构造出的对象是引用型

## 四、作用域

### 1、全局变量

#### a、包含
- 在函数体外定义的变量
- 在函数体内定义的无var声明的变量

#### b、调用
- 任何位置

### 2、局部变量

#### a、包含
- 在函数内部使用var声明的变量
- 函数的参数变量

#### b、调用
- 当前函数体部

### 3、优先级
- 局部变量高于同名全局变量
- 参数变量高于同名全局变量
- 局部变量高于同名参数变量

### 4、热性

#### a、忽略块级作用域

#### b、全局变量是全局对象的属性

#### c、局部变量是调用对象的属性

#### d、作用域链
- 内层函数可访问外层函数局部变量
- 外层函数不能访问内层函数局部变量

#### e、生命周期
- 全局变量：除非被显示删除，否则一直存在
- 局部变量：自声明起至函数运行完毕或被显示删除
- 回收机制
  - 标记清除
  - 引用计数

































