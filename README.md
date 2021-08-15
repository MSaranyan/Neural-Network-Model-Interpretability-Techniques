# Neural-Network-Model-Interpretability-Techniques
Different techniques for interpreting the Decisions of Convolution Neural Network using Tensorflow and Keras
Codes for the Class Activation Map, Gradient weighted Class Activation Map, pixel-space saliency maps and Layer CAM.

Layer CAM

Layer CAM is the technique of visualizing the gradient weighted feature maps of the shallow layers of the Convolutional neural networks to identify the regions of the input used for the target predictions. It is the generalized version of the Gradient CAM which applied to the final convolution layer only.

![1](https://user-images.githubusercontent.com/86059500/129474306-966905ea-6333-4e7d-9ae8-69178e234ada.png)
![2](https://user-images.githubusercontent.com/86059500/129474309-1ffd1bc0-2b79-484e-89c7-4327da8a8551.png)

The Layer CAM technique is published in the research paper: https://arxiv.org/pdf/1901.07683

The Class Activation Map Technique
![image](https://user-images.githubusercontent.com/86059500/123368764-032ea300-d59a-11eb-850c-5341ee5e67df.png)

The CAM framework is published in the research paper: http://arxiv.org/pdf/1512.04150.pdf 

The Pixel-space Saliency Map Technique


![Screenshot from 2021-06-25 09-52-34](https://user-images.githubusercontent.com/86059500/123369378-48070980-d59b-11eb-89fb-08878b41aac9.png)
![Screenshot from 2021-06-25 09-52-49](https://user-images.githubusercontent.com/86059500/123369386-4b01fa00-d59b-11eb-9ad8-231aebfddd3f.png)



The saliency map for an input image is generated corresponding to the output label of interest. The procedure followed is from the paper "Deep Inside Convolutional Networks".
The saliency map generation is inspired by the basics of back propagation algorithm, which states that the deltas obtained at a layer L equal the gradient of the loss incurred by the subgraph (subnet) below L with respect to the outputs at L. Thus, backpropagating till the input data layer will yield us the gradient of the loss incurred by the whole CNN with respect to the input itself, thereby providing us the importance / saliency over the input image.
