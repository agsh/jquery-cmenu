testTask
========
Есть jquery-плагин выпадающего меню jquery.cmenu.js и стиль для него style.less. Статья про него тут: http://habrahabr.ru/post/43111/
Добавляются выпадающие меню методом bindMenu как-то так:
``` javascript
$('#one').bindMenu([['Я пункт меню', 'arrow_left', function(e) {alert('hi');}]]);
```
Для каждого меню создаются свои div, которые появляются при клике. В примере ```test.html``` это выглядит так:
``` html
<div class="cmenu" iuid="3"></div>
<div class="cmenu" iuid="4"></div>
<div class="cmenu" iuid="5"></div>
<div class="cmenu" iuid="0" style="display: none; left: 208px; top: 9px;">
<div class="cmenu" iuid="1" style="display: none; left: 208px; top: 209px;">
<div class="cmenu" iuid="2" style="display: none; left: 208px; top: 409px;">
```
Это не очень хорошо. Хочется доработать плагин, чтобы div, представляющий меню, был один. А при клике на какой-либо div меню соответствующим образом заполнялось, он позиционировался и появлялся.
