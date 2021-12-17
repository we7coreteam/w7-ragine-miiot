[![Php Version](https://img.shields.io/badge/php-%3E=7.1-brightgreen.svg)](https://secure.php.net/)
[![Swoole Version](https://img.shields.io/badge/swoole-%3E=4.3.0-brightgreen.svg)](https://github.com/swoole/swoole-src)
[![Rangine Framework Version](https://img.shields.io/badge/rangine-%3E=0.0.1-brightgreen.svg)](https://github.com/we7coreteam/w7-rangine)
[![Illuminate Database Version](https://img.shields.io/badge/illuminate/database-%3E=5.6.0-brightgreen.svg)](https://github.com/illuminate/database)
[![Rangine Doc](https://img.shields.io/badge/docs-passing-green.svg?maxAge=2592000)](https://wiki.w7.cc/chapter/1?id=1175#)


# 介绍

本项目是基于软擎框架开发，可接入米家Iot平台。实现自有硬件与小米平台互联。

# 项目配置

使用前请先配置 config/common.php 下的相关信息。

oauth.client_id 随机生成，将来填写到小米Iot平台

oauth.client_secret 随机生成，将来填写到小米Iot平台

oauth.redirect_uri 小米Iot平台回调地址，由平台生成，填写到项目中


key.encrypt_key 加密串，随机生成，32位即可

key.private 私钥，通过 openssl genrsa -out private.key 2048 命令生成

key.public 公钥，通过 openssl rsa -in private.key -pubout -out public.key 命令生成


#小米Iot平台配置

账号授权URL： http://mydomain/oauth/authorize

Client ID： common.php 中定义的 oauth.client_id

Client Secret： common.php 中定义的 oauth.client_secret

Access Token URL：http://mydomain/oauth/access-token/code

Refresh URL：http://mydomain/oauth/access-token/refresh

设备指令接受URL：


# 教程

 - 第一节 https://www.bilibili.com/video/BV1e34y167Y5/
 - 第二节 https://www.bilibili.com/video/BV1FL4y1n7ne/
 - 第三节 https://www.bilibili.com/video/BV1Mi4y1o7vL/











