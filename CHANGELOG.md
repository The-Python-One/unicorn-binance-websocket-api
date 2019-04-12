# unicorn-binance-websocket-api Change Log

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to [Semantic Versioning](http://semver.org/).

## 1.1.6.dev (development stage)

## 1.1.6
### Fix
- catching "ssl.SSLError" BinanceWebSocketApiConnection.receive()
- improvment of reconnect on invalid URI caused by no network issue and a missing listen_key from Binance

## 1.1.5
### Fix
- Reconnect issue on userData stream
- Reset "has_stopped" attr from "stream_list" after a conncection restart
- Modyfied docstrings descriptions
- Tabs in print_summary() on windows
### Adding
- 30 min cache for Binance "listenKey" from rest api to avoid weight costs and hammering the Binance API on a 
flapping network connection