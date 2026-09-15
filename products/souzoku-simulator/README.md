# Souzoku Simulator Releases

`Souzoku_simulator`（相続対策シミュレーター）の公開更新ファイル用名前空間です。

## 公開順序

1. 更新済み `.xlsm` を `products/souzoku-simulator/releases/<version>/` 配下へ配置する。
2. 配布ファイルの SHA-256 を計算する。
3. `latest.json` の `version`、`downloadUrl`、`sha256`、`releaseNotes` を更新する。
4. 最後に `customerReady` を `true` にする。

`latest.json` を先に公開しないでください。更新ファイルとSHA-256が揃うまで `customerReady: false` を維持します。

## 例

配布パス:

`products/souzoku-simulator/releases/1.3.1/SouzokuSimulator_1.3.1.xlsm`

`downloadUrl` は、この公開リポジトリ内の raw URL または GitHub Release URL を指定します。

## 安全設計

クライアント側は、この公開リポジトリを指すURL以外を拒否し、ダウンロード後に `latest.json` の SHA-256 と一致する場合だけ更新を適用します。
