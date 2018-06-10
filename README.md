# js-utils-toolbox
Useful copy &amp; paste util functions written in vanilla JS - Continiously grow and maintained.

* [Enforcing HTTPS](#enforcing-https)

# <a name="enforcing-https"></a>Enforcing HTTPS
```javascript
if (location.protocol != 'https:')
{
 location.href = 'https:' + window.location.href.substring(window.location.protocol.length);
}
```
