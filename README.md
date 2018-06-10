# js-utils-toolbox
Useful copy &amp; paste util functions written in vanilla JS

__Enforsing HTTPS__
```javascript
if (location.protocol != 'https:')
{
 location.href = 'https:' + window.location.href.substring(window.location.protocol.length);
}
```
