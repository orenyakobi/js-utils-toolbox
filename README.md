# js-utils-toolbox
Useful copy &amp; paste util functions written in vanilla JS - Continiously grow and maintained.

* [Enforcing HTTPS](#enforce-https)
* [Checking the existence of a nested object key](#is-defined)

# <a name="enforce-https"></a>Enforcing HTTPS
```javascript
function enforceHTTPS(){
  if (location.protocol != 'https:'){
    location.href = 'https:' + window.location.href.substring(window.location.protocol.length);
  }
}
```

# <a name="is-defined"></a>Checking the existence of a nested object key
```javascript
function isDefined(obj, path) {
  let pathItems = path.split('.');

  for (let i = 0; i < pathItems.length; i++) {
    if (!obj || !obj[pathItems[i]]) {
      return false;
    }
    obj = obj[pathItems[i]];
  }
  return true;
}
```
