# third-party-queries-caching

## 1.0.1

### Patch Changes

- 👩‍💻 improved HydrogenSession typing. ([#1590](https://github.com/Shopify/hydrogen/pull/1590)) by [@michenly](https://github.com/michenly)

  In order to ensure utilies from @shopify/hydrogen will work properly using user implemented HydrogenSession class. We encourage the use of `HydrogenSession` type to ensure all the interface needed had been implemented.

  Update implementation of HydrogenSession using type

  ```diff
  import {
  + type HydrogenSession,
  } from '@shopify/hydrogen';
  - class HydrogenSession {
  + class AppSession implements HydrogenSession {
      ...
  }
  ```

- Updated dependencies [[`8c477cb5`](https://github.com/Shopify/hydrogen/commit/8c477cb565c3e018bf4e13bad01804c21611fb8a), [`fb38d3b7`](https://github.com/Shopify/hydrogen/commit/fb38d3b7cf108aecca6f7eb6f08c88bc7f46aa4c), [`07d1b0b5`](https://github.com/Shopify/hydrogen/commit/07d1b0b5e62ff2d149deac80ce6fbe95d2b0f8ce), [`4d6ba3ff`](https://github.com/Shopify/hydrogen/commit/4d6ba3ffc7ddc72f1b97eff3c7188fe72b8568e7), [`d6d01322`](https://github.com/Shopify/hydrogen/commit/d6d01322b430761c6ac3be71aa8fee798c85de37), [`a69c21ca`](https://github.com/Shopify/hydrogen/commit/a69c21caa15dfedb88afd50f262f17bf86f74836), [`970073e7`](https://github.com/Shopify/hydrogen/commit/970073e78258880505e0de563136b5379d5d24af), [`94509b75`](https://github.com/Shopify/hydrogen/commit/94509b750afefd686971198ed86277e2c70f3176), [`cce65795`](https://github.com/Shopify/hydrogen/commit/cce6579580f849bec9a28cf575f7130ba3627f6b), [`b1a1d7cb`](https://github.com/Shopify/hydrogen/commit/b1a1d7cba9f6eac50cbf459965e92814e4de1be9), [`b0d727d1`](https://github.com/Shopify/hydrogen/commit/b0d727d1f2bb643827e2fda438cfc447de7ee2e7), [`f6e6d194`](https://github.com/Shopify/hydrogen/commit/f6e6d1943680304b15f0892c64c726d79291fe0a), [`306d302a`](https://github.com/Shopify/hydrogen/commit/306d302ab401f22e5317fd84587c6a37cf931912)]:
  - @shopify/cli-hydrogen@6.2.0
  - @shopify/hydrogen@2023.11.0
