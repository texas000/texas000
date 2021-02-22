# How to use github api for blogging

_You can still manage your website contents by using CMS, but as a developer it is much easier to use github repository as a CMS_

Here is the basic instruction for the [github api](https://docs.github.com/en/rest)

1. Github API Base URI - https://api.github.com
2. Get Client ID and Client Secrte credentials from github setting
3. Try API with credentials **Base Uri + /repos/yourUsername/yourUsername/readme**

Here is how you can encode with base64 at javascript

```javascript
Buffer.from(`${CLIENT_ID}:${CLIENT_SECRTE}`, "binary").toString("base64");
```

Save this as a variable and place this at the api header, Authorization, and it will all set

Thank you for reading ;)
