Student performance prediction using data of multiple courses by recurrent neural network
===

2017/03/13 	
F. Okubo	Kyushu University, Japan
T. Yamashita	Chubu University, Japan
A. Shimada	Kyushu University, Japan
H. Ogata	Kyushu University, Japan

https://dl.acm.org/citation.cfm?id=3029479

（まとめ：KaazTech）

---

## どんなもの？

九州大学内のＭ２Ｂと呼ばれる
学習支援システムから得られるログ（９種類の学習活動データ（出席日数、クイズ、レポート、コースビュー、マーカー、メモ、行動、単語数）を
ポイント付け基準に沿ってポイント化し、
ＲＮＮに入力し、最終週（８週間後）の成績（Ａ～Ｆ）を予想するモデル。
４週目時点で最終的な成績を重回帰分析より高い精度で予測できる。

---

## どうやって有効だと検証した？

（従来手法の）重回帰分析による結果とＲＮＮによる結果を比較して検証。
６コースのデータ（学生数９３７人）を訓練用とテスト用に分けてモデルに投入。

---

## 技術や手法の肝は？

９種類の学習活動データをポイント換算表に基づき、単一のポイントデータにまとめる
 （ポイント換算表作成には経験則が必要か？）

---

## 議論はある？

 ＲＮＮによる最終成績の予測の精度は、コースが進行するにつれて向上する。
 （訓練及び予測のためのデータが増加しているから）
 ５週目以降の予測精度は重回帰分析とＲＮＮの予測精度はほぼ同じだが、４週前の予測精度はＲＮＮの方が高い。
 データ母数が少ないグレード（Ａ以外）の予測精度もＲＮＮの方が高い。

---

## 先行研究と比べて何がすごい？

---

## 次に読むべき論文は？