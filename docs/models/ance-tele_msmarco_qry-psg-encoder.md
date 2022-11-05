# ANCE-Tele (MS MARCO)

This model is ANCE-Tele trained on MS MARCO, described in the EMNLP 2022 paper ["Reduce Catastrophic Forgetting of Dense Retrieval Training with Teleportation Negatives"](https://arxiv.org/pdf/2210.17167.pdf). The associated GitHub repository is available at https://github.com/OpenMatch/ANCE-Tele.

ANCE-Tele only trains with self-mined negatives (teleportation negatives) without using additional negatives (e.g., BM25, other DR systems) and eliminates the dependency on filtering strategies and distillation modules.


|MS MARCO (Dev)|MRR@10|R@1K|
|:---|:---|:---|
|ANCE-Tele|39.1|98.4|


```
@inproceedings{sun2022ancetele,
  title={Reduce Catastrophic Forgetting of Dense Retrieval Training with Teleportation Negatives},
  author={Si Sun, Chenyan Xiong, Yue Yu, Arnold Overwijk, Zhiyuan Liu and Jie Bao},
  booktitle={Proceedings of EMNLP 2022},
  year={2022}
}
```