# Analyzing-co-authorship-network-top-authors-identification-link-prediction-community-detection

In this research project, I have to extract a network of co-authorship relations between researchers
identified to be among the top researchers in machine learning (i.e., those in the top-300 highest hindex according to Google scholar and have collaborated at least once with each other). The parts of this projects. 

## Network data creation 

The goal is to create a co-authorship network from the
given input files (DBLP XML Files) and store their relation in an output ASCII text file named coauthor.csv,
which contains 2 comma-separated columns, (authorID1, authorID2), if the two authors have
collaborated at least once in the past. The mapping from author name to author ID is given
in the file authors.txt.

## Data exploration

<ol>
<li>Compute the number of nodes (vertices) and links (edges) of the network</li>
  <li><strong>Centrality Measure:</strong></li>
  <ol>
  <li>**Degree Centrality**: Compute the degree (i.e., number of collaborators) associated
with each author.</li>
  <li>**Eigenvalue Centrality**: Find the principal eigenvector of the adjacency matrix
using power method. </li>
    <li>**Local Clustering Coefficient**: Compute the local clustering coefficient of each node in the graph. </li>
  </ol>  
</ol>

## Co-authorship network

Network visualization with co-authorship links

## Link Prediction 
The objective of link prediction in network analysis is to infer missing
links or recommend new links in a network. For this step, tasks include:
<ol>
<li>Removing some of the links in the original network to create a new, modified network.</li>
<li>Using the modified network to train a logistic regression model.</li>
<li>Applying the logistic regression model to predict the links that were removed in part 1.</li>
</ol>

## Community Detection

The objective of community detection is to partition the network
into a set of connected components (communities) such that nodes in the same community are
more similar (connected) to each other compared to those belonging to different communities.
