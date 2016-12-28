# 設計

## Ruby バージョン
 - ruby 2.1.3p242 (2014-09-19 revision 47630) [x86_64-darwin14.0]

## 開発環境
 - Mac OS 10.10.5

## データベース設計
 * Userモデル
   - name:string(名前)
   - id :integer
   - email :varchar(メールアドレス)
   - group_id (所属グループ)
 * chat_gruop(グループ)モデル
   - group_id :integer
   - relative_id :integer
   - user_id :integer
 * massage(投稿)モデル
   - type :string
   - group_id :integer
   - relative_id :integer
   - user_id :integer
 * image(画像)モデル
   - image : image
 * text(投稿内容)モデル
   - text :text