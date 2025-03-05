# HTTP メソッド一覧

HTTP メソッドは、クライアントとサーバー間の通信でどのような処理を要求するかを指定するために使用されます。

## **1. GET**
- **概要**: リソースの取得
- **特性**: 
  - 安全（リソースを変更しない）
  - 冪等（同じリクエストを何回送っても結果が変わらない）
  - キャッシュ可能
- **使用例**:
  ```bash
  curl -X GET https://api.example.com/users
  ```

## **2. POST**
- **概要**: リソースの作成・データの送信
- **特性**: 
  - 非冪等（同じリクエストを複数回送ると異なる結果になることがある）
  - リクエストボディを送信可能
- **使用例**:
  ```bash
  curl -X POST https://api.example.com/users -d '{"name": "Alice"}' -H "Content-Type: application/json"
  ```

## **3. PUT**
- **概要**: 指定したリソースの作成または更新（上書き）
- **特性**: 
  - 冪等（同じリクエストを何回送っても結果が変わらない）
  - リクエストボディを送信可能
- **使用例**:
  ```bash
  curl -X PUT https://api.example.com/users/1 -d '{"name": "Bob"}' -H "Content-Type: application/json"
  ```

## **4. PATCH**
- **概要**: 指定したリソースの部分的な更新
- **特性**: 
  - 非冪等（通常、リクエストの適用順によって結果が変わる可能性がある）
  - リクエストボディを送信可能
- **使用例**:
  ```bash
  curl -X PATCH https://api.example.com/users/1 -d '{"age": 30}' -H "Content-Type: application/json"
  ```

## **5. DELETE**
- **概要**: 指定したリソースの削除
- **特性**: 
  - 冪等（同じリクエストを複数回送っても結果は変わらない）
- **使用例**:
  ```bash
  curl -X DELETE https://api.example.com/users/1
  ```

## **6. HEAD**
- **概要**: `GET` と同じだが、レスポンスボディを返さない
- **特性**: 
  - 安全、冪等
  - キャッシュ可能
- **使用例**:
  ```bash
  curl -X HEAD https://api.example.com/users
  ```

## **7. OPTIONS**
- **概要**: サーバーがサポートするメソッドを問い合わせる
- **特性**: 
  - 安全、冪等
- **使用例**:
  ```bash
  curl -X OPTIONS https://api.example.com/users
  ```

## **8. CONNECT**
- **概要**: プロキシサーバーとのトンネル接続を確立
- **特性**: 
  - 通常はHTTPプロキシで使用
- **使用例**:
  ```bash
  curl -X CONNECT https://example.com
  ```

## **9. TRACE**
- **概要**: ループバックテストを行い、リクエストがどのように処理されるかを確認
- **特性**: 
  - セキュリティ上の理由から、多くのサーバーで無効化されている
- **使用例**:
  ```bash
  curl -X TRACE https://api.example.com
  ```