# FriedPotato：プロセカ創作譜面サーバー

https://potato.purplepalette.net に少しだけ機能を追加したサーバー。
https://fp.sevenc7c.com から遊ぶことが出来ます。
また、 https://fp.sevenc7c.com/tests/テストサーバーID でテストサーバーに接続できます。

## 追加機能

- 背景画像の追加
- 中間点の音変更
- 旧譜面変換
- エンジンの差し替え

## 必須事項

- Ruby 3.0以上
- DXRubyが動く環境
- bundler

## 動かし方

1. [Rubyをインストールします。](https://rubyinstaller.org)[Ruby3.0、x86](https://github.com/oneclick/rubyinstaller2/releases/download/RubyInstaller-3.0.3-1/rubyinstaller-devkit-3.0.3-1-x86.exe)が推奨です。
1. PCを再起動します。
1. 右上のCodeボタンから`Download ZIP`でZipをダウンロードします。
1. 適当なところに解凍します。
1. `setup.bat`を起動します。
1. `launch.bat`を起動します。
1. Sonolusに画面のサーバーをカスタムサーバーとして登録します。
2. `（サーバー）/tests/テストサーバーID` でテストサーバーに接続できます。

2回目以降は`launch.bat`を動かせばサーバーを起動できます。

## 背景生成

背景の生成を有効にするには3つの方法があります。

### Web(Python)
1. 1度FriedPotatoを起動します。
3. config.ymlを開き、`background_engine`を`web`にします。

### DXRuby(Ruby)

1. 1度FriedPotatoを起動します。
2. [DXRubyの環境を整えます。](https://qiita.com/noanoa07/items/7df5886c619781d8d2ee#-d3dx9_40dll%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E6%96%B9%E6%B3%95)
3. config.ymlを開き、`background_engine`を`dxruby`にします。

### Pillow(Python)

1. 1度FriedPotatoを起動します。
2. [ここ](https://python.org/downloads/)か[ここ](https://pythonlinks.python.jp/ja/index.html)からPythonをダウンロードします。推奨は3.9.xです。
3. PCを再起動します。
4. `setup_python.bat`を起動します。
5. `background_engine`を`pillow`にします。


## ライセンス

GPLv3で公開しています。
