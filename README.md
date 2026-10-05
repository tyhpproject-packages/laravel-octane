<!-- tyhp-readme:start -->
# tyhpdef/laravel-octane

Tyhp type definitions for `laravel/octane` `2.19.1`.

```bash
composer require --dev tyhpdef/laravel-octane:2.19.1
```

This is a metapackage. Composer also installs `tyhpdef/laravel-octane-impl` (type files).
Require **this** name, not `tyhpdef/laravel-octane-impl`.

See https://tyhplang.com.

## Maintain `laravel/octane`? Ship the types yourself

If you are a Packagist maintainer of `laravel/octane`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-octane-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/octane` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-octane": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/octane` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/octane` with a real constraint,
   `"replace": { "tyhpdef/laravel-octane": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/octane` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-octane` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
