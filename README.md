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
### 通过js来打开弹窗设置
``` js
//打开弹窗
modal.init({
    el: '#js-modal', //挂载值，必须是标签元素的#id
    open: 'show' //show为打开
});

//关闭弹窗
modal.init({
    el: '#js-modal', //挂载值，必须是标签元素的#id
    open: 'hide' //hide为关闭
});

```

| 属性          | 说明 | 类型 | 可选值 | 默认值 |
|:------------- |:--------------|:---------------|:--------------------------|:--|
| el            | 挂载元素ID     | string        | 必须是元素ID   | ---|
| open          | 打开或关闭弹窗  | string        | show、hide | ---|
| fixed         | 弹窗随滚动条而上下移动  | boolean| true、false | false      |
| animation     | up-弹窗从上到下出现动画，soak-弹窗从小到大出现动画| string        | up、soak、none   | none |
| backClose | 背景关闭  | boolean        | true、false   | true      |

```html
<div id="js-modal2" class="modal up" data-backClose="static">
    <div class="modal-dialog">
        <div class="modal-header">
            <h1>标题2</h1>
            <button type="button" class="close" data-close="modal">&times;</button>
        </div>
        <div class="modal-content" style="height: 300px;">
            内容随便写
        </div>
        <div class="modal-foot">
            <button class="btn btn-default" data-close="modal">取消</button>
            <button class="btn btn-primary">确定</button>
       </div>
    </div>
</div>      
```
| 属性          | 说明 | 类型 | 可选值 | 默认值 |
|:------------- |:--------------|:---------------|:--------------------------|:--|
| class | up-弹窗从上到下出现动画，soak-弹窗从小到大出现动画 | string        | up、soak | --- |
| data-backClose | 禁止背景关闭弹窗     | string        | 必须是static   | ---|
| data-close          | 关闭弹窗  | string        | 必须是modal | ---|
