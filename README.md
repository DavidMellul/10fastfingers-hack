# 10fastfingers-hack
Copy-paste this in your browser console to get maximal words per minute  -> https://10fastfingers.com/typing-test/english

```javascript
var n_words = 100
var input = $('#inputfield')[0]
var ev = $.Event('keyup')
ev.which = 32
setInterval(function() {
    if ($('.highlight')[0]) {
        input.focus()
        input.value = $('.highlight').text()
        $(input).trigger(ev)
    }
}, 60000/n_words)
```
