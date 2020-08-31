我是光年实验室高级招聘经理。
我在github上访问了你的开源项目，你的代码超赞。你最近有没有在看工作机会，我们在招软件开发工程师，拉钩和BOSS等招聘网站也发布了相关岗位，有公司和职位的详细信息。
我们公司在杭州，业务主要做流量增长，是很多大型互联网公司的流量顾问。公司弹性工作制，福利齐全，发展潜力大，良好的办公环境和学习氛围。
公司官网是http://www.gnlab.com,公司地址是杭州市西湖区古墩路紫金广场B座，若你感兴趣，欢迎与我联系，
电话是0571-88839161，手机号：18668131388，微信号：echo 'bGhsaGxoMTEyNAo='|base64 -D ,静待佳音。如有打扰，还请见谅，祝生活愉快工作顺利。

# Consul [![Build Status](https://travis-ci.org/hashicorp/consul.png)](https://travis-ci.org/hashicorp/consul)

* Website: http://www.consul.io
* IRC: `#consul` on Freenode
* Mailing list: [Google Groups](https://groups.google.com/group/consul-tool/)

Consul is a tool for service discovery and configuration. Consul is
distributed, highly available, and extremely scalable.

Consul provides several key features:

* **Service Discovery** - Consul makes it simple for services to register
  themselves and to discover other services via a DNS or HTTP interface.
  External services such as SaaS providers can be registered as well.

* **Health Checking** - Health Checking enables Consul to quickly alert
  operators about any issues in a cluster. The integration with service
  discovery prevents routing traffic to unhealthy hosts and enables service
  level circuit breakers.

* **Key/Value Storage** - A flexible key/value store enables storing
  dynamic configuration, feature flagging, coordination, leader election and
  more. The simple HTTP API makes it easy to use anywhere.

* **Multi-Datacenter** - Consul is built to be datacenter aware, and can
  support any number of regions without complex configuration.

Consul runs on Linux, Mac OS X, and Windows. It is recommended to run the
Consul servers only on Linux, however.

## Quick Start

An extensive quick quick start is viewable on the Consul website:

http://www.consul.io/intro/getting-started/install.html

## Documentation

Full, comprehensive documentation is viewable on the Consul website:

http://www.consul.io/docs

## Developing Consul

If you wish to work on Consul itself, you'll first need [Go](https://golang.org)
installed (version 1.4+ is _required_). Make sure you have Go properly installed,
including setting up your [GOPATH](https://golang.org/doc/code.html#GOPATH).

Next, clone this repository into `$GOPATH/src/github.com/hashicorp/consul` and
then just type `make`. In a few moments, you'll have a working `consul` executable:

```
$ go get -u ./...
$ make
...
$ bin/consul
...
```

*note: `make` will also place a copy of the binary in the first part of your $GOPATH*

You can run tests by typing `make test`.

If you make any changes to the code, run `make format` in order to automatically
format the code according to Go standards.

### Building Consul on Windows

Make sure Go 1.4+ is installed on your system and that the Go command is in your
%PATH%.

For building Consul on Windows, you also need to have MinGW installed.
[TDM-GCC](http://tdm-gcc.tdragon.net/) is a simple bundle installer which has all
the required tools for building Consul with MinGW.

Install TDM-GCC and make sure it has been added to your %PATH%.

If all goes well, you should be able to build Consul by running `make.bat` from a
command prompt.

See also [golang/winstrap](https://github.com/golang/winstrap) and
[golang/wiki/WindowsBuild](https://github.com/golang/go/wiki/WindowsBuild)
for more information of how to set up a general Go build environment on Windows
with MinGW.

