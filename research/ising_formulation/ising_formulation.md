# 組合せ最適化問題のイジングモデル表現 “Ising formulations of many NP problems” by Andrew Lucas (2014)

```{contents} 目次
---
local: true
---
```

## 文献情報
- タイトル: [Ising formulations of many NP problems](https://www.frontiersin.org/articles/10.3389/fphy.2014.00005/full)
- 著者: [Andrew Lucas](https://web.stanford.edu/~ajlucas/)([Google Scholar](https://scholar.google.com/citations?user=6ipiQb8AAAAJ))
- 書誌情報: Frontiers in Physics 2, 5 (2014). (doi: [10.3389/fphy.2014.00005](https://doi.org/10.3389/fphy.2014.00005))

## 概要
近年、NP完全、あるいはNP困難な組合せ最適化問題の断熱量子最適化（AQO, Adiabatic Quantum Optimization）を用いた解法が注目されている。
全ての組合せ最適化問題はIsingスピングラスの基底状態探索へと定式化することが可能であり、そのための手法としてAQOを用いる。

本論文では、組合せ最適化問題の累計パターンを集めたKarpの21のNP完全問題 ([Karp’s 21 NP-complete problems](https://en.wikipedia.org/wiki/Karp%27s_21_NP-complete_problems))を含む組合せ最適化問題のIsingスピングラスによる定式化のハミルトニアンを網羅している。

**取り扱われている組合せ最適化問題**

- 分割問題 (Partitioning Problems)
  - 数分割 (Number Partitioning)
  - [グラフ分割 (Graph Partitioning)](http://qard.is.tohoku.ac.jp/T-Wave/?p=122)
  - [最大クリーク問題 (Cliques)](http://qard.is.tohoku.ac.jp/T-Wave/?p=97)
- 二値整数線型計画 (Binary Integer Linear Programming)
  - 被覆・パッキング問題 (Covering and Packing Problems)
  - 厳密被覆問題 (Exact Cover)
  - 集合パッキング問題 (Set Packing)
  - [頂点被覆問題 (Vertex Cover)](https://qard.is.tohoku.ac.jp/T-Wave/?p=1136)
  - [充足可能性問題 (SAT; Satisfiability)](http://qard.is.tohoku.ac.jp/T-Wave/?p=651)
  - 最小重み最大マッチング問題 (Minimal Maximal Matching)
- 不等式を伴う問題
  - 集合被覆問題 (Set Cover)
  - [整数重みナップサック問題 (Knapsack with Integer Weights)](http://qard.is.tohoku.ac.jp/T-Wave/?p=69)
- 彩色問題 (Coloring Problems)
  - [グラフ彩色問題 (Graph Coloring)](http://qard.is.tohoku.ac.jp/T-Wave/?p=418)
  - [クリーク被覆問題 (Clique Cover)](http://qard.is.tohoku.ac.jp/T-Wave/?p=434)
  - [ジョブスケジューリング問題 (Job Sequencing with Integer Lengths)](http://qard.is.tohoku.ac.jp/T-Wave/?p=133)
- ハミルトンサイクル (Hamiltonian Cycles)
  - ハミルトンサイクル・ハミルトン路探索 (Hamiltonian Cycles and Paths)
  - 巡回セールスマン問題 (Traveling Salesman)
- 木問題 (Tree Problems)
  - 最大次数制約付き最小全域木（スパニング・ツリー）問題 (Minimal Spanning Tree with a Maximal Degree Constraint)
  - シュタイナー木 (Steiner Trees)
  - 有向フィードバック頂点集合問題 (Directed Feedback Vertex Set)
  - 無向フィードバック頂点集合問題 (Undirected Feedback Vertex Set)
  - フィードバック辺集合問題 (Feedback Edge Set)
- グラフ同型性判定問題 (Graph Isomorphism)

## あとがき
D-Waveマシンのプログラミングの核心とは、問題を表現するIsingスピングラスのハミルトニアンを書き下すことに他ならない。
本論文では、類型化された多くの組合せ最適化問題に対するハミルトニアンを網羅しており、実問題のハミルトニアンを設計する上で大変参考になるであろう。

### 本記事の担当者
みやままさみち