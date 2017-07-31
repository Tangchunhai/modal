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

| 参数          | 说明           | 类型     | 可选值       | 默认值|
|:------------- |:--------------|:---------------|:-----------------|:-------------|
| el            | 挂载元素ID     | string        | 必须是元素ID   | ---|
| open          | 打开或关闭弹窗  | string        | show、hide   | ---|
| fixed         | 弹窗随滚动条而上下移动  | boolean| true、false   | false|
| animation     | 弹窗动画，up-弹窗从上到下出现动画，soak-弹窗从小到大出现动画  | string        | up、soak   | up|
| backdropClose | 背景关闭  | boolean        | true、false   | true|

```html
      
```
