# photo-organizer-color-palette

写真整理・色パレット抽出 は、写真選別理由と抽出パレットを制作メモとして残すAndroidツールです。

## Closed Alpha Scope

- Rank: 27
- Tier / Score: P1 / 63
- Domain / Idea No: AndroidApp / 9
- 主な公開先: Google Play
- GitHub: https://github.com/Sunmax0731/photo-organizer-color-palette
- Prerelease: https://github.com/Sunmax0731/photo-organizer-color-palette/releases/tag/v0.1.0-alpha.1

## 実装概要

- `src/core`: 製品プロファイルと代表シナリオ評価
- `src/validators`: 期待結果検証
- `src/report`: 検証レポート生成
- `src/review-model`: レビューゲートと責務モデル
- `src/cli`: `samples/representative-suite.json` の自動検証

## 代表データ

`samples/representative-suite.json` は `happy-path`、`missing-required`、`warning`、`mixed-batch` を含みます。

## 検証

```powershell
cd D:\AI\AndroidApp\photo-organizer-color-palette
cmd.exe /d /s /c npm test
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` を参照してください。
