# Changelog

## Unpublished

### 🛠 Breaking changes

- Removed support for the Classic Updates service for SDK 50 ([announcement](https://blog.expo.dev/sunsetting-expo-publish-and-classic-updates-6cb9cd295378)). Specifically, references to the Classic Updates CDN were removed. [Migrate](https://docs.expo.dev/eas-update/migrate-from-classic-updates/) to EAS or other service that conforms to the modern [Expo Updates protocol](https://docs.expo.dev/technical-specs/expo-updates-1/). ([#25613](https://github.com/expo/expo/pull/25613) by [@ide](https://github.com/ide))

### 🎉 New features

- Added support for React Native 0.73.0. ([#24971](https://github.com/expo/expo/pull/24971), [#25453](https://github.com/expo/expo/pull/25453) by [@gabrieldonadel](https://github.com/gabrieldonadel))

### 🐛 Bug fixes

### 💡 Others

- Removed references to legacy `bundledAssets` constant from `expo-file-system` that was used only in standalone apps. ([#25484](https://github.com/expo/expo/pull/25484) by [@tsapeta](https://github.com/tsapeta))

## 8.14.0 — 2023-11-14

### 🐛 Bug fixes

- fix URLs in development. ([#25202](https://github.com/expo/expo/pull/25202) by [@EvanBacon](https://github.com/EvanBacon))

### 💡 Others

- Collapse re-export of `react-native/Libraries/Image/AssetRegistry` to `@react-native/assets-registry/registry`. ([#25265](https://github.com/expo/expo/pull/25265) by [@EvanBacon](https://github.com/EvanBacon))
- Migrate to new standard `URL` support on native. ([#24941](https://github.com/expo/expo/pull/24941) by [@EvanBacon](https://github.com/EvanBacon))
- Renamed `unimodule.json` to `expo-module.config.json`. ([#25100](https://github.com/expo/expo/pull/25100) by [@reichhartd](https://github.com/reichhartd))

## 8.13.0 — 2023-10-17

### 🐛 Bug fixes

- URL encode asset paths defined as query parameter. ([#24562](https://github.com/expo/expo/pull/24562) by [@byCedric](https://github.com/byCedric))

## 8.12.1 — 2023-09-16

_This version does not introduce any user-facing changes._

## 8.12.0 — 2023-09-04

### 🛠 Breaking changes

- Convert `../` to `_` for the property `httpServerLocation` in `hashAssetFiles` (Metro asset pre-processor) to support assets in monorepos the same everywhere. ([#24090](https://github.com/expo/expo/pull/24090) by [@EvanBacon](https://github.com/EvanBacon))

## 8.11.0 — 2023-08-02

_This version does not introduce any user-facing changes._

## 8.10.1 — 2023-06-24

_This version does not introduce any user-facing changes._

## 8.10.0 — 2023-06-13

_This version does not introduce any user-facing changes._

## 8.9.2 — 2023-05-08

### 🐛 Bug fixes

- Fixed monorepo asset resolution in production for Metro web. ([#22094](https://github.com/expo/expo/pull/22094) by [@EvanBacon](https://github.com/EvanBacon))

## 8.9.1 - 2023-03-08

### 🐛 Bug fixes

- Fixed `@react-native/assets-registry` module not found issue on Web. ([#21469](https://github.com/expo/expo/pull/21469) by [@kudo](https://github.com/kudo))

## 8.9.0 — 2023-02-09

_This version does not introduce any user-facing changes._

## 8.8.0 — 2023-02-03

### 🐛 Bug fixes

- Fix loading Metro web assets from origins other than `/`. ([#20258](https://github.com/expo/expo/pull/20258) by [@EvanBacon](https://github.com/EvanBacon))

### 💡 Others

- Remove unused web features. ([#20258](https://github.com/expo/expo/pull/20258) by [@EvanBacon](https://github.com/EvanBacon))

## 8.6.2 — 2022-10-25

_This version does not introduce any user-facing changes._

## 8.6.1 — 2022-07-19

_This version does not introduce any user-facing changes._

## 8.6.0 — 2022-07-07

_This version does not introduce any user-facing changes._

## 8.5.0 — 2022-04-18

### 💡 Others

- Swap out Cloudfront CDN for `classic-assets.eascdn.net`. ([#15781](https://github.com/expo/expo/pull/15781)) by [@quinlanj](https://github.com/quinlanj)

## 8.4.6 - 2022-01-13

### 🐛 Bug fixes

- Fix missing `getManifest2()` function on web. ([#15891](https://github.com/expo/expo/pull/15891)) by [@jonsamp](https://github.com/jonsamp) ([#15891](https://github.com/expo/expo/pull/15891) by [@jonsamp](https://github.com/jonsamp))

## 8.4.5 — 2021-12-21

### 🐛 Bug fixes

- Fix an issue preventing the loading of assets using expo-updates manifests during local development. ([#15667](https://github.com/expo/expo/pull/15667)) by [@jonsamp](https://github.com/jonsamp)

## 8.4.4 — 2021-11-17

### 🐛 Bug fixes

- Fix `fromModule` on restrictive (Snack) web environments. ([#14435](https://github.com/expo/expo/pull/14435) by [@IjzerenHein](https://github.com/IjzerenHein))

## 8.4.1 — 2021-10-01

### 💡 Others

- Updated `@testing-library/react-hooks` to version `7.0.1`. ([#14552](https://github.com/expo/expo/pull/14552)) by [@Simek](https://github.com/Simek))

## 8.4.0 — 2021-09-08

### 🎉 New features

- Reapply [#12624](https://github.com/expo/expo/pull/12624) ([#13789](https://github.com/expo/expo/pull/13789) by [@jkhales](https://github.com/jkhales))

## 8.3.2 — 2021-04-21

### 🎉 New features

- Find local assets without extensions. ([#12624](https://github.com/expo/expo/pull/12624) by [@jkhales](https://github.com/jkhales))

## 8.3.1 — 2021-03-23

### 🐛 Bug fixes

- Removed annoying yellowbox warning message in bare workflow when there's no manifest available. ([#12237](https://github.com/expo/expo/pull/12237) by [@bbarthec](https://github.com/bbarthec))

## 8.3.0 — 2021-03-10

### 🐛 Bug fixes

- Remove peerDependencies and unimodulePeerDependencies from Expo modules. ([#11980](https://github.com/expo/expo/pull/11980) by [@brentvatne](https://github.com/brentvatne))

## 8.2.2 — 2021-01-15

_This version does not introduce any user-facing changes._

## 8.2.1 — 2020-11-17

_This version does not introduce any user-facing changes._

## 8.2.0 — 2020-08-18

### 🎉 New features

- Add `useAssets` hook to simplify assets handling. ([#8928](https://github.com/expo/expo/pull/8928) by [@bycedric](https://github.com/bycedric))

### 🐛 Bug fixes

- Fixed `Asset.loadAsync()` TypeScript signature to match `Asset.fromModule()` types. ([#9246](https://github.com/expo/expo/pull/9246) by [@barthap](https://github.com/barthap))

## 8.1.7 — 2020-05-29

_This version does not introduce any user-facing changes._

## 8.1.6 — 2020-05-27

_This version does not introduce any user-facing changes._

## 8.1.5

### 🎉 New features

- `asset.downloadAsync()` returns the resolved `Asset` when it resolves. ([#8646](https://github.com/expo/expo/pull/8646) by [@EvanBacon](https://github.com/EvanBacon))
- `Asset.loadAsync()` returns an array of resolved `Asset`s when it finishes loading the resources. ([#8646](https://github.com/expo/expo/pull/8646) by [@EvanBacon](https://github.com/EvanBacon))
- Added support for the `expo-updates` **no-publish workflow**. ([#8003](https://github.com/expo/expo/pull/8003) by [@esamelson](https://github.com/esamelson))
