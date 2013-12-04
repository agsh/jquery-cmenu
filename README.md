jquery-cmenu
========
``` javascript
$.cmenu.showMenu([{
  caption: 'Caption'
  , icon: 'arrow_right'
  , disabled: true
  , execute: function() {
    alert('yo');
  }
}, {
  caption: 'Caption'
  , icon: 'arrow_right'
  , disabled: true
  , execute: function() {
    alert('yo');
  }
  , submenu: [{
    caption: 'Inner caption'
    , type: 'checkbox'
  }]
}]);
```
