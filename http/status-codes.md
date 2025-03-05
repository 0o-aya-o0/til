# HTTP ステータスコード一覧

## 1xx: 情報レスポンス
| ステータスコード | 意味 |
|---|---|
| 100 | Continue（継続） |
| 101 | Switching Protocols（プロトコル変更） |
| 102 | Processing（処理中） |
| 103 | Early Hints（早期ヒント） |

## 2xx: 成功レスポンス
| ステータスコード | 意味 |
|---|---|
| 200 | OK（成功） |
| 201 | Created（作成成功） |
| 202 | Accepted（受理） |
| 203 | Non-Authoritative Information（非権威情報） |
| 204 | No Content（内容なし） |
| 205 | Reset Content（コンテンツリセット） |
| 206 | Partial Content（部分コンテンツ） |

## 3xx: リダイレクト
| ステータスコード | 意味 |
|---|---|
| 300 | Multiple Choices（複数の選択肢） |
| 301 | Moved Permanently（恒久的に移動） |
| 302 | Found（発見、以前は"Moved Temporarily"） |
| 303 | See Other（他を参照） |
| 304 | Not Modified（未更新） |
| 307 | Temporary Redirect（一時的リダイレクト） |
| 308 | Permanent Redirect（恒久的リダイレクト） |

## 4xx: クライアントエラー
| ステータスコード | 意味 |
|---|---|
| 400 | Bad Request（不正なリクエスト） |
| 401 | Unauthorized（認証が必要） |
| 403 | Forbidden（アクセス拒否） |
| 404 | Not Found（見つからない） |
| 405 | Method Not Allowed（許可されていないメソッド） |
| 406 | Not Acceptable（受理できない） |
| 407 | Proxy Authentication Required（プロキシ認証が必要） |
| 408 | Request Timeout（リクエストタイムアウト） |
| 409 | Conflict（競合） |
| 410 | Gone（消滅） |
| 411 | Length Required（長さが必要） |
| 412 | Precondition Failed（前提条件が失敗） |
| 413 | Payload Too Large（ペイロードが大きすぎる） |
| 414 | URI Too Long（URIが長すぎる） |
| 415 | Unsupported Media Type（サポートされていないメディアタイプ） |
| 429 | Too Many Requests（リクエストが多すぎる） |

## 5xx: サーバーエラー
| ステータスコード | 意味 |
|---|---|
| 500 | Internal Server Error（内部サーバーエラー） |
| 501 | Not Implemented（未実装） |
| 502 | Bad Gateway（不正なゲートウェイ） |
| 503 | Service Unavailable（サービス利用不可） |
| 504 | Gateway Timeout（ゲートウェイタイムアウト） |
| 505 | HTTP Version Not Supported（サポートされていないHTTPバージョン） |
