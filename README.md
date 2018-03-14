<<<<<<< HEAD
# XMRig AMD
[![Github All Releases](https://img.shields.io/github/downloads/xmrig/xmrig-amd/total.svg)](https://github.com/xmrig/xmrig-amd/releases)
[![GitHub release](https://img.shields.io/github/release/xmrig/xmrig-amd/all.svg)](https://github.com/xmrig/xmrig-amd/releases)
[![GitHub Release Date](https://img.shields.io/github/release-date-pre/xmrig/xmrig-amd.svg)](https://github.com/xmrig/xmrig-amd/releases)
[![GitHub license](https://img.shields.io/github/license/xmrig/xmrig-amd.svg)](https://github.com/xmrig/xmrig-amd/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/xmrig/xmrig-amd.svg)](https://github.com/xmrig/xmrig-amd/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/xmrig/xmrig-amd.svg)](https://github.com/xmrig/xmrig-amd/network)

XMRig is high performance Monero (XMR) OpenCL miner, with the official full Windows support.

GPU mining part based on [Wolf9466](https://github.com/OhGodAPet) and [psychocrypt](https://github.com/psychocrypt) code.

* This is the AMD (OpenCL) GPU mining version, there is also a [CPU version](https://github.com/xmrig/xmrig) and [NVIDIA GPU version](https://github.com/xmrig/xmrig-nvidia).
* [Roadmap](https://github.com/xmrig/xmrig/issues/106) for next releases.

:warning: Suggested values for GPU auto configuration can be not optimal or not working, you may need tweak your threads options. Please fell free open an [issue](https://github.com/xmrig/xmrig-amd/issues) if auto configuration suggest wrong values.

<img src="https://i.imgur.com/TFncsi7.png" width="696" >

#### Table of contents
* [Features](#features)
* [Download](#download)
* [Usage](#usage)
* [Build](https://github.com/xmrig/xmrig-amd/wiki/Build)
* [Donations](#donations)
* [Contacts](#contacts)

## Features
* High performance.
* Official Windows support.
* Support for backup (failover) mining server.
* CryptoNight-Lite support for AEON.
* Automatic GPU configuration.
* Nicehash support.
* It's open source software.

## Download
* Binary releases: https://github.com/xmrig/xmrig-amd/releases
* Git tree: https://github.com/xmrig/xmrig-amd.git
  * Clone with `git clone https://github.com/xmrig/xmrig-amd.git`  :hammer: [Build instructions](https://github.com/xmrig/xmrig-amd/wiki/Build).

## Usage
Use [config.xmrig.com](https://config.xmrig.com/amd) to generate, edit or share configurations.
=======
# Xrig
Xrig is a high performance cryptonight miner for AMD cards. Optimized for large-scale use of RX Vega.

GPU mining based on [Wolf9466](https://github.com/OhGodAPet) and [psychocrypt](https://github.com/psychocrypt) code. Forked from [XMRig AMD](https://github.com/xmrig/xmrig-amd)
<!--
<img src="https://i.imgur.com/TFncsi7.png" width="696" >
-->
## Features
* High performance
* Optimized for large-scale use of RX Vega
* Powerful API
* Hardware monitoring
* Built-in OverdriveN capabilities
* High level of auto configuration
* Windows and Linux support
* 1% dev donation

## Usage
>>>>>>> initial commit

### Command line options
```
  -a, --algo=ALGO           cryptonight (default) or cryptonight-lite
  -o, --url=URL             URL of mining server
<<<<<<< HEAD
  -O, --userpass=U:P        username:password pair for mining server
  -u, --user=USERNAME       username for mining server
  -p, --pass=PASSWORD       password for mining server
  -k, --keepalive           send keepalived for prevent timeout (need pool support)
  -r, --retries=N           number of times to retry before switch to backup server (default: 5)
  -R, --retry-pause=N       time to pause between retries (default: 5)
      --opencl-devices=N    list of OpenCL devices to use.
      --opencl-launch=IxW   list of launch config, intensity and worksize
      --opencl-affinity=N   affine GPU threads to a CPU
      --opencl-platform=N   OpenCL platform index
      --no-color            disable colored output
      --donate-level=N      donate level, default 5% (5 minutes in 100 minutes)
      --user-agent          set custom user-agent string for pool
  -B, --background          run the miner in the background
=======
  -u, --user=USERNAME       username for mining server
  -p, --pass=PASSWORD       password for mining server
  -k, --keepalive           send keepalive to prevent timeout (needs pool support)
      --intensity=N         thread intensity
      --platform-index=N    OpenCL platform index
      --no-color            disable colored output
  -b, --background          run the miner in the background
>>>>>>> initial commit
  -c, --config=FILE         load a JSON-format configuration file
  -l, --log-file=FILE       log all output to a file
      --nicehash            enable nicehash support
      --print-time=N        print hashrate report every N seconds
<<<<<<< HEAD
      --api-port=N          port for the miner API
      --api-access-token=T  access token for API
      --api-worker-id=ID    custom worker-id for API
  -h, --help                display this help and exit
  -V, --version             output version information and exit
```

## Donations
Default donation 5% (5 minutes in 100 minutes) can be reduced to 1% via command line option `--donate-level`.

* XMR: `48edfHu7V9Z84YzzMa6fUueoELZ9ZRXq9VetWzYGzKt52XU5xvqgzYnDK9URnRoJMk1j8nLwEVsaSWJ4fhdUyZijBGUicoD`
* BTC: `1P7ujsXeX7GxQwHNnJsRMgAdNkFZmNVqJT`

## Contacts
* support@xmrig.com
* [reddit](https://www.reddit.com/user/XMRig/)
=======
      --port=N              port for the miner API
      --api-access-token=T  access token for API
      --id=ID               miner id (defaults to machine name)
  -h, --help                display this help and exit
  -v, --version             output version information and exit
```

### Config file.
Sample config for an array of Vega's:
```json
{
    "algo": "cryptonight",
    "platform-index": 0,
    "intensity": 1932,
    "pools": [
        {
            "url": "pool.monero.hashvault.pro:5555",
            "user": "",
            "pass": "x"
        }
    ],
    "api": {
        "port": 4444
    }
}
```
>>>>>>> initial commit
