# Improving-Pitch-Inflection-Graphs-Using-K-means-Clustering
### Inspiration/Background: Recently watched Tread Athletic’s video on how to interpret pitch inflection points (link) which outlines how can we find ideal or optimal zones for how effective a pitch is … I also happened to be learning about k-means clustering in my data science classes, and I got to thinking … maybe I could use clustering to create more specific pitch inflection point graphs. 
More background: I’ve started to hear a lot about supination/pronation-biased pitchers, maybe I can show how both can succeed in different ways

###  End goal: Remember end goal is to come up with more specific inflection graphs that tell you the sweet spot for each pitch in each cluster to get most effective pitch. In layman's terms, what are the different ways that a pitch can succeed? Overarching goal is to find "archetypes of pitchers" and how to optimize a player's arsenal based on the kind of pitcher they are.

###  Current plan:
- Use statcast pitch metric data and typical season-performance statistics
- Start with clustering by pitch for simplicity
  - Even though this doesn't take into account the full arsenal
- Start with clustering for 4 seam fastballs
- Start with only using 3 dimensions for simplicity and easy visualization
  - Add on more dimensions after

### Brainstorming:

3 possible ways to split up pitchers (or do a combination of them), answers the question: what kind of pitcher is someone? 
- Physical Characteristics (height/weight, vertical/horizontal release point, extension) 
- Pitch usage/pitch movements
- Performance statistics (swing and miss guy vs gb vs flyball pitcher)
- Guaranteed split: lefty vs righty

Other possibilities/ideas:
- ####  Could just cluster by pitch, although that doesn’t take into account the full arsenal
- Could include a ton of dimensions → scale down dimensions using SVD
- Most important features to defining what kind of pitcher someone is:
- VAA
- Release height
- Does VAA matter for pitches that aren’t fastballs?
- If 2D or 3D can graph easily on nice pitch plot graph
  - If just plotting horizontal and vertical, can form a nice plot graph

Important Considerations
- Need to normalize data before performing kmeans clustering
- kmeans clustering limitations:
- Need to assess how good my clustering is:
  - Inertia/elbow method
    - Sum of squared errors from points in cluster to centroids
    - measure of how tight clustering is 
    - lower inertia = tighter cluster
    - good model has low inertia and low clusters (unless super complex data)
  - Silhoutte score
    - a measure of how similar a data point is within-cluster (cohesion) compared to other clusters (separation)
- #### The curse of high dimensionality
- 
