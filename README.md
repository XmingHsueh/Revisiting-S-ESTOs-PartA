# How to Exploit Experience? Revisiting Evolutionary Sequential Transfer Optimization: Part A

This repository provides the MATLAB implementations of producing the benchmark suite developed in the above article, which contains 12 individual sequential transfer optimization problems (STOPs). To instantiate an STOP, we need to configure the following six aspects: target task, transfer scenario, the parameter that determines optimum coverage, similarity distribution, problem dimension, and the number of source tasks. Their available configurations are as follows:

* target task (F): `Sphere`, `Ellipsoid`, `Schwefel`, `Quartic`, `Ackley`, `Rastrigin`, `Griewank`, and `Levy`
* transfer scenario (T): `Ta` and `Te`
* the parameter of controlling optimum coverage (xi): a real number from 0 to 1
* similarity distribution (S): `Sc`, `Su`, `Si` and `Sd`
* problem dimension (d): a positive integer
* the number of source tasks (k): a positive integer

In the article, we name a black-box STOP as F-T-xi-S-d-k, where F denotes the target family, T represents the transfer scenario, xi is the optimum coverage-related parameter, S represents the similarity distribution, d denotes the problem dimension, k is the number of source tasks. According to this naming rule, we specify the following 12 individual STOPs to form the benchmark suite,

|Problem ID|Problem Specification|
|:-|:-|:-|
|STOP 1|Sphere-Ta-0-Sc-50-1000|
|STOP 2|Ellipsoid-Te-0-Su-25-1000|
|STOP 3|Schwefel-Ta-0-Si-30-1000|
|STOP 4|Quartic-Te-0-Sd-50-1000|
|STOP 5|Ackley-Ta-0.7-Sc-50-1000|
|STOP 6|Rastrigin-Te-0.7-Su-30-1000|
|STOP 7|Griewank-Ta-0.7-Si-25-1000|
|STOP 8|Levy-Te-0.7-Sd-30-1000|
|STOP 9|Rastrigin-Ta-1-Sc-50-1000|
|STOP 10|Sphere-Te-1-Su-50-1000|
|STOP 11|Ackley-Ta-1-Si-25-1000|
|STOP 12|Ellipsoid-Te-1-Sd-30-1000|
