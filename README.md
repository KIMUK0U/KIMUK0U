<div align="center">

### Kota KIMURA

AI エンジニア / フルスタックエンジニア / 修士課程（28卒）— 岐阜大学大学院 自然科学技術研究科

[Portfolio](https://KIMUK0U.github.io) &nbsp;·&nbsp; [Email](mailto:kt2g.kimura@gmail.com)

</div>

---

#### About

画像AIとXRで、現実空間とAIをつなぐ。

大学院では、Apple Vision Pro などの XR デバイスと画像認識・LLM を組み合わせ、現実空間とAIをつなぐシステムを研究しています。主な題材は医用画像で、CT 画像や 3D 点群の解剖モデルを XR 空間に表示し、操作したり対話したりできるようにしています。

MirumeAI では、果樹の摘果・剪定を AI が支援する Web アプリを開発しています。モデルの学習から、画面・API（TypeScript・Python）、AWS 上のサーバーレス構成まで手がけています。

`画像認識` `コンピュータビジョン` `LLM` `XR` `Apple Vision Pro` `3D点群処理`

---

#### Experience

- **岐阜大学大学院 自然科学技術研究科** — 修士課程
- **[MirumeAI](https://mirumeai.com/)** — AI エンジニア / フルスタックエンジニア（アルバイト）

---

#### Projects

| # | Project | Year |
|---|---------|------|
| R-001 | [顔認証を用いたエッジAI](https://github.com/KIMUK0U/Bus-Occupant-Detection) — エッジデバイスでリアルタイム顔認証 | 2024 |
| R-002 | [XR空間でのCTスライス実物大可視化](https://github.com/KIMUK0U/VisionOS-CTSlice-Viewer) — Apple Vision Pro でCT画像をリアルスケール投影 | 2024–2025 |
| R-003 | [CT由来3D解剖モデルのAR重畳](https://github.com/KIMUK0U/CTAndPhantomRegistrationProject) — 実物頭部模型にセグメンテーション3DモデルをAR重畳 | 2025 |
| R-004 | [生徒支援AI「ユメカタリ」](https://github.com/Mugi323/student-support-ai) — LLMで生徒の深刻な悩みを早期検知・教師負担軽減。**ユメカタリ生成AIコンテスト 開発部門優秀賞** | 2025 |
| R-005 | [PointLLMを用いた解剖構造対話システム](https://github.com/KIMUK0U/InteractiveAnatomyChat) — 3D点群解剖モデルとLLMで対話学習 | 2025–2026 |
| R-006 | **果樹の摘果・剪定アノテーションアプリ**（MirumeAI・非公開） — AI が果実・枝の輪郭と房ごとの「残す順位」を下書きし、人が直した分で AI が学び直す。画面と構成図は [Portfolio](https://KIMUK0U.github.io) に掲載 | 2026 |

---

#### MirumeAI：果樹アノテーションアプリ

果樹の写真を開くと AI が摘果の順位や剪定の枝を下書きし、人が PC やスマホで直してサーバーへ保存する Web アプリ。保存した修正データで AI を学び直し、組織ごとに AI の版を持って切替・巻き戻しができる。リポジトリは非公開。

**AWS の活用**（すべて AWS CDK / TypeScript で定義）

- **CloudFront** を唯一の入口にし、画面（**S3**）・データ管理 API（**Lambda**）・AI 推論（**Lambda** コンテナ）へパスで振り分け
- **Aurora MySQL Serverless v2**（未使用時は 0 ACU で停止）で組織・ラベル・モデルの版を管理
- 画像は **S3** の署名付き URL で直接アップロードし、Lambda を通さない
- AI の学び直しは **SageMaker** の学習ジョブで、使うときだけ動かす
- NAT・ALB・WAF などの常時課金を置かないサーバーレス構成で、月 3,000 円以内が目標

---

#### Presentations

- **2026.03** 医用画像処理一般・メディカルイメージング連合フォーラム — XR空間における点群解剖モデルのLLM対話システム（口述・査読なし）
- **2025.08** 第10回 歯科AI研究会 — スマートグラスを利用した実物頭部模型への歯科CBCT画像3D重畳表示（口述・査読なし）

---

#### Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat-square&logo=swift&logoColor=white)
![visionOS](https://img.shields.io/badge/visionOS-000000?style=flat-square&logo=apple&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Unity](https://img.shields.io/badge/Unity-000000?style=flat-square&logo=unity&logoColor=white)

経験あり: `顔認証` `点群処理` `3DGS` `Apple DepthPro` `DICOM処理` `メッシュ処理` `レジストレーション`
