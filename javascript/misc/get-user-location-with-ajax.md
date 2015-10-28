#Get user location with ajax

```js
$.ajax({
  url: 'http://ipinfo.io/',
  type: 'GET',
  dataType: 'jsonp',
  timeout: 5000,

  success: (response) => {
    /*
    response = {
      "ip": "xxx.xx.xxx.xxx",
      "hostname": "xxx.xx.xxx.xxx.xxxxxx.xxxx.xx",
      "city": "City",
      "region": "State",
      "country": "XX",
      "loc": "-11.5167,-31.9333",
      "org": "Telecom",
      "postal": "XXXXX"
    }
    */
  },

  error: (XHR, textStatus, errorThrown) => {
    if (textStatus === 'timeout') {
      // error
    }
  }
});
```
