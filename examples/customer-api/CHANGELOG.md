# customer-api

## 0.0.3

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

## 0.0.2

### Patch Changes

- Sync up environment variable names across all example & type files. ([#1542](https://github.com/Shopify/hydrogen/pull/1542)) by [@michenly](https://github.com/michenly)

- Update all Node.js dependencies to version 18. (Not a breaking change, since Node.js 18 is already required by Remix v2.) ([#1543](https://github.com/Shopify/hydrogen/pull/1543)) by [@michenly](https://github.com/michenly)

- Update the return types of the Customer Account API query and mutation methods. Also update Customer Account API default version to 2024-01. ([#1537](https://github.com/Shopify/hydrogen/pull/1537)) by [@blittle](https://github.com/blittle)

- Updated dependencies [[`b2a350a7`](https://github.com/Shopify/hydrogen/commit/b2a350a754ea2d29bc267c260dc298a02f8f4470), [`9b4f4534`](https://github.com/Shopify/hydrogen/commit/9b4f453407338874bd8f1a1f619b607670e021d0), [`74ea1dba`](https://github.com/Shopify/hydrogen/commit/74ea1dba9af37a146882df7ed9674be5659862b5), [`2be9ce82`](https://github.com/Shopify/hydrogen/commit/2be9ce82fd4a5121f1772bbb7349e96ed530e84e), [`a9b8bcde`](https://github.com/Shopify/hydrogen/commit/a9b8bcde96c22cedef7d87631d429199810b4a7a), [`bca112ed`](https://github.com/Shopify/hydrogen/commit/bca112ed7db49e533fe49898b663fa0dd318e6ba), [`848c6260`](https://github.com/Shopify/hydrogen/commit/848c6260a2db3a9cb0c86351f0f7128f61e028f0), [`d53b4ed7`](https://github.com/Shopify/hydrogen/commit/d53b4ed752eb0530622a666ea7dcf4b40239cafa), [`961fd8c6`](https://github.com/Shopify/hydrogen/commit/961fd8c630727784f77b9f693d2e8ff8601969fc), [`2bff9fc7`](https://github.com/Shopify/hydrogen/commit/2bff9fc75916fa95f9a9279d069408fb7a33755c), [`c8e8f6fd`](https://github.com/Shopify/hydrogen/commit/c8e8f6fd233e52cf5570b1904af710d6b907aae5), [`8fce70de`](https://github.com/Shopify/hydrogen/commit/8fce70de32bd61ee86a6d895ac43cc1f78f1bf49), [`f90e4d47`](https://github.com/Shopify/hydrogen/commit/f90e4d4713c6c1fc1e921a7ecd08e95fe5da1744), [`e8cc49fe`](https://github.com/Shopify/hydrogen/commit/e8cc49feff18f5ee72d5f6965ff2094addc23466)]:
  - @shopify/cli-hydrogen@6.1.0
  - @shopify/remix-oxygen@2.0.2
  - @shopify/hydrogen@2023.10.3

## 1.0.0

### Breaking changes

- The Customer Account API example now uses an API client [included with Hydrogen](https://shopify.dev/docs/api/hydrogen/2023-10/utilities/createcustomerclient) (#38507) by @blittle.
