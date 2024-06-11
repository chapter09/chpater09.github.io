---
layout: page
title: Critical Learning Periods
category: fl
img: /assets/img/critical-learning-periods.png
importance: 2
---



<div class="row">
    <div class="col-sm col-md-9 mt-3 mt-md-0 mx-auto d-block">
        <img class="img-fluid" src="{{ '/assets/img/critical-learning-periods-motivation.png' | relative_url }}" alt="" />
    </div>
</div>
<div class="caption">
    Critical learning periods. 
</div>
<br />


<div class="title"><strong>Seizing Critical Learning Periods in Federated Learning</strong></div>
<div class="author">
    Gang Yan, Hao Wang, and Jian Li
</div>
<!-- <div class="periodical"> -->
------Accepted by the AAAI 2022, [[PDF]](/assets/pdf/gang-clp-aaai.pdf), [[Code]](https://github.com/GYan58/AAAI-2022-CLP)
<!-- </div> -->

<br />


#### Abstract

Federated learning (FL) is a popular technique to train machine learning (ML) models with decentralized data. Extensive works have studied the performance of the global model; however, it is still unclear how the training process affects the final test accuracy. Exacerbating this problem is the fact that FL executions differ significantly from traditional ML with heterogeneous data characteristics across clients, involving more hyperparameters. In this work, we show that the final test accuracy of FL is dramatically affected by the early phase of the training process, i.e., FL exhibits critical learning periods, in which small gradient errors can have irrecoverable impact on the final test accuracy. To further explain this phenomenon, we generalize the trace of the Fisher Information Matrix (FIM) to FL and define a new notion called FedFIM, a quantity reflecting the local curvature of each clients from the beginning of the training in FL. Our findings suggest that the initial learning phase plays a critical role in understanding the FL performance. This is in contrast to many existing works which generally do not connect the final accuracy of FL to the early phase training. Finally, seizing critical learning periods in FL is of independent interest and could be useful for other problems such as the choices of hyperparameters such as the number of client selected per round, batch size, and more, so as to improve the performance of FL training and testing.


---

<div class="title"><strong>DeFL: Defending Against Model Poisoning Attacks in Federated Learning via Critical Learning Periods Awareness</strong></div>
<div class="author">
    Gang Yan, Hao Wang, Xu Yuan, and Jian Li
</div>
------Accepted by the AAAI 2023, [[PDF]](/assets/pdf/defl-yangang-aaai2023.pdf), [[Code]](https://github.com/GYan58/AAAI-2023-DeFL)


<!-- <div>
    <div class="title">Harvesting Idle Resources in Serverless Computing via Reinforcement Learning</div>
    <div class="author">
        Hanfei Yu, <em>Hao Wang</em>,Jian Li, and Seung-Jong Park
    </div>

    <div class="periodical">
        Available at <a href="https://arxiv.org/abs/2108.12717">arXiv:2108.12717</a>, 2021
    </div>
</div> -->

<br />

#### Abstract
Federated learning (FL) is known to be susceptible to model poisoning attacks in which malicious clients hamper the accuracy of the global model by sending manipulated model updates to the central server during the FL training process. Existing defenses mainly focus on Byzantine-robust FL aggregations, and largely ignore the impact of the underlying deep neural network (DNN) that is used to FL training. Inspired by recent findings on critical learning periods (CLP) in DNNs, where small gradient errors have irrecoverable impact on the final model accuracy, we propose a new defense, called a CLP-aware defense against poisoning of FL (DeFL). The key idea of DeFL is to measure fine-grained differences between DNN model updates via an easy-to-compute federated gradient norm vector (FGNV) metric. Using FGNV, DeFL simultaneously detects malicious clients and identifies CLP, which in turn is leveraged to guide the adaptive removal of detected malicious clients from aggregation. As a result, DeFL not only mitigates model poisoning attacks on the global model but also is robust to detection errors. Our extensive experiments on three benchmark datasets demonstrate that DeFL produces significant performance gain over conventional defenses against state-of-the-art model poisoning attacks.



---

<div class="title"><strong>CriticalFL: A Critical Learning Periods Augmented Client Selection Framework for Efficient Federated Learning</strong></div>
<div class="author">
    Gang Yan, Hao Wang, Xu Yuan, and Jian Li
</div>
------Accepted by the KDD 2023, [[PDF]](/assets/pdf/CriticalFL.pdf), [[Code]](https://github.com/GYan58/KDD-2023-CriticalFL)


<!-- <div>
    <div class="title">Harvesting Idle Resources in Serverless Computing via Reinforcement Learning</div>
    <div class="author">
        Hanfei Yu, <em>Hao Wang</em>,Jian Li, and Seung-Jong Park
    </div>

    <div class="periodical">
        Available at <a href="https://arxiv.org/abs/2108.12717">arXiv:2108.12717</a>, 2021
    </div>
</div> -->

<br />

#### Abstract
Federated learning (FL) is a distributed optimization paradigm that learns from data samples distributed across a number of clients. Adaptive client selection that is cognizant of the training progress of clients has become a major trend to improve FL efficiency but not yet well-understood. Most existing FL methods such as FedAvg and its state-of-the-art variants implicitly assume that all learning phases during the FL training process are equally important. Unfortunately, this assumption has been revealed to be invalid due to recent findings on critical learning periods (CLP), in which small gradient errors may lead to an irrecoverable deficiency on final test accuracy. In this paper, we develop CriticalFL, a CLP augmented FL framework to reveal that adaptively augmenting exiting FL methods with CLP, the resultant performance is significantly improved when the client selection is guided by the discovered CLP. Experiments based on various machine learning models and datasets validate that the proposed CriticalFL framework consistently achieves an improved model accuracy while maintains better communication efficiency as compared to state-of-the-art methods, demonstrating a promising and easily adopted method for tackling the heterogeneity of FL training.
