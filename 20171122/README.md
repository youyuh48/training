# ニュートリゲノミクス機能性評価データベースの使い方

東京農業大学  生命科学部　分子微生物学科
Department of Molecular Microbiology, Faculty of Life Sciences, Tokyo University of Agriculture

志波　優
Yuh Shiwa, PhD
youyuh48@gmail.com

Update: July 15, 2020

## ニュートリゲノミクスとは？

ニュートリゲノミクスは、食品成分と生物の持つ全ての遺伝子（ゲノム）との関わりを明らかにすることによって、食品の機能の本質に近づこうとする研究分野。DNAマイクロアレイを用いて動物組織での遺伝子発現を網羅解析するトランスクリプトミクス等により、食品成分の作用が詳細に研究されている（出典：[農研機構](http://foodfunction.dc.affrc.go.jp/ja/)）

出典：[神奈川科学技術アカデミー「健康・アンチエイジング」プロジェクト](https://www.newkast.or.jp/innovation/archives/researches/abe_project_2014.html)

![](http://www.bureau.tohoku.ac.jp/manabi/manabi43/43_6_1.jpg)

出典：[東北大学「機能性食品成分や微量栄養素による抗メタボ研究」](http://www.bureau.tohoku.ac.jp/manabi/manabi43/mm43-6.html)

![](https://www.gelifesciences.co.jp/newsletter/biodirect_mail/technical_tips/image/principle_microarray.gif)

マイクロアレイの原理

![](https://www.gelifesciences.co.jp/newsletter/biodirect_mail/technical_tips/image/principle_microarray2.gif)

マイクロアレイの定量

出典：[GEヘルスケア・ジャパン「遺伝子発現差異解析～マイクロアレイとは」](https://www.gelifesciences.co.jp/newsletter/biodirect_mail/technical_tips/tips21.html)

![](http://www.naro.affrc.go.jp/nfri/introduction/files/kinousei_1.png)

出典：[農研機構「機能性評価技術ユニット」](http://www.naro.affrc.go.jp/nfri/introduction/chart/0304/index.html)

## ニュートリゲノミクス機能性評価データベース

[ニュートリゲノミクス機能性評価データベース](http://foodfunction.dc.affrc.go.jp/ja/)では、各種食品成分の動物試験による機能性評価法及びその結果（DNAマイクロアレイ解析、生化学的データ等）を検索が可能。

<img width="946" src="https://user-images.githubusercontent.com/27807944/33877991-7e299b68-df6d-11e7-95e4-36ad6e92ca0e.png">

### DNAマイクロアレイ解析の結果の閲覧

このWebサイトを利用するには`Flash Player`を有効にする必要がある。以下のサイトが参考になる。
* [Flash Playerを使ったWebサイトを表示できません](https://flets-w.com/user/point-otoku/knowledge/pc-operate/pc-operate97.html)

1. トップページの`実験一覧`をクリック
2. 興味ある実験の行をクリック（例：1行目のID1の実験）
3. `実験詳細`タブでは当該実験に関する様々な情報が表示される
4. `実験データ解析`をクリック
  * できない場合は上記の説明を参考に`Flash Player`を有効にする

<img width="640"  src="https://user-images.githubusercontent.com/27807944/34070516-2383f55a-e2ab-11e7-8fec-f94b605ab370.png">

* 左側のヒートマップが各実験における遺伝子の発現量を色で示している
* 下段の表が遺伝子名・遺伝子の発現量を示している

5. `Zoom 1x`をクリックし、`Zoom 10x`にする

<img width="640"  src="https://user-images.githubusercontent.com/27807944/34070549-9aa7fda2-e2ab-11e7-8404-cb97187ca9ee.png">

* 列：が実験条件（コントロールと各種成分を添加した）
* 行：ある遺伝子とその発現量（青：低、黄色：中、オレンジ：高発現）
* 上段の遺伝子（オレンジ）：コントロールと比較して成分添加で高発現
* 中央の遺伝子（青）：コントロールと比較して成分添加で低発現
* 下段の遺伝子（黄）：コントロールと成分添加の両方で低発現

6. ヒートマップの行をクリックすると、下の表に遺伝子情報や発現量が表示される
7. `Gene Symbol`をクリックすると、当該遺伝子をNCBIで検索した結果が表示される

<img width="640"  src="https://user-images.githubusercontent.com/27807944/87491250-9c62f300-c682-11ea-95a2-fc257cb1560c.png">

* `Name/Gene ID`をクリックすると、当該遺伝子のNCBIに登録されている情報が表示される
  - `Official Full Name`は遺伝子のアノテーション
  - `Expression`はトランスクリプトーム解析から得られた当該遺伝子が強く発現している臓器の情報

<img width="640"  src="https://user-images.githubusercontent.com/27807944/87491336-d7fdbd00-c682-11ea-8704-798bc4d06635.png">

8. 各実験条件における遺伝子の発現量が表に表示される

<img width="640"  src="https://user-images.githubusercontent.com/27807944/87491139-4e4def80-c682-11ea-9b86-16e169c1e1d8.png">

* `raw data`は生データの蛍光強度（実験間で比較不可）
* `normalized data`は実験間で比較できるように蛍光強度を正規化（ノーマライゼーション）した値。コントールサンプルの中央値で各サンプルの値を割った値なので、正ならコントロールよりも発現量が高く、負なら低い傾向を示す。
  - 実験ID1「0.1及び0.5%ケルセチン投与」実験のデータの場合
  - 遺伝子No1の`Ly6a`遺伝子の発現量は、ストレプトゾトシンで糖尿病を誘発させた群の正規化した発現量`STZ normalized data`と比較して、0.5%ケルセチン投与した群の正規化した発現量`STZ + 0.5% Quer normalized data`の数値は低下している。
  - 上記の遺伝子は、0.5%ケルセチン投与により発現量が低下したことを示す。

***

## 課題

ニュートリゲノミクス機能性評価データベースで、興味あるマイクロアレイ実験を一つ選び調査する。
下記の内容をレポートとして以下のリンクからFormsで回答してください。

https://forms.office.com/Pages/ResponsePage.aspx?id=LkP55PRkh0KJHSRfz3SiAsXGspOc-ltEvV16RsiCCipUOEpWNEpaWFVJVFpIVDVHUzhUVlI4R0dEMC4u

* 実験情報
  - 食品成分とその由来（何の食品に多く含まれる？）
  - その成分の機能性（具体的にどのような健康効果？）
  - 実験方法（どのようなマウスに何を摂取させた？）

* マイクロアレイ実験結果を`実験データ解析`から閲覧する。リストの最上位の遺伝子（No1の遺伝子）について、以下の情報を記載してください。ただし、No1の遺伝子名(Gene Symbol)が空欄の場合は、No2以降の遺伝子名が記載がある物を選んでください。
  - 遺伝子名(Gene Symbol)は？
  - 成分添加群の遺伝子の発現量(normalized xxx dataの値)は？複数の成分添加条件がある場合は、次のように条件名と値を記載してください（例：STZ +0.1% Quer normalized, 2.6500905）
  - `Gene Symbol`をクリックして飛んだ、NCBIのページに記載されている遺伝子情報は？
    - `Official Full Name`
    - `Expression`欄に記載されている遺伝子が発現している組織名は？

***

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">クリエイティブ・コモンズ 表示 4.0 国際 ライセンス</a>の下に提供されています。
