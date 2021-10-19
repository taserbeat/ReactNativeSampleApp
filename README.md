# ReactNativeSampleApp

React Native のサンプルアプリ

# 環境構築

- Xcode

  開発中に iOS シミュレータを使用するために必要  
  また、ビルドして実機確認するためにも必須

- yarn または npm

  インストールについては割愛

- [CocoaPods](https://cocoapods.org/)

  iOS のライブラリ管理ツール  
  [参考](https://qiita.com/satoken0417/items/479bcdf91cff2634ffb1)

  Homebrew でもインストールできるみたいだが、うまくいかなかったので`gem`でインストールした。

  ```bash
  sudo gem install cocoapods
  ```

- [Watchman](https://facebook.github.io/watchman/)

  React Native を開発した facebook が推奨しているファイル変更管理ツール

  ```bash
  brew install watchman
  ```

# 実行方法

```bash
# iOSシミュレータを起動
open -a Simulator

# CocoaPodsで管理しているライブラリをios/Podfile.lockから復元
cd ios
pod install
cd ..

# iOSシミュレータでアプリを起動
yarn ios
```

# 参考

[【入門】はじめての React Native](https://qiita.com/nskydiving/items/41e446ef5c821359ab79)
