你好！
很冒昧用这样的方式来和你沟通，如有打扰请忽略我的提交哈。我是光年实验室（gnlab.com）的HR，在招Golang开发工程师，我们是一个技术型团队，技术氛围非常好。全职和兼职都可以，不过最好是全职，工作地点杭州。
我们公司是做流量增长的，Golang负责开发SAAS平台的应用，我们做的很多应用是全新的，工作非常有挑战也很有意思，是国内很多大厂的顾问。
如果有兴趣的话加我微信：13515810775  ，也可以访问 https://gnlab.com/，联系客服转发给HR。
# autobatch

Autobatch is an implementation of
[go-datastore](https://github.com/ipfs/go-datastore) that automatically batches
together writes by holding puts in memory until a certain threshold is met.
This can improve disk performance at the cost of memory in certain situations.

## Usage

Simply wrap your existing datastore in an autobatching layer like so:

```go
bds := NewAutoBatching(basedstore, 128)
```

And make all future calls to the autobatching object.

## License
MIT
