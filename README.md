# Dock-less Bike Sharing with Network

## Dock-less Bike Sharing

## Data


Singapore (https://github.com/dkondor/bikesharing_data)
Shanghai (http://shanghai.sodachallenges.com/data.html?lang=en)
Beijing (https://biendata.com/competition/mobike/data/)
Los Angeles, San Francisco (https://datadryad.org/stash/dataset/doi:10.25338/B8X064)


## Method

### DBSCAN

Even Daqing Li group completed their researches successfully, there are big suspicious component that they build the network by grid, plus they insist that its network must be power-law -scale-free- neglecting the grid has only 100 or more, and it's difference between highest value and lowest was 100. 

I caught such a problems is from they formed network in grid way. The challenge is to find out natural dock- or station- of bike to solve every engaged problems otherwise grid-network ruined its property.

So, I tried to build **real** (nearly) network by adopting DBSCAN. And, also some inceptions about these problems

### Power-law fitting

[Power-law distributions in empirical data](https://arxiv.org/abs/0706.1062)(Clauset et al., 2007) 

### Clustering Validation

>Evaluation (or "validation") of clustering results is as difficult as the clustering itself. Popular approaches involve "_internal_" evaluation, where the clustering is summarized to a single quality score, "_external_" evaluation, where the clustering is compared to an existing "ground truth" classification, "_manual_" evaluation by a human expert, and "_indirect_" evaluation by evaluating the utility of the clustering in its intended application. (Wikipedia)


Based on Performance evaluation of some clustering algorithms and validity indices[(U. Maulik et al., 2002)](https://ieeexplore.ieee.org/document/1114856?reload=true), built a code and apply it to various hyper-parameters. 

<img width="640" alt="image" src="https://user-images.githubusercontent.com/45617987/184480210-767e3c60-c20f-45b6-acdd-a0ba0dc30d53.png">


> [CH](https://www.researchgate.net/publication/233096619_A_Dendrite_Method_for_Cluster_Analysis)
> [XB](https://ieeexplore.ieee.org/document/85677)
> [I-index](https://ieeexplore.ieee.org/document/1114856?reload=true)
> [Dunn's indices](https://www.tandfonline.com/doi/abs/10.1080/01969727408546059)



### Scale

By [Emergence of scaling in dockless bike-sharing systems](https://arxiv.org/abs/2202.06352)(Ruiqi Li et al., 2022) , I could get a insight about scaling of human mobility in city. 

![image](https://user-images.githubusercontent.com/45617987/184480287-134129ae-d2ed-47e1-8ff8-d36e3e342344.png)
