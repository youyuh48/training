# ニュートリゲノミクス機能性評価データベースの使い方

東京農業大学  生命科学部　分子微生物学科
Department of Molecular Microbiology, Faculty of Life Sciences, Tokyo University of Agriculture

志波　優
Yuh Shiwa, PhD
youyuh48@gmail.com

Update: December 22, 2017

## ニュートリゲノミクスとは？

ニュートリゲノミクスは、食品成分と生物の持つ全ての遺伝子（ゲノム）との関わりを明らかにすることによって、食品の機能の本質に近づこうとする研究分野。DNAマイクロアレイを用いて動物組織での遺伝子発現を網羅解析するトランスクリプトミクス等により、食品成分の作用が詳細に研究されている（出典：[農研機構](http://foodfunction.dc.affrc.go.jp/ja/)）

![](https://www.newkast.or.jp/innovation/archives/researches/images/abe_Fig2.jpg)

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

1. トップページの`実験一覧`をクリック
2. 興味ある実験の行をクリック
3. `実験詳細`タブでは当該実験に関する様々な情報が表示される
4. `実験データ解析`をクリック

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

* `Name/Gene ID`をクリックすると、当該遺伝子のNCBIに登録されている情報が表示される
* `Summary`セクションに`Orthologs`欄がある場合、`human`からヒトのオルソログ遺伝子のページが表示される

8. 各実験条件における遺伝子の発現量が表に表示される

* `raw data`は生データの蛍光強度（実験間で比較不可）
* `normalized data`は実験間で比較できるように蛍光強度を正規化（ノーマライゼーション）した値。コントールサンプルの中央値で各サンプルの値を割った値なので、正ならコントロールよりも発現量が高く、負なら低い傾向を示す（参考：[マイクロアレイデータ解析例](http://www.hssnet.co.jp/9/dl/array-17011301.pdf)）

***

## 課題

ニュートリゲノミクス機能性評価データベースで、興味あるマイクロアレイ実験を一つ選び調査する。
下記の内容をレポートにまとめること（Wordファイル）

* 実験情報
  - 食品成分とその由来（何の食品に多く含まれる？）
  - 機能性（具体的にどのような健康効果？）
  - 実験方法（どのようなマウスに何を摂取させた？）
* マイクロアレイ実験結果（`実験データ解析`から閲覧）
  - 成分添加群で発現が上昇した上位3遺伝子（表のNo1-3）の遺伝子を調べる。成分添加群が２つ以上ある場合は一つの条件だけで良い、その実験条件名を記載すること。
  - それらの遺伝子名(Gene Symbol)は？
  - それらの遺伝子の発現量(normalizedの値)は？
  - それらの遺伝子はヒトのオルソログはあるか？あればその遺伝子名は？
    - 上記の手順7で当該遺伝子のヒトのオルソログ遺伝子名を表示させる
  - ヒトのオルソログがある場合、[GeneCards](http://www.genecards.org)で調べた遺伝子の機能は？（日本語で説明）
    - オルソログ遺伝子名を`GeneCards`の検索窓に入力し検索
    - 対応するヒトのオルソログ遺伝子が見つからない場合は飛ばして良い

***

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">クリエイティブ・コモンズ 表示 4.0 国際 ライセンス</a>の下に提供されています。
