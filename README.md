# Hypomnema — 覚書

> ヒュポムネーマ（ὑπόμνημα）— 自分のための覚書。

スマホで書く、やさしいメモ。マークダウンの記号（`#` や `**`）は出てこない。
太字ボタンを押せば、本当に太字になる。書いたものは**すべて端末の中だけ**に保存され、
どこにも送られない。

Ataraxia Works の一つ。バニラ JS の単一ファイル PWA、オフライン動作。

## できること

- 見たまま編集（WYSIWYG）— 記号を覚える必要はない
- 見出し / 太字 / 斜体 / 取り消し / 箇条書き / 番号 / チェックリスト / 引用 / リンク
- チェックリストは丸をタップして完了
- 「マークダウンでコピー」で、書いたものを Markdown として書き出せる
- 共有・コピー・削除
- 端末内 localStorage のみ。アカウント不要・通信なし

## 構成

| ファイル | 役割 |
|---|---|
| `index.html` | アプリ本体（単一ファイル） |
| `manifest.json` | PWA マニフェスト |
| `sw.js` | オフライン用 Service Worker |
| `icons/` | アイコン（SVG + PNG） |
| `.well-known/assetlinks.json` | TWA（Android APK）の Digital Asset Links |
| `hypomnema.apk` | サイドロード用 Android APK |

公開先: https://hypomnema.xdcyw.net

## アップデート履歴

## 2026-06-16
- OGタグ追加（og:title / og:description / og:image / og:url / og:type / twitter:card）
- キーボードアクセシビリティ改善（:focus-visible スタイル追加）
- manifest.json 整備（scope・categories・orientation 修正）
