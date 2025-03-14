# Markdownテーブルの書き方

1. 基本的なテーブル
```
| 名前 | 年齢 | 職業 |
|------|----|------|
| 太郎 | 25 | エンジニア |
| 花子 | 30 | デザイナー |
```

表示結果：
| 名前 | 年齢 | 職業 |
|------|----|------|
| 太郎 | 25 | エンジニア |
| 花子 | 30 | デザイナー |

---

2. カラムの幅を揃える（読みやすくする）
```
| 名前   | 年齢 | 職業      |
|------|----|---------|
| 太郎   | 25  | エンジニア |
| 花子   | 30  | デザイナー |
```
ポイント：
- -（ハイフン）の本数は**最低3本以上**ならOK
- カラムの幅を揃えると、見やすい

---

3. テキストを中央・右寄せにする

| 位置調整 | 記述方法 | 表示結果 |
|----|----|----|
|左寄せ(デフォルト)|`:---`|左寄せのテキスト|
|中央寄せ|`:---:`|中央寄せのテキスト|
|右寄せ|`---:`|右寄せのテキスト|

Markdown 記述例：
```
| 名前  | 年齢 | 職業      |
|:------|:----:|------:|
| 太郎   |  25  | エンジニア |
| 花子   |  30  | デザイナー |
```
表示結果：
| 名前  | 年齢 | 職業      |
|:------|:----:|------:|
| 太郎   |  25  | エンジニア |
| 花子   |  30  | デザイナー |

---

1. テーブル内に改行を入れる
```
| 名前  | メモ               |
|------|------------------|
| 太郎  | - エンジニア  <br> - 会社員 |
| 花子  | - デザイナー <br> - フリーランス |
```
表示結果：
| 名前  | メモ               |
|------|------------------|
| 太郎  | - エンジニア  <br> - 会社員 |
| 花子  | - デザイナー <br> - フリーランス |