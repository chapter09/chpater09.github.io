---
layout: page
title: Distributed DRL with Serverless Computing
category: serverless
description:
img: /assets/img/serverless-RL.png
importance: 2
---



<div class="row">
    <div class="col-sm col-md-8 mt-3 mt-md-0 mx-auto d-block">
        <img class="img-fluid" src="{{ '/assets/img/minionsRL.png' | relative_url }}" alt="" />
    </div>
</div>
<div class="caption">
    Distributed DRL with Serverless Computing
</div>
<br />


<div class="title"><strong>Cheaper and Faster: Distributed Deep Reinforcement Learning with Serverless Computing</strong></div>
<div class="author">
    Hanfei Yu, Jian Li, Yang Hua, Xu Yuan, and Hao Wang
</div>
<!-- <div class="periodical"> -->
------Accepted by the AAAI 2024
<!-- [[PDF]](/assets/pdf/gang-clp-aaai.pdf), [[Code]](https://github.com/GYan58/AAAI-2022-CLP) -->
<!-- </div> -->

<br />


#### Abstract

Deep reinforcement learning (DRL) has gained immense success in many applications, including gaming AI, robotics, and system scheduling. Distributed algorithms and architectures have been vastly proposed (e.g., actor-learner architecture) to accelerate DRL training with large-scale server-based clusters. However, training on-policy algorithms with the actor-learner architecture unavoidably induces resource wasting due to synchronization between learners and actors, thus resulting in significantly extra billing. As a promising alternative, serverless computing naturally fits on-policy synchronization and alleviates resource wasting in distributed DRL training with pay-as-you-go pricing. Yet, none has leveraged serverless computing to facilitate DRL training. This paper proposes MinionsRL, the first serverless distributed DRL training framework that aims to accelerate DRL training- and cost-efficiency with dynamic actor scaling. We prototype MinionsRL on top of Microsoft Azure Container Instances and evaluate it with popular DRL tasks from OpenAI Gym. Extensive experiments show that MinionsRL reduces total training time by up to 52% and training cost by 86% compared to latest solutions.

