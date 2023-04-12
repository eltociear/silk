# SiLK - Simple Learned Keypoints

SiLK is a framework for learning keypoints, as described in our [paper](TODO).

<p float="middle">
  <img src="doc/images/keypoints.png" width="33%"/>
  <img src="doc/images/matches.png" width="66%"/>
</p>

Pre-trained models are also provided.

The released code has been tested on Linux, with two Tesla V100-SXM2 GPUs and takes about 5 hours to train.

## Requirements
* [conda](https://www.anaconda.com/) should be installed in order to setup the silk environment.
* __Two__ GPUs are required to train SiLK.

## Usage

* [How to setup the python environment ?](doc/usage/setup.md)
* [How to setup datasets ?](doc/usage/dataset.md)
* [How to train SiLK ?](doc/usage/train.md)
* [How to add a backbone ?](doc/usage/backbone.md)
* [How to run the evaluation pipeline ?](doc/usage/evaluation.md)
* [How to run inference ?](doc/usage/inference.md)
* [How to convert SiLK to torch script ?](doc/usage/torch_script.md)

## Results

The results below have been computed using our VGG-4 backbone (checkpoint [pvgg-4.ckpt](https://dl.fbaipublicfiles.com/silk/assets/models/silk/analysis/alpha/pvgg-4.ckpt) for tab 2,3,6 and [coco-rgb-aug](https://dl.fbaipublicfiles.com/silk/assets/models/silk/coco-rgb-aug.ckpt) for tab 4,5).

<img src="doc/images/results-hpatches-sparse.png" width="100%"/>
<p float="middle">
  <img src="doc/images/results-hpatches-dense.png" width="46%"/>
  <img src="doc/images/results-imc.png" width="53%"/>

</p>
<p float="middle">
    <img src="doc/images/results-scannet-pose.png" width="36%"/>
    <img src="doc/images/results-scannet-pcloud.png" width="63%"/>
</p>

## Full Documentation

We provide a documentation, but it is non-exhaustive. Please create a new issue if clarification is required regarding some part of the code. We will add documentation if required by the community.

Our documentation can be found [here](doc/silk/index.html).

## Contributions

See the [CONTRIBUTING](CONTRIBUTING.md) file for how to help out.

## License
**SiLK** is licensed under a *Attribution-NonCommercial 4.0 International License*, as specified in the [LICENSE](LICENSE) file.