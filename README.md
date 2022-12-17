<p align="center">

  <h1 align="center">RelTR - Intro to ML Project</h1>
  
  <p align="center">
  </p>
</p>

## Overview

In this project, we summarize the paper RelTR: Relational Transformer for scene graph generation and validate a claim made by the authors.

<p align="center">
    <img src="./assets/img/reltr-arch.png" alt="RelTR architecture"> 
  <h5 align="center">
    Overall architecture of RelTR[1]
  </h5>
</p>

## Claim Validation
The authors claim RelTR[1] has lower number of parameters compared to other scene graph generation models such as FCSGG[2].
<p align="center">
    <img src="./assets/img/table1-reltr.png" alt="RelTR comparison"> 
  <h5 align="center">
    Performance and parameter comparison of RelTR with other models[]
  </h5>
</p>

FCSGG[] has multiple configurations with varying backbone architectures. Since the authors of RelTR do not specify which configuration is used and RelTR uses the ResNet50 as a backbone, we decided it would only be fair to test when both architectures use the same backbone.


### Claim Validation: results and discussion
|Model                |Parameters (M) ↓         |
|------------------|----------------------------|
|RelTR              |67.9         |
|FCSGG              |26.4           |

<i>Table comparing the number of parameters (M) for the models RelTR[1] and FCSGG[2]. ↓ lower is better</i>

We observe that RelTR has more parameters than FCSGG when both architectures use ResNet50 as their backbone.

<b>Result</b>: The claim RelTr has lesser parameters than FCSGG is False.


## References
- [1] https://github.com/yrcong/RelTR
- [2] https://github.com/liuhengyue/fcsgg
### Authors
- [Shubham Gupta](https://github.com/IamShubhamGupto)
- [Karan Sharma](https://github.com/ks47)

