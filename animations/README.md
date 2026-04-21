# Rigchecker — アニメーションファイル

このディレクトリにMixamoからダウンロードしたFBXファイルを配置してください。

## ダウンロード手順

1. https://www.mixamo.com/ にアクセス（Adobe IDでログイン）
2. 「Animations」タブでアニメーションを選択
3. ダウンロード設定：
   - **Format:** FBX Binary (.fbx)
   - **Skin:** Without Skin（スキンなし）
   - **Frames per Second:** 30
   - **Keyframe Reduction:** none
4. ダウンロードしたファイルをこのディレクトリに配置
5. ファイル名を以下に合わせてリネーム

## 必要なファイル

| ファイル名 | アニメーション | Mixamo検索キーワード例 |
|-----------|-------------|---------------------|
| idle.fbx | 待機ポーズ | "Idle", "Breathing Idle" |
| dance.fbx | ダンス | "Hip Hop Dancing", "Silly Dancing" |
| walk.fbx | 歩行 | "Walking", "Slow Walk" |
| jump.fbx | ジャンプ | "Jumping", "Jump" |
| wave.fbx | 手振り | "Waving", "Happy Hand Gesture" |

※ 追加したい場合は、FBXファイルを配置し `index.html` の `.anim-grid` にボタンを追加してください。
