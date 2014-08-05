jQuery源码分析

  源码分析博客
  www.cnblogs.com/AaronJs


jQuery源码分析目录（2.1.1版本）
-----------------------------------

  
大家最关注的问题，我能学到什么？
-----------------------------------
###  本书围绕的几个核心点：
1.	设计理念
2.	结构组织
3.	抽象设计
4.	模式运用
5.	场景套用


###  第一章：语言基础
### 
    1.1 基本类型与引用类型
    1.2 参数的值传递
    1.3 执行环境与作用域链
    1.4 理解原型链
    1.5 理解闭包
    1.6 面向对象设计
        1.6.1 类继承
        1.6.2 原型继承


###  第二章：设计模式
### 
    2.1 单体模式
    2.2 门面模式
    2.3 工厂模式
    2.4 观察者模式
    2.5 中介模式
    2.6 适配器模式
    2.7 装饰者模式
    2.8 桥接模式
    2.9 代理模式

###  第三章：理解jQuery
### 
    3.1 库与框架
    3.2 初步认识jQuery
        3.2.1 jQuery与dom对象的区别
        3.2.2 类数组
        3.2.3 ready与load事件
    3.3 jQuery体系结构
        3.4.1 基础设施模块
        3.4.2 选择器模块
        3.4.3 节点模块
        3.4.4 AJAX模块
        3.4.5 动画模块
        3.4.6 其余的扩展
    3.5 高级运用    
        3.7.1 惰性加载
        3.7.2 函数重载
        3.7.3 curry化
        3.7.4 函数节流
        3.7.5 函数重载
    3.6 jQuery使用的设计手法
        3.6.1 无new构建
        3.6.2 链式调用
        3.6.3 静态与实例方法共享
        3.6.4 归并调用
        3.6.5 模块化
        3.6.6 钩子机制
    3.7 jQuery引入的模式
        3.7.1 工厂模式
        3.7.2 观察者模式
        3.7.3 适配器模式
        3.7.4 外观模式
        3.7.5 组合模式
        3.7.6 迭代器



###  第四章：核心模块
### 
    4.1 理解静态与实例
    4.2 如何实现无new构建
    4.3 分离作用域
    4.4 jQuery的Internal DSL
    4.5 方法链式调用的实现
    4.6 插件接口的设计
    4.7 动手设计一个简写的jQuery原型库


###  第五章：回调系统
### 
    5.1 回调用途
    5.2 设计思路
    5.3 一个简单回调实现
    5.4 jQuery.Callbacks实现


###  第六章：数据缓存
### 
    6.1 缓存介绍
    6.2 jQuery引入缓存中解决的问题
    6.3 运用场景
    6.5 一个简单数据缓存实现
    6.4 jQuery.Data数据缓存实现


###  第七章：异步机制
### 
    7.1 介绍
        7.2 理解同步与异步差别
        7.3 深入定时器
    7.4 实际运用中的处理
        7.5 一个简单模型的实现
        7.6 原理剖析
    7.7 jQuery.Deferred
        7.7.1 什么是deferred对象
        7.7.2 deferred与回调的区别
        7.7.3 deferred涉及的接口
        7.7.4 deferred的设计思路及实现
        7.7.5 when的设计思路及实现


###  第八章：模块加载
### 
	8.1	AMD与CMD规范
	8.2	如何设计
	8.3	轻巧的实现

###  第九章：选择器引擎
### 
    9.1 CSS选择器
    9.2 浏览器提供的接口与兼容问题
        9.2.1 浏览器提供的六大接口
        9.2.2 querySelectorAll兼容问题
        9.2.3 getElementById处理
        9.2.4 getElementsByTagName处理
        9.2.5 getElementsByClassName处理
        9.2.6 getAttribute和getAttributeNode的处理
    9.3 正则表达式
        9.4.1 理解正则
        9.4.2 选择分组与引用
        9.4.3 分析jQuery中的正则
    9.4 选择器引擎设计的思路与知识点 
    9.5 解析sizzle引擎
        9.5.1 词法解析器
        9.5.2 解析原理
        9.5.3 编译函数
        9.5.4 超级匹配
        9.5.6 基础选择器
        9.5.7 层级选择器
        9.5.8 属性选择器
        9.5.9 伪类选择器
        9.5.10 过滤器
        9.5.11 表单选择器
    9.6 jQuery选择器的优化
    9.7 小结


