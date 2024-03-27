## Things to improve
> Convertion of 'string' dtypes to one-hot vectors is      very inefficient.
> > For Ex: Converting a Title to one hot vector just gives a array without any information of what the title meant.
> - One other way to do this more efficiently and keep the semantic relationship between the words of title is by using word2vec.
> > This will keep all the semantic relations and will give more accurate results when trained with a CNN.
    - Learn more about tf and its algorithms.
## Things to do differently
>  Classifying each author at a time without any semantic relation between all the authors is not the way forward.
> - One way is to make a semantic map of given data. 
>> which will provide us with the crude relations between authors and then we will train our model on that. It will be easier and more efficient for a neural network to learn the patterns.
>  - Other way can be converting the given data into images and then classfying.
      - This way is also more efficient but very hard.
      - The images captures all the necessary information including title, authors, years etc.. 
      - This will make the images of more related athors more similar and will be easy to train.     
      - Problem with this implementation:
    >> - This method requires unsupervised classification of images, which is hard to really get into right now.
   >>- Paper [Unsupervised Img Classification](https://github.com/wvangansbeke/Unsupervised-Classification)
                    
## Things learned:
- usage of numpy, pandas, and other useful libraries
- Basics of tensorflow
- Understading ontologies

## Things to learn: 
- word2vec
- ontology
- tensorflow/ pytorch / sklearn


## Resources / References:
- author name disambuguation
    - [ADANA](https://www.aminer.org/disambiguation)
    - [S2AND](https://github.com/allenai/S2AND)
    - [Unsupervised Author Disambiguation using Heterogeneous Graph Convolutional Network Embedding](https://github.com/joe817/name-disambiguation)
    - [RandomForestClassifierCV](https://github.com/diging/author-disambiguation)
- [tensorflow](https://www.tensorflow.org/tutorials)
- [Unsupervised image classification](https://github.com/wvangansbeke/Unsupervised-Classification)
