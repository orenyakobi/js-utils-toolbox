# js-utils-toolbox
Useful copy &amp; paste util functions written in vanilla JS - Continiously grow and maintained.

__Enforsing HTTPS__
```javascript
if (location.protocol != 'https:')
{
 location.href = 'https:' + window.location.href.substring(window.location.protocol.length);
}
```
