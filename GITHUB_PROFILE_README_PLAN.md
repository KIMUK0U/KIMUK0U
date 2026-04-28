# GitHub Profile README 作成計画

## 仕組み

GitHub は `{username}/{username}` という名前のパブリックリポジトリの `README.md` を、プロフィールページ (`github.com/KIMUK0U`) に自動表示する。

- 作成先: `github.com/KIMUK0U/KIMUK0U`（このリポジトリとは別に作成）
- ファイル: `README.md`（リポジトリルート直下）
- 条件: Public リポジトリであること

---

## 作業手順

1. GitHub 上で `KIMUK0U/KIMUK0U` リポジトリを新規作成（Public）
2. ローカルに clone（例: `~/Desktop/KIMUK0U`）
3. ブランチ `feat/initial-profile-readme` を作成
4. 下記ドラフトの `README.md` を配置
5. `.gitignore`（`.DS_Store` 除外）を追加
6. コミット → プッシュ → main へマージ
7. `https://github.com/KIMUK0U` で表示を確認

---

## README.md ドラフト

`src/data/profile.ts`（コミット dc8851a）の内容をそのまま使用。

```markdown
<div align="center">

### Kota KIMURA

AI エンジニア / 修士課程（28卒）— 岐阜大学大学院 自然科学技術研究科

[Portfolio](https://KIMUK0U.github.io) &nbsp;·&nbsp; [Email](mailto:kt2g.kimura@gmail.com)

</div>

---

#### About

画像AI・LLMを扱い、XRとAIの融合を研究。  
Apple Vision Pro などの XR デバイスを活用し、現実空間とAIを接続するシステムを研究・開発しています。  
コンピュータビジョン・3D点群・医用画像処理を組み合わせた応用研究に取り組んでいます。

`画像認識` `コンピュータビジョン` `LLM` `XR` `Apple Vision Pro` `3D点群処理`

---

#### Experience

- **岐阜大学大学院 自然科学技術研究科** — 修士課程
- **[MirumeAI](https://mirumeai.com/)** — AI エンジニア（アルバイト）

---

#### Projects

| # | Project | Year |
|---|---------|------|
| R-000 | [生徒支援AI「ユメカタリ」](https://github.com/Mugi323/student-support-ai) — LLMで生徒の深刻な悩みを早期検知・教師負担軽減。**ユメカタリ生成AIコンテスト 開発部門優秀賞** | 2024 |
| R-001 | [顔認証を用いたエッジAI](https://github.com/KIMUK0U/Bus-Occupant-Detection) — エッジデバイスでリアルタイム顔認証 | 2024 |
| R-002 | [XR空間でのCTスライス実物大可視化](https://github.com/KIMUK0U/VisionOS-CTSlice-Viewer) — Apple Vision Pro でCT画像をリアルスケール投影 | 2024–2025 |
| R-003 | [CT由来3D解剖モデルのAR重畳](https://github.com/KIMUK0U/CTAndPhantomRegistrationProject) — 実物頭部模型にセグメンテーション3DモデルをAR重畳 | 2025 |
| R-004 | [PointLLMを用いた解剖構造対話システム](https://github.com/KIMUK0U/InteractiveAnatomyChat) — 3D点群解剖モデルとLLMで対話学習 | 2025–2026 |

---

#### Presentations

- **2026.03** 医用画像処理一般・メディカルイメージング連合フォーラム — XR空間における点群解剖モデルのLLM対話システム（口述・査読なし）
- **2025.08** 第10回 歯科AI研究会 — スマートグラスを利用した実物頭部模型への歯科CBCT画像3D重畳表示（口述・査読なし）

---

#### Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![visionOS](https://img.shields.io/badge/visionOS-000000?style=flat-square&logo=apple&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white)

経験あり: `3DGS` `Apple DepthPro` `DICOM処理` `モデリング`
```

---

## 参照元

- `src/data/profile.ts` — プロフィール・研究・発表・スキルの全データ（dc8851a）
- `src/components/about/About.astro` — About セクションの文章

## 注意

このファイルは計画書。`KIMUK0U/KIMUK0U` リポジトリへの実装完了後は削除してよい。
