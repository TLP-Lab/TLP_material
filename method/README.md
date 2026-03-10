# A summary of state-of-the-art methods for TLP

**时序链接预测 (TLP)** 是动态图（Temporal / Dynamic Graph）分析中的一个核心问题，研究如何 **预测图中未来可能出现的边**。  
动态图可以表示为：

- **离散时间图**: $($ $G_1$ $,$ $G_2$ $,$ $...$ $,$ $G_T$ $)$, 其中 $G_T$ 表示第 $T$ 个时间步的快照
- **连续时间图**: $($ $u$ $,$ $v$ $,$ $t$ $)$ 表示节点 $u$ 与 $v$ 在时间 $t$ 发生交互

TLP 在实际场景中广泛应用于：

- 社交网络好友推荐
- 知识图谱更新
- 交易网络预测
- 通信网络异常检测

根据不同的图建模方式，TLP的方法可以大致分为：

| 类别 | 特点 | 代表方法 |
|---|---|---|
| Snapshot-based（离散时间） | 将动态图拆成离散时间片，使用序列模型建模 | EvolveGCN[5], DynGEM[2], DySAT[6] |
| Continuous-time（连续时间） | 使用事件级时间戳建模，每条边带时间 | TGN[12], JODIE[10], TGAT[11] |

## References
### Snapshot-based TLP Modeling
1. Dynamic Network Embedding by Modelling Triadic Closure Process (AAAI'2018) [[`pdf`](https://dl.acm.org/doi/pdf/10.5555/3504035.3504106)] [[`code`](https://github.com/luckiezhou/DynamicTriad)] 

2. DynamicGEM: A Library for Dynamic Graph Embedding Methods [[`pdf`](https://arxiv.org/pdf/1811.10734)] [[`code`](https://github.com/palash1992/DynamicGEM)]

3. Structured Sequence Modeling with Graph Convolutional Recurrent Networks (ICONIP'2018) [[`pdf`](https://arxiv.org/pdf/1612.07659)] [[`code`](https://github.com/youngjoo-epfl/gconvRNN)]

4. Variational graph recurrent neural networks (NeurIPS'2019) [[`pdf`](https://arxiv.org/pdf/1908.09710)] [[`code`](https://github.com/VGraphRNN/VGRNN)]

5. Evolvegcn: Evolving graph convolutional networks for dynamic graphs (AAAI'2020) [[`pdf`](https://arxiv.org/pdf/1902.10191)] [[`code`](https://github.com/IBM/EvolveGCN)] 

6. DySAT: Deep Neural Representation Learning on Dynamic Graphs via Self‑Attention Networks (ICLR'2020) [[`pdf`](https://arxiv.org/pdf/1812.09430)] [[`code`](https://github.com/aravindsankar28/DySAT)]

7. Discrete-time Temporal Network Embedding via Implicit Hierarchical Learning in Hyperbolic Space (KDD'2021)
[[`pdf`](https://arxiv.org/pdf/2107.03767)] [[`code`](https://github.com/marlin-codes/HTGN)]

8. HGWaveNet: A Hyperbolic Graph Neural Network for Temporal Link Prediction (WWW'2023) [[`pdf`](https://arxiv.org/pdf/2304.07302)] [[`code`](https://github.com/TaiLvYuanLiang/HGWaveNet)]

### Continue-time TLP Modeling
9. Continuous-Time Dynamic Network Embeddings (WWW'2018) [[`pdf`](http://ryanrossi.com/pubs/nguyen-et-al-WWW18-BigNet.pdf)] [[`code`](https://github.com/LogicJake/CTDNE)]

10. Predicting Dynamic Embedding Trajectory in Temporal Interaction Networks (KDD'2019) [[`pdf`](https://dl.acm.org/doi/epdf/10.1145/3292500.3330895)] [[`code`](https://github.com/claws-lab/jodie)]

11. Inductive Representation Learning on Temporal Graphs (ICLR'2020) [[`pdf`](https://arxiv.org/pdf/2002.07962)] [[`code`](https://github.com/dongkwan-kim/TGAT-REF)]

12. Temporal Graph Networks for Deep Learning on Dynamic Graphs (ICML'2020) [[`pdf`](https://arxiv.org/pdf/2006.10637)] [[`code`](https://github.com/twitter-research/tgn)]

13. Do We Really Need Complicated Model Architectures For Temporal Networks (ICLR'2023) [[`pdf`](https://arxiv.org/pdf/2302.11636)] [[`code`](https://github.com/CongWeilin/GraphMixer)]

14. Zebra: When temporal graph neural networks meet temporal personalized PageRank (VLDB'2023) [[`pdf`](https://www.vldb.org/pvldb/vol16/p1332-li.pdf)] [[`code`](https://github.com/LuckyLYM/Zebra)]

15. Temporal SIR-GN: Efficient and Effective Structural Representation Learning for Temporal Graphs (VLDB'2023)
[[`pdf`](https://www.vldb.org/pvldb/vol16/p2075-layne.pdf)] [[`code`](https://github.com/janetlayne2/Temporal-SIR-GN)]

16. Towards better dynamic graph learning: New architecture and unified library (NeurIPS'2023) [[`pdf`](https://arxiv.org/pdf/2303.13047)] [[`code`](https://github.com/yule-BUAA/DyGLib)]

17. When Speed meets Accuracy: an Efficient and Effective Graph Model for Temporal Link Prediction (VLDB'2025)
[[`pdf`](https://arxiv.org/pdf/2507.13825)] [[`code`](https://github.com/TreeAI-Lab/EAGLE)]

18.  Node-Time Conditional Prompt Learning in Dynamic Graphs (ICLR'2025) [[`pdf`](https://openreview.net/pdf?id=kVlfYvIqaK)] [[`code`](https://github.com/gmcmt/DyGPrompt)] 

19. Data-centric Prompt Tuning for Dynamic Graphs (CIKM'2025) [[`pdf`](https://arxiv.org/html/2601.11954v1)] [[`code`](https://github.com/astral-requiem/DDGPrompt)] 

### Suvey Papers (其他方法可参考一下综述论文)

20. Temporal Link Prediction: A Unified Framework, Taxonomy, and Review (ACM Comput. Surv. ,2023) [[`pdf`](https://arxiv.org/pdf/2210.08765)] [[`code`](https://github.com/KuroginQin/OpenTLP)] 

21. A Survey of Link Prediction in Temporal Network (SN Computer Science, 2026) [[`pdf`](https://arxiv.org/pdf/2502.21185)]



