#WebBench

***

Web Bench is very simple tool for benchmarking WWW or proxy servers. Uses fork() for simulating multiple clients and can use HTTP/0.9-HTTP/1.1 requests. This benchmark is not very realistic, but it can test if your HTTPD can realy handle that many clients at once (try to run some CGIs) without taking your machine down. Displays pages/min and bytes/sec. Can be used in more aggressive mode with -f switch.

[source code](http://home.tiscali.cz/~cz210552/webbench.html)

***

Webbench是一个在linux下使用的非常简单的网站压测工具。它使用fork()模拟多个客户端同时访问我们设定的URL，测试网站在压力下工作的性能，最多可以模拟3万个并发连接去测试网站的负载能力。Webbench使用C语言编写, 代码实在太简洁，源码加起来不到600行

***

## Example Usage

	/webbench http://www.zhihu.com/
	

## Output
	
	Webbench - Simple Web Benchmark 1.5
	Copyright (c) Radim Kolar 1997-2004, GPL Open Source Software.

	Benchmarking: GET http://www.zhihu.com/ (using HTTP/1.1)
	1 client, running 30 sec.

	Speed=124 pages/min, 20814 bytes/sec.
	Requests: 62 susceed, 0 failed.


> This open source C code is worth reading and I add some comment to the original file. Let's study together.

***
Follow [@louis1992](https://github.com/gzc) on github.