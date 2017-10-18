# jquery-mourseDragScroll
鼠标拖动容器进行滚动
# 简介
```text
dragscroll的最小版本dragscroll_micro.js大小为410个字节，仅支持基本的拖放滚动功能。

dragscroll的完整版本dragscroll.js大小有741个字节，它比最小版本多了一些额外的功能：

    添加了一个UMD模块。
    可以在页面加载后才被调用，插件会自动查找带有dragscroll class的元素，并将这些元素进行转换。
    最小化版本不能再页面初始化之后再加载，必须写在页面的<head>中。
    可以动态的添加或删除带有dragscroll class的元素。如果你执行了这些操作，要使用dragscroll.reset()方法来更新元素
```
    
# 使用方法

要使用该鼠标拖动滚动元素js插件，先要在页面中引入dragscroll_micro.js或dragscroll.js文件。

```JavaScript
<script src="dragscroll.js"></script>            
```
然后在你需要进行拖动滚动的元素上添加class dragscroll。
```html
<div class="dragscroll">
    Big text goes here...
</div>                
```
```text
就这么简单，现在这个元素就可以进行鼠标拖动滚动了。你也可以在<body>元素上添加dragscroll，使整个页面都可以进行鼠标拖动滚动。
注意：
-在使用这个插件之后，你将不可以对已经转换为拖动滚动的区域用鼠标来选择文本，所以你可以设置cursor: default;
-CSS样式来提醒用户该区域不能被选择。如果内容不是文本，你也可以设置为：cursor: grab;。
```
