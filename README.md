## About t-SNE
- t-SNE stands for T-distributed Stochastic Neighbour Embedding.
- It is a machine learning algorithm for dimensioanlity reduction and used for visualization.
- The very first research paper for t-SNE was published in  2008 by Laurens van der Maaten and Geoffrey Hinton
- t-SNE is very good for visualization in 2-d.
- t-SNE is neighbuorhood preserving embedding.

## Some other dimensionality reduction technques are:
- Principal Component Analysis (PCA)
- Multi-Dimensional Scaling (MDS)
- Sammon Mapping
- Graph based techniques

I also have a repository on PCA. Check it out [here](https://github.com/deveshSingh06/Principal-Component-Analysis-PCA-on-MNIST-dataset).

## Difference between PCA and t-SNE:
- One of the prime differences between PCA and t-SNE is that PCA preserves only the global structure of the data while t-SNE preserves the local structure of the data and can choose to preserve the global structure as well.
- PCA only cares about the direction that maximizes variance and not distances between points. On the other hand, t-SNE preserves the local structure by keeping the distances between points intact(though scale/range might change).

## Main terms in t-SNE:
- Neighbourhood: The neighbourhood of a given point are the points that fall under a given distance from that point.
- Embedding: Embedding is converting a point, in d-dimensions, to a point in 2-d(or according to the need) for visualization purpose.

## Geometric interpretation of t-SNE:
- In t-SNE, the distances between a given point, in d-dimensions, and the points in its neighbourhood are preserved.
- When a given point is embedded to a point in low-dimensions(say 2-d), the actual distances between the given point and the points in its neighbourhood are similar(might be same or slightly different) to the distances that were in d-dimensions(d >>> 2).
- Also, there is NO GAURANTEE that the distances between the given point and the points NOT in its neighbourhood are preserved/similar.

## Limitations of t-SNE
- Sometimes it is impossible to preserve the distances in all the  neighbourhood(especially in the case of hypercubes). This problem is called the *crowding problem*. 
- There is NO GAURANTEE that the distances between the given point and the points NOT in its neighbourhood are preserved/similar.
- Since t-SNE is not a deterministic alogrithm but a *stochastic/probabilistic algorithm*, the results could be slightly different everytime it is applied.
