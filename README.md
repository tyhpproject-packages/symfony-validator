<!-- tyhp-readme:start -->
# tyhpdef/symfony-validator

Tyhp type definitions for `symfony/validator` `7.4.19`.

```bash
composer require --dev tyhpdef/symfony-validator:7.4.19
```

This is a metapackage. Composer also installs `tyhpdef/symfony-validator-impl` (type files).
Require **this** name, not `tyhpdef/symfony-validator-impl`.

See https://tyhplang.com.

## Maintain `symfony/validator`? Ship the types yourself

If you are a Packagist maintainer of `symfony/validator`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-validator-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/validator` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-validator": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/validator` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/validator` with a real constraint,
   `"replace": { "tyhpdef/symfony-validator": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/validator` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-validator` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
