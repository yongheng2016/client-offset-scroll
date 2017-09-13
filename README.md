
> 注意区分window和document的区别  

> Window对象表示浏览器中打开的窗口；window对象可以省略。比如alert()、window.alert()。
> Document对象是Window对象的一部分。那么document.body 我们可以写成window.document.body；浏览器的HTML文档成为Document对象。

---

# window

+ ## window.screen.height
```javascript
iHeight = window.screen.height
```

[参考](https://developer.mozilla.org/zh-CN/docs/Web/API/Screen/height)   


+ ## window.screen.avialHeight【只读】
```javascript
availHeight = window.screen.availHeight
```

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Screen/availHeight)


+ ## window.screenY【只读】
```javascript
lLoc = window.screenY 
```

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Window/screenY)


+ ## window.innerHeight【只读】  
```javascript
intViewportHeight = window.innerHeight
```

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Window/innerHeight)


+ ## window.outerHeight【只读】
```javascript
outWindowHeight = window.outerHeight
```

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Window/outerHeight)


+ ## window.scrollTo
```javascript
window.scrollTo(x-coord, y-coord)
```

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Window/scrollTo)


---
---

# document

+ ## element.clientHeight【只读】
```javascript
var h = element.clientHeight   //cssHeight + padding
```
![](https://developer.mozilla.org/@api/deki/files/185/=Dimensions-client.png)

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Element/clientHeight)


+ ## HTMLElement.offsetHeight【只读】
```javascript
var intElemOffsetHeight = element.offsetHeight   //cssHeight + padding +border
```
![](https://developer.mozilla.org/@api/deki/files/186/=Dimensions-offset.png)

[参考](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/offsetHeight)


+ ## Element.scrollHeight【只读】
```javascript
var intElemScrollHeight = element.scrollHeight   //entireHeight(容器总高度)
```
![](https://developer.mozilla.org/@api/deki/files/840/=ScrollHeight.png)

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Element/scrollHeight)


+ ## Element.clientTop【只读】
```javascript
vartop = element.clientTop   //border
```

[参考](https://developer.mozilla.org/zh-CN/docs/Web/API/Element/clientTop)


+ ## HTMLElement.offsetTop【只读】
```javascript
topPos = element.offsetTop   //offsetParent 距离
```

[参考](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/offsetTop)


+ ## Element.scrollTop【可写】
```javascript
var  intElemScrollTop = someElement.scrollTop
element.scrollTop = intValue   //滚动高度
```

[参考](https://developer.mozilla.org/en-US/docs/Web/API/Element/scrollTop)

---
---

# Event对象坐标

+ screenX和screenY （相对于用户屏幕）
+ clientX和clientY （相对于浏览器窗口）
+ pageX和pageY （相对于整张页面/包括隐藏部分）
+ offsetX和offsetY （相对于事件源）

---
---


参考：
+ [stackoverflow1](https://stackoverflow.com/questions/22675126/what-is-offsetheight-clientheight-scrollheight)  ：
+ [stackoverflow2](https://stackoverflow.com/questions/21064101/understanding-offsetwidth-clientwidth-scrollwidth-and-height-respectively) 
+ [掘金](https://juejin.im/entry/59772e9ef265da6c322e24f9)   
+ [读你](http://duni.sinaapp.com/?p=750)   
