## ExaProxy

ExaProxy is a a high-performance non-caching proxy. It is able to filter HTTP traffic using your favorite programming language.

It was part of Exa Networks' [SurfProtect](http://www.surfprotect.co.uk/) solution, but has been replaced by a new codebase in Golang.

Exaproxy is used in production since early 2013, and proxies millions of URL per day, one installation sees Gb/s of HTTP traffic, with hundreds of Mb/s per server, and several tens of thousands of connections per machine, but this does not mean our work is finished. We continue to improve it.

## News

August 21st 2014, released ExaProxy 1.2.1

## Features

 * Non-caching HTTP/HTTPS (with CONNECT) Proxy
  * forward, reverse or transparent proxy
  * IPv6 and/or IPv4 support (can act as a 4to6 or 6to4 gateway)
 * High Performance
 * Working with the "upcoming" web services
   * support for unknown HTTP versions
   * websocket and TLS support (Upgrade header support)
 * Traffic interception
   * [SQUID compatible](http://www.squid-cache.org/Doc/config/url_rewrite_program/) interface
   * [ICAP like](http://www.faqs.org/rfcs/rfc3507.html) interface via local program
 * Support for [HAProxy proxy protocol](http://haproxy.1wt.eu/download/1.5/doc/proxy-protocol.txt)
 * Built-in web servers to monitor the proxy via local webpage ( default http://127.0.0.1:8080 )
   * dynamic configuration change
   * running information in json format (/json)

## Usage

Start ExaProxy on your local machine and point your browser to 127.0.0.1 port 8000
