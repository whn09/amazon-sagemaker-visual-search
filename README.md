## Visual image search
This repository is part of AWS blog to create a visual search application using Amazon SageMaker and Amazon Elasticsearch

## How does it work?

We will use Fashion Images from feidegger, a zalandoresearch dataset as a reference image to generate a 2048 feature vector using a convolutional neural networks and gets stored into Amazon Elasticsearch KNN index

![diagram](../master/ref.png)

When we present a new query image, it's computing the related feature vector from Amazon SageMaker hosted model and query Amazon Elasticsearch KNN index to find similar images

![diagram](../master/query.png)

## Use Keras

Refer to [src](src) and [visual-image-search.ipynb](visual-image-search.ipynb)

## Use GluonCV

Refer to [endpoint](endpoint) and [visual-image-search-gluoncv.ipynb](visual-image-search-gluoncv.ipynb), train script is [transfer_learning.ipynb](transfer_learning.ipynb)

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
