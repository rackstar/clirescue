你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
# CLI Rescue exercise

## Setup

1. Start by forking this repo so you have your own copy.
2. clone the repo in your Go path:

``` bash
go get github.com/$github_user/clirescue.git
cd $GOPATH/src/github.com/clirescue
```

Install the dependencies:

``` bash
go get github.com/codegangsta/cli
```

Load the project into your editor and do a search and replace:

* Replace: `github.com/GoBootcamp`
* With: `github.com/<github-username>`

Commit the change:

``` bash
git commit -a -m "forking repo requires internal code changes"
```

If everything is properly setup, you should be able to run your code:

``` bash
go run main.go me
```

You can use the following demo Pivotal Tracker account:

* Username: gobootcamp
* Password: santamonica


## Start rescuing

This code was written by someone who just started learning Go.
Beginners often make the same mistakes so assume that this is your code
and you are now tasked to refactor it.
The end goal is to create a CLI to interface with the [Pivotal Tracker
API](https://www.pivotaltracker.com/help/api/rest/v5).

The current code is asking the user for a username and password, the user details are fetched.
Your first step might be to store the user token on the drive so next time the program is called, it can automatically load the user details be without asking for the user's username and password.

### A few hints:

* Understanding Go path's system might be a bit tricky at first.
* Forking the repo might affect your import statements.
* The original author might not have made a good use of packages.
* You more thna likely have some OOP experience, you might want to
  leverage it in this exercise.
* Checkout the `init` function.
* Curious about how a 3rd party lib works? Try go doc.
* Simpler is better.
* Look into how to write tests.
* Bonus point for removing 3rd part dependencies.

As always, refer to the [Effective Go doc](http://golang.org/doc/effective_go.html) and [the go bootcamp book](http://www.golangbootcamp.com/book) if you have any questions.


### Existing refactors

* [@campoy](https://github.com/campoy) and [@evanphx](https://github.com/evanphx) did a public refactor in Santa Monica (March 2014) [see fork](https://github.com/campoy/cliRescue) and [godoc](http://godoc.org/github.com/campoy/clirescue)
