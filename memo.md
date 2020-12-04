# 様々なことメモ

## 注意

・bibtex だけでは不十分。資料を見て参考文献の表記法を確認すること

## 何の役に立つのか

・作成したモデルの検証が可能（実際のモデルと比較して良いモデルにできているのか？）
. In particular, evaluating similarity between graphs is crucial to network analysis and
graph-based anomaly detection (Papadimitriou et al., 2010;　 Akoglu et al., 2015; Ranshous et al., 2015).

## 流れ

従来研究
・VNGE: 前処理ができない
・NetLSD: 前処理ができても、指標が複雑で意味を捉えにくい

スペクトルを用いた計算法
従来手法とは異なる方法の計算。
→ 前計算が可能。cos dist なら検索が早い（これは NetLSD は L2 ノルムを用いているが、これにも適用可能？）

## VNGE

the von Neumann graph entropy (VNGE) (Braunstein et al., 2006; Passerini & Severini,
2008; 2009) facilitates the measure of (quantum) JensenShannon divergence and distance (Endres & Schindelin,
2003; Briet & Harremo ¨ es¨ , 2009) between graphs.

## original contribution(もっと洗練させる

先行研究でのネットワークの距離を計算する手法は、「スケールしない」or「大規模グラフにも適応可能だが、グラフの距離を同時に複数計算するのに時間がかかる」という欠点がありました。

今回はその欠点を解消する、以下の利点を持つネットワークの距離の計算手法を、材料科学の分野の手法を元にして提案しています。

- 大規模ネットワークのサイズにスケールする
- あらかじめ DOS(固有値の分布)を前計算しておけば、ネットワーク間の距離の複数計算や、類似した DOS を持つネットワークの検索が高速に行える

また、大規模ネットワークの DOS の計算方法は近年計算手法が考案されたばかりで、応用方法などは多くありません。

今回の手法の提案によって、ネットワークの DOS が有用であることの 1 つの例示になると言えます。

## 論文

- [Braunstein, S. L., Ghosh, S., and Severini, 2006]

  - 量子力学の文脈で使われていた Von Neumann entropy をグラフに応用した論文として紹介しています。
    （VNGE という用語自体が出てくるのはもう少し後の論文だと思います。）

- [De Domenico et al., 2015]

  - Kullback–Liebler divergence を用いて定義される Jensen-Shannon divergence を von Neumann entropy で表現した論文として用いています。
    （こちらは発表資料から参考文献として抜けていたみたいです。申し訳ありません）

  - > その論文には若干違和感を感じます。理由は、
    > Shannon entropy ---> von Neumann entropy
    > KL-divergence ---> quantum divergence
    > (or, relative entropy)
    > と量子情報分野では拡張されているからです。quantum divergence で Jensen 流にすることはできるわけで。このあたり、その論文ではどう書かれてるでしょうか。

  - De Domenico, Manlio, Vincenzo Nicosia, Alexandre Arenas, and Vito Latora. "Structural reducibility of multilayer networks." Nature communications 6, no. 1 (2015): 1-9.

- [Dominik M. Endres and Johannes E. Schindelin, 2003]

  - Jensen-Shannon divergence の平方根が、距離を表現するものとして適切な指標であることを証明しています。
  - 前述の Jensen-Shannon divergence の式と、後述の Von Neumann Graph Entropy の近似計算アルゴリズムを用いることで、2 つのグラフ間の距離が計算できることが分かります。
  - > 情報理論では、KL-divergence の次に、Hellinger distance というのがよく知られてます。ある意味、Hellinger distance は L_1 norm 的です。それと関係あるでしょうか？

- [Chen, Pin-Yu, Lingfei Wu, Sijia Liu, and Indika Rajapakse, 2019] & [Tsitsulin, Anton, Marina Munkhoeva, and Bryan Perozzi, 2020]

  - 大規模グラフにスケールするような、Von Neumann Graph Entropy の近似計算アルゴリズムについての紹介です。
  - > この研究あったのですね。density matrix で marginal distribution 的なものを考えると、submodular function が出てきます。平石さんは submodular function をよく知っています。この関数の submodularit は Lieb, Ruskai という物理の有名な研究者がいて、一方 combinatorial optimization では submodular function の minimization は関数計算をオラクルとすると多項式時間でできます（最大化は NP-hard で、一方で greedy algorithm が定数近似値比の近似アルゴリズムになります）。そういうことで、計算法にかつて興味があったのですが、その答えが今井はようやくでわかりました

- [Geilhufe, R.M., Borysov, S.S., Kalpakchi, D. and Balatsky, A.V., 2018.]
  - materials science で使用された DOS 応用方法の紹介と、その手法の流用を提案するために用いました。論文中では DOS のデータベースから、類似した DOS を持つ結晶を検索する方法について述べています。

## 参考

Spectral Graph Theory については、有名な本の著者の Fan Chung の Web ページ
http://www.math.ucsd.edu/~fan/
で、下の方にある some talks for general audience のもの
http://www.math.ucsd.edu/~fan/talks/jmm1.pdf
http://www.math.ucsd.edu/~fan/talks/graph.pdf
を一度見て、感じ（page rank, random
walk などへの展開も含め）をつかんでおくとよいかもしれません。
