# lint-debug

Provides [`elm-lint`](https://package.elm-lang.org/packages/jfmengels/elm-lint/latest) rules to detect debug code.


## Provided rules

- [`NoDebug`](./NoDebug) - Reports uses or imports of the [`Debug` module](https://package.elm-lang.org/packages/elm/core/latest/Debug).


## Configuration

```elm
module LintConfig exposing (config)

import Lint.Rule exposing (Rule)
import NoDebug

config : List Rule
config =
    [ NoDebug.rule
    ]
```
