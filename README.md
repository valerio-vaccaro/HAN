# HAN
Han: ANother SOLOminer

![main screen](https://github.com/valerio-vaccaro/HAN/raw/main/screenshots/main.jpeg)

WARNING: you may have to wait longer than the current age of the universe to find a valid block.

## Introduction
HAN is a solo miner in a M5stack, using the ckpool. 

HAN is multicore and multithreads, each thread mine a different block template. After 1,000,000 trials the block in refreshed in order to avoid mining on old template.

Community available on telegram channel [t.me/hansolominer](https://t.me/hansolominer).

## Configurations
All configurations are saved in the file `config.h`.

Wifi can be set using `WIFI_SSID` and `WIFI_PASSWORD` constants.

`THREADS` defines the number of concurrent threads used, every thread will work on a different template.

Every thread will use a progressive nonce from 0 to `MAX_NONCE`, when nonce will be equal to `MAX_NONCE` a new template will be downloaded and nonce will be reset to 0.

Funds will go to the address writte in `ADDRESS`.

`POOL_URL` and `POOL_PORT` are used for select the solo pool.

## Todos

- improve hasing using sha256 middle state 
- move on M5Unified
- move on esp-idf
- log on sdcard

