# GAN Fingerprints
**Unofficial PyTorch** implementation of Paper titled "Attributing Fake Images to GANs: Learning and Analyzing GAN Fingerprints. ICCV 2019". <br>


The respository is mainly referenced from two repos: 
[PGAN](https://github.com/akanimax/pro_gan_pytorch/tree/master) and  [TF implementation](https://github.com/ningyu1991/GANFingerprints).<br>  
 
**How to run**

1. Clone this repo and install:

```
pip install -e .
```

```
pip install -r requirements-dev.txt
```

2. Training:

```
CUDA_VISIBLE_DEVICES="0" python pro_gan_pytorch_scripts/train.py <data> <output_folder> --depth 7 --latent_size 4 --num_feedback_samples 20
```

where `data` folder is organized in following way:
```
data
|---ProGAN
|		|--- 000001.png
|		|--- 000002.png
|		|--- ...
|---SNGAN
|		|--- ...
|---real
|		|--- ...
```


**TODO**: Implement the test code. It is straightforward, just load the pre-trained model and forward your test images through the `EncoderDecoder`
#
*Star if you find it useful.* ⭐
