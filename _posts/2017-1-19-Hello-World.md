---
layout: post
title: 啊哦，First..Start..
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

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub.
