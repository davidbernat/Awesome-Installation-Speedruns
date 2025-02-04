# Awesome-Benchmarks-DeepLearning

These are a collection of out-of-the-box easy-to-install data-plus-model deep learning benchmarks to solve a critical
and frustrating bottleneck in deep learning consumer research: research labs are not publishing their results, in terms
of processing speed and data bandwidth, nor across their variety of GPU hardware, meaning that very little comprehensive
data exists to answer the question: "what will this hardware do that this other hardware cannot?" These results would be
very easy to infer and analytically model with moderately large crowd-sourced datasets using benchmarks that are easily 
launched within one single docker container server; yet none of these results seem to be made available at scale, and 
even simple heuristics such as hyperparameter optimization for batch sizes and memory remain black arts and voodoo magics.

## Mission
The results here are informal and part of a longer term multi-year open source project, and this work is early enough
that even the results below are not optimized for performance or speed or code efficiency; just model implementation
and launched with a set of ad hoc reasonable parameters. The specific code and model implementations will be made 
available and eventually a docker contain provided in the near term of the next several months. We want to rapidly 
move away from classical task-based fulfillment tasks like categorizations and generations to process-oriented solutions,
such as research queries and software installation, ergo the [Awesome-Installation-Speedruns](https://github.com/davidbernat/Awesome-Installation-Speedruns).
We will lean heavily on the excellent [Papers With Code](https://paperswithcode.com/) and open source repository models
(e.g. deep learning projects with GitHub repositories linked to their peer-review or conference proceedings papers), 
with an eye on the obvious blaring alarm silence of the undiscussed-by-others-and-major-players: we are already beyond
the era at which open source should have provided us an algorith to point toward a peer-reviewed paper or repository 
and say "install that on my machine and I will be back in a few hours." We feel that this system should not only be
capable already of installing generic only git repositories and design pyTorch code from written paper diagrams; but 
that entire open source repositories of bug fixes and posts to git issues should be generated responsibly by these 
algorithms, i.e., identifying when installation bugs require contact with its developers or querying into its own 
peer-review library of bug fixes, which, of course, is the essence of "computer" itself, and so we are setting out to 
build this ourselves. A machine capable of installing its own compute algorithm needs is itself the solution to the
computer industry itself, and we make no hesitation of its importance and the criminality revealed in its absence by 
the so-called open source communities generations of AI algorithms before the current wave of off-line on-prem one-GPU
algorithms the size of DeepSeek and GPU technology affordable to most consumers; period, as an official position of 
Starlight Industries LLC, and part of a project started under a previously ascribed keyword years ago. The next fundamental leaps 
forward are them small-scale geometry proofs, Lagrangian mechanics formulations in self-reinforcement environments, and 
large-scale voxel networked distributed compute sensors. We remain vendor agnostic.


### MNIST 
MNIST is the classic handwritten digits classification test for the U.S. Postal Service from 1989, and in many
ways the birth of the invention of deep learning for applications in modern digital processes. We include this
benchmark for its historical relevance and ease of use on modern processors to highlight the complexity of deep
learning models today and the raw speed differences of linear algebra and data ingestion optimizations which
remain the fundamental bottlenecks of speed even when not utilizing the maximum in-GPU GB limitations for 
extremely large models. This solution uses the original LeNet-5 with 60K parameters (about 250KB), nearly one million times
smaller than current large models allowing us to do very large batch sizes with ease. 

[Papers With Code](https://paperswithcode.com/sota/image-classification-on-mnist)

| Dataset   | GPU           | CPU                   | RAM  | Epoch / Batch | Total s | Load s | Calc s | Acc  |
|-----------|---------------|-----------------------|------|---------------|---------|-------|--------|------|
| MNIST     |               | M1 2020 x8            | 8GB  | 40 / 512      | 227.3   | 0.0   | 164.4  | .987 |
| MNIST     | Metal         | M1 2020 x8            | 8GB  | 40 / 512      | 106.0   | 20.0  | 21.6   | .989 |
| MNIST     |               | AMD Ryzen5 3.6GHz x12 | 32GB | 40 / 512      | 138.7   | 0.1   | 131.4  | .988 |
| MNIST     | RTX 3050 8GB  | AMD Ryzen5 3.6GHz x12 | 32GB | 40 / 512      | 36.4    | 3.7   | 10.9   | .989 |


## Notes

We want to add ImageNet 2012, Caltech 101, CoCo, one of early NER models, and several others while we move on to modern
large scale models and applications of deep learning elsewhere, and classical game engines such as Agent 57 and long range
outlook predication such as Alpha Go. We also intend to include rudimentary video driven benchmarks for GPU enablement of packages such as FFMPEG. 




## Hire us to build.
Starlight LLC <br />
Copyright 2025 <br />
Not licensed for commercial use <br />



