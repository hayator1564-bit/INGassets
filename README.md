# INGassets

Instagram Graph API 用の画像配信リポジトリ。

Graph API はファイルアップロードに対応せず、**公開HTTPSのURLからしか画像を取得しない**ため、
投稿する画像だけをここに置いて公開配信する。

## 置き場所の規則

```
ig/<batch_id>/<content_id>/slide_NN.jpg
```

- 形式は **JPEG のみ**（Graph API は PNG を受け付けない）
- サイズは 1080x1350（4:5）
- 生成元は `affiliate-operations-state` リポジトリの `scripts/content_pipeline.py carousel`

## 配信URL

```
https://raw.githubusercontent.com/hayator1564-bit/INGassets/main/ig/<batch_id>/<content_id>/slide_NN.jpg
```

## 入れてはいけないもの

- トークン、APIキー、Cookie、個人情報（このリポジトリは public）
- 投稿しない下書き画像
- 運用データ（案件・媒体・実績の正本は `affiliate-operations-state` 側にある）
