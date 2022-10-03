---
pipeline_tag: sentence-similarity
tags:
- sentence-transformers
- feature-extraction
- sentence-similarity
- mteb
language: en
license: apache-2.0
datasets:
- s2orc
- flax-sentence-embeddings/stackexchange_xml
- MS Marco
- gooaq
- yahoo_answers_topics
- code_search_net
- search_qa
- eli5
- snli
- multi_nli
- wikihow
- natural_questions
- trivia_qa
- embedding-data/sentence-compression
- embedding-data/flickr30k-captions
- embedding-data/altlex
- embedding-data/simple-wiki
- embedding-data/QQP
- embedding-data/SPECTER
- embedding-data/PAQ_pairs
- embedding-data/WikiAnswers
model-index:
- name: all-mpnet-base-v2
  results:
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_counterfactual
      name: MTEB AmazonCounterfactualClassification (en)
      config: en
      split: test
      revision: 2d8a100785abf0ae21420d2a55b0c56e3e1ea996
    metrics:
    - type: accuracy
      value: 65.26865671641791
    - type: ap
      value: 28.47453420428918
    - type: f1
      value: 59.3470101009448
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_polarity
      name: MTEB AmazonPolarityClassification
      config: default
      split: test
      revision: 80714f8dcf8cefc218ef4f8c5a966dd83f75a0e1
    metrics:
    - type: accuracy
      value: 67.13145
    - type: ap
      value: 61.842060778903786
    - type: f1
      value: 66.79987305640383
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_reviews_multi
      name: MTEB AmazonReviewsClassification (en)
      config: en
      split: test
      revision: c379a6705fec24a2493fa68e011692605f44e119
    metrics:
    - type: accuracy
      value: 31.920000000000005
    - type: f1
      value: 31.2465193896153
  - task:
      type: Retrieval
    dataset:
      type: arguana
      name: MTEB ArguAna
      config: default
      split: test
      revision: 5b3e3697907184a9b77a3c99ee9ea1a9cbb1e4e3
    metrics:
    - type: map_at_1
      value: 23.186
    - type: map_at_10
      value: 37.692
    - type: map_at_100
      value: 38.986
    - type: map_at_1000
      value: 38.991
    - type: map_at_3
      value: 32.622
    - type: map_at_5
      value: 35.004999999999995
    - type: ndcg_at_1
      value: 23.186
    - type: ndcg_at_10
      value: 46.521
    - type: ndcg_at_100
      value: 51.954
    - type: ndcg_at_1000
      value: 52.087
    - type: ndcg_at_3
      value: 35.849
    - type: ndcg_at_5
      value: 40.12
    - type: precision_at_1
      value: 23.186
    - type: precision_at_10
      value: 7.510999999999999
    - type: precision_at_100
      value: 0.9860000000000001
    - type: precision_at_1000
      value: 0.1
    - type: precision_at_3
      value: 15.078
    - type: precision_at_5
      value: 11.110000000000001
    - type: recall_at_1
      value: 23.186
    - type: recall_at_10
      value: 75.107
    - type: recall_at_100
      value: 98.649
    - type: recall_at_1000
      value: 99.644
    - type: recall_at_3
      value: 45.235
    - type: recall_at_5
      value: 55.547999999999995
  - task:
      type: Clustering
    dataset:
      type: mteb/arxiv-clustering-p2p
      name: MTEB ArxivClusteringP2P
      config: default
      split: test
      revision: 0bbdb47bcbe3a90093699aefeed338a0f28a7ee8
    metrics:
    - type: v_measure
      value: 48.37886340922374
  - task:
      type: Clustering
    dataset:
      type: mteb/arxiv-clustering-s2s
      name: MTEB ArxivClusteringS2S
      config: default
      split: test
      revision: b73bd54100e5abfa6e3a23dcafb46fe4d2438dc3
    metrics:
    - type: v_measure
      value: 39.72488615315985
  - task:
      type: Reranking
    dataset:
      type: mteb/askubuntudupquestions-reranking
      name: MTEB AskUbuntuDupQuestions
      config: default
      split: test
      revision: 4d853f94cd57d85ec13805aeeac3ae3e5eb4c49c
    metrics:
    - type: map
      value: 65.85199009344481
    - type: mrr
      value: 78.47700391329201
  - task:
      type: STS
    dataset:
      type: mteb/biosses-sts
      name: MTEB BIOSSES
      config: default
      split: test
      revision: 9ee918f184421b6bd48b78f6c714d86546106103
    metrics:
    - type: cos_sim_pearson
      value: 84.47737119217858
    - type: cos_sim_spearman
      value: 80.43195317854409
    - type: euclidean_pearson
      value: 82.20496332547978
    - type: euclidean_spearman
      value: 80.43195317854409
    - type: manhattan_pearson
      value: 81.4836610720397
    - type: manhattan_spearman
      value: 79.65904400101908
  - task:
      type: Classification
    dataset:
      type: mteb/banking77
      name: MTEB Banking77Classification
      config: default
      split: test
      revision: 44fa15921b4c889113cc5df03dd4901b49161ab7
    metrics:
    - type: accuracy
      value: 81.8603896103896
    - type: f1
      value: 81.28027245637479
  - task:
      type: Clustering
    dataset:
      type: mteb/biorxiv-clustering-p2p
      name: MTEB BiorxivClusteringP2P
      config: default
      split: test
      revision: 11d0121201d1f1f280e8cc8f3d98fb9c4d9f9c55
    metrics:
    - type: v_measure
      value: 39.616605133625185
  - task:
      type: Clustering
    dataset:
      type: mteb/biorxiv-clustering-s2s
      name: MTEB BiorxivClusteringS2S
      config: default
      split: test
      revision: c0fab014e1bcb8d3a5e31b2088972a1e01547dc1
    metrics:
    - type: v_measure
      value: 35.02442407186902
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackAndroidRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 36.036
    - type: map_at_10
      value: 49.302
    - type: map_at_100
      value: 50.956
    - type: map_at_1000
      value: 51.080000000000005
    - type: map_at_3
      value: 45.237
    - type: map_at_5
      value: 47.353
    - type: ndcg_at_1
      value: 45.207
    - type: ndcg_at_10
      value: 56.485
    - type: ndcg_at_100
      value: 61.413
    - type: ndcg_at_1000
      value: 62.870000000000005
    - type: ndcg_at_3
      value: 51.346000000000004
    - type: ndcg_at_5
      value: 53.486
    - type: precision_at_1
      value: 45.207
    - type: precision_at_10
      value: 11.144
    - type: precision_at_100
      value: 1.735
    - type: precision_at_1000
      value: 0.22100000000000003
    - type: precision_at_3
      value: 24.94
    - type: precision_at_5
      value: 17.997
    - type: recall_at_1
      value: 36.036
    - type: recall_at_10
      value: 69.191
    - type: recall_at_100
      value: 89.423
    - type: recall_at_1000
      value: 98.425
    - type: recall_at_3
      value: 53.849999999999994
    - type: recall_at_5
      value: 60.107
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackEnglishRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 32.92
    - type: map_at_10
      value: 45.739999999999995
    - type: map_at_100
      value: 47.309
    - type: map_at_1000
      value: 47.443000000000005
    - type: map_at_3
      value: 42.154
    - type: map_at_5
      value: 44.207
    - type: ndcg_at_1
      value: 42.229
    - type: ndcg_at_10
      value: 52.288999999999994
    - type: ndcg_at_100
      value: 57.04900000000001
    - type: ndcg_at_1000
      value: 58.788
    - type: ndcg_at_3
      value: 47.531
    - type: ndcg_at_5
      value: 49.861
    - type: precision_at_1
      value: 42.229
    - type: precision_at_10
      value: 10.299
    - type: precision_at_100
      value: 1.68
    - type: precision_at_1000
      value: 0.213
    - type: precision_at_3
      value: 23.673
    - type: precision_at_5
      value: 17.006
    - type: recall_at_1
      value: 32.92
    - type: recall_at_10
      value: 63.865
    - type: recall_at_100
      value: 84.06700000000001
    - type: recall_at_1000
      value: 94.536
    - type: recall_at_3
      value: 49.643
    - type: recall_at_5
      value: 56.119
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackGamingRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 40.695
    - type: map_at_10
      value: 53.787
    - type: map_at_100
      value: 54.778000000000006
    - type: map_at_1000
      value: 54.827000000000005
    - type: map_at_3
      value: 50.151999999999994
    - type: map_at_5
      value: 52.207
    - type: ndcg_at_1
      value: 46.52
    - type: ndcg_at_10
      value: 60.026
    - type: ndcg_at_100
      value: 63.81099999999999
    - type: ndcg_at_1000
      value: 64.741
    - type: ndcg_at_3
      value: 53.83
    - type: ndcg_at_5
      value: 56.928999999999995
    - type: precision_at_1
      value: 46.52
    - type: precision_at_10
      value: 9.754999999999999
    - type: precision_at_100
      value: 1.2670000000000001
    - type: precision_at_1000
      value: 0.13799999999999998
    - type: precision_at_3
      value: 24.096
    - type: precision_at_5
      value: 16.689999999999998
    - type: recall_at_1
      value: 40.695
    - type: recall_at_10
      value: 75.181
    - type: recall_at_100
      value: 91.479
    - type: recall_at_1000
      value: 98.06899999999999
    - type: recall_at_3
      value: 58.707
    - type: recall_at_5
      value: 66.295
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackGisRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 29.024
    - type: map_at_10
      value: 38.438
    - type: map_at_100
      value: 39.576
    - type: map_at_1000
      value: 39.645
    - type: map_at_3
      value: 34.827999999999996
    - type: map_at_5
      value: 36.947
    - type: ndcg_at_1
      value: 31.299
    - type: ndcg_at_10
      value: 44.268
    - type: ndcg_at_100
      value: 49.507
    - type: ndcg_at_1000
      value: 51.205999999999996
    - type: ndcg_at_3
      value: 37.248999999999995
    - type: ndcg_at_5
      value: 40.861999999999995
    - type: precision_at_1
      value: 31.299
    - type: precision_at_10
      value: 6.949
    - type: precision_at_100
      value: 1.012
    - type: precision_at_1000
      value: 0.11900000000000001
    - type: precision_at_3
      value: 15.518
    - type: precision_at_5
      value: 11.366999999999999
    - type: recall_at_1
      value: 29.024
    - type: recall_at_10
      value: 60.404
    - type: recall_at_100
      value: 83.729
    - type: recall_at_1000
      value: 96.439
    - type: recall_at_3
      value: 41.65
    - type: recall_at_5
      value: 50.263999999999996
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackMathematicaRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 17.774
    - type: map_at_10
      value: 28.099
    - type: map_at_100
      value: 29.603
    - type: map_at_1000
      value: 29.709999999999997
    - type: map_at_3
      value: 25.036
    - type: map_at_5
      value: 26.657999999999998
    - type: ndcg_at_1
      value: 22.139
    - type: ndcg_at_10
      value: 34.205999999999996
    - type: ndcg_at_100
      value: 40.844
    - type: ndcg_at_1000
      value: 43.144
    - type: ndcg_at_3
      value: 28.732999999999997
    - type: ndcg_at_5
      value: 31.252000000000002
    - type: precision_at_1
      value: 22.139
    - type: precision_at_10
      value: 6.567
    - type: precision_at_100
      value: 1.147
    - type: precision_at_1000
      value: 0.146
    - type: precision_at_3
      value: 14.386
    - type: precision_at_5
      value: 10.423
    - type: recall_at_1
      value: 17.774
    - type: recall_at_10
      value: 48.32
    - type: recall_at_100
      value: 76.373
    - type: recall_at_1000
      value: 92.559
    - type: recall_at_3
      value: 33.478
    - type: recall_at_5
      value: 39.872
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackPhysicsRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 31.885
    - type: map_at_10
      value: 44.289
    - type: map_at_100
      value: 45.757999999999996
    - type: map_at_1000
      value: 45.86
    - type: map_at_3
      value: 40.459
    - type: map_at_5
      value: 42.662
    - type: ndcg_at_1
      value: 39.75
    - type: ndcg_at_10
      value: 50.975
    - type: ndcg_at_100
      value: 56.528999999999996
    - type: ndcg_at_1000
      value: 58.06099999999999
    - type: ndcg_at_3
      value: 45.327
    - type: ndcg_at_5
      value: 48.041
    - type: precision_at_1
      value: 39.75
    - type: precision_at_10
      value: 9.557
    - type: precision_at_100
      value: 1.469
    - type: precision_at_1000
      value: 0.17700000000000002
    - type: precision_at_3
      value: 22.073
    - type: precision_at_5
      value: 15.765
    - type: recall_at_1
      value: 31.885
    - type: recall_at_10
      value: 64.649
    - type: recall_at_100
      value: 87.702
    - type: recall_at_1000
      value: 97.327
    - type: recall_at_3
      value: 48.61
    - type: recall_at_5
      value: 55.882
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackProgrammersRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 26.454
    - type: map_at_10
      value: 37.756
    - type: map_at_100
      value: 39.225
    - type: map_at_1000
      value: 39.332
    - type: map_at_3
      value: 34.115
    - type: map_at_5
      value: 35.942
    - type: ndcg_at_1
      value: 32.42
    - type: ndcg_at_10
      value: 44.165
    - type: ndcg_at_100
      value: 50.202000000000005
    - type: ndcg_at_1000
      value: 52.188
    - type: ndcg_at_3
      value: 38.381
    - type: ndcg_at_5
      value: 40.849000000000004
    - type: precision_at_1
      value: 32.42
    - type: precision_at_10
      value: 8.482000000000001
    - type: precision_at_100
      value: 1.332
    - type: precision_at_1000
      value: 0.169
    - type: precision_at_3
      value: 18.683
    - type: precision_at_5
      value: 13.539000000000001
    - type: recall_at_1
      value: 26.454
    - type: recall_at_10
      value: 57.937000000000005
    - type: recall_at_100
      value: 83.76
    - type: recall_at_1000
      value: 96.82600000000001
    - type: recall_at_3
      value: 41.842
    - type: recall_at_5
      value: 48.285
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 27.743666666666666
    - type: map_at_10
      value: 38.75416666666667
    - type: map_at_100
      value: 40.133250000000004
    - type: map_at_1000
      value: 40.24616666666667
    - type: map_at_3
      value: 35.267250000000004
    - type: map_at_5
      value: 37.132749999999994
    - type: ndcg_at_1
      value: 33.14358333333333
    - type: ndcg_at_10
      value: 44.95916666666667
    - type: ndcg_at_100
      value: 50.46375
    - type: ndcg_at_1000
      value: 52.35508333333334
    - type: ndcg_at_3
      value: 39.17883333333334
    - type: ndcg_at_5
      value: 41.79724999999999
    - type: precision_at_1
      value: 33.14358333333333
    - type: precision_at_10
      value: 8.201083333333333
    - type: precision_at_100
      value: 1.3085
    - type: precision_at_1000
      value: 0.1665833333333333
    - type: precision_at_3
      value: 18.405583333333333
    - type: precision_at_5
      value: 13.233166666666666
    - type: recall_at_1
      value: 27.743666666666666
    - type: recall_at_10
      value: 58.91866666666667
    - type: recall_at_100
      value: 82.76216666666666
    - type: recall_at_1000
      value: 95.56883333333333
    - type: recall_at_3
      value: 42.86925
    - type: recall_at_5
      value: 49.553333333333335
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackStatsRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 25.244
    - type: map_at_10
      value: 33.464
    - type: map_at_100
      value: 34.633
    - type: map_at_1000
      value: 34.721999999999994
    - type: map_at_3
      value: 30.784
    - type: map_at_5
      value: 32.183
    - type: ndcg_at_1
      value: 28.681
    - type: ndcg_at_10
      value: 38.149
    - type: ndcg_at_100
      value: 43.856
    - type: ndcg_at_1000
      value: 46.026
    - type: ndcg_at_3
      value: 33.318
    - type: ndcg_at_5
      value: 35.454
    - type: precision_at_1
      value: 28.681
    - type: precision_at_10
      value: 6.304
    - type: precision_at_100
      value: 0.992
    - type: precision_at_1000
      value: 0.125
    - type: precision_at_3
      value: 14.673
    - type: precision_at_5
      value: 10.245
    - type: recall_at_1
      value: 25.244
    - type: recall_at_10
      value: 49.711
    - type: recall_at_100
      value: 75.928
    - type: recall_at_1000
      value: 91.79899999999999
    - type: recall_at_3
      value: 36.325
    - type: recall_at_5
      value: 41.752
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackTexRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 18.857
    - type: map_at_10
      value: 27.794
    - type: map_at_100
      value: 29.186
    - type: map_at_1000
      value: 29.323
    - type: map_at_3
      value: 24.779
    - type: map_at_5
      value: 26.459
    - type: ndcg_at_1
      value: 23.227999999999998
    - type: ndcg_at_10
      value: 33.353
    - type: ndcg_at_100
      value: 39.598
    - type: ndcg_at_1000
      value: 42.268
    - type: ndcg_at_3
      value: 28.054000000000002
    - type: ndcg_at_5
      value: 30.566
    - type: precision_at_1
      value: 23.227999999999998
    - type: precision_at_10
      value: 6.397
    - type: precision_at_100
      value: 1.129
    - type: precision_at_1000
      value: 0.155
    - type: precision_at_3
      value: 13.616
    - type: precision_at_5
      value: 10.116999999999999
    - type: recall_at_1
      value: 18.857
    - type: recall_at_10
      value: 45.797
    - type: recall_at_100
      value: 73.615
    - type: recall_at_1000
      value: 91.959
    - type: recall_at_3
      value: 31.129
    - type: recall_at_5
      value: 37.565
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackUnixRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 27.486
    - type: map_at_10
      value: 39.164
    - type: map_at_100
      value: 40.543
    - type: map_at_1000
      value: 40.636
    - type: map_at_3
      value: 35.52
    - type: map_at_5
      value: 37.355
    - type: ndcg_at_1
      value: 32.275999999999996
    - type: ndcg_at_10
      value: 45.414
    - type: ndcg_at_100
      value: 51.254
    - type: ndcg_at_1000
      value: 53.044000000000004
    - type: ndcg_at_3
      value: 39.324999999999996
    - type: ndcg_at_5
      value: 41.835
    - type: precision_at_1
      value: 32.275999999999996
    - type: precision_at_10
      value: 8.144
    - type: precision_at_100
      value: 1.237
    - type: precision_at_1000
      value: 0.15
    - type: precision_at_3
      value: 18.501
    - type: precision_at_5
      value: 13.134
    - type: recall_at_1
      value: 27.486
    - type: recall_at_10
      value: 60.449
    - type: recall_at_100
      value: 85.176
    - type: recall_at_1000
      value: 97.087
    - type: recall_at_3
      value: 43.59
    - type: recall_at_5
      value: 50.08899999999999
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackWebmastersRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 26.207
    - type: map_at_10
      value: 37.255
    - type: map_at_100
      value: 39.043
    - type: map_at_1000
      value: 39.273
    - type: map_at_3
      value: 33.487
    - type: map_at_5
      value: 35.441
    - type: ndcg_at_1
      value: 31.423000000000002
    - type: ndcg_at_10
      value: 44.235
    - type: ndcg_at_100
      value: 50.49
    - type: ndcg_at_1000
      value: 52.283
    - type: ndcg_at_3
      value: 37.602000000000004
    - type: ndcg_at_5
      value: 40.518
    - type: precision_at_1
      value: 31.423000000000002
    - type: precision_at_10
      value: 8.715
    - type: precision_at_100
      value: 1.7590000000000001
    - type: precision_at_1000
      value: 0.257
    - type: precision_at_3
      value: 17.523
    - type: precision_at_5
      value: 13.161999999999999
    - type: recall_at_1
      value: 26.207
    - type: recall_at_10
      value: 59.17099999999999
    - type: recall_at_100
      value: 86.166
    - type: recall_at_1000
      value: 96.54700000000001
    - type: recall_at_3
      value: 41.18
    - type: recall_at_5
      value: 48.083999999999996
  - task:
      type: Retrieval
    dataset:
      type: BeIR/cqadupstack
      name: MTEB CQADupstackWordpressRetrieval
      config: default
      split: test
      revision: 2b9f5791698b5be7bc5e10535c8690f20043c3db
    metrics:
    - type: map_at_1
      value: 20.342
    - type: map_at_10
      value: 29.962
    - type: map_at_100
      value: 30.989
    - type: map_at_1000
      value: 31.102999999999998
    - type: map_at_3
      value: 26.656000000000002
    - type: map_at_5
      value: 28.179
    - type: ndcg_at_1
      value: 22.551
    - type: ndcg_at_10
      value: 35.945
    - type: ndcg_at_100
      value: 41.012
    - type: ndcg_at_1000
      value: 43.641999999999996
    - type: ndcg_at_3
      value: 29.45
    - type: ndcg_at_5
      value: 31.913999999999998
    - type: precision_at_1
      value: 22.551
    - type: precision_at_10
      value: 6.1
    - type: precision_at_100
      value: 0.943
    - type: precision_at_1000
      value: 0.129
    - type: precision_at_3
      value: 13.184999999999999
    - type: precision_at_5
      value: 9.353
    - type: recall_at_1
      value: 20.342
    - type: recall_at_10
      value: 52.349000000000004
    - type: recall_at_100
      value: 75.728
    - type: recall_at_1000
      value: 95.253
    - type: recall_at_3
      value: 34.427
    - type: recall_at_5
      value: 40.326
  - task:
      type: Retrieval
    dataset:
      type: climate-fever
      name: MTEB ClimateFEVER
      config: default
      split: test
      revision: 392b78eb68c07badcd7c2cd8f39af108375dfcce
    metrics:
    - type: map_at_1
      value: 7.71
    - type: map_at_10
      value: 14.81
    - type: map_at_100
      value: 16.536
    - type: map_at_1000
      value: 16.744999999999997
    - type: map_at_3
      value: 12.109
    - type: map_at_5
      value: 13.613
    - type: ndcg_at_1
      value: 18.046
    - type: ndcg_at_10
      value: 21.971
    - type: ndcg_at_100
      value: 29.468
    - type: ndcg_at_1000
      value: 33.428999999999995
    - type: ndcg_at_3
      value: 17.227999999999998
    - type: ndcg_at_5
      value: 19.189999999999998
    - type: precision_at_1
      value: 18.046
    - type: precision_at_10
      value: 7.192
    - type: precision_at_100
      value: 1.51
    - type: precision_at_1000
      value: 0.22499999999999998
    - type: precision_at_3
      value: 13.312
    - type: precision_at_5
      value: 10.775
    - type: recall_at_1
      value: 7.71
    - type: recall_at_10
      value: 27.908
    - type: recall_at_100
      value: 54.452
    - type: recall_at_1000
      value: 76.764
    - type: recall_at_3
      value: 16.64
    - type: recall_at_5
      value: 21.631
  - task:
      type: Retrieval
    dataset:
      type: dbpedia-entity
      name: MTEB DBPedia
      config: default
      split: test
      revision: f097057d03ed98220bc7309ddb10b71a54d667d6
    metrics:
    - type: map_at_1
      value: 6.8180000000000005
    - type: map_at_10
      value: 14.591000000000001
    - type: map_at_100
      value: 19.855999999999998
    - type: map_at_1000
      value: 21.178
    - type: map_at_3
      value: 10.345
    - type: map_at_5
      value: 12.367
    - type: ndcg_at_1
      value: 39.25
    - type: ndcg_at_10
      value: 32.088
    - type: ndcg_at_100
      value: 36.019
    - type: ndcg_at_1000
      value: 43.649
    - type: ndcg_at_3
      value: 35.132999999999996
    - type: ndcg_at_5
      value: 33.777
    - type: precision_at_1
      value: 49.5
    - type: precision_at_10
      value: 25.624999999999996
    - type: precision_at_100
      value: 8.043
    - type: precision_at_1000
      value: 1.7409999999999999
    - type: precision_at_3
      value: 38.417
    - type: precision_at_5
      value: 33.2
    - type: recall_at_1
      value: 6.8180000000000005
    - type: recall_at_10
      value: 20.399
    - type: recall_at_100
      value: 42.8
    - type: recall_at_1000
      value: 68.081
    - type: recall_at_3
      value: 11.928999999999998
    - type: recall_at_5
      value: 15.348999999999998
  - task:
      type: Classification
    dataset:
      type: mteb/emotion
      name: MTEB EmotionClassification
      config: default
      split: test
      revision: 829147f8f75a25f005913200eb5ed41fae320aa1
    metrics:
    - type: accuracy
      value: 39.725
    - type: f1
      value: 35.19385687310605
  - task:
      type: Retrieval
    dataset:
      type: fever
      name: MTEB FEVER
      config: default
      split: test
      revision: 1429cf27e393599b8b359b9b72c666f96b2525f9
    metrics:
    - type: map_at_1
      value: 31.901000000000003
    - type: map_at_10
      value: 44.156
    - type: map_at_100
      value: 44.901
    - type: map_at_1000
      value: 44.939
    - type: map_at_3
      value: 41.008
    - type: map_at_5
      value: 42.969
    - type: ndcg_at_1
      value: 34.263
    - type: ndcg_at_10
      value: 50.863
    - type: ndcg_at_100
      value: 54.336
    - type: ndcg_at_1000
      value: 55.297
    - type: ndcg_at_3
      value: 44.644
    - type: ndcg_at_5
      value: 48.075
    - type: precision_at_1
      value: 34.263
    - type: precision_at_10
      value: 7.542999999999999
    - type: precision_at_100
      value: 0.9400000000000001
    - type: precision_at_1000
      value: 0.104
    - type: precision_at_3
      value: 18.912000000000003
    - type: precision_at_5
      value: 13.177
    - type: recall_at_1
      value: 31.901000000000003
    - type: recall_at_10
      value: 68.872
    - type: recall_at_100
      value: 84.468
    - type: recall_at_1000
      value: 91.694
    - type: recall_at_3
      value: 52.272
    - type: recall_at_5
      value: 60.504999999999995
  - task:
      type: Retrieval
    dataset:
      type: fiqa
      name: MTEB FiQA2018
      config: default
      split: test
      revision: 41b686a7f28c59bcaaa5791efd47c67c8ebe28be
    metrics:
    - type: map_at_1
      value: 24.4
    - type: map_at_10
      value: 41.117
    - type: map_at_100
      value: 43.167
    - type: map_at_1000
      value: 43.323
    - type: map_at_3
      value: 35.744
    - type: map_at_5
      value: 38.708
    - type: ndcg_at_1
      value: 49.074
    - type: ndcg_at_10
      value: 49.963
    - type: ndcg_at_100
      value: 56.564
    - type: ndcg_at_1000
      value: 58.931999999999995
    - type: ndcg_at_3
      value: 45.489000000000004
    - type: ndcg_at_5
      value: 47.133
    - type: precision_at_1
      value: 49.074
    - type: precision_at_10
      value: 13.889000000000001
    - type: precision_at_100
      value: 2.091
    - type: precision_at_1000
      value: 0.251
    - type: precision_at_3
      value: 30.658
    - type: precision_at_5
      value: 22.593
    - type: recall_at_1
      value: 24.4
    - type: recall_at_10
      value: 58.111999999999995
    - type: recall_at_100
      value: 81.96900000000001
    - type: recall_at_1000
      value: 96.187
    - type: recall_at_3
      value: 41.661
    - type: recall_at_5
      value: 49.24
  - task:
      type: Retrieval
    dataset:
      type: hotpotqa
      name: MTEB HotpotQA
      config: default
      split: test
      revision: 766870b35a1b9ca65e67a0d1913899973551fc6c
    metrics:
    - type: map_at_1
      value: 22.262
    - type: map_at_10
      value: 31.266
    - type: map_at_100
      value: 32.202
    - type: map_at_1000
      value: 32.300000000000004
    - type: map_at_3
      value: 28.874
    - type: map_at_5
      value: 30.246000000000002
    - type: ndcg_at_1
      value: 44.524
    - type: ndcg_at_10
      value: 39.294000000000004
    - type: ndcg_at_100
      value: 43.296
    - type: ndcg_at_1000
      value: 45.561
    - type: ndcg_at_3
      value: 35.013
    - type: ndcg_at_5
      value: 37.177
    - type: precision_at_1
      value: 44.524
    - type: precision_at_10
      value: 8.52
    - type: precision_at_100
      value: 1.169
    - type: precision_at_1000
      value: 0.147
    - type: precision_at_3
      value: 22.003
    - type: precision_at_5
      value: 14.914
    - type: recall_at_1
      value: 22.262
    - type: recall_at_10
      value: 42.6
    - type: recall_at_100
      value: 58.46
    - type: recall_at_1000
      value: 73.565
    - type: recall_at_3
      value: 33.005
    - type: recall_at_5
      value: 37.286
  - task:
      type: Classification
    dataset:
      type: mteb/imdb
      name: MTEB ImdbClassification
      config: default
      split: test
      revision: 8d743909f834c38949e8323a8a6ce8721ea6c7f4
    metrics:
    - type: accuracy
      value: 70.7156
    - type: ap
      value: 64.89470531959896
    - type: f1
      value: 70.53051887683772
  - task:
      type: Retrieval
    dataset:
      type: msmarco
      name: MTEB MSMARCO
      config: default
      split: dev
      revision: e6838a846e2408f22cf5cc337ebc83e0bcf77849
    metrics:
    - type: map_at_1
      value: 21.174
    - type: map_at_10
      value: 33.0
    - type: map_at_100
      value: 34.178
    - type: map_at_1000
      value: 34.227000000000004
    - type: map_at_3
      value: 29.275000000000002
    - type: map_at_5
      value: 31.341
    - type: ndcg_at_1
      value: 21.776999999999997
    - type: ndcg_at_10
      value: 39.745999999999995
    - type: ndcg_at_100
      value: 45.488
    - type: ndcg_at_1000
      value: 46.733999999999995
    - type: ndcg_at_3
      value: 32.086
    - type: ndcg_at_5
      value: 35.792
    - type: precision_at_1
      value: 21.776999999999997
    - type: precision_at_10
      value: 6.324000000000001
    - type: precision_at_100
      value: 0.922
    - type: precision_at_1000
      value: 0.10300000000000001
    - type: precision_at_3
      value: 13.696
    - type: precision_at_5
      value: 10.100000000000001
    - type: recall_at_1
      value: 21.174
    - type: recall_at_10
      value: 60.488
    - type: recall_at_100
      value: 87.234
    - type: recall_at_1000
      value: 96.806
    - type: recall_at_3
      value: 39.582
    - type: recall_at_5
      value: 48.474000000000004
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_domain
      name: MTEB MTOPDomainClassification (en)
      config: en
      split: test
      revision: a7e2a951126a26fc8c6a69f835f33a346ba259e3
    metrics:
    - type: accuracy
      value: 92.07934336525308
    - type: f1
      value: 91.93440027035814
  - task:
      type: Classification
    dataset:
      type: mteb/mtop_intent
      name: MTEB MTOPIntentClassification (en)
      config: en
      split: test
      revision: 6299947a7777084cc2d4b64235bf7190381ce755
    metrics:
    - type: accuracy
      value: 70.20975832193344
    - type: f1
      value: 48.571776628850074
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_intent
      name: MTEB MassiveIntentClassification (en)
      config: en
      split: test
      revision: 072a486a144adf7f4479a4a0dddb2152e161e1ea
    metrics:
    - type: accuracy
      value: 69.56624075319435
    - type: f1
      value: 67.64419185784621
  - task:
      type: Classification
    dataset:
      type: mteb/amazon_massive_scenario
      name: MTEB MassiveScenarioClassification (en)
      config: en
      split: test
      revision: 7d571f92784cd94a019292a1f45445077d0ef634
    metrics:
    - type: accuracy
      value: 76.01210490921318
    - type: f1
      value: 75.1934366365826
  - task:
      type: Clustering
    dataset:
      type: mteb/medrxiv-clustering-p2p
      name: MTEB MedrxivClusteringP2P
      config: default
      split: test
      revision: dcefc037ef84348e49b0d29109e891c01067226b
    metrics:
    - type: v_measure
      value: 35.58002813186373
  - task:
      type: Clustering
    dataset:
      type: mteb/medrxiv-clustering-s2s
      name: MTEB MedrxivClusteringS2S
      config: default
      split: test
      revision: 3cd0e71dfbe09d4de0f9e5ecba43e7ce280959dc
    metrics:
    - type: v_measure
      value: 32.872725562410444
  - task:
      type: Reranking
    dataset:
      type: mteb/mind_small
      name: MTEB MindSmallReranking
      config: default
      split: test
      revision: 3bdac13927fdc888b903db93b2ffdbd90b295a69
    metrics:
    - type: map
      value: 30.965343604861328
    - type: mrr
      value: 31.933710165863594
  - task:
      type: Retrieval
    dataset:
      type: nfcorpus
      name: MTEB NFCorpus
      config: default
      split: test
      revision: 7eb63cc0c1eb59324d709ebed25fcab851fa7610
    metrics:
    - type: map_at_1
      value: 4.938
    - type: map_at_10
      value: 12.034
    - type: map_at_100
      value: 15.675
    - type: map_at_1000
      value: 17.18
    - type: map_at_3
      value: 8.471
    - type: map_at_5
      value: 10.128
    - type: ndcg_at_1
      value: 40.402
    - type: ndcg_at_10
      value: 33.289
    - type: ndcg_at_100
      value: 31.496000000000002
    - type: ndcg_at_1000
      value: 40.453
    - type: ndcg_at_3
      value: 37.841
    - type: ndcg_at_5
      value: 36.215
    - type: precision_at_1
      value: 41.796
    - type: precision_at_10
      value: 25.294
    - type: precision_at_100
      value: 8.381
    - type: precision_at_1000
      value: 2.1260000000000003
    - type: precision_at_3
      value: 36.429
    - type: precision_at_5
      value: 32.446000000000005
    - type: recall_at_1
      value: 4.938
    - type: recall_at_10
      value: 16.637
    - type: recall_at_100
      value: 33.853
    - type: recall_at_1000
      value: 66.07
    - type: recall_at_3
      value: 9.818
    - type: recall_at_5
      value: 12.544
  - task:
      type: Retrieval
    dataset:
      type: nq
      name: MTEB NQ
      config: default
      split: test
      revision: 6062aefc120bfe8ece5897809fb2e53bfe0d128c
    metrics:
    - type: map_at_1
      value: 27.124
    - type: map_at_10
      value: 42.418
    - type: map_at_100
      value: 43.633
    - type: map_at_1000
      value: 43.66
    - type: map_at_3
      value: 37.766
    - type: map_at_5
      value: 40.482
    - type: ndcg_at_1
      value: 30.794
    - type: ndcg_at_10
      value: 50.449999999999996
    - type: ndcg_at_100
      value: 55.437999999999995
    - type: ndcg_at_1000
      value: 56.084
    - type: ndcg_at_3
      value: 41.678
    - type: ndcg_at_5
      value: 46.257
    - type: precision_at_1
      value: 30.794
    - type: precision_at_10
      value: 8.656
    - type: precision_at_100
      value: 1.141
    - type: precision_at_1000
      value: 0.12
    - type: precision_at_3
      value: 19.37
    - type: precision_at_5
      value: 14.218
    - type: recall_at_1
      value: 27.124
    - type: recall_at_10
      value: 72.545
    - type: recall_at_100
      value: 93.938
    - type: recall_at_1000
      value: 98.788
    - type: recall_at_3
      value: 49.802
    - type: recall_at_5
      value: 60.426
  - task:
      type: Retrieval
    dataset:
      type: quora
      name: MTEB QuoraRetrieval
      config: default
      split: test
      revision: 6205996560df11e3a3da9ab4f926788fc30a7db4
    metrics:
    - type: map_at_1
      value: 69.33500000000001
    - type: map_at_10
      value: 83.554
    - type: map_at_100
      value: 84.237
    - type: map_at_1000
      value: 84.251
    - type: map_at_3
      value: 80.456
    - type: map_at_5
      value: 82.395
    - type: ndcg_at_1
      value: 80.06
    - type: ndcg_at_10
      value: 87.46199999999999
    - type: ndcg_at_100
      value: 88.774
    - type: ndcg_at_1000
      value: 88.864
    - type: ndcg_at_3
      value: 84.437
    - type: ndcg_at_5
      value: 86.129
    - type: precision_at_1
      value: 80.06
    - type: precision_at_10
      value: 13.418
    - type: precision_at_100
      value: 1.536
    - type: precision_at_1000
      value: 0.157
    - type: precision_at_3
      value: 37.103
    - type: precision_at_5
      value: 24.522
    - type: recall_at_1
      value: 69.33500000000001
    - type: recall_at_10
      value: 95.03200000000001
    - type: recall_at_100
      value: 99.559
    - type: recall_at_1000
      value: 99.98700000000001
    - type: recall_at_3
      value: 86.404
    - type: recall_at_5
      value: 91.12400000000001
  - task:
      type: Clustering
    dataset:
      type: mteb/reddit-clustering
      name: MTEB RedditClustering
      config: default
      split: test
      revision: b2805658ae38990172679479369a78b86de8c390
    metrics:
    - type: v_measure
      value: 54.824256698437324
  - task:
      type: Clustering
    dataset:
      type: mteb/reddit-clustering-p2p
      name: MTEB RedditClusteringP2P
      config: default
      split: test
      revision: 385e3cb46b4cfa89021f56c4380204149d0efe33
    metrics:
    - type: v_measure
      value: 56.768972678049366
  - task:
      type: Retrieval
    dataset:
      type: scidocs
      name: MTEB SCIDOCS
      config: default
      split: test
      revision: 5c59ef3e437a0a9651c8fe6fde943e7dce59fba5
    metrics:
    - type: map_at_1
      value: 5.192
    - type: map_at_10
      value: 14.426
    - type: map_at_100
      value: 17.18
    - type: map_at_1000
      value: 17.580000000000002
    - type: map_at_3
      value: 9.94
    - type: map_at_5
      value: 12.077
    - type: ndcg_at_1
      value: 25.5
    - type: ndcg_at_10
      value: 23.765
    - type: ndcg_at_100
      value: 33.664
    - type: ndcg_at_1000
      value: 39.481
    - type: ndcg_at_3
      value: 21.813
    - type: ndcg_at_5
      value: 19.285
    - type: precision_at_1
      value: 25.5
    - type: precision_at_10
      value: 12.690000000000001
    - type: precision_at_100
      value: 2.71
    - type: precision_at_1000
      value: 0.409
    - type: precision_at_3
      value: 20.732999999999997
    - type: precision_at_5
      value: 17.24
    - type: recall_at_1
      value: 5.192
    - type: recall_at_10
      value: 25.712000000000003
    - type: recall_at_100
      value: 54.99699999999999
    - type: recall_at_1000
      value: 82.97200000000001
    - type: recall_at_3
      value: 12.631999999999998
    - type: recall_at_5
      value: 17.497
  - task:
      type: STS
    dataset:
      type: mteb/sickr-sts
      name: MTEB SICK-R
      config: default
      split: test
      revision: 20a6d6f312dd54037fe07a32d58e5e168867909d
    metrics:
    - type: cos_sim_pearson
      value: 84.00280838354293
    - type: cos_sim_spearman
      value: 80.5854192844009
    - type: euclidean_pearson
      value: 80.55974827073891
    - type: euclidean_spearman
      value: 80.58541460172292
    - type: manhattan_pearson
      value: 80.27294578437488
    - type: manhattan_spearman
      value: 80.33176193921884
  - task:
      type: STS
    dataset:
      type: mteb/sts12-sts
      name: MTEB STS12
      config: default
      split: test
      revision: fdf84275bb8ce4b49c971d02e84dd1abc677a50f
    metrics:
    - type: cos_sim_pearson
      value: 83.2801353818369
    - type: cos_sim_spearman
      value: 72.63427853822449
    - type: euclidean_pearson
      value: 79.01343235899544
    - type: euclidean_spearman
      value: 72.63178302036903
    - type: manhattan_pearson
      value: 78.65899981586094
    - type: manhattan_spearman
      value: 72.26646573268035
  - task:
      type: STS
    dataset:
      type: mteb/sts13-sts
      name: MTEB STS13
      config: default
      split: test
      revision: 1591bfcbe8c69d4bf7fe2a16e2451017832cafb9
    metrics:
    - type: cos_sim_pearson
      value: 83.20700572036095
    - type: cos_sim_spearman
      value: 83.48499016384896
    - type: euclidean_pearson
      value: 82.82555353364394
    - type: euclidean_spearman
      value: 83.48499008964005
    - type: manhattan_pearson
      value: 82.46034885462956
    - type: manhattan_spearman
      value: 83.09829447251937
  - task:
      type: STS
    dataset:
      type: mteb/sts14-sts
      name: MTEB STS14
      config: default
      split: test
      revision: e2125984e7df8b7871f6ae9949cf6b6795e7c54b
    metrics:
    - type: cos_sim_pearson
      value: 82.27113025749529
    - type: cos_sim_spearman
      value: 78.0001371342168
    - type: euclidean_pearson
      value: 80.62651938409732
    - type: euclidean_spearman
      value: 78.0001341029446
    - type: manhattan_pearson
      value: 80.25786381999085
    - type: manhattan_spearman
      value: 77.68750207429126
  - task:
      type: STS
    dataset:
      type: mteb/sts15-sts
      name: MTEB STS15
      config: default
      split: test
      revision: 1cd7298cac12a96a373b6a2f18738bb3e739a9b6
    metrics:
    - type: cos_sim_pearson
      value: 84.98824030948605
    - type: cos_sim_spearman
      value: 85.66275391649481
    - type: euclidean_pearson
      value: 84.88733530073506
    - type: euclidean_spearman
      value: 85.66275062257034
    - type: manhattan_pearson
      value: 84.70100813924223
    - type: manhattan_spearman
      value: 85.50318526944764
  - task:
      type: STS
    dataset:
      type: mteb/sts16-sts
      name: MTEB STS16
      config: default
      split: test
      revision: 360a0b2dff98700d09e634a01e1cc1624d3e42cd
    metrics:
    - type: cos_sim_pearson
      value: 78.82478639193744
    - type: cos_sim_spearman
      value: 80.03011315645662
    - type: euclidean_pearson
      value: 79.84794502236802
    - type: euclidean_spearman
      value: 80.03011258077692
    - type: manhattan_pearson
      value: 79.47012152325492
    - type: manhattan_spearman
      value: 79.60652985087651
  - task:
      type: STS
    dataset:
      type: mteb/sts17-crosslingual-sts
      name: MTEB STS17 (en-en)
      config: en-en
      split: test
      revision: 9fc37e8c632af1c87a3d23e685d49552a02582a0
    metrics:
    - type: cos_sim_pearson
      value: 90.90804154377126
    - type: cos_sim_spearman
      value: 90.59523263123734
    - type: euclidean_pearson
      value: 89.8466957775513
    - type: euclidean_spearman
      value: 90.59523263123734
    - type: manhattan_pearson
      value: 89.82268413033941
    - type: manhattan_spearman
      value: 90.68706496728889
  - task:
      type: STS
    dataset:
      type: mteb/sts22-crosslingual-sts
      name: MTEB STS22 (en)
      config: en
      split: test
      revision: 2de6ce8c1921b71a755b262c6b57fef195dd7906
    metrics:
    - type: cos_sim_pearson
      value: 66.78771571400975
    - type: cos_sim_spearman
      value: 67.94534221542501
    - type: euclidean_pearson
      value: 68.62534447097993
    - type: euclidean_spearman
      value: 67.94534221542501
    - type: manhattan_pearson
      value: 68.35916011329631
    - type: manhattan_spearman
      value: 67.58212723406085
  - task:
      type: STS
    dataset:
      type: mteb/stsbenchmark-sts
      name: MTEB STSBenchmark
      config: default
      split: test
      revision: 8913289635987208e6e7c72789e4be2fe94b6abd
    metrics:
    - type: cos_sim_pearson
      value: 84.03996099800993
    - type: cos_sim_spearman
      value: 83.421898505618
    - type: euclidean_pearson
      value: 83.78671249317563
    - type: euclidean_spearman
      value: 83.4219042133061
    - type: manhattan_pearson
      value: 83.44085827249334
    - type: manhattan_spearman
      value: 83.02901331535297
  - task:
      type: Reranking
    dataset:
      type: mteb/scidocs-reranking
      name: MTEB SciDocsRR
      config: default
      split: test
      revision: 56a6d0140cf6356659e2a7c1413286a774468d44
    metrics:
    - type: map
      value: 88.65396986895777
    - type: mrr
      value: 96.60209525405604
  - task:
      type: Retrieval
    dataset:
      type: scifact
      name: MTEB SciFact
      config: default
      split: test
      revision: a75ae049398addde9b70f6b268875f5cbce99089
    metrics:
    - type: map_at_1
      value: 51.456
    - type: map_at_10
      value: 60.827
    - type: map_at_100
      value: 61.595
    - type: map_at_1000
      value: 61.629999999999995
    - type: map_at_3
      value: 57.518
    - type: map_at_5
      value: 59.435
    - type: ndcg_at_1
      value: 53.333
    - type: ndcg_at_10
      value: 65.57
    - type: ndcg_at_100
      value: 68.911
    - type: ndcg_at_1000
      value: 69.65299999999999
    - type: ndcg_at_3
      value: 60.009
    - type: ndcg_at_5
      value: 62.803
    - type: precision_at_1
      value: 53.333
    - type: precision_at_10
      value: 8.933
    - type: precision_at_100
      value: 1.0699999999999998
    - type: precision_at_1000
      value: 0.11299999999999999
    - type: precision_at_3
      value: 23.333000000000002
    - type: precision_at_5
      value: 15.8
    - type: recall_at_1
      value: 51.456
    - type: recall_at_10
      value: 79.011
    - type: recall_at_100
      value: 94.167
    - type: recall_at_1000
      value: 99.667
    - type: recall_at_3
      value: 64.506
    - type: recall_at_5
      value: 71.211
  - task:
      type: PairClassification
    dataset:
      type: mteb/sprintduplicatequestions-pairclassification
      name: MTEB SprintDuplicateQuestions
      config: default
      split: test
      revision: 5a8256d0dff9c4bd3be3ba3e67e4e70173f802ea
    metrics:
    - type: cos_sim_accuracy
      value: 99.65940594059406
    - type: cos_sim_ap
      value: 90.1455141683116
    - type: cos_sim_f1
      value: 82.26044226044226
    - type: cos_sim_precision
      value: 80.8695652173913
    - type: cos_sim_recall
      value: 83.7
    - type: dot_accuracy
      value: 99.65940594059406
    - type: dot_ap
      value: 90.1455141683116
    - type: dot_f1
      value: 82.26044226044226
    - type: dot_precision
      value: 80.8695652173913
    - type: dot_recall
      value: 83.7
    - type: euclidean_accuracy
      value: 99.65940594059406
    - type: euclidean_ap
      value: 90.14551416831162
    - type: euclidean_f1
      value: 82.26044226044226
    - type: euclidean_precision
      value: 80.8695652173913
    - type: euclidean_recall
      value: 83.7
    - type: manhattan_accuracy
      value: 99.64950495049504
    - type: manhattan_ap
      value: 89.5492617367771
    - type: manhattan_f1
      value: 81.58280410356619
    - type: manhattan_precision
      value: 79.75167144221585
    - type: manhattan_recall
      value: 83.5
    - type: max_accuracy
      value: 99.65940594059406
    - type: max_ap
      value: 90.14551416831162
    - type: max_f1
      value: 82.26044226044226
  - task:
      type: Clustering
    dataset:
      type: mteb/stackexchange-clustering
      name: MTEB StackExchangeClustering
      config: default
      split: test
      revision: 70a89468f6dccacc6aa2b12a6eac54e74328f235
    metrics:
    - type: v_measure
      value: 53.80048409076929
  - task:
      type: Clustering
    dataset:
      type: mteb/stackexchange-clustering-p2p
      name: MTEB StackExchangeClusteringP2P
      config: default
      split: test
      revision: d88009ab563dd0b16cfaf4436abaf97fa3550cf0
    metrics:
    - type: v_measure
      value: 34.280269334397545
  - task:
      type: Reranking
    dataset:
      type: mteb/stackoverflowdupquestions-reranking
      name: MTEB StackOverflowDupQuestions
      config: default
      split: test
      revision: ef807ea29a75ec4f91b50fd4191cb4ee4589a9f9
    metrics:
    - type: map
      value: 51.97907654945493
    - type: mrr
      value: 52.82873376623376
  - task:
      type: Summarization
    dataset:
      type: mteb/summeval
      name: MTEB SummEval
      config: default
      split: test
      revision: 8753c2788d36c01fc6f05d03fe3f7268d63f9122
    metrics:
    - type: cos_sim_pearson
      value: 28.364293841556304
    - type: cos_sim_spearman
      value: 27.485869639926136
    - type: dot_pearson
      value: 28.364295910221145
    - type: dot_spearman
      value: 27.485869639926136
  - task:
      type: Retrieval
    dataset:
      type: trec-covid
      name: MTEB TRECCOVID
      config: default
      split: test
      revision: 2c8041b2c07a79b6f7ba8fe6acc72e5d9f92d217
    metrics:
    - type: map_at_1
      value: 0.19499999999999998
    - type: map_at_10
      value: 1.218
    - type: map_at_100
      value: 7.061000000000001
    - type: map_at_1000
      value: 19.735
    - type: map_at_3
      value: 0.46499999999999997
    - type: map_at_5
      value: 0.672
    - type: ndcg_at_1
      value: 60.0
    - type: ndcg_at_10
      value: 51.32600000000001
    - type: ndcg_at_100
      value: 41.74
    - type: ndcg_at_1000
      value: 43.221
    - type: ndcg_at_3
      value: 54.989
    - type: ndcg_at_5
      value: 52.905
    - type: precision_at_1
      value: 66.0
    - type: precision_at_10
      value: 55.60000000000001
    - type: precision_at_100
      value: 43.34
    - type: precision_at_1000
      value: 19.994
    - type: precision_at_3
      value: 59.333000000000006
    - type: precision_at_5
      value: 57.199999999999996
    - type: recall_at_1
      value: 0.19499999999999998
    - type: recall_at_10
      value: 1.473
    - type: recall_at_100
      value: 10.596
    - type: recall_at_1000
      value: 42.466
    - type: recall_at_3
      value: 0.49899999999999994
    - type: recall_at_5
      value: 0.76
  - task:
      type: Retrieval
    dataset:
      type: webis-touche2020
      name: MTEB Touche2020
      config: default
      split: test
      revision: 527b7d77e16e343303e68cb6af11d6e18b9f7b3b
    metrics:
    - type: map_at_1
      value: 1.997
    - type: map_at_10
      value: 7.5569999999999995
    - type: map_at_100
      value: 12.238
    - type: map_at_1000
      value: 13.773
    - type: map_at_3
      value: 4.334
    - type: map_at_5
      value: 5.5
    - type: ndcg_at_1
      value: 22.448999999999998
    - type: ndcg_at_10
      value: 19.933999999999997
    - type: ndcg_at_100
      value: 30.525999999999996
    - type: ndcg_at_1000
      value: 43.147999999999996
    - type: ndcg_at_3
      value: 22.283
    - type: ndcg_at_5
      value: 21.224
    - type: precision_at_1
      value: 24.490000000000002
    - type: precision_at_10
      value: 17.551
    - type: precision_at_100
      value: 6.4079999999999995
    - type: precision_at_1000
      value: 1.463
    - type: precision_at_3
      value: 23.128999999999998
    - type: precision_at_5
      value: 20.816000000000003
    - type: recall_at_1
      value: 1.997
    - type: recall_at_10
      value: 13.001999999999999
    - type: recall_at_100
      value: 40.98
    - type: recall_at_1000
      value: 79.40899999999999
    - type: recall_at_3
      value: 5.380999999999999
    - type: recall_at_5
      value: 7.721
  - task:
      type: Classification
    dataset:
      type: mteb/toxic_conversations_50k
      name: MTEB ToxicConversationsClassification
      config: default
      split: test
      revision: edfaf9da55d3dd50d43143d90c1ac476895ae6de
    metrics:
    - type: accuracy
      value: 60.861200000000004
    - type: ap
      value: 11.39641747026629
    - type: f1
      value: 47.80230380517065
  - task:
      type: Classification
    dataset:
      type: mteb/tweet_sentiment_extraction
      name: MTEB TweetSentimentExtractionClassification
      config: default
      split: test
      revision: 62146448f05be9e52a36b8ee9936447ea787eede
    metrics:
    - type: accuracy
      value: 55.464063384267114
    - type: f1
      value: 55.759039643764666
  - task:
      type: Clustering
    dataset:
      type: mteb/twentynewsgroups-clustering
      name: MTEB TwentyNewsgroupsClustering
      config: default
      split: test
      revision: 091a54f9a36281ce7d6590ec8c75dd485e7e01d4
    metrics:
    - type: v_measure
      value: 49.74455348083809
  - task:
      type: PairClassification
    dataset:
      type: mteb/twittersemeval2015-pairclassification
      name: MTEB TwitterSemEval2015
      config: default
      split: test
      revision: 70970daeab8776df92f5ea462b6173c0b46fd2d1
    metrics:
    - type: cos_sim_accuracy
      value: 86.07617571675507
    - type: cos_sim_ap
      value: 73.85398650568216
    - type: cos_sim_f1
      value: 68.50702798531087
    - type: cos_sim_precision
      value: 65.86316045775506
    - type: cos_sim_recall
      value: 71.37203166226914
    - type: dot_accuracy
      value: 86.07617571675507
    - type: dot_ap
      value: 73.85398346238429
    - type: dot_f1
      value: 68.50702798531087
    - type: dot_precision
      value: 65.86316045775506
    - type: dot_recall
      value: 71.37203166226914
    - type: euclidean_accuracy
      value: 86.07617571675507
    - type: euclidean_ap
      value: 73.85398625060357
    - type: euclidean_f1
      value: 68.50702798531087
    - type: euclidean_precision
      value: 65.86316045775506
    - type: euclidean_recall
      value: 71.37203166226914
    - type: manhattan_accuracy
      value: 85.98676759849795
    - type: manhattan_ap
      value: 73.86874126878737
    - type: manhattan_f1
      value: 68.55096559662361
    - type: manhattan_precision
      value: 66.51774633904195
    - type: manhattan_recall
      value: 70.71240105540898
    - type: max_accuracy
      value: 86.07617571675507
    - type: max_ap
      value: 73.86874126878737
    - type: max_f1
      value: 68.55096559662361
  - task:
      type: PairClassification
    dataset:
      type: mteb/twitterurlcorpus-pairclassification
      name: MTEB TwitterURLCorpus
      config: default
      split: test
      revision: 8b6510b0b1fa4e4c4f879467980e9be563ec1cdf
    metrics:
    - type: cos_sim_accuracy
      value: 88.51631932316529
    - type: cos_sim_ap
      value: 85.10831084479727
    - type: cos_sim_f1
      value: 77.14563397129186
    - type: cos_sim_precision
      value: 74.9709386806161
    - type: cos_sim_recall
      value: 79.45026178010471
    - type: dot_accuracy
      value: 88.51631932316529
    - type: dot_ap
      value: 85.10831188797107
    - type: dot_f1
      value: 77.14563397129186
    - type: dot_precision
      value: 74.9709386806161
    - type: dot_recall
      value: 79.45026178010471
    - type: euclidean_accuracy
      value: 88.51631932316529
    - type: euclidean_ap
      value: 85.10829618408616
    - type: euclidean_f1
      value: 77.14563397129186
    - type: euclidean_precision
      value: 74.9709386806161
    - type: euclidean_recall
      value: 79.45026178010471
    - type: manhattan_accuracy
      value: 88.50467652423643
    - type: manhattan_ap
      value: 85.08329502055064
    - type: manhattan_f1
      value: 77.11157455683002
    - type: manhattan_precision
      value: 74.67541834968263
    - type: manhattan_recall
      value: 79.71204188481676
    - type: max_accuracy
      value: 88.51631932316529
    - type: max_ap
      value: 85.10831188797107
    - type: max_f1
      value: 77.14563397129186
