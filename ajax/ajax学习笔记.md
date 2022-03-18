# Ajax学习笔记
## 1 客户端和服务器的概念

- 使用请求-处理-相应 三步走的模式来对网页中的每一个过程进行处理
- 网页中请求数据的方法：**XMLHttpRequest (简称为xhr)**
- 这是一个由浏览器提供的js成员
- 最简单的使用举例：

    var xhrObj = new XMLHttpRequest()

- xhr有一些请求方式：**GET** 和 **POST**

## 2 Ajax的概念

- 在网页中使用xhr与服务器相互进行数据交互的技术

## 3 jQuery中的Ajax

jQuery对Ajax进行了封装，使之更为易用

    $.get(url, [data], [callback])

    //发起不带参数的get请求的时候只用提供url和回调函数[callback]即可，可以使用res来代表服务器传回的数据

    // 发起带参数的的请求，则需要使用[data]

    $.post(url, [data], [callback])
    
    //把[data]传给服务器

    $.ajax({  
        type: '',  //定义请求类型
        url: '',  //该请求的URL地址
        data: {},  //该请求携带的数据
        success: function(res){}  //回调函数
    }) 
    
    //复合的综合工具

## 4 接口的概念
使用Ajax发送请求的时候的URL地址就叫做接口

## 5 接口的测试工具
1 什么是接口测试工具？  
使用PostMan工具，在不写代码的前提下，用来验证接口是否可以被访问，进行调用和测试
