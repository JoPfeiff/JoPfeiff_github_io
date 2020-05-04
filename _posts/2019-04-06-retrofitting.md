---
layout: post
title: Retrofitting
---

Last month I picked up Ivan to give a talk at our Lab about postspecialization of embedding spaces. During the one hour car ride, we quickly came to the point where I questioned the relevance of retrofitting, postspecialization or non-contextualized embeddings in general as BERT and co have been disrupting the NLP domain, and many research directions have been shattered. This was a provoking question from my side, and largely because I was personally worrying about this, given that parts of my own research have been in this direction. Ivan mentioned that these large pre-trained LMs have been shown to work well for a set of tasks, but that they don't solve everything. 

His talk later that day was on using postspecialized embedding spaces for dialogue state tracking, or in other words chat-bots (but we need to give it a researchy name). The big problems which current models have is that they are not able to distinguish the relations between entities. For example if you were to ask a chatbot to recommend a cheap asian restaurant in the west part of the city, using normal embedding representaions we might get a recommendation for an expensive french restaurant in the north, as the respective word representations are very similar. Inducing (retrofitting) external domain specific knowledge (e.g. north != west, french != asian, cheap != expensive) would thus help the model understand that this restaurant is not relevant for the users asks. 

Even though contextualized embeddings like BERT and Elmo, represent words much better than static representations like Word2Vec, Glove, or FastText, they still lack worldly knowledge in many cases. Current research is thus directed at inducing external knowledge into contextualized word representations, which makes "old" retrofitting aproaches still highly relevant. 

