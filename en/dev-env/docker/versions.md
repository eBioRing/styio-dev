# Versions

## Standard

```sh
docker build -t sio https://github.com/eBioRing/styio-dev-env.git#main:docker/std
```

{% embed url="https://github.com/eBioRing/styio-dev-env/blob/main/docker/std/Dockerfile" %}

### Pre-Installed Packages

* [**Debian**](https://www.debian.org/)
* [CMake](https://cmake.org/)
* [Clang](https://releases.llvm.org/16.0.0/tools/clang/docs/index.html) + [LLVM](https://releases.llvm.org/16.0.0/docs/ReleaseNotes.html) (Version **16**)
* [Python](https://www.python.org/)
* [Node.js](https://nodejs.org/en)
* [GitHub Client](https://cli.github.com/manual/)

### Customized Environment Variables

* `clang` : Alias of `/usr/bin/clang-16`
* `clang++` : Alias of `/usr/bin/clang++-16`
* `CC` : Let CMake use Clang instead of GCC.
* `CXX` : Let CMake use Clang++ instead of G++.

### Directories

1. `/root/styio` : Styio compiler workspace, which is a `git` repository with a `.devcontainer/devcontainer.json` configuration file. For more details:&#x20;
   * [Dev container specification.](https://containers.dev/implementors/spec/)
   * [Change the default source code mount.](https://code.visualstudio.com/remote/advancedcontainers/change-default-source-mount)
   * [Develop on a remote container host.](https://code.visualstudio.com/remote/advancedcontainers/develop-remote-host)
