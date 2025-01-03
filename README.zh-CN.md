<p align="center">
    <a href="https://github.com/swoft-cloud/swoft" target="_blank">
        <img src="http://qiniu.daydaygo.top/swoft-logo.png?imageView2/2/w/300" alt="swoft"/>
    </a>
</p>

[![Latest Stable Version](http://img.shields.io/packagist/v/swoft/swoft.svg)](https://packagist.org/packages/swoft-fork/swoft)
[![Build Status](https://travis-ci.org/swoft-cloud/swoft.svg?branch=master)](https://travis-ci.org/swoft-cloud/swoft)
[![Docker Build Status](https://img.shields.io/docker/build/swoft/swoft.svg)](https://hub.docker.com/r/swoft/swoft/)
[![Php Version](https://img.shields.io/badge/php-%3E=8.0-brightgreen.svg?maxAge=2592000)](https://secure.php.net/)
[![Swoole Version](https://img.shields.io/badge/swoole-%3E=4.3.3-brightgreen.svg?maxAge=2592000)](https://github.com/swoole/swoole-src)
[![Swoft Doc](https://img.shields.io/badge/docs-passing-green.svg?maxAge=2592000)](https://www.swoft.org)
[![Swoft License](https://img.shields.io/hexpm/l/plug.svg?maxAge=2592000)](https://github.com/swoft-cloud/swoft/blob/master/LICENSE)
[![Gitter](https://img.shields.io/gitter/room/swoft-cloud/swoft.svg)](https://gitter.im/swoft-cloud/community)

![start-http-server](https://raw.githubusercontent.com/swoft-cloud/swoft/master/public/image/start-http-server.jpg)

PHP 高性能微服务协程框架

**注意：**

本仓库fork于github swoft库，只测试了swoole4.8.13，php8.2对应版本环境，请慎用于你的生产环境，不负责积极代码维护。如需查看文档请访问原框架文档。

> **[EN README](README.md)**

## 简介

Swoft 是一款基于 Swoole 扩展实现的 PHP 微服务协程框架。Swoft 能像 Go 一样，内置协程网络服务器及常用的协程客户端且常驻内存，不依赖传统的 PHP-FPM。有类似 Go 语言的协程操作方式，有类似 Spring Cloud 框架灵活的注解、强大的全局依赖注入容器、完善的服务治理、灵活强大的 AOP、标准的 PSR 规范实现等等。

Swoft 通过长达三年的积累和方向的探索，把 Swoft 打造成 PHP 界的 Spring Cloud, 它是 PHP 高性能框架和微服务治理的最佳选择。

## 功能特色

- 内置高性能网络服务器（Http/Websocket/RPC/TCP）
- 灵活的组件功能
- 强大的注解功能
- 多样化的命令终端（控制台）
- 强大的面向切面编程（AOP）
- 容器管理，依赖注入（DI）
- 灵活的事件机制
- 基于PSR-7的HTTP消息的实现
- 基于PSR-14的事件管理
- 基于PSR-15的中间件
- 国际化（i18n）支持
- 简单有效的参数验证器
- 高性能连接池（Mysql/Redis/RPC），自动重新连接
- 数据库高度兼容Laravel的使用方式
- Redis高度兼容Laravel的使用方式
- 秒级定时任务
- 进程池
- 高效的任务处理
- 灵活的异常处理
- 强大的日志系统
- 服务注册与发现
- 配置中心
- 服务限流
- 服务降级
- 服务熔断
- Apollo
- Consul

## 在线文档

- [中文文档](https://www.swoft.org/documents/v2/index.html)
- [English](http://swoft.io/docs/2.x/en)

## 学习交流

- QQ Group3: 541038173
- QQ Group2: 778656850(已满)
- QQ Group1: 548173319(已满)
- [swoft-cloud/community](https://gitter.im/swoft-cloud/community)

## 免费技术支持

![support](https://www.swoft.org/src/images/technical-support.png)

## Requirement

- [PHP 7.1+](https://github.com/php/php-src/releases)
- [Swoole 4.8.13](https://github.com/swoole/swoole-src/releases)
- [Composer](https://getcomposer.org/)

## Install

### Composer

```bash
composer create-project swoft-fork/swoft swoft
```

## Start

- Http server

```bash
[root@swoft swoft]# php bin/swoft http:start
```

- WebSocket server

```bash
[root@swoft swoft]# php bin/swoft ws:start
```

- RPC server

```bash
[root@swoft swoft]# php bin/swoft rpc:start
```

## 核心组件

Component Name   | Packagist Version
--------------------|---------------------
swoft-annotation          |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/annotation.svg)](https://packagist.org/packages/swoft-fork/annotation)
swoft-config              |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/config.svg)](https://packagist.org/packages/swoft-fork/config)
swoft-db                  |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/db.svg)](https://packagist.org/packages/swoft-fork/db)
swoft-framework           |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/framework.svg)](https://packagist.org/packages/swoft-fork/framework)
swoft-i18n                |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/i18n.svg)](https://packagist.org/packages/swoft-fork/i18n)
swoft-proxy               |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/proxy.svg)](https://packagist.org/packages/swoft-fork/proxy)
swoft-rpc-client          |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/rpc-client.svg)](https://packagist.org/packages/swoft-fork/rpc-client)
swoft-stdlib              |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/stdlib.svg)](https://packagist.org/packages/swoft-fork/stdlib)
swoft-tcp-server          |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/tcp-server.svg)](https://packagist.org/packages/swoft-fork/tcp-server)
swoft-aop                 |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/aop.svg)](https://packagist.org/packages/swoft-fork/aop)
swoft-connection-pool     |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/connection-pool.svg)](https://packagist.org/packages/swoft-fork/connection-pool)
swoft-error               |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/error.svg)](https://packagist.org/packages/swoft-fork/error)
swoft-http-message        |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/http-message.svg)](https://packagist.org/packages/swoft-fork/http-message)
swoft-log                 |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/log.svg)](https://packagist.org/packages/swoft-fork/log)
swoft-redis               |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/redis.svg)](https://packagist.org/packages/swoft-fork/redis)
swoft-rpc-server          |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/rpc-server.svg)](https://packagist.org/packages/swoft-fork/rpc-server)
swoft-task                |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/task.svg)](https://packagist.org/packages/swoft-fork/task)
swoft-validator           |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/validator.svg)](https://packagist.org/packages/swoft-fork/validator)
swoft-bean                |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/bean.svg)](https://packagist.org/packages/swoft-fork/bean)
swoft-console             |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/console.svg)](https://packagist.org/packages/swoft-fork/console)
swoft-event               |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/event.svg)](https://packagist.org/packages/swoft-fork/event)
swoft-http-server         |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/http-server.svg)](https://packagist.org/packages/swoft-fork/http-server)
swoft-process             |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/process.svg)](https://packagist.org/packages/swoft-fork/process)
swoft-rpc                 |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/rpc.svg)](https://packagist.org/packages/swoft-fork/rpc)
swoft-server              |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/server.svg)](https://packagist.org/packages/swoft-fork/server)
swoft-tcp                 |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/tcp.svg)](https://packagist.org/packages/swoft-fork/tcp)
swoft-websocket-server    |   [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/websocket-server.svg)](https://packagist.org/packages/swoft-fork/websocket-server)

## 扩展组件

Component Name   | Packagist Version
-----------------|---------------------
swoft-apollo  | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/apollo.svg)](https://packagist.org/packages/swoft-fork/apollo)
swoft-breaker | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/breaker.svg)](https://packagist.org/packages/swoft-fork/breaker)
swoft-cache  | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/cache.svg)](https://packagist.org/packages/swoft-fork/cache)
swoft-crontab | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/crontab.svg)](https://packagist.org/packages/swoft-fork/crontab)
swoft-consul  | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/consul.svg)](https://packagist.org/packages/swoft-fork/consul)
swoft-limiter | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/limiter.svg)](https://packagist.org/packages/swoft-fork/limiter)
swoft-view    | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/view.svg)](https://packagist.org/packages/swoft-fork/view)
swoft-whoops  | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/whoops.svg)](https://packagist.org/packages/swoft-fork/whoops)
swoft-session  | [![Latest Stable Version](http://img.shields.io/packagist/v/swoft/session.svg)](https://packagist.org/packages/swoft-fork/session)

## License

Swoft is an open-source software licensed under the [LICENSE](LICENSE)
