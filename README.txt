Transformer-based architecture for vision typically requires a larger dataset than usual, as well as a longer 
pre-training schedule. ImageNet-1k (which has about a million images) is considered to fall under the medium-sized
data regime with respect to ViTs. This is primarily because, unlike CNNs, ViTs (or a typical Transformer-based 
architecture) do not have well-informed inductive biases (such as convolutions for processing images). This begs
the question: can't we combine the benefits of convolution and the benefits of Transformers in a single network 
architecture? These benefits include parameter-efficiency, and self-attention to process long-range and global 
dependencies (interactions between different regions in an image).

In Escaping the Big Data Paradigm with Compact Transformers, Hassani et al. present an approach for doing exactly
this. They proposed the Compact Convolutional Transformer (CCT) architecture. In this example, we will work on 
an implementation of CCT and we will see how well it performs on the Kavasir dataset.

Kvasir dataset containing images from inside the gastrointestinal (GI) tract. The collection of images are 
classified into three important anatomical landmarks and three clinically significant findings. In addition, it
contains two categories of images related to endoscopic polyp removal. Sorting and annotation of the dataset is 
performed by medical doctors (ex- perienced endoscopists). In this respect, Kvasir is important for research on
both single- and multi-disease computer aided detec- tion. By providing it, we invite and enable multimedia 
researcher into the medical domain of detection and retrieval.