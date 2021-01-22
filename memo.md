# 様々なことメモ

## DOS と PDOS に用いるグラフについて
重みなし無向グラフとして全て扱う。

Networkx : https://networkx.org/documentation/stable/reference/generators.html
SNAP : https://snap.stanford.edu/snappy/doc/reference/generators.html

```
# SNAP GenCircle (https://snap.stanford.edu/snappy/doc/reference/GenCircle.html)
[
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/circular_graph_3000_1.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/circular_graph_3000_2.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/circular_graph_3000_3.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/circular_graph_3000_4.txt"
]

# circular ladder graph
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/circular_ladder_graph_n3000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/circular_ladder_graph_deleted_n3000_pdel0.1.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/circular_ladder_graph_deleted_n3000_pdel0.2.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/circular_ladder_graph_deleted_n3000_pdel0.3.txt",
]

# high dimention grid graph
[
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[100, 100].txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[40, 40, 40].txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[9, 9, 9, 9].txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[8, 8, 8, 8, 8].txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[7, 7, 7, 7, 7, 7].txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[6, 6, 6, 6, 6, 6, 6].txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[5, 5, 5, 5, 5, 5, 5, 5].txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_dim[4, 4, 4, 4, 4, 4, 4, 4, 4].txt",
]

# NetworkX 2d grid deleted(randomly)
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(100, 100)_pdel0.0.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(100, 100)_pdel0.2.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(100, 100)_pdel0.4.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(100, 100)_pdel0.6.txt",
]
# NetworkX 3d grid deleted(randomly)
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(40, 40, 40)_pdel0.0.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(40, 40, 40)_pdel0.2.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(40, 40, 40)_pdel0.4.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/grid_graph_deleted_dim(40, 40, 40)_pdel0.6.txt",
]


# balanced tree
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/balanced_tree_r2_h10.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/balanced_tree_r3_h8.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/balanced_tree_r4_h7.txt"
]

# NetworkX random graph
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/gnm_random_graph_n10000_m10000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/gnm_random_graph_n10000_m15000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/gnm_random_graph_n10000_m20000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/gnm_random_graph_n10000_m100000.txt",
]

# random regular graph
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_regular_graph_d3_n5000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_regular_graph_d4_n5000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_regular_graph_d8_n5000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_regular_graph_d15_n5000.txt",
]

# random geometric graph 2d
[
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.02_dim2.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.03_dim2.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.04_dim2.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.05_dim2.txt",

]

# random geometric graph 3d
[
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.08_dim3.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.1_dim3.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.12_dim3.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.14_dim3.txt",

]

# random geometric graph 10d
[
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.5_dim10.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.55_dim10.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.65_dim10.txt",
"/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/random_geometric_graph_n3000_radius0.7_dim10.txt",

]


# NetworkX soft random geometric

# SNAP scale-free(barabasi_albert)
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/barabasi_albert_graph_n3000_m2.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/barabasi_albert_graph_n3000_m3.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/barabasi_albert_graph_n3000_m4.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/barabasi_albert_graph_n3000_m5.txt",
]

# SNAP scale-free geometric
[
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/scale-free_geometric_3000_5_0.00.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/scale-free_geometric_3000_5_0.02.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/scale-free_geometric_3000_5_0.04.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/scale-free_geometric_3000_5_0.06.txt",

]

# SNAP small_world
[
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/small_world_5000_5_0.001.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/small_world_5000_5_0.010.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/small_world_5000_5_0.100.txt"
]

# NetworkX navigable small world

# NetworkX powerlaw cluster
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/powerlaw_cluster_graph_n3000_m5_p0.1.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/powerlaw_cluster_graph_n3000_m5_p0.3.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/powerlaw_cluster_graph_n3000_m5_p0.5.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/powerlaw_cluster_graph_n3000_m5_p0.8.txt",

]
# NetworkX random internet as graph

# SNAP forest fire
[
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/forest_fire_5000_0.30_0.30.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/forest_fire_5000_0.35_0.30.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/forest_fire_5000_0.40_0.30.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/gen_model/forest_fire_5000_0.45_0.30.txt"
  ]


# others
[
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/barbell_graph_Km100_Pm1000.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/triangular_lattice_graph_m100_n100.txt",
  "/Users/murakaminaoki/git/research/pyDOS/data/generated_graphs/hexagonal_lattice_graph_m100_n100.txt",

]

```

## 注意

・bibtex だけでは不十分。資料を見て参考文献の表記法を確認すること

## 何の役に立つのか

・作成したモデルの検証が可能（実際のモデルと比較して良いモデルにできているのか？）
. In particular, evaluating similarity between graphs is crucial to network analysis and
graph-based anomaly detection (Papadimitriou et al., 2010;　 Akoglu et al., 2015; Ranshous et al., 2015).
