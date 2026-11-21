# Irodori-TTS で「その子の声」を作る SKILL

Muse のエージェントが、Irodori-TTS を公式経路だけで導入・高速化し、声を固定して運用するための実装仕様書（SKILL）です。note 記事「Muse のエージェントが、Irodori-TTS を改造して『その子の声』を作った話」で紹介する SKILL の、GitHub 置き版です。

## 使い方

あなたの Muse に、このリポジトリの URL を渡してください。

> このスキルをインストールして：https://github.com/eris-roomie/irodori-tts-voice-skill

あとは Muse が SKILL（`SKILL.md`）を読んで進めます。人間がやるのは、3つの関門で声を聴いて選ぶだけです。

## この SKILL の方針

- **公式経路のみ**：モデルの取得・環境構築は公式 GitHub リポジトリと公式 Hugging Face リポジトリからのみ行います。第三者の導入スクリプトや変換済みモデルは使いません。
- **コードは同梱しません**：手順書として「仕様・詰まった点と解決策・検証基準」を渡し、受け手の Muse が自分の環境で実装し、公式実装との数値突き合わせで正しさを証明します。
- **声の良し悪しはユーザーの耳が決めます**：数値で声を決めません。
- **生成音声を公開する際の注意**：高速化後の自前ドライバ経路では公式の電子透かし（SilentCipher）が入りません。生成した音声を外部へ公開する場合は、AI 音声である旨を明示してください。

## 出典・きっかけ

- きっかけは、カガミカミさんの note 記事「[【無料】museアバターがキミ好みのアニメボイスで喋ってくれる！ muse-irodori-voice 専用スキルの紹介](https://note.com/kagami_kami/n/nd282e8cced5e)」です。同記事の進め方（シードを振って候補を選び、勝ち残った声を参照で固定する）を着想元にしています。ただし同記事の配布スクリプトや変換済みモデルは使っていません。
- Irodori-TTS 公式リポジトリ：https://github.com/Aratako/Irodori-TTS
- 本 SKILL の解説記事（note）：[Muse のエージェントが、Irodori-TTS を改造して「その子の声」を作った話](https://note.com/eris_roomie/n/n43ea612b8d48)

## ライセンス

MIT License です（`LICENSE` ファイル同梱、著作権者名は「eris-roomie」）。自由に使ってください。
