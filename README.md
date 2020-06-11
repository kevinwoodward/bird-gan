

# BirdGAN
Progressive implementations of GAN architectures applied to the CUB200 dataset to generate unique images conditioned on attributes and caption embeddings.

### Prerequisites

- The [CUB200](http://www.vision.caltech.edu/visipedia/CUB-200-2011.html) dataset
- [Captions](https://github.com/taoxugit/AttnGAN) for the CUB200 dataset
- Pretrained [BERT-large (uncased)](https://github.com/google-research/bert) model for embedding captions to 1024D vectors
- [bert-as-service](https://github.com/hanxiao/bert-as-service) for utilizing the pretrained BERT model
- A python notebook environment
- Python 3.7 
	- TensorFlow 2.0 or greater
	- Pandas
	- OpenCV3


## Implementation Categories (ordered old → new)
1. Vanilla DCGAN 
2. Multilabel ACGAN
3. Multilabel ACGAN with a split discriminator (for finer tuning)
4. Multilabel ACGAN with a split discriminator with BERT captions
5. Multilabel ACGAN with a split discriminator with BERT captions V2

## Sample Generations (ordered old → new)
Vanilla DCGAN:

![Vanilla DCGAN](https://github.com/kevinwoodward/bird-gan/blob/master/results/samples/bird-gan-deeper-smaller-z-balanced/samples1.png?raw=true)

Multilabel ACGAN:

![Multilabel ACGAN](https://github.com/kevinwoodward/bird-gan/blob/master/results/samples/bird-gan-attributes/samples1.png?raw=true)

Multilabel ACGAN w/split Discriminator:

![Multilabel ACGAN w/split Discriminator](https://github.com/kevinwoodward/bird-gan/blob/master/results/samples/bird-gan-attributes-split-sigmoid-simple-tuning/manifold3.png?raw=true)

Multilabel ACGAN w/split Discriminator and Captions:

![Multilabel ACGAN w/split Discriminator and Captions](https://github.com/kevinwoodward/bird-gan/blob/master/results/samples/bird-gan-attributes-split-captions-concat-caption-loss-autoencoder/samples2.png?raw=true)

Multilabel ACGAN w/split Discriminator and Captions V2

![Multilabel ACGAN w/split Discriminator and Captions V2](https://github.com/kevinwoodward/bird-gan/blob/master/results/samples/bird-gan-attributes-split-captions-concat-caption-loss-autoencoder-34-weighted/samples4.png?raw=true)


