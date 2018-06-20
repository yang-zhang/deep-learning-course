# Lesson 2
- differential/discriminative learning rates: https://youtu.be/JNxcznsrRb8?t=2636
- Test Time Augmentation (TTA): https://youtu.be/JNxcznsrRb8?t=3669

# Lesson 3
- bn_freeze = True: In case you are using a deeper network anything greater than resnet34 (like resnext50), bn_freeze = True should be used when you unfreeze and your new dataset is very similar to the original data used in pretrained model (source26) Pytorch is probably the only library which offers this much needed switch. (http://forums.fast.ai/t/30-best-practices/12344)
  - https://youtu.be/9C06ZPF8Uuc?t=1109
- differential/discriminative learning rates: https://youtu.be/9C06ZPF8Uuc?t=5855  

# Lesson 5
- Momentum: https://youtu.be/J99NV9Cr75I?t=1h53m45s

# Lesson 7
- Concat adp max and avg pooling: https://youtu.be/H3g26EVADgY?t=7611

# Lesson 8
- `get_lrg` and the 4 coordinates: https://youtu.be/Z0ssNAbe81M?t=5185
- `crop_type=CropType.NO`: https://youtu.be/Z0ssNAbe81M?t=5465
- iterating data loader: https://youtu.be/Z0ssNAbe81M?t=5641
- show image data from data loader: https://youtu.be/Z0ssNAbe81M?t=5739
- `tfm` code and `denorm`: https://youtu.be/Z0ssNAbe81M?t=5819
- debug and `pdb`: https://youtu.be/Z0ssNAbe81M?t=6125
- `custom_head`: https://youtu.be/Z0ssNAbe81M?t=7049

# Lesson 9
- how to view model input and output (`eval`): https://youtu.be/0frKXR-2PBY?t=119


# Lesson 10
- 1cycle: 
  - https://youtu.be/h5Tz7gZT9Fo?t=6550
  - https://github.com/fastai/fastai/blob/master/courses/dl2/imdb.ipynb

# Lesson 12
## CIFAR10 Darknet 
- New arch; fast
- Notebook: https://github.com/fastai/fastai/blob/master/courses/dl2/cifar10-darknet.ipynb
- Good numpy **exercise**: calculate image data stats: https://youtu.be/ondivPiwQho?t=551
- LeakyRelu good for smaller data set, and no harm to use as default: https://youtu.be/ondivPiwQho?t=847
- One-cycle from Leslie Smith; 
  - use_clr_beta clr: https://youtu.be/ondivPiwQho?t=2707; 
  - Paper: A DISCIPLINED APPROACH TO NEURAL NETWORK HYPER-PARAMETERS: PART 1 – LEARNING RATE, BATCH SIZE, MOMENTUM, AND WEIGHT DECAY
## GAN: 
- https://youtu.be/ondivPiwQho?t=2942
- https://github.com/fastai/fastai/blob/master/courses/dl2/wgan.ipynb
- Example of tqdm bar update
- Wasserstein GAN paper: https://arxiv.org/abs/1701.07875; recommended **read**
- Deconv: 
- https://youtu.be/ondivPiwQho?t=4209; 
- Animation: https://youtu.be/ondivPiwQho?t=4607
- Upsampling v.s. deconv discussion and checkerboard: 
  - https://youtu.be/ondivPiwQho?t=4695
  - https://distill.pub/2016/deconv-checkerboard/
- Examples of usage: https://youtu.be/ondivPiwQho?t=6070
## Cycle-consistent GAN
- https://github.com/fastai/fastai/blob/master/courses/dl2/cyclegan.ipynb
- Paper: https://arxiv.org/abs/1703.10593

# Lesson 13
- Stochastic weight averaging (swa): https://youtu.be/xXXiC4YRGrQ?t=103
# Train phase API: 
- https://youtu.be/xXXiC4YRGrQ?t=161
- https://github.com/fastai/fastai/blob/master/courses/dl2/training_phase.ipynb
- Revisit: why use smaller images first and larger ones later for training and how this API supports it.
# Inception
  - https://youtu.be/xXXiC4YRGrQ?t=1047
  - Factored convoluation: instead of (7x7)conv, do (7x1) then (1x7) convs - same shape, less parameters (7+7=14 instead of 7*7=49)
  - Stem: https://youtu.be/xXXiC4YRGrQ?t=1712
# Image Enhancement
  - Progressive GAN: https://youtu.be/xXXiC4YRGrQ?t=1885
  - Artistic style: https://youtu.be/xXXiC4YRGrQ?t=3692
  
# Lesson 14
## Super resolution
- Ideas to get label from tranforming images in some way: https://youtu.be/nG3tT31nPmQ?t=366
- Upsampling: https://youtu.be/nG3tT31nPmQ?t=2110
  - Sub-pixel conv net: https://youtu.be/nG3tT31nPmQ?t=2293
- Parallel/multiple gpus: https://youtu.be/nG3tT31nPmQ?t=2924
- Hook: https://youtu.be/nG3tT31nPmQ?t=3217
- Load model load_state_dict stric=False: https://youtu.be/nG3tT31nPmQ?t=3623
- Threadpool executor: https://youtu.be/nG3tT31nPmQ?t=5690
## Image segmentation
- Lambda layer: https://youtu.be/nG3tT31nPmQ?t=5992
- U-net: https://youtu.be/nG3tT31nPmQ?t=6298
- cut_model: https://youtu.be/nG3tT31nPmQ?t=6669
- Hook: https://youtu.be/nG3tT31nPmQ?t=6700
- `m.close()`: https://youtu.be/nG3tT31nPmQ?t=6983
- U-net bounding box (Feature Pyramid Networks for Object Detection): https://youtu.be/nG3tT31nPmQ?t=7151
