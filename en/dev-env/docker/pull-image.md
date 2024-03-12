# Pull Image

## Build From Dockerfile

#### Standard Version

Debian 12, LLVM 18

```bash
docker build -t styio https://github.com/eBioRing/styio-dev-env.git#main:docker/std
```

#### Lite Version

Debian 12, LLVM 18

```
docker build -t styio-lite https://github.com/eBioRing/styio-dev-env.git#main:docker/lite
```

#### Lite Image for China

Debian 12, LLVM 18

```bash
docker build -t styio-cn-d12-l18 https://github.com/eBioRing/styio-dev-env.git#main:docker/cn/debian-12-llvm-18
```

### Download Image

