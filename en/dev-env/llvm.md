# LLVM

## Official Guides

{% embed url="https://llvm.org/" %}

{% embed url="https://llvm.org/docs/LangRef.html" %}

### Kaleidoscope

{% embed url="https://llvm.org/docs/tutorial/index.html" %}

{% embed url="https://llvm.org/docs/tutorial/MyFirstLanguageFrontend/index.html" %}

### Garbage Collection

{% embed url="https://llvm.org/docs/GarbageCollection.html" %}

### LLVM Pass

{% embed url="https://llvm.org/docs/WritingAnLLVMPass.html" %}

{% embed url="https://llvm.org/docs/Passes.html" %}

## Issues

#### Could NOT find ZSTD (missing: ZSTD\_LIBRARY ZSTD\_INCLUDE\_DIR)

{% embed url="https://reviews.llvm.org/D128465" %}

{% embed url="https://bugs.launchpad.net/ubuntu/+source/libzstd/+bug/1941956" %}

{% embed url="https://reviews.llvm.org/D134990" %}

```
sudo apt install -y libzstd-dev libdwarf-dev
```

#### FileCheck Not Found

```bash
ln /usr/bin/FileCheck-16 /usr/bin/FileCheck
```

#### ZLIB Not Found

```log
[cmake] CMake Error at /usr/lib/llvm-18/lib/cmake/llvm/LLVMExports.cmake:73 (set_target_properties):
[cmake]   The link interface of target "LLVMSupport" contains:
[cmake] 
[cmake]     ZLIB::ZLIB
[cmake] 
[cmake]   but the target was not found.  Possible reasons include:
[cmake] 
[cmake]     * There is a typo in the target name.
[cmake]     * A find_package call is missing for an IMPORTED target.
[cmake]     * An ALIAS target is missing.
[cmake] 
[cmake] Call Stack (most recent call first):
[cmake]   /usr/lib/llvm-18/cmake/LLVMConfig.cmake:369 (include)
[cmake]   CMakeLists.txt:25 (find_package)
```
