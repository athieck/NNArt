# NNArt
These are implementations of the paper Neural Algorithm for Artistic Style (https://arxiv.org/pdf/1508.06576v2.pdf) using the Keras framework and TensorFlow.

REQUIREMENTS
------------
• Keras is required
• Tensorflow

FILES
------------
nn_style_transfer.py:
• Basic implementation of the paper using the VGG19 network.
• To run, simply use the following command in the directory:
		python nn_style_transfer.py path_to_your_base_image.jpg path_to_your_reference.jpg prefix_for_results

nn_multiple_style_transfer.py:
• Basic implementation using the VGG19 network with a variable number of style images. Each style image is given equal weight.
• To run, simply use the following command in the directory:
	python nn_multiple_style_transfer.py --content path_to_your_base_image.jpg --style path_to_your_reference0.jpg path_to_your_reference1.jpg --dir_prefix prefix_for_results

vgg19.py:
• Modification of the Keras VGG19 model
• Gives the possibility of using a different filter size or stride size. Also allows for switch between max pooling (default) and the favored average pooling