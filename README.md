<!-- tyhp-readme:start -->
# tyhpdef/phpstan-phpstan-doctrine

Tyhp type definitions for `phpstan/phpstan-doctrine` `2.0.28`.

```bash
composer require --dev tyhpdef/phpstan-phpstan-doctrine:2.0.28
```

This is a metapackage. Composer also installs `tyhpdef/phpstan-phpstan-doctrine-impl` (type files).
Require **this** name, not `tyhpdef/phpstan-phpstan-doctrine-impl`.

See https://tyhplang.com.

## Maintain `phpstan/phpstan-doctrine`? Ship the types yourself

If you are a Packagist maintainer of `phpstan/phpstan-doctrine`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/phpstan-phpstan-doctrine-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `phpstan/phpstan-doctrine` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/phpstan-phpstan-doctrine": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `phpstan/phpstan-doctrine` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `phpstan/phpstan-doctrine` with a real constraint,
   `"replace": { "tyhpdef/phpstan-phpstan-doctrine": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `phpstan/phpstan-doctrine` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/phpstan-phpstan-doctrine` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
