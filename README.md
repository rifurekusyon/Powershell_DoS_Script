
# Powershell_DoS_Script(田代砲)


ただhttpリクエストをUA等を偽装して送りまくるだけです。


# 重要

- ##実験用又は教育目的の物です。他人のサイトやサービスに対しては絶対に使用しないでください。これに関する一切の責任は負いかねます。 Only for Educational Purposes ##

## お知らせ

- Microsoft edge がインストールしてある必要があります。
- PowerShell 7の使用を強く推奨
- ps1ファイルで実行するとパフォーマンスが低下します。
- TLSフィンガープリントをspoofする機能はありません。  



## 使い方

- Windows Powershelにコピペして実行できます。




## proxy
いくつかのproxyサーバを経由させる場合は以下のように記述されたproxy.txtをPowershellの実行するディレクトリに設置してください。
```
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
```


## 履歴

- http_flood6: DoS攻撃検知回避機能とproxyに対応しました。
- http_flood5: リクエストヘッダにUser Agent Client Hintsを追加
- http_flood4: リクエストヘッダの内容を変更しました。
- http_flood3: ユーザエージェントの他にリファラ等も偽装します。
- http_flood2: ダミーユーザエージェントの数が非常に多いやつです。
## Gif
![a](https://github.com/rifurekusyon/Powershell_DoS_Script/assets/108679694/5449735b-7366-40e0-bf89-fd864494f9ad)
