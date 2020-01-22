# algoDiffArrayJS
Compare two arrays and return a new array with any items only found in one of the two given arrays, but not both. In other words, return the symmetric difference of the two arrays.
```javascript
function diffArray(arr1, arr2) {
  var newArr =arr1.concat(arr2);
  // Same, same; but different.
  function diff(x){
    if(arr1.indexOf(x)==-1|| arr2.indexOf(x)==-1){
      return x;
    }
    
  }
  return newArr.filter(diff);
}

diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);

```
