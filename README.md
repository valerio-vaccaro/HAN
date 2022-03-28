# HAN
Han: ANother SOLOminer

## Introduction
HAN is a solo miner in a M5stack, using the ckpool. 

HAN is multicore and multithreads, each thread mine a different block template. After 1,000,000 trials the block in refreshed in order to avoid mining on old template.

# Configurations
All configurations are saved in the file `config.h`.

## Todos
- correctly calculate merkle root
- check if block match with provided target
- move on esp-idf
- log on sdcard
