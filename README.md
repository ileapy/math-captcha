<h1 align="left"><a href="https://www.kuzuozhou.cn">math-aptcha</a></h1>

一个简单的学术运算验证码库，基于GD库编写。

## 依赖

PHP >= 5.6  
GD库扩展

## 安装

```shell
$ composer require cfn/math-captcha
```


## 示例

```php
<?php

use MathCaptcha\Captcha;

$ca = new Captcha();
$code = $ca->setDigits(1)->setPoint(100)->setLine(2)->setFontSize(24)->result();
print_r("验证码结果：" . $code . "\n");
$image = $ca->base64();
print_r($image);

```

## 作者

邮箱：cfn@leapy.cn<br/>
微信：SH-CFN<br/>

## 支持🌙

您的支持就是我们最大的动力，本项目接受任何形式的捐赠，您也可以star支持本项目。

## License

MIT
