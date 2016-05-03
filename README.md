![deepid@460](http://imgur.com/1AQ1zjz.png)

DeepID-implementation
=========

DeepID-implementation is an implementation of paper "[Deep Learning Face Representation from Predicting 10,000 Classes](http://mmlab.ie.cuhk.edu.hk/pdf/YiSun_CVPR14.pdf)", which proposes to learn a set of compact, 160-dims high level feature representations through deep learning, referred to as Deep hidden IDentity features (DeepID), for face verification.

Dataset
-----------------------

|Dataset|People|Image|Size|
| ----|----|----- |----- |
|CASIA-WebFace-custom|10,575|392,304|62x62|
|LFW|6,000 pairs| |62x62|

Train, Test Model
-----------------------

|Model|People|Training images|Validation images|Train|Test|
| ----|----|----- |----- |----- |----- |
|62x62_3_e2_0264|264|9,554|939|[train](http://goo.gl/ogJFHg)|[test](http://goo.gl/12sjXD)|
|62x62_3_e2_0528|528|16,076|1,544|[train](http://goo.gl/JuoXj0)|[test](http://goo.gl/3f8KlE)|
|62x62_3_e2_1057|1,057|37,977|3,686|[train](http://goo.gl/cFwXHv)|[test](http://goo.gl/ZaKB50)|
|62x62_3_e2_2115|2,115|72,126|6,978|[train](http://goo.gl/pe7zBn)|[test](http://goo.gl/J4xMbb)|
|62x62_3_e2_4230|4,230|143,939|13,977|[train](http://goo.gl/M3HtN2)|[test](http://goo.gl/E4xluL)|
|62x62_3_e2_8460|8,460|284,466|27,498|[train](http://goo.gl/0Yhq07)|[test](http://goo.gl/t4KXwg)|
|62x62_3_e1_conventional|8,460|284,466|27,498|[train](http://goo.gl/4Rh652)|[test](http://goo.gl/ZsQYGB)|

Experiments
-----------------------

- The classification ability of Multi-scale ConvNets
    - [\[paper\]](http://goo.gl/4Pvw8S#D.5.1.1-The-classification-ability-of-Multi-scale-ConvNets) | [\[model_62x62_3\]](http://goo.gl/r66owt)
- The effectiveness of the learned hidden representations for face verification
    - [\[paper\]](http://goo.gl/4Pvw8S#D.5.1.2-The-effectiveness-of-the-learned-hidden-representations-for-face-verification) | [\[model_62x62_3\]](http://goo.gl/b4D0lG)
- The learned features extract identity information
    - [\[paper\]](http://goo.gl/4Pvw8S#D.5.1.3-The-learned-features-extract-identity-information) | [\[model_62x62_3\]](http://goo.gl/FxQy9a)
- Various face patches combination contributes to the performance
    - [\[paper\]](http://goo.gl/4Pvw8S#D.5.1.4--Various-face-patches-combination-contributes-to-the-performance)
- Method comparison
    - [\[paper\]](http://goo.gl/4Pvw8S#D.5.1.5-Method-comparison) | [\[model_62x62_3\]](http://goo.gl/9MX9Tl)

Test accuracy on LFW
-----------------------

with Joint Bayesian, Cosine Similarity, Euclidean Distance method.

|Model|Joint Bayesian|Cosine Similarity|Euclidean Distance|
| ----|----|----- |----- |
|62x62_3_e2_0264|0.61|0.735|0.6745|
|62x62_3_e2_0528|0.60|0.749333|0.701|
|62x62_3_e2_1057|0.61|0.758333|0.709167|
|62x62_3_e2_2115|0.65|0.778167|0.7365|
|62x62_3_e2_4230|0.66|0.793167|0.756833|
|62x62_3_e2_8460|0.66|0.7985|0.757|
|62x62_3_e1_conventional|0.64|0.797667|0.763167|
