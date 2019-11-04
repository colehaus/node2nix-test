Nix expressions created with:

```sh
node2nix --development --nodejs-10 --input package.json --lock package-lock.json
```

and `node2nix` 1.7.0.

`nix-build` results in:

```
...
unpacking source archive /nix/store/c5ypihc9zspkbss213k6bkg37y7lzppn-yargs-8.0.2.tgz
unpacking source archive /nix/store/x1rklhxzrn40yyphrfv68k28nmfjsyph-yargs-parser-7.0.0.tgz
pinpointing versions of dependencies...
undefined:1
{
^

SyntaxError: Unexpected token  in JSON at position 0
    at JSON.parse (<anonymous>)
    at resolveDependencyVersion (/nix/store/xd73i06lnwlz8jz1b7h2x85qa0r0hf83-pinpointDependencies.js:11:45)
    at resolveDependencyVersion (/nix/store/xd73i06lnwlz8jz1b7h2x85qa0r0hf83-pinpointDependencies.js:17:20)
    at resolveDependencyVersion (/nix/store/xd73i06lnwlz8jz1b7h2x85qa0r0hf83-pinpointDependencies.js:17:20)
    at replaceDependencies (/nix/store/xd73i06lnwlz8jz1b7h2x85qa0r0hf83-pinpointDependencies.js:25:35)
    at Object.<anonymous> (/nix/store/xd73i06lnwlz8jz1b7h2x85qa0r0hf83-pinpointDependencies.js:40:1)
    at Module._compile (internal/modules/cjs/loader.js:776:30)
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:787:10)
    at Module.load (internal/modules/cjs/loader.js:653:32)
    at tryModuleLoad (internal/modules/cjs/loader.js:593:12)
builder for '/nix/store/7m4ragd0jidq2qi4bzmc6ng502516sp3-node_node2nix-test-0.1.0.drv' failed with exit code 1
error: build of '/nix/store/7m4ragd0jidq2qi4bzmc6ng502516sp3-node_node2nix-test-0.1.0.drv', '/nix/store/r3q9m1sm4g7bmsbhzbg7bd8rn40mga9c-node-shell-node2nix-test-0.1.0.drv' failed

```
