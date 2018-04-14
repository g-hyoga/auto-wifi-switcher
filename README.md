# auto-wifi-switcher

macのネットワーク環境を自動で切り替えるツールです

SSID一覧を監視し、変更があった場合にjobを実行します.
ここではKE-101-1というwifiが存在した場合nislabと名前のついたネットワーク環境に自動で切り替えます.

## Requirement 

 * nislabと名前のついたネットワーク環境をあらかじめ作成しておく必要があります.
 * SSIDがKE-101-1である前提で作られています.

![2018-04-14 13 19 59](https://user-images.githubusercontent.com/12538942/38764428-c00d2eaa-3fe9-11e8-8227-c5644b92eb2b.png)

### ネットワーク環境の名前もしくは、SSIDを指定のものと別のものを用いる場合

環境変数を変更することで変更できます.

```
LAB_NETWORK
LAB_SSID
```

という環境変数になっていますので、
変更してください.

もしくは,
./bin/auto-switch.sh の値を書き換えても良いです.

## 使いかた

```sh
make install
```
で終わりです

## アンインストールする

```sh
make uninstall
```

