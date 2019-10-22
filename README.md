# 10fastfingers-hack
Copy-paste this in your browser console to get maximal words per minute  -> https://10fastfingers.com/typing-test/english

```javascript
(function () {
    const input = document.querySelector('input[type=text]');

    const e = new KeyboardEvent('keyup', {
        which: 32,
        keyCode: 32,
    });

    setInterval(function() {
        const highlight = document.querySelector('.highlight');

        input.focus();
        input.value = highlight && highlight.textContent || '';
        input.dispatchEvent(e);
    }, 200);
})();
```
