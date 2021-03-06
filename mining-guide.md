---
title: Slimcoin mining guide
lang: en
category: help
ref: powguide
layout: page
permalink: /mining-guide/
---

### Solo mining

Solo mining is the simplest way to mine Slimcoin. It is done simply with the regular client or with a mining software ("miner"). When the difficulty is low, then solo mining becomes a profitable option.

You can mine Slimcoin with CPUs (recommended) or with GPUs (experimental).

#### Graphical client (Slimcoin-QT)

If you are using the graphical client, you can mine simply by introducing the following command in the RPC console (go to *Help* -> *Debug window* and open the *Console* tab):

```setgenerate true```

You can also specify how many cores of your CPU to use:

```setgenerate true NUMBER_OF_CORES```

with NUMBER_OF_CORES being the number you want to use. If you want to use all cores, type:

```setgenerate true -1```

To finalize mining, simply type:

```setgenerate false```


To get general mining information:

```getmininginfo```


**Important**: With the Slimcoin client - graphical or daemon - you only will be able to mine with the CPU, and the algorithm isn't optimized. So if you want maximal efficiency or use GPUs, use miner programs (see below).


#### Daemon (slimcoind)

You can start mining using the following command:

```slimcoind -gen```

followed by other options if you wand.

While the daemon is running, the same commands are available in the terminal like in the GUI client debug window. So you can start mining with the *setgenerate true* command like in the Debug console.


#### CPU Mining software (experimental)

To optimize mining, you can use the **Slimminer** software. It is experimental and may contain bugs.

Go to the [Slimminer Github Page](https://github.com/JonnyLatte/slimminer) and follow the instructions to install and mine.

#### GPU Mining software (experimental)

To be able to mine with a GPU, you can use the **SlimminerGPU** software. It is experimental and may contain bugs.

Go to the [Slimminer Github Page](https://github.com/JonnyLatte/slimminerGPU) and follow the instructions to install and mine.


### Pools

There are currently no working pools for Slimcoin. However there are initiatives to create a mining pool. Stay tuned!
