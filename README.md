# Json Web Tokens(JWT) Authorization Example

This repository contains code for the article found at: https://medium.com/@maison.moa/using-jwt-json-web-tokens-to-authorize-users-and-protect-api-routes-3e04a1453c3e

This example is not meant to be production ready, rather an example of how to use JWT. This codebase utalizes Node.js with an Express server.

#### To install:
```bash
{
  git clone https://github.com/MichaelDimmitt/jwt_auth_example.git;
  cd jwt_auth_example;
  npm install; 
  node server/server.js
}
```

#### To use
In browser console

```javascript
authToken= "add your token"
fetch('/user/data', {
  method: 'GET',
  headers: {
    'Authorization': 'Bearer' + authToken
  }
})
.then(res => res.json())
.then(data => { console.log(data) })
.catch(err => { console.log(err) })
```

Thanks for looking 💙

