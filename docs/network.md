---
layout: default
---

# Network

In this section we will go over the created networks and in depth analysis of the GitHub contributor network and based on the analysis draw conclusions.

## Network Including Bot Node

We constructed a graph using...

The graph is illustrated with the node size corresponding to the node degree. 

<figure style="display: flex; justify-content: space-around;">
  <figcaption><strong>Github Contributor Networks</strong></figcaption>
  <div>
    <img src="assets/images/graph_size.png" alt="NS1" style="width: 45%;">
    <figcaption>Network Graph 1 - Node size corresponding to node degree</figcaption>
  </div>
  <div>
    <img src="assets/images/graph_no_bot_size.png" alt="NS2" style="width: 45%;">
    <figcaption>Network Graph without the bot - Node size corresponding to node degree</figcaption>
  </div>
</figure>

This illustration highlights that this bot node is clearly an outlier. This makes sense because it's a GitHub-provided bot designed to help repositories with tasks like monitoring for security vulnerabilities, which is especially beneficial for large companies that own many of these great repositories.
