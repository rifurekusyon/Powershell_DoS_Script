
# Powershell_DoS_Script(田代砲)


ただhttp GET/POSTをUA等を偽装して送りまくるだけです。


# 重要

- 実験用又は教育目的の物です。他人のサイトやサービスに対しては絶対に使用しないでください。これに関する一切の責任は負いかねます。 Only for Educational Purposes

## 要件
- Microsoft edge がインストールしてある必要があります。
- PowerShell-7.3.6の使用を強く推奨 (既存のPowershellでも動くが7のほうがパフォーマンスが良い)
  - x64msi https://github.com/PowerShell/PowerShell/releases/download/v7.3.6/PowerShell-7.3.6-win-x64.msi
  - x64zip https://github.com/PowerShell/PowerShell/releases/download/v7.3.6/PowerShell-7.3.6-win-x64.zip


## 使い方とか諸々

- Windows Powershellにコピペして実行できます。
- cookieは送信しない場合何も入力せずEnterを押してください。


## お知らせ

- 低スぺの方はhttp_flood6を使用してください。
- ps1ファイルとして実行するとパフォーマンスが低下します。
- 性能に余裕のある端末では複数のターミナルウィンドウで同時に実行可能です。(proxyを使うときはこれをおすすめします)
- bypass Dos detectionを有効にするとスループットが低下します。


## proxy
いくつかのproxyサーバを経由させる場合は以下のように記述されたproxy.txtをPowershellの実行するカレントディレクトリに設置してください。  
(http_flood6,7のみ)
(例) 
```
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
XX.XX.XX.XX:port
```


## 履歴
- http_flood7: URLと<href>タグから得たサーバのディレクトリをランダムに選んで訪問するように仕様変更しました。
- http_flood6: DoS攻撃検知回避機能とproxyに対応しました。
  - これらの機能を使うとスループットが低下します。
- http_flood5: リクエストヘッダにUser Agent Client Hintsを追加
- http_flood4: リクエストヘッダの内容を変更しました。
- http_flood3: ユーザエージェントの他にリファラ等も偽装します。
- http_flood2: ダミーユーザエージェントの数が非常に多いやつです。
## Gif
![a](https://github.com/rifurekusyon/Powershell_DoS_Script/assets/108679694/5449735b-7366-40e0-bf89-fd864494f9ad)
