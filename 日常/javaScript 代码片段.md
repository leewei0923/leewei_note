
## # Intl
```javaScript
const number = "12345678";

const f = new Intl.NumberFormat('zh-hans-cn', {
    currency: 'RMB',
    style: 'currency'
});

console.log(f.format(number));

```