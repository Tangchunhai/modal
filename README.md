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

| 参数        | 说明           |
| ------------- |:-------------:|
| el  | 挂载值，必须是标签元素的#id |
| open      | show-开打弹窗，hide关闭弹窗 |
| fixed |     true-不会随着滚动条而移动，false-随着滚动条移动  |
| animation | up-弹窗从上到下出现动画，soak-弹窗从小到大出现动画，默认为up  |
| backdropClose |     true-开启背景关闭，false-关闭背景关闭，默认为true  |

```html
      
```