---


# all-mpnet-base-v2
This is a [sentence-transformers](https://www.SBERT.net) model: It maps sentences & paragraphs to a 768 dimensional dense vector space and can be used for tasks like clustering or semantic search.

## Usage (Sentence-Transformers)
Using this model becomes easy when you have [sentence-transformers](https://www.SBERT.net) installed:

```
pip install -U sentence-transformers
```

Then you can use the model like this:
```python
from sentence_transformers import SentenceTransformer
sentences = ["This is an example sentence", "Each sentence is converted"]

model = SentenceTransformer('sentence-transformers/all-mpnet-base-v2')
embeddings = model.encode(sentences)
print(embeddings)
```

## Usage (HuggingFace Transformers)
Without [sentence-transformers](https://www.SBERT.net), you can use the model like this: First, you pass your input through the transformer model, then you have to apply the right pooling-operation on-top of the contextualized word embeddings.

```python
from transformers import AutoTokenizer, AutoModel
import torch
import torch.nn.functional as F

#Mean Pooling - Take attention mask into account for correct averaging
def mean_pooling(model_output, attention_mask):
    token_embeddings = model_output[0] #First element of model_output contains all token embeddings
    input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
    return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)


# Sentences we want sentence embeddings for
sentences = ['This is an example sentence', 'Each sentence is converted']

# Load model from HuggingFace Hub
tokenizer = AutoTokenizer.from_pretrained('sentence-transformers/all-mpnet-base-v2')
model = AutoModel.from_pretrained('sentence-transformers/all-mpnet-base-v2')

# Tokenize sentences
encoded_input = tokenizer(sentences, padding=True, truncation=True, return_tensors='pt')

# Compute token embeddings
with torch.no_grad():
    model_output = model(**encoded_input)

# Perform pooling
sentence_embeddings = mean_pooling(model_output, encoded_input['attention_mask'])

# Normalize embeddings
sentence_embeddings = F.normalize(sentence_embeddings, p=2, dim=1)

print("Sentence embeddings:")
print(sentence_embeddings)
```

## Evaluation Results

For an automated evaluation of this model, see the *Sentence Embeddings Benchmark*: [https://seb.sbert.net](https://seb.sbert.net?model_name=sentence-transformers/all-mpnet-base-v2)

------

## Background

The project aims to train sentence embedding models on very large sentence level datasets using a self-supervised 
contrastive learning objective. We used the pretrained [`microsoft/mpnet-base`](https://huggingface.co/microsoft/mpnet-base) model and fine-tuned in on a 
1B sentence pairs dataset. We use a contrastive learning objective: given a sentence from the pair, the model should predict which out of a set of randomly sampled other sentences, was actually paired with it in our dataset.

We developped this model during the 
[Community week using JAX/Flax for NLP & CV](https://discuss.huggingface.co/t/open-to-the-community-community-week-using-jax-flax-for-nlp-cv/7104), 
organized by Hugging Face. We developped this model as part of the project:
[Train the Best Sentence Embedding Model Ever with 1B Training Pairs](https://discuss.huggingface.co/t/train-the-best-sentence-embedding-model-ever-with-1b-training-pairs/7354). We benefited from efficient hardware infrastructure to run the project: 7 TPUs v3-8, as well as intervention from Googles Flax, JAX, and Cloud team member about efficient deep learning frameworks.

## Intended uses

Our model is intented to be used as a sentence and short paragraph encoder. Given an input text, it ouptuts a vector which captures 
the semantic information. The sentence vector may be used for information retrieval, clustering or sentence similarity tasks.

By default, input text longer than 384 word pieces is truncated.


## Training procedure

### Pre-training 

We use the pretrained [`microsoft/mpnet-base`](https://huggingface.co/microsoft/mpnet-base) model. Please refer to the model card for more detailed information about the pre-training procedure.

### Fine-tuning 

We fine-tune the model using a contrastive objective. Formally, we compute the cosine similarity from each possible sentence pairs from the batch.
We then apply the cross entropy loss by comparing with true pairs.

#### Hyper parameters

We trained ou model on a TPU v3-8. We train the model during 100k steps using a batch size of 1024 (128 per TPU core).
We use a learning rate warm up of 500. The sequence length was limited to 128 tokens. We used the AdamW optimizer with
a 2e-5 learning rate. The full training script is accessible in this current repository: `train_script.py`.

#### Training data

We use the concatenation from multiple datasets to fine-tune our model. The total number of sentence pairs is above 1 billion sentences.
We sampled each dataset given a weighted probability which configuration is detailed in the `data_config.json` file.


| Dataset                                                  | Paper                                    | Number of training tuples  |
|--------------------------------------------------------|:----------------------------------------:|:--------------------------:|
| [Reddit comments (2015-2018)](https://github.com/PolyAI-LDN/conversational-datasets/tree/master/reddit) | [paper](https://arxiv.org/abs/1904.06472) | 726,484,430 |
| [S2ORC](https://github.com/allenai/s2orc) Citation pairs (Abstracts) | [paper](https://aclanthology.org/2020.acl-main.447/) | 116,288,806 |
| [WikiAnswers](https://github.com/afader/oqa#wikianswers-corpus) Duplicate question pairs | [paper](https://doi.org/10.1145/2623330.2623677) | 77,427,422 |
| [PAQ](https://github.com/facebookresearch/PAQ) (Question, Answer) pairs | [paper](https://arxiv.org/abs/2102.07033) | 64,371,441 |
| [S2ORC](https://github.com/allenai/s2orc) Citation pairs (Titles) | [paper](https://aclanthology.org/2020.acl-main.447/) | 52,603,982 |
| [S2ORC](https://github.com/allenai/s2orc) (Title, Abstract) | [paper](https://aclanthology.org/2020.acl-main.447/) | 41,769,185 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title, Body) pairs  | - | 25,316,456 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title+Body, Answer) pairs  | - | 21,396,559 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) (Title, Answer) pairs  | - | 21,396,559 |
| [MS MARCO](https://microsoft.github.io/msmarco/) triplets | [paper](https://doi.org/10.1145/3404835.3462804) | 9,144,553 |
| [GOOAQ: Open Question Answering with Diverse Answer Types](https://github.com/allenai/gooaq) | [paper](https://arxiv.org/pdf/2104.08727.pdf) | 3,012,496 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Title, Answer) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 1,198,260 |
| [Code Search](https://huggingface.co/datasets/code_search_net) | - | 1,151,414 |
| [COCO](https://cocodataset.org/#home) Image captions | [paper](https://link.springer.com/chapter/10.1007%2F978-3-319-10602-1_48) | 828,395|
| [SPECTER](https://github.com/allenai/specter) citation triplets | [paper](https://doi.org/10.18653/v1/2020.acl-main.207) | 684,100 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Question, Answer) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 681,164 |
| [Yahoo Answers](https://www.kaggle.com/soumikrakshit/yahoo-answers-dataset) (Title, Question) | [paper](https://proceedings.neurips.cc/paper/2015/hash/250cf8b51c773f3f8dc8b4be867a9a02-Abstract.html) | 659,896 |
| [SearchQA](https://huggingface.co/datasets/search_qa) | [paper](https://arxiv.org/abs/1704.05179) | 582,261 |
| [Eli5](https://huggingface.co/datasets/eli5) | [paper](https://doi.org/10.18653/v1/p19-1346) | 325,475 |
| [Flickr 30k](https://shannon.cs.illinois.edu/DenotationGraph/) | [paper](https://transacl.org/ojs/index.php/tacl/article/view/229/33) | 317,695 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (titles) | | 304,525 |
| AllNLI ([SNLI](https://nlp.stanford.edu/projects/snli/) and [MultiNLI](https://cims.nyu.edu/~sbowman/multinli/) | [paper SNLI](https://doi.org/10.18653/v1/d15-1075), [paper MultiNLI](https://doi.org/10.18653/v1/n18-1101) | 277,230 | 
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (bodies) | | 250,519 |
| [Stack Exchange](https://huggingface.co/datasets/flax-sentence-embeddings/stackexchange_xml) Duplicate questions (titles+bodies) | | 250,460 |
| [Sentence Compression](https://github.com/google-research-datasets/sentence-compression) | [paper](https://www.aclweb.org/anthology/D13-1155/) | 180,000 |
| [Wikihow](https://github.com/pvl/wikihow_pairs_dataset) | [paper](https://arxiv.org/abs/1810.09305) | 128,542 |
| [Altlex](https://github.com/chridey/altlex/) | [paper](https://aclanthology.org/P16-1135.pdf) | 112,696 |
| [Quora Question Triplets](https://quoradata.quora.com/First-Quora-Dataset-Release-Question-Pairs) | - | 103,663 |
| [Simple Wikipedia](https://cs.pomona.edu/~dkauchak/simplification/) | [paper](https://www.aclweb.org/anthology/P11-2117/) | 102,225 |
| [Natural Questions (NQ)](https://ai.google.com/research/NaturalQuestions) | [paper](https://transacl.org/ojs/index.php/tacl/article/view/1455) | 100,231 |
| [SQuAD2.0](https://rajpurkar.github.io/SQuAD-explorer/) | [paper](https://aclanthology.org/P18-2124.pdf) | 87,599 |
| [TriviaQA](https://huggingface.co/datasets/trivia_qa) | - | 73,346 |
| **Total** | | **1,170,060,424** |