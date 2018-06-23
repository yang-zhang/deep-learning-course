# Lesson 2
- differential/discriminative learning rates: https://youtu.be/JNxcznsrRb8?t=2636
- Test Time Augmentation (TTA): https://youtu.be/JNxcznsrRb8?t=3669

# Lesson 3
- bn_freeze = True: In case you are using a deeper network anything greater than resnet34 (like resnext50), bn_freeze = True should be used when you unfreeze and your new dataset is very similar to the original data used in pretrained model (source26) Pytorch is probably the only library which offers this much needed switch. (http://forums.fast.ai/t/30-best-practices/12344)
  - https://youtu.be/9C06ZPF8Uuc?t=1109
- differential/discriminative learning rates: https://youtu.be/9C06ZPF8Uuc?t=5855  
- how to determine embedding size of categorical variables: 
  - http://localhost:8887/notebooks/git/fastai/courses/dl1/lesson3-rossman.ipynb 
  - We use the *cardinality* of each variable (that is, its number of unique values) to decide how large to make its *embeddings*. 
- `md.get_learner`: http://localhost:8887/notebooks/git/fastai/courses/dl1/lesson3-rossman.ipynb

# Lesson 4
- http://localhost:8887/notebooks/git/fastai/courses/dl1/lesson4-imdb.ipynb
- `review = !cat {TRN}{trn_files[6]}`: 
- check how many words are in the dataset: `!find {TRN} -name '*.txt' | xargs cat | wc -w`
- spacy example
- `torchtext.data.Field`
- `partial`

# Lesson 5
- http://localhost:8887/notebooks/git/fastai/courses/dl1/lesson5-movielens.ipynb
- custom module example: `EmbeddingDot`
- Momentum: https://youtu.be/J99NV9Cr75I?t=1h53m45s

# Lesson 6
- http://localhost:8887/notebooks/git/fastai/courses/dl1/lesson6-rnn.ipynb
- `.cuda()` example
- different names of anchor boxes: https://youtu.be/0frKXR-2PBY?t=3306


# Lesson 7
## CAM
- http://localhost:8887/notebooks/git/fastai/courses/dl1/lesson7-CAM.ipynb
- `nn.Sequential(*children(m)[:-2], ...` example
- hook example
-`accuracy(*learn.TTA())`
- `bn_freeze` example
## CIFAR10
- Concat adp max and avg pooling: https://youtu.be/H3g26EVADgY?t=7611


# Lesson 8
## Single Object Detection
- `get_lrg` and the 4 coordinates: https://youtu.be/Z0ssNAbe81M?t=5185
- `crop_type=CropType.NO`: https://youtu.be/Z0ssNAbe81M?t=5465
- iterating data loader: https://youtu.be/Z0ssNAbe81M?t=5641
- show image data from data loader: https://youtu.be/Z0ssNAbe81M?t=5739
- `tfm` code and `denorm`: https://youtu.be/Z0ssNAbe81M?t=5819
- debug and `pdb`: https://youtu.be/Z0ssNAbe81M?t=6125
- `custom_head`: https://youtu.be/Z0ssNAbe81M?t=7049
- pytorch `max` function: https://youtu.be/0frKXR-2PBY?t=3507

# Lesson 9
## Single Object Detection
- how to view model input and output (`eval`): https://youtu.be/0frKXR-2PBY?t=119
- `ImageClassifierData.from_csv(continuous=True)`: https://youtu.be/0frKXR-2PBY?t=224
- augmentation transformation  https://youtu.be/0frKXR-2PBY?t=311
- augmentation issue with bbox: https://youtu.be/0frKXR-2PBY?t=470
- `learn.summary()`: https://youtu.be/0frKXR-2PBY?t=593
- 2 model data objects and custom `ConcatLblDataset` class: https://youtu.be/0frKXR-2PBY?t=732
- `head_reg4`: https://youtu.be/0frKXR-2PBY?t=888
- `detn_loss`: https://youtu.be/0frKXR-2PBY?t=1017
- batch_norm before or after relu - after: https://youtu.be/0frKXR-2PBY?t=1090
- dropout after/vs batchnorm: https://youtu.be/0frKXR-2PBY?t=1179
- compare bbox loss vs classification loss in size in debugger: https://youtu.be/0frKXR-2PBY?t=1270
- how to create custom metrics: https://youtu.be/0frKXR-2PBY?t=1289

## Multiple Object Detection
- code example of recursion for method of an object: https://github.com/fastai/fastai/blob/master/fastai/dataloader.py#L63
- model input output example: https://youtu.be/0frKXR-2PBY?t=3196
- mapping ground truth: https://youtu.be/0frKXR-2PBY?t=3662
- `actn_to_bb` activation to bbox: https://youtu.be/0frKXR-2PBY?t=3862
- `BCE_Loss` binary classifcation entropy: https://youtu.be/0frKXR-2PBY?t=3962
- zero padding: https://youtu.be/0frKXR-2PBY?t=4272

# Lesson 10
- 1cycle: 
  - https://youtu.be/h5Tz7gZT9Fo?t=6550
  - https://github.com/fastai/fastai/blob/master/courses/dl2/imdb.ipynb
- keep jupyter notebook running via vnc: https://youtu.be/h5Tz7gZT9Fo?t=7123
- more anchor boxes: https://youtu.be/0frKXR-2PBY?t=4490


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
