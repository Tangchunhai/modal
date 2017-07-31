# 介绍
一个原生写的简单模态框，兼容IE8。

# 功能特性
<p>1.支持标签属性关闭弹窗。</p>
<p>2.支持点击弹窗区域外背景关闭弹窗。</p>
<p>3.支持两种打开弹窗动画效果，也可以禁止动画效果。</p>
<p>4.支持ESC快捷键关闭弹窗。</p>
<p>5.支持打开多个弹窗。</p>

# 目录结构

```
│ //跟目录
│  modal.html //示例文件
│  
├─css //样式目录
│      modal.css //modal样式
│      
└─js //js目录
        modal.js //modal脚本
```
# 使用说明
```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>弹窗</title>
    <link rel="stylesheet" href="css/modal.css">
</head>
<body>	
        <div id="js-modal" class="modal">
                <div class="modal-dialog">
                        <div class="modal-header">
                                <h1>标题</h1>
                                <button type="button" class="close" data-close="modal">&times;</button>
                        </div>
                        <div class="modal-content" style="height: 400px;">
                                内容随便写
                        </div>
                        <div class="modal-foot">
                                <button class="btn btn-default" onclick="closes()">取消</button>
                                <button class="btn btn-primary" style="margin-left: 5px;" onclick="open2()">确定</button>
                        </div>
                </div>
        </div>
<body>
</html>        
```
