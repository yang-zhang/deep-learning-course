# Lesson 2
- Test Time Augmentation (TTA): https://youtu.be/JNxcznsrRb8?t=3669
# Lesson 3
- bn_freeze = True: In case you are using a deeper network anything greater than resnet34 (like resnext50), bn_freeze = True should be used when you unfreeze and your new dataset is very similar to the original data used in pretrained model (source26) Pytorch is probably the only library which offers this much needed switch. (http://forums.fast.ai/t/30-best-practices/12344)
  - https://youtu.be/9C06ZPF8Uuc?t=1109
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
  
