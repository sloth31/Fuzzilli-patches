# Target: JavaScriptCore

To build JavaScriptCore (jsc) for fuzzing:

1. Clone the WebKit mirror from https://github.com/WebKit/webkit
2. Apply Patches/\*. The patches should apply cleanly to the git revision specified in [./REVISION](./REVISION)
   (_Note_: If you clone WebKit from `git.webkit.org`, the commit hash will differ)
3. Run the fuzzbuild.sh script in the webkit root directory
4. FuzzBuild/Debug/bin/jsc will be the JavaScript shell for the fuzzer

### Tips 💡

```shell
$ clang -v

clang version 17.0.0 (https://github.com/swiftlang/llvm-project.git 2e6139970eda445d9c6872c0ca293088b4e63dd2)
Target: x86_64-unknown-linux-gnu
Thread model: posix
InstalledDir: /root/swift-6.0.3-RELEASE-ubuntu22.04/usr/bin
Found candidate GCC installation: /usr/lib/gcc/x86_64-linux-gnu/11
Selected GCC installation: /usr/lib/gcc/x86_64-linux-gnu/11
Candidate multilib: .;@m64
Selected multilib: .;@m64
```



