---
layout: default
---

# Network
In this section we will go over the created networks and in depth analysis of the GitHub contributor network and based on the analysis draw conclusions.

Based on the data collected of the GitHub contributations (To read about data collection details click here: [Data](data.md)) a graph was constructed. To ensure a very informative network we ensured that all ensured that an edge only was created people had collaborated on multiple repositories. This ensures that the relationship between the persons is stronger and provides a less noisy understanding of the graph. Each person in the graph was given their company they worked for as attribute if it was listed. 

## Basic Network Analysis 
The constructed network now consists of 22318 GitHub users and 122304 collaboration links between the users with an average degree of almost 11. The network is not fully connected so there are small islands of users who has no connection to the largest component. The user with the most different collaborations is dependabot with 2344 unique contributor connections, which is extremely high as the second largest is TensorFlow at 500. 

The dependabot is a bot provided by GitHub to help GitHub repositories with varias things such as, **dependency dpdates**, **Security Vulnerabilities** and **Testing**. This simple analysis helped us indecate how very popular this tool is for many of the top repositories, however as this network analysis want to investigate the real git contributor landscape for the best rated repositories and potetial commication pipelines.

When removing the dependabot we get a network containing 22317 users, 119960 collaborations. The network is not very dense, and the network now consists of 370 components which is almost doubled. This means that only the dependabot connected multiple nodes indirectly, furthermore we also have 193 isolated nodes which means that these users most likely only have been contributing to two repositories where the only consisting of user was dependabot therefore not having a direct connection to other real users. However, the largest component of the network is still almost consisting of 96% of the nodes, this giant component suggests a interconnective network meaning a broad collaboration diversity. Even though the average degree is almost 11 in the network but approximately 90% of the users only have 1 edge, illustrating the degree distribution being a heavy tail distribution. This means as the [Figure 1](#fig1) shows that we have some hubs potentially organization accounts or extremely active developers.

To emphasize the how the dependabot is influencing the network structure and the size of the hub, we present a figure containing both the network structure with and without the dependabot. To further illustrate how the dependabot corrupt the network, the size of nodes are directly related to the degree of the node. 

<figure id="fig1">
  <figcaption style="font-size: 2em;"><strong>GitHub Contributors Networks</strong></figcaption>
  <img src="assets/images/graph_size.png" alt="NS1">
  <figcaption><em>Network Graph - Node size corresponding to node degree</em></figcaption>
  <img src="assets/images/graph_no_bot_size.png" alt="NS2">
  <figcaption><em>Network Graph without the bot - Node size corresponding to node degree</em></figcaption>
  <figcaption><strong>Fig1. - This is the network plotted with and without dependabot.</strong></figcaption>
<br>  
</figure>

[Figure 1](#fig1) highlights that this bot node is clearly an outlier. This makes sense because it's a GitHub-provided bot designed to help repositories with tasks like monitoring for security vulnerabilities, which is especially beneficial for large companies that own many of these great repositories. Furthermore we see the hubs created to the different clusters in the graph.

## Advanced Graph Analysis
To investigate how these very active developers or organizational accounts are connected two assortativity analysis where conducted. The degree assortativity is -0.05 as it is close to 0 it alludes to the network being close to randomly connected between big and small nodes. The attribute assortativity coefficient when performed for company is also 0.01 which alludes to random connections accross companies, however almost half of the users had not specified an organization which of cause pushes the assortativity towards 0. 

Cluster coefficient 0.2 which is a low coefficient which alludes to a hierarchical structure, this is typical in professional networks as we have organizational hubs with a lot of connected employees. 



