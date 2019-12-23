# スタートアップスクリプト(sakuracloud_note)

---

**全ゾーン共通のグローバルリソースです。**

### 設定例

```hcl
data "sakuracloud_note" "mynote" {
  name_selectors = ["foobar"]
}
```

### パラメーター

|パラメーター         |必須  |名称                |初期値     |設定値                    |補足                                          |
|-------------------|:---:|--------------------|:--------:|------------------------|----------------------------------------------|
| `name_selectors`  | -   | 検索条件(名称)      | -        | リスト(文字列)           | 複数指定した場合はAND条件  |
| `tag_selectors`   | -   | 検索条件(タグ)      | -        | リスト(文字列)           | 複数指定した場合はAND条件  |
| `filter`          | -   | 検索条件(その他)    | -        | オブジェクト             | APIにそのまま渡されます。検索条件を指定してもAPI側が対応していない場合があります。 |


### 属性

|属性名                | 名称                    | 補足                                        |
|---------------------|------------------------|--------------------------------------------|
| `id`                | スクリプトID             | -                                          |
| `name`              | スクリプト名           | - |
| `class`             | クラス                | - |
| `content`           | スクリプト内容         | - |
| `icon_id`           | アイコンID         | - |
| `description`       | 説明  | - |
| `tags`              | タグ | - |
