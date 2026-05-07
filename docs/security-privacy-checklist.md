# Security / Privacy Checklist

        ## 方針

        写真は端末内参照だけにし、READ_MEDIA_IMAGES はユーザー選択時に限定する

        ## チェック

        - [x] 外部送信をMVP外にした。
        - [x] サンプルに実個人情報を含めない。
        - [x] 手動テストで確認すべき権限を列挙。
        - [x] release asset に手動テスト手順を添付。

        ## Android / Host 権限

        - READ_MEDIA_IMAGES はユーザー選択フローでのみ要求
- ネットワーク送信なし

        ## Adobe 公式参照

        - 対象ドメイン docs と created_idea metadata を優先。
