# 仕様

        ## 対象レコード

        - `photoReference`
- `palette`
- `selectionReason`
- `exportMemo`

        ## 必須項目

        `title`, `palette`, `nextAction`

        ## 警告項目

        `permissionReason`, `reviewDate`

        ## フロー

        1. 入力レコードを受け取る。
        2. `src/core/scenarioEngine.js` が必須項目と警告項目を評価する。
        3. `src/report/reportBuilder.js` が検証結果を集計する。
        4. `dist/validation-result.json` を release evidence の前提証跡にする。

        ## 保存方針

        写真は端末内参照だけにし、READ_MEDIA_IMAGES はユーザー選択時に限定する