###  第十章：文档处理
### 
    10.1 节点层次关系的理解
    10.2 忽略的细节
         10.2.1 Document.body与DocumentElement区别
         10.2.2 contentWindow、contentDocument、document区别
         10.2.3 DocumentFragment存在的问题
         10.2.4 iframe存在的问题
         10.3.5 HTML5引入的高级API
    10.3 DOM的CRUD操作技术
         10.3.1 创建节点
         10.3.2 插入节点
         10.3.3 删除节点
         10.3.4 替换节点
    10.4 jQuery文档整体思路
         10.4.1 domManip
         10.4.2 buildFragment
    10.5 jQuery文档处理
         10.5.1 内部插入
         10.5.2 外部插入
         10.5.3 包裹
         10.5.4 替换
         10.5.5 删除
         10.5.6 复制
    10.6 筛选
         10.6.1 过滤
         10.6.2 查找
         10.6.3 串联
 


第十一章：样式操作
-----------------------------------
### 
    11.1 盒子模型
         11.1 padding
         11.2 border
         11.3 margin
    11.2 样式操作的规则
         11.2.1 样式访问接口
         11.1.2 不同浏览下的兼容性
    11.3 样式表操作
    11.4 元素的位置
    11.5 元素的尺寸
    11.6 jQuery样式解析流程
    11.7 jQuery的样式钩子
    11.8 jQuery的css接口
    11.9 jQuery的位置操作
    11.10 jQuery的尺寸操作


###  第十二章：属性操作
### 
	12.1 属性与特性
	12.2 关于jQuery属性钩子
    12.3 属性钩子处理的兼容问题
         12.3.1 保留值属性名字修正
         12.3.2 与表单操作相关


###  第十三章：事件
### 
    13.1 事件概述
         13.1.1 冒泡与捕获
         13.1.2 事件的异步
         13.1.3 事件兼容处理
    13.2 事件特性
         13.2.1 事件对象
         13.2.2 事件中的上下文
         13.2.3 事件引发的循环引用
    13.3 事件系统设计需要考虑的问题
    13.4 jQuery事件体系结构   
    13.5 jQuery中bind/live/delegate/on的区别
    13.6 jQuery绑定设计
    13.7 jQuery委托设计
    13.8 jQuery自定义事件设计
    13.9 jQuery模拟事件 
    13.10 小结    


###  第十四章：AJAX
### 
    14.1 关于http
    14.2 处理数据
    14.3 表单序列化
    14.4 一个完整的Ajax
    14.5 jQuery针对AJax的处理流程
    14.6 Deferred与Callback的改造
    14.7 前置过滤器与请求分发器
    14.8 预处理jsonp
    14.9 Jsonp的原理与实现
    14.10 类型转化器
    14.11 小结


###  第十五章：动画
### 
    15.1 队列操作
    15.2 动画队列
    15.3 动画原理
    15.4 jQuery动画效果  
         15.4.1 基本
         15.4.2 滑动
         15.4.3 淡入淡出
         15.4.4 自定义
    15.4 实现一个简单的动画原型

	
###  第十六章：SPA应用架构开发经验
### 
    16.1 关于SPA
    16.2 大型应用如何架构？
    16.3 分层设计
    16.4 引入模式
    16.5 异步与同步的处理
    16.6 单线程模拟多线程
    16.7 音频线程问题
    16.8 内存优化

		

待完善。。。	
-----------------------------------

