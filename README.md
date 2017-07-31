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

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

```html
      
```
