# Changelog

## [1.0.0](https://github.com/Meatwo310/custom-mdk-playground/compare/v0.1.0...v1.0.0) (2026-05-29)


### ⚠ BREAKING CHANGES

* GameTest Server runs and Fabric GameTest configuration are no longer created for Minecraft versions older than 26.1, and CI server runtime checks now branch by Minecraft version.

### Features

* **1.18.2-forge,1.19.2-forge,1.20.1-forge:** Mixin対応 ([9c19183](https://github.com/Meatwo310/custom-mdk-playground/commit/9c1918379e1a8aa01f3dfb172ed41c1efa0da6b2))
* **1.18.2,1.19.2,1.20.1,1.21.1:** バージョン別commonを実装 ([9d75b44](https://github.com/Meatwo310/custom-mdk-playground/commit/9d75b4487665d44b1a53aeb8f9c6e966f8697925))
* 1.18.2及び1.19.2のForgeをサブプロジェクトとして追加 ([a9f7269](https://github.com/Meatwo310/custom-mdk-playground/commit/a9f7269a785ee4ef35854e1ee6a68f7170d3d474))
* 1.18.2及び1.19.2のForgeをサブプロジェクトとして追加 ([26e3fb5](https://github.com/Meatwo310/custom-mdk-playground/commit/26e3fb53bdc86160fb91e84a5f7f4ddead74834f))
* **1.20.1-fabric,1.21.1-fabric:** fabricの対応バージョンを部分的に拡張 ([dbe585a](https://github.com/Meatwo310/custom-mdk-playground/commit/dbe585ad5da59da855c96354643740e80a64f1b6))
* 1.20.1-forge サブプロジェクトを追加 ([93df8c7](https://github.com/Meatwo310/custom-mdk-playground/commit/93df8c77bc80542f7aa340ce354794a05b390f7e))
* 1.21.1-neoをサポート ([32ad70d](https://github.com/Meatwo310/custom-mdk-playground/commit/32ad70dee13396c0c63d26be2aabb0b9d270fbcd))
* **1.21.11-fabric:** バージョン追加 ([557a178](https://github.com/Meatwo310/custom-mdk-playground/commit/557a178c45ccb7e14811e4acc95cc6ada25ed066))
* **1.21.8-fabric:** バージョン追加 ([e4b2938](https://github.com/Meatwo310/custom-mdk-playground/commit/e4b2938c3ad64693d9c2d2bd6d9f663462b4d4b6))
* **26.1-fabric:** GameTestを有効化 ([590e449](https://github.com/Meatwo310/custom-mdk-playground/commit/590e4496a64f6051c606494dc817b84d328de924))
* 26.1-fabricをサポート ([3fcfeb3](https://github.com/Meatwo310/custom-mdk-playground/commit/3fcfeb32ef3621c5f6827b33996e97b95e482d0f))
* 26.1.2サブプロジェクトを追加 ([a2e48f9](https://github.com/Meatwo310/custom-mdk-playground/commit/a2e48f994fac42f58552dd4c909b92bdb3472eef))
* add 26.1-common subproject with ModDevGradle Vanilla Mode ([cb6e59d](https://github.com/Meatwo310/custom-mdk-playground/commit/cb6e59d62129742e5afcddea4c9bbfabcafc6b41))
* add 26.1-common subproject with ModDevGradle Vanilla Mode ([a679a93](https://github.com/Meatwo310/custom-mdk-playground/commit/a679a93498115c944e563ad12f5122805bbc83ca))
* add common subproject and move MODID to Constants ([846cc06](https://github.com/Meatwo310/custom-mdk-playground/commit/846cc0695313b177f4e83874cb7bf6722cf4ce01))
* Constantsをインスタンス化不可能に ([3630eab](https://github.com/Meatwo310/custom-mdk-playground/commit/3630eab4039fbca9a48a02730534fa31421dff66))
* gate server runtime checks by Minecraft version ([45a6a2d](https://github.com/Meatwo310/custom-mdk-playground/commit/45a6a2d2740bb68ea083c12e3714675f31baea89))
* コンフィグの抽象化と共通化 ([#54](https://github.com/Meatwo310/custom-mdk-playground/issues/54)) ([605821e](https://github.com/Meatwo310/custom-mdk-playground/commit/605821ec6b8c608ee1c1469b0bd838b4f30bcd77))
* マルチプロジェクトのテストも兼ねて起動時のロギングを追加 ([888b159](https://github.com/Meatwo310/custom-mdk-playground/commit/888b159beed3b19932eaa34835c4223657a56790))


### Bug Fixes

* :common を api 依存に変更して Constants クラスを推移的に公開する ([c5462f4](https://github.com/Meatwo310/custom-mdk-playground/commit/c5462f45e3ba0c760a68817b07c0fc6bd5e81ace))
* **1.18.2-common,1.19.2-common,1.20.1-common,1.21.1-common:** Forge/Neoの介入が入っていないソースを使用するように ([2fafaec](https://github.com/Meatwo310/custom-mdk-playground/commit/2fafaec9fd446ed952fe159c2af408aee49c6d98)), closes [#34](https://github.com/Meatwo310/custom-mdk-playground/issues/34)
* **1.18.2-forge,1.19.2-forge,1.20.1-forge:** Mixinクラスが一つもないときでもビルドが通るように ([1974c85](https://github.com/Meatwo310/custom-mdk-playground/commit/1974c859339518035d9cdd7154c4c99323237625))
* **1.18.2-forge,1.19.2-forge,1.20.1-forge:** ランタイムでmixins.jsonが読めるように ([8862aa6](https://github.com/Meatwo310/custom-mdk-playground/commit/8862aa6fa1abe782b6bfe09d988e2a7c4065eaf4))
* **1.21.1-neo,26.1-neo:** mixins.jsonにminVersionを指定 ([23b27fe](https://github.com/Meatwo310/custom-mdk-playground/commit/23b27feacb358cb33aeaf3a62e68c1f24075b25b))
* 26.1-common のソースセットを NeoForge の mods ブロックに追加 ([5d282c1](https://github.com/Meatwo310/custom-mdk-playground/commit/5d282c1800cd04eae996e76e4f974d200276200f))
* **26.1-fabric:** modidの正しい指定 ([5dbb570](https://github.com/Meatwo310/custom-mdk-playground/commit/5dbb570bf8c1b97678a651ed84663bc33047107a))
* **26.1-neo:** runDataを別ディレクトリで実行 ([8aff573](https://github.com/Meatwo310/custom-mdk-playground/commit/8aff573a6fd7f35fbfb2d3b028f8efba7ce2752a))
* commonサブプロジェクトをModから正しく呼び出せるように ([7700420](https://github.com/Meatwo310/custom-mdk-playground/commit/77004206235067fb20cae596d2e0d088643a16c6))
* enable stdin for Fabric runServer task ([aee1f8a](https://github.com/Meatwo310/custom-mdk-playground/commit/aee1f8a831d6e09537a078e8a44c76889ef4caba))
* **forge:** デバッグログが正しく表示されるように ([746a1a7](https://github.com/Meatwo310/custom-mdk-playground/commit/746a1a7598bf3a582b82e250fcfdfa73e0558141))
* ModDevGradleおよびLegacyのバージョンを統一しIDEAで正しく同期できるように ([d5b93c0](https://github.com/Meatwo310/custom-mdk-playground/commit/d5b93c0a5b86f5ee40031b34f06bc445ab50656f))
* namespaceにスラッシュは使えないらしい(なんで動いてたんだ？) ([4f52b39](https://github.com/Meatwo310/custom-mdk-playground/commit/4f52b39ea5acc0eff6732f205b6b8a25b791cb62))
* 実環境にサブプロジェクトのコードが含まれるように ([6bf8120](https://github.com/Meatwo310/custom-mdk-playground/commit/6bf81200bc5e316d227bf26293dca29aac77e9d8))
* 正しいコンストラクタ ([9f160d3](https://github.com/Meatwo310/custom-mdk-playground/commit/9f160d39d19c4de77823740fc8558e2c1cebaf79))
* 残留コンフィグを削除 ([ca898e9](https://github.com/Meatwo310/custom-mdk-playground/commit/ca898e927ae0bab2a34b252e88bfe0a4e7d6a4d2))


### Reverts

* build: rootProject.nameをmodIdから自動設定 ([6172262](https://github.com/Meatwo310/custom-mdk-playground/commit/61722628629c567136647e3f9033835059b8ead4))

## Changelog
