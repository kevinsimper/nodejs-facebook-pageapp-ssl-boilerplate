Boilerplate Node.js Facebook app
=======================================

A boilerplate on how to get started with self signed node.js express app.

Since Facebook made Secure Browsing default and no way for developers to avoid I have countless times used time to setup this boilerplate code to be able to debug directly on facebook.com.

This boilerplate is also made with Heroku in mind where you can get free SSL on ".herokuapp.com", but since you do not have to use SSL between the load balancer and the node, you do not use the same code on production.

This also contains a key and a crt with no real details, and since the key and crt is now public, do not use them in production, do only use them for development.

The way you are going to use it is by changing your host file to the same url that your real app is going to be. So is your app going to on myawesomeapp.com you type in your host file:

  127.0.0.1 myawesomeapp.com
  
Then you start this node.js application up and now you are running on localhost and can use your app exactly like you would in production.

Now you can access the signed_request that facebook sends.

https://developers.facebook.com/docs/reference/login/signed-request/
