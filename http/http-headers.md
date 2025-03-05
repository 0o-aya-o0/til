# HTTP ヘッダー一覧

HTTPヘッダーは、クライアントとサーバーがリクエストやレスポンス時に追加情報をやり取りするためのキーと値のセットです。

## **1. 一般ヘッダー (General Headers)**
| ヘッダー名 | 説明 |
|---|---|
| `Cache-Control` | キャッシュの動作を制御する |
| `Connection` | 接続の管理 (`keep-alive` や `close` など) |
| `Date` | メッセージが送信された日時 |
| `Via` | プロキシサーバーを経由した情報 |

---

## **2. リクエストヘッダー (Request Headers)**
| ヘッダー名 | 説明 |
|---|---|
| `Accept` | クライアントが受け入れ可能なコンテンツの種類 (例: `text/html, application/json`) |
| `Accept-Encoding` | クライアントが受け入れ可能なエンコーディング (例: `gzip, deflate`) |
| `Authorization` | 認証情報 (例: `Bearer <token>`) |
| `Content-Type` | リクエストボディのデータの種類 (例: `application/json`) |
| `Host` | リクエスト対象のサーバーホスト名 (例: `example.com`) |
| `Origin` | クロスオリジンリクエストの送信元 |
| `Referer` | リクエストの元になったページのURL |
| `User-Agent` | クライアントの情報 (例: ブラウザの種類やバージョン) |

---

## **3. レスポンスヘッダー (Response Headers)**
| ヘッダー名 | 説明 |
|---|---|
| `Access-Control-Allow-Origin` | CORS (クロスオリジンリクエスト) の許可設定 |
| `Content-Length` | レスポンスボディのサイズ (バイト単位) |
| `Content-Type` | レスポンスボディのデータの種類 (例: `application/json`) |
| `Set-Cookie` | クライアントに送るクッキー情報 |
| `WWW-Authenticate` | クライアントに認証方法を指示する |

---

## **4. キャッシュ関連のヘッダー**
| ヘッダー名 | 説明 |
|---|---|
| `Cache-Control` | キャッシュの有効期限や動作 (`no-cache`, `max-age=3600` など) |
| `ETag` | リソースのバージョン識別子 (変更検知用) |
| `Expires` | キャッシュの有効期限 |
| `Last-Modified` | 最後にリソースが変更された日時 |
| `Pragma` | レガシーなキャッシュ制御 (`no-cache` など) |

---

## **5. セキュリティ関連のヘッダー**
| ヘッダー名 | 説明 |
|---|---|
| `Content-Security-Policy (CSP)` | コンテンツのロード制御 (XSS 対策) |
| `Strict-Transport-Security (HSTS)` | HTTPS 接続を強制する設定 |
| `X-Content-Type-Options` | MIME タイプのスニッフィング防止 (`nosniff`) |
| `X-Frame-Options` | クリックジャッキング対策 (`DENY` や `SAMEORIGIN`) |
| `X-XSS-Protection` | クロスサイトスクリプティング (XSS) 防御 |

