---
layout: post
title: First..Start..
---


node.js
readStream对象读取文件  

方法：createReadStream(path,[options]);

var fs=require('fs');  

var file=fs.createReadStream('./message.txt');  

file.on('open',function(fd){  

    console.log('开始读取数据');   
   
});  

file.data('data',function(data){  

    console.log('读取数据:');  
  
    console.log(data);  
  
});  

