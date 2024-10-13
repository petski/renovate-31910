# 31910

## Current behavior

In the PR that bumps `gedmo/doctrine-extensions` [^1], Renovate bumps `symfony/cache` (dependency of `gedmo/doctrine-extensions`) to version `7.x`

[^1]: https://github.com/petski/renovate-31910/pull/1/files

## Expected behavior

Because `symfony/flex` is installed and `extra.symfony.require` is set to `6.4.*`, and `symfony/cache` is under the Symfony umbrella (see discussion), Renovate should keep `symfony/cache` in `6.4.*`

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/31910

# Handy commands

```
docker run -i -t --rm -v $(pwd):/src -w /src composer:latest bash
```

```
docker run -i -t --rm -v $(pwd):/src -w /src -e LOG_LEVEL=debug renovate/renovate --platform=local
```
