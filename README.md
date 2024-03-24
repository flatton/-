# 概要
NLP2024にて発表する「P2-10 ソーシャルメディア上の発話の攻撃性推定と会話補助」の資料を公開する。

- [ポスター＋補足資料](https://github.com/flatton/-/blob/main/%E3%83%9B%E3%82%9A%E3%82%B9%E3%82%BF%E3%83%BC%E3%81%A8%E8%A3%9C%E8%B6%B3%E8%B3%87%E6%96%99.pdf)
- 原稿：https://www.anlp.jp/proceedings/annual_meeting/2024/pdf_dir/P2-10.pdf
- 攻撃性推定モデルのデモ: https://huggingface.co/spaces/TomokiFujihara/japanese_offensiveness_estimation
- 公開するモデル: https://huggingface.co/TomokiFujihara
- データセットについては

# 更新（2024/3/24）
## 攻撃性推定モデルの比較
4種類の事前学習済み言語モデルをFine-tuningした結果の性能を以下に示す。
Fine-tuningしたモデルはいずれもHuggingFace上に公開している。

| 評価指標 | luke-japanese-base-lite | luke-japanese-large-lite |twhin-bert-base | twhin-bert-large |
| ----- | ----- | ----- | ----- | ----- |
| F値_NOT | 71.3 | 73.9 % | 73.8 | **75.0 %** |
| F値_GRY | 55.5 | 55.4 % | 56.8 | **57.3 %** |
| F値_OFF | 61.8 | 62.67 % | **63.7** | 62.0 % |
| マクロ平均F値 | 62.9 | 64.0 % | 64.7 | **64.8 %** |
| 正解率 | 63.8 | 65.0 % | 65.6 | **66.1 %** |

## 連絡先
E-mail: tomoki.fujihara.p3@dc.tohoku.ac.jp
X: https://twitter.com/flaton_11
