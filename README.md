# Rigchecker

ブラウザ上で動作する 3D キャラクターリギング＆アニメーションビューア。  
Nomad Sculpt で作成したプリミティブ人体モデルに、Mixamo 風のマーカー配置で簡易リグを生成し、アニメーションを再生します。

> OYAA × 浦添パルコ 3DCG教室 — 体験回（T01）用ツール

## 概要

- **技術:** Three.js（WebGL）、単一 HTML ファイル
- **対応形式:** FBX（モデル）、FBX（アニメーション / Mixamo）
- **動作環境:** iPad Safari（主対象）、Chrome / Edge
- **ホスティング:** GitHub Pages

## セットアップ

```bash
git clone https://github.com/wontonsaporia/rigchecker.git
cd rigchecker
```

### アニメーションファイルの準備

1. [Mixamo](https://www.mixamo.com/) にログイン
2. Animations タブでアニメーションを選択
3. ダウンロード設定:  
   - Format: **FBX Binary (.fbx)**  
   - Skin: **Without Skin**  
   - Frames per Second: **30**
4. ダウンロードしたファイルを `animations/` にそのまま配置（リネーム不要）

| ファイル名 | 内容 | Mixamo 検索キーワード |
|-----------|------|----------------------|
| `Breathing Idle.fbx` | 待機ポーズ | Breathing Idle |
| `Shopping Cart Dance.fbx` | ダンス① | Shopping Cart Dance |
| `Northern Soul Spin Combo.fbx` | ダンス② | Northern Soul Spin Combo |
| `Walking.fbx` | 歩行 | Walking |
| `Standing Jump.fbx` | ジャンプ | Standing Jump |
| `Waving.fbx` | 手振り | Waving |

### ローカル確認

```bash
# VS Code Live Server、または
npx serve .
```

### GitHub Pages で公開

Settings → Pages → Source: main / root → Save  
URL: `https://wontonsaporia.github.io/rigchecker/`

## 使い方

1. **アップロード** — Nomad Sculpt で作った FBX をアップロード
2. **マーカー配置** — モデル上の 5 箇所をタップ（CHIN → WRISTS → ELBOWS → KNEES → GROIN）
3. **リグ生成** — ボタンをタップで自動リギング
4. **アニメーション** — 再生ボタンでアニメーション切替・自由閲覧

## ファイル構成

```
rigchecker/
├── index.html                       ← アプリ本体
├── README.md
└── animations/
    ├── README.md                    ← アニメーション配置ガイド
    ├── Breathing Idle.fbx
    ├── Shopping Cart Dance.fbx
    ├── Northern Soul Spin Combo.fbx
    ├── Walking.fbx
    ├── Standing Jump.fbx
    └── Waving.fbx
```

## 関連ドキュメント

- 要件定義書: `rigtester_spec.md`（OYAA-portal プロジェクト内）
- 体験回プランシート: `plan_trial.html`（T01）

## ライセンス

OYAA 内部利用
