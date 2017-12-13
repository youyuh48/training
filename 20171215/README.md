# ヒトゲノムデータベース GeneCards の使い方

東京農業大学 生命科学部 分子微生物学科

Department of Molecular Microbiology, Faculty of Life Sciences, Tokyo University of Agriculture

志波 優

Yuh Shiwa, PhD

youyuh48@gmail.com

Update: December 15, 2017

## アルコール代謝関連遺伝子

* ADH2(ADH1B): アルコール脱水素酵素 (alcohol dehydrogenases)
* ALDH2: アルデヒド脱水素酵素 (aldehyde dehydrogenases)

<img src="http://epi.ncc.go.jp/files/11_publications/E382B9E383A9E382A4E383891.PNG" width="640px">

出典：[多目的コホート研究(JPHC Study) アルコール代謝関連遺伝子（アルコール・アルデヒド脱水素酵素）と飲酒量に基づく胃がん罹患について](http://epi.ncc.go.jp/jphc/outcome/3499.html)

## GeneCards: The Human Gene Database

[GeneCards](http://www.genecards.org)

ヒトゲノム情報のデータベース。遺伝子機能、遺伝子発現、疾患関連、SNPs、オーソロジーなどの関連情報へのリンクが豊富。

<img width="640" src="https://user-images.githubusercontent.com/27807944/33800653-8db9644c-dd87-11e7-8a74-02196722e96c.png">

### 使い方

1. Keywords ボタンの隣の検索窓に遺伝子名 `ADH1B` を入力して検索します。
2. ヒットした遺伝子が表示されます。各種情報へのリンクが以下の表示されます。

<img width="640" src="https://user-images.githubusercontent.com/27807944/33800752-34207e4a-dd8a-11e7-85c9-80587708d2bf.png">

各セクションの情報

* Aliases
  * 当該遺伝子の別名
* Summaries
  * 当該遺伝子の概要
* Genomics
  * 当該遺伝子のゲノム情報（位置や制御因子など）
  * `Genomic Location` 染色体上の位置情報
  * `RefSeq DNA sequence` NCBIの遺伝子情報・配列へのリンク
* Proteins
  * 当該遺伝子のタンパク質情報
  * `Protein attributes` アミノ酸の残基数、分子量など
  * `Three dimensional structures` 立体構造情報へのリンク
* Domains & Families
  * タンパク質のドメイン・ファミリー情報
* Function
  * 当該遺伝子の機能情報
  * `Molecular function` 化学反応式
  * `Enzyme Numbers (IUBMB)` 酵素のEC番号
* Localization
  * 当該遺伝子産物の細胞内局在
* Pathways & Interactions
  * 当該遺伝子のパスウェイ・相互作用情報
* Drugs & Compounds
  * 当該遺伝子に関する薬剤・化合物情報
* Transcripts
  * 当該遺伝子の転写産物情報へのリンク
* Expression
  * 当該遺伝子の主要組織における発現量
  * mRNA expression in normal human tissues
    * 複数手法により得られた正常組織の発現量
* Orthologs
  * 当該遺伝子のオルソログ遺伝子
* Paralogs
  * 当該遺伝子のパラログ遺伝子
* Variants
  * 当該遺伝子の変異情報
  * Sequence variations from dbSNP and Humsavar
    * `SNP ID` dbSNPへのリンク、リンク先の説明は下記
    * `Type` 変異の遺伝子上の位置と影響
* Disorders
  * 当該遺伝子の疾患情報
* Publications
  * 当該遺伝子の論文情報

## dbSNP

[dbSNP](https://www.ncbi.nlm.nih.gov/projects/SNP/)

ヒトゲノムの多型情報（一から数塩基の置換、挿入/欠失、反復等）のデータベース。
SNPの集団間での多型頻度を比較も可能。

SNP（一塩基多型）とアレル

![](http://genomicsinitiative.com/fwimages/alleles_320x210.gif)

出典：[What's a SNP, what's a chip,
and why does all this matter?](http://genomicsinitiative.com/tutorial_a1.html)

### 多型の遺伝子への影響

`GeneView`セクション

<img width="1179" src="https://user-images.githubusercontent.com/27807944/33814453-a3e8035e-de6d-11e7-9fa3-6e5d0c926b13.png">

### SNPの各集団での頻度情報

`Population Diversity`セクション、日本人は`HapMap-JPT`

<img width="1023" src="https://user-images.githubusercontent.com/27807944/33814465-b01b917c-de6d-11e7-852b-b454093b9fce.png">

***

## 課題

[GeneCards](http://www.genecards.org)で`ALDH2`遺伝子について調査する。
下記の内容をレポートにまとめること（Wordファイル）

* 代表的な遺伝子産物の名前は？（先頭のタイトル部分）
* 遺伝子の染色体上の位置、塩基長は？
* 遺伝子がタンパク質の場合
  * アミノ酸残基数、分子量(Da)は？
  * 化学反応式 (UniProtKB/Swiss-Prot CatalyticActivity)は？
  * 酵素のEC番号 (Enzyme Numbers)は？
  * 細胞内局在 (Subcellular locations)はどこか？
* 遺伝子が最も高発現している臓器は？
  * mRNA expression in normal human tissuesの`RNAseq`における棒グラフが最も右端の臓器
* 遺伝子の変異
  * `Variants`セクションに非同義置換(missense)の変異があるか？あればそのrsIDは？
  * 上記の変異はアミノ酸を何から何へ変化させるか？
    * rsIDをクリックした先の`GeneView`セクションの`Gene Model`の`Residue change`
  * 上記の変異の日本人における各アレル (A/A,A/G,G/G) の頻度は？
    * `Population Diversity`セクションの最初に登場する`HapMap-JPT`における頻度

***

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">クリエイティブ・コモンズ 表示 4.0 国際 ライセンス</a>の下に提供されています。
