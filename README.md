# python-wechaty-getting-started

Python Wechaty Starter Project Template that Works Out-of-the-Box

![PyPI Version](https://img.shields.io/pypi/v/wechaty?color=blue)
[![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-370/)

## Connecting Chatbots

[![Powered by Wechaty](https://img.shields.io/badge/Powered%20By-Wechaty-brightgreen.svg)](https://github.com/Wechaty/wechaty)

Wechaty is a RPA SDK for Wechat **Individual** Account that can help you create a chatbot in 6 lines of Python.

## The World's Shortest Python ChatBot: 6 lines of Code

```python
from wechaty import Wechaty

Wechaty.instance() // Global Instance
  .on('scan', lambda qrcode, status : print('Scan QR Code to login: {}\nhttps://api.qrserver.com/v1/create-qr-code/?data={}'.format(status, encodeURIComponent(qrcode))))
  .on('login', lambda user: print('User {} logined'.format(user)))
  .on('message', lambda message: print('Message: {}'.format(message)))
  .start()
```

## Requirements

1. Python 3.7+

## Install

```shell
make install
```

## Run

```shell
make bot
```

## Wechaty Getting Started in Multiple Languages

- [TypeScript Wechaty Getting Started](https://github.com/wechaty/wechaty-getting-started)
- [Python Wechaty Getting Started](https://github.com/wechaty/python-wechaty-getting-started)
- [Java Wechaty Getting Started](https://github.com/wechaty/java-wechaty-getting-started)
- [Go Wechaty Getting Started](https://github.com/wechaty/go-wechaty-getting-started)

## Copyright & License

- Code & Docs © 2020-now Wechaty <https://github.com/wechaty>
- Code released under the Apache-2.0 License
- Docs released under Creative Commons