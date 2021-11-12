## Docker image for cpuminer-gr-aarch64

Build:
```
./build.sh
```

Usage:
```
docker run --rm -e POOL=stratum+tcp://eu.flockpool.com:4444 -e WALLET=<WALLET.WORKER> mthoring/cpuminer-gr-aarch64
```

