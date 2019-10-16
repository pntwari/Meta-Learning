# Meta-Learning
A short introduction to Meta-Learning

## Introduction to Topic
Meta-learning has seen exponential growth in interest as a subfield of machine learning. It is not a concept unique to computer science; it is rooted in philosophical understanding of knowledge and its acquisition by human beings. Humans are able to ingest information, recognize the patterns within that information, and leverage it this process to new information and tasks. This in short is what one may call learning to learn. 
The idea is similar in computer science. Algorithms may be trained for a task with certain data, or perhaps for several specific tasks. These algorithms, however, do not necessarily rely on the originally created models. They perform tasks on a multi-level basis that includes data and meta-data. The latter can be performance measures, or previously learned patterns about specific data. In this sense, the algorithms applies previous learnings to design an approach toward new tasks and information – thus in a way becoming “aware” of their learning. 

## References
Wolf, Thomas, Julien Chaumond, Clément Delangue. “Meta-Learning a Dynamical Language Model”. ICLR 2018. 
Finn, Chelsea, Aravind Rajeswaran, Sham Kakade, Sergey Levine. “Online Meta-Learning”. 2019. 
Andreas, Jacob, Dan Klein, Sergey Levine. “Language Learning as Meta-Learning”. 
Gupta, Ashish. “An Introduction to Meta-Learning”. Walmart Labs: medium.com. 2019. Web
Weng, Lilian. “Meta-Learning: Learning to Learn Fast”. Git-Hub: Lil-Log. 2018. Web
Wolf, Thomas. “From zero to research – An introduction to Meta-Learning”. medium.com. 2018. Web

## Analysis
Meta-learning algorithms are named as such due to the presence of data to be worked upon and the meta-data which works upon the data. 
In these models, there are several layers. One such figure is given in Fig. (1) by Thomas Wolf. The layer shows the initial parameters, represented by a square and the parameters of the optimizer. Generally, the optimizer parameters are updated based on the gradients from the loss function until a good solution exists. 
 
Figure 1. Representation of a single step of neural training 
Meta-learning takes this model to another level, which trains the optimizer to pick the best parameters that give the best lower-model parameters. These optimizer parameters are the high-level model or the meta-learner and contains the meta-data. The lower-level model contains the data. These models begin to optimize themselves, hence learning to learn. The first trained task builds the background that a model may use for further tasks. There are other subtypes of meta-learning models such as recurrent neural networks.
Such models are believed to have high potential in Natural Language Processing (NLP). Where as conventional machine learning might be able to recognize sentences and their meanings, meta-learning is seen to be more efficient in cases of predicting, say, the end of a complex sentence, given the beginning. An ICLR (International Conference on Learning Representations) paper shows some of the progress achieved with the prediction of the end of a sentence given the beginning by a previously trained model (Wolf, Chaumond & Delangue). Indeed, Google Translate® has evolved to be a tool that can perform at a high level for a pair of languages on which it was not trained in an explicit manner. In the past, it was a tool that translated between a language to English then to a third language. It has advanced to directly translate between two languages.  Further uses are in automatic assistants such as chat bots that one may encounter on online platforms. 
These sorts of models may be preferable to traditional unsupervised models because they may require less data to train. Instead of training a model for each task, one may only train it for one task, and the model relies on its own learning process to train itself for further downstream tasks. Hence, there is less required amount of data.
In the example of Google Translate, the advantage is clear. Google Translate can scale its operations to languages at a speed its competitors with traditional machine learning methods may not afford. This is an advantage whose impact is incalculable. 
These models have also shown to be more accurate on predictions such as is described by Finn, Rajeswaran, Kakade, Levine in their article “Online Meta-Learning”, in which the discussed approach works best in a changing environment such as the one in which we currently live.  
It should be noted however, that these models are very complex and therefore computationally expensive. This continues to be a major challenge for the advancement of meta-learning. 
A flagrant disadvantage of some meta-learning algorithms with natural language processing is the difficulty with context. Languages are different, and they provide information in various ways. Some languages force the speaker to give all the information, while others let the audience fill in the information. This proves tricky for meta-learning models to explore all the possibilities that it has not encountered before, that would otherwise be snappy for a human. 

## Recommendations
As a growing field, meta-learning is not quite as developed as other methods of unsupervised learning. This is an aspect of meta-learning that is important to consider prior to starting a model. 
There are also proposed approaches that have at their core the aim of saving the GPU’s and CPU’s memory. Performance is not necessarily a question of how the model does in prediction, but also how it saves the hardware’s performance. Heavy consideration of the specific model is necessary if hardware performance is an important factor.
While meta-learning is computationally expensive, there is specific hardware that can be utilized for such models. Instead of conventional CPUs (Central Processing Unit), there are options for higher performance units. An example of this is Google’s Tensor Processing Unit (TPU), which powers the neural networks that are behind the Google Translate and such. 
Like many unsupervised models, meta-learning runs into the challenge of needing an expert on data for training. 

## Conclusion
In the age of machine learning, many types of models are being developed to get ahead in the competition of the most accurate predictor.  Their potential is being hailed in all corners of the technology community. Google, a beacon of the technology world, has transitioned some of its services to meta-learning. Its lower requirement of data is very attractive given that data is quickly becoming a valuable commodity. Its speed and scalability are also a game-changers. 
However, it has serious drawbacks that deserve careful consideration for those hoping it can be of aid in their endeavours. They are notoriously complex and are still being studied closely. In addition, as far as anyone can tell, a negotiation of performance with cost is required. Many of these models are expensive, in terms of hardware and time. 
Notwithstanding, computational power is increasing by the year. Soon meta-learning’s potential may be an inescapable reality. 
