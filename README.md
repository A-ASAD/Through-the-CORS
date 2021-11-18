# Through-the-CORS
A service to bypass CORS from client side. The application is hosted on heroku at following URL:  
```
https://through-the-cors.herokuapp.com
```
There's no homepage, so you'll get nothing at this URL.
## USAGE

Through the CORS is really simple to use. You just need to copy the following URL, use it as the target URL, and replace "your url" with the respective URL.
```
`https://through-the-cors.herokuapp.com/get?url=${encodeURIComponent("your url")}`
```

It will return the exact JSON response received from the server.

A sample request will look like this:
```
fetch(`https://through-the-cors.herokuapp.com/get?url=${encodeURIComponent('http://example.com/movies.json')}`)
  .then(response => response.json())
  .then(data => console.log(data));
```

#### This service is intended to be used for developemnt purposes only.
