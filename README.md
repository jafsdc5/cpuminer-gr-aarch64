## Docker image for cpuminer-gr-aarch64

Verified working on Apple M1 Air with Docker Desktop for MacOS.

Build:
```
./build.sh
```

Usage:
```
docker run --rm -e POOL=stratum+tcp://eu.flockpool.com:4444 -e WALLET=<WALLET.WORKER> mthoring/cpuminer-gr-aarch64
```

License: MIT
