Simple Go script demonstrating use of the [Heroku Platform API build resource](https://devcenter.heroku.com/articles/build-and-release-using-the-api)

How to use:

```term
$ git clone git@github.com:heroku/buildapi-go-example.git
...
$ go build
$ heroku create
Creating limitless-fjord-5604... done, stack is cedar
...
$ ./main -apikey <api-key> -app limitless-fjord-5604 -archive https://github.com/heroku/node-js-sample/archive/master.tar.gz
.........
-----> Node.js app detected
-----> Requested node range:  0.10.x
-----> Resolved node version: 0.10.28
-----> Downloading and installing node
...
```

You can get your api key by running `heroku auth:token` or from the [account page on Dashboard](https://dashboard.heroku.com/account).
