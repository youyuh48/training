# 課題

ニュートリゲノミクス機能性評価データベースには、以下のマイクロアレイ実験が収録されている。

大豆に含まれる主要なイソフラボンアグリコンであるゲニステインをラットに摂取させたところ、コントロール試料と比較して、血清中性脂肪濃度の低下効果が認められた。詳しいマイクロアレイ解析の結果、ゲニステインが脂質合成関連遺伝子の発現を低下させることにより、血清脂質濃度を低下を引き起こすことが示唆された。

0.2%ゲニステイン食でコントロールと比べて有意に発現が減少した遺伝子の一つに `Hsd3b` が見つかった。この遺伝子のヒトのオルソログ遺伝子は `HSD3B2` であった。このヒトの遺伝子について、`GeneCards` と `KEGG`データベースを用いて、以下の項目を調査しレポートにまとめること（Wordファイル）

- 代表的な遺伝子産物の名前は？
  - `Aliases`セクションの先頭に登場する酵素名を記載
- 遺伝子は染色体の位置と塩基長は？
  - `Genomics`セクションの`Genomic Locations`の`GRCh38/hg38`の位置
- タンパク質のアミノ酸残基数、分子量(Da)は？
- 酵素が触媒する化学反応式は？
  - `Function`セクションの`Molecular function`の`UniProtKB/Swiss-Prot CatalyticActivity`に記載
- タンパク質の細胞内局在は？
  - `Localization`セクションの`Subcellular locations`の表、Confidenceが高い上位２つを記入
- 遺伝子が最も高発現している臓器は？
  - `Expression`セクションの`mRNA expression in normal human tissues`の最も左端の棒グラフが長い組織は？
- KEGGデータベースでその遺伝子が登場する代謝マップの名前は？
  - `Pathways & Interactions`セクションの`Pathways by source`の`KEGG pathways`に記載されている
