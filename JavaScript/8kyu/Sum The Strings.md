```javascript
function sumStr(a,b) {
  return ((parseInt(a) || 0) + (parseInt(b) || 0)).toString();
}
```

```javascript
function sumStr(a,b) {
return ((parseInt('0' + a)) + parseInt('0' + b)).toString();
}
```