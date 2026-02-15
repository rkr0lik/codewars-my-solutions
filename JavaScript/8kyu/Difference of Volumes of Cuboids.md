```javascript
function findDifference(a, b) {
 a = a[0]*a[1]*a[2];
 b = b[0]*b[1]*b[2];
  return (a>=b) ? a-b : b-a;
}
```