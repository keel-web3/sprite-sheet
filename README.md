# sprite-sheet

Equal-cell and JSON-atlas sprite sheet helpers with crisp pixel drawing.

A [KEEL](https://github.com/Ravonus/keel-modules) module: strict, readable
TypeScript that the platform minifies into the exact bytes published on chain,
with a hash-linked receipt binding the two.

## Verify it yourself

```bash
keel module build .
```

The build is deterministic, so it must print exactly:

```
output digest:  0xff354364eddaaa27628c03d8c80c77ed9e0c6f3c0f1d66b2023a3a920b62e624
```

If it prints anything else, the readable source in this repository is not the
source the published bytes were built from, and you should not trust it. You do
not have to take anyone's word for that, which is the entire point.

Run `keel module test .` to run the vectors in `test/vectors.mjs` against
both the readable source and the minified bytes.

## Where this comes from

This repository is a mirror. The source of truth is
[`keel-web3/render/sprite-sheet`](https://github.com/Ravonus/keel-modules/tree/master/modules/keel-web3/render/sprite-sheet)
in the keel-modules monorepo, at commit `c2e15084c24c7f8d4187f06b3a85347d6f4a0354`. Both trees build
to the same digest above; the mirror exists so this module can be depended on,
starred, and forked on its own.

## Licence

MIT. See LICENSE.
