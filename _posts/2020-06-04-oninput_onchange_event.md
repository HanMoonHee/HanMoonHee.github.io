---
layout: post
title:  "[javascript]oninput, onchange란?"
date:   2020-06-04 00:00:00 +0700
categories: [javascript]
---
### 1. oninput

***oninput*** 요소의 값이 변경된 직후 발생하는 이벤트이다.

```html
<input type="text" id="myInput" value="Mickey">
```

```javascript
document.getElementById("myInput").oninput = function() {myFunction()};

function myFunction() {
    alert("The value of the input field was changed.");
}
```

### 2. onchange

***onchange*** 는 SELECT BOX를 이용해 어떤 이벤트를 실행하고자 할 때는 주로 onchange 이벤트를 사용한다.

input이나 select 등의 데이터가 변경될 때 호출되는 이벤트이다.

```html
<input type="text" id="myInput" onchange="myFunction()">
```

```javascript
function myFunction() {
  var x = document.getElementById("myInput").value;
  document.getElementById("demo").innerHtml = "You Wrote: " + x;
}
```
