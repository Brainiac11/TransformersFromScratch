# Why did I do this

i know that transformers are extremely niche and not very known. However, the important thing with transformers is that they are one of the most powerful ways to compress litterally Quadrillions of Bytes of data, into something that is small enough to generate seamingly new data. This is why I made a simple, albiet pretty capable transformer. Mostly as a training excercise, but also to show myself that the math it takes to understand transformers is actually fairly simple, and that most of the complexity comes from ALL the other challenges around getting data, storing data, training fast, deploying to GPUs, etc. 

## What methods I used

Although there are a lot of different designs and such for LLM's, my main focus was just getting an LLM that I could understand. 

The specific methodologies and such are commented, but essentially the majority of the technical features are such:

1. This is Multi headed attention that uses pre-layer normalization
2. This uses GeLU and is also slightly modified in the compute to be faster
3. the training data is really small, so its a lot different than a normal LLM, so it trains a lot faster for less time