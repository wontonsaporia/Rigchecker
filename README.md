# Rigchecker

ブラウザ上で動作する 3D キャラクターリギング＆アニメーションビューア。  
Nomad Sculpt で作成したプリミティブ人体モデルに、Mixamo 風のマーカー配置で簡易リグを生成し、アニメーションを再生します。

> OYAA × 浦添パルコ 3DCG教室 — 体験回（T01）用ツール

# 概要

- **技術:** Three.js（WebGL）、単一 HTML ファイル
- **対応形式:** FBX（モデル）、FBX（アニメーション / Mixamo）GLT
- **動作環境:** iPad Safari（主対象）、Chrome / Edge
- **ホスティング:** GitHub Pages

# セットアップ

```bash
git clone https://github.com/wontonsaporia/rigchecker.git
cd rigchecker
```



Settings → Pages → Source: main / root → Save  
URL: `https://wontonsaporia.github.io/rigchecker/`

## 使い方

1. **アップロード** — Nomad Sculpt で作った FBXorGLT GLTだと頂点カラーを保持できるはず？をアップロード
2. **マーカー配置** — モデル上の 5 箇所をタップ（CHIN → WRISTS → ELBOWS → KNEES → GROIN）→結局またの付け根とかいろいろ増やした。
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

OYAA 内部利用かな。どうしよう。あんま、かんがえてないわ
