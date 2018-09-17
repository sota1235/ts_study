test_filesize
====

Type definition of [filesize](https://www.npmjs.com/package/filesize) does not work well.

This is for investigating the reason.

### Error

```
> test_filesize@1.0.0 build /Users/sota1235/src/ts_study/test_filesize
> tsc

src/index.ts:3:13 - error TS2349: Cannot invoke an expression whose type lacks a call signature. Type '{ partial: (options: Options) => (bytes: number) => string; }' has no compatible call signatures.

3 console.log(fileSize(10));
              ~~~~~~~~~~~~

  src/index.ts:1:1
    1 import * as fileSize from 'filesize';
      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    Type originates at this import. A namespace-style import cannot be called or constructed, and will cause a failure at runtime. Consider using a default import or import require here instead.
```
