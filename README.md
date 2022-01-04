Using `packages` `entrypointStrategy`, cross-package references are broken.

Reproduce steps:

- Install dependencies: `yarn`
- Generate TypeDoc: `yarn typedoc`

Output:

```
$ yarn typedoc
Warning: A, defined at packages/a/lib/index.d.ts:3, is referenced by @typedoc-packages-missing-export/b.B.__type.a but not included in the documentation.
Info: Documentation generated at ./docs
```
