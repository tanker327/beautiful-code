#Utitly

#[camelcase](https://github.com/sindresorhus/camelcase/blob/master/index.js)
```js
   function camelize(str) {
      str = str.trim();
    
      if (str.length === 1 || !(/[_.\- ]+/).test(str)) {
        return str;
      }
    
      return str
        .replace(/^[_.\- ]+/, '')
        .toLowerCase()
        .replace(/[_.\- ]+(\w|$)/g, function (m, p1) {
          return p1.toUpperCase();
        });
    };
```
