
# BirdGAN
Progressive implementations of GANs applied to the CUB200 dataset to generate unique images.

### Prerequisites

- The [CUB200](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html) dataset.
- A python notebook environment
- Python 3.7 
	- TensorFlow 2.0 or greater
	- Pandas
	- OpenCV3


## Implementations
1. Plain DCGAN based off of [TF2](https://www.tensorflow.org/tutorials/generative/dcgan) code.
2. A deeper variant of the above, also using layer-wise Gaussian noise and label smoothing.
3. Each of the two above with an MSE metric in tandem with BCE in the generator.
4. A variant of #2 with Z size cut in half.

## TODO

- Implement IS and/or FID, evaluate model performance on these. Results are getting better, so model performance can't be evaluated visually for much longer.

- Log real and fake losses for discriminator individually.

- Look into balancing G and D losses more closely. (See [AC-GAN](https://arxiv.org/pdf/1610.09585.pdf) architectures in appendix).

- Train better of the two (100 vs 200 Z) with MSE added to BCE in generator.

- Keep MSE if results are promising
	
- Make the best model so far conditional on CUB200 classes.

Eventually:

- Implement WGAN-GP.

- Conditionality on captions.


