# Neural-Network-Model-Interpretability-Techniques
Different techniques for interpreting the Decisions of Convolution Neural Network using Tensorflow and Keras
Codes for the Class Activation Map, Gradient weighted Class Activation Map and pixel-space saliency maps.

The Class Activation Map Technique
![image](https://user-images.githubusercontent.com/86059500/123368764-032ea300-d59a-11eb-850c-5341ee5e67df.png)

The CAM framework is published in the research paper: http://arxiv.org/pdf/1512.04150.pdf 

The Pixel-space Saliency Map Technique

The saliency map for an input image is generated corresponding to the output label of interest. The procedure followed is from the paper "Deep Inside Convolutional Networks".
The saliency map generation is inspired by the basics of back propagation algorithm, which states that the deltas obtained at a layer L equal the gradient of the loss incurred by the subgraph (subnet) below L with respect to the outputs at L. Thus, backpropagating till the input data layer will yield us the gradient of the loss incurred by the whole CNN with respect to the input itself, thereby providing us the importance / saliency over the input image.
