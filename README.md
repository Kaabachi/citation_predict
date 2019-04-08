# citation_predict
Predicting missing links in citation network : Kaggle competition

## Problem 

Edges have been deleted at random from a citation network. Our mission is to accurately reconstruct the
initial network. We define a citation network as a graph where nodes are research papers and there is an
edge between two nodes if one of the two papers cite the other.

## Data description

### Training set :
615,512 labeled node pairs (1 if there is an edge between the two nodes, 0 else). One
pair and label per row, as: source node ID, target node ID, and 1 or 0. The IDs match the papers in
the node information file (see below).
### Testing set :
32,648 node pairs. One pair per row, as: source node ID, target node ID.
### Node information :
for each paper out of 27,770, contains the paper (1) unique ID, (2) publication
year (between 1993 and 2003), (3) title, (4) authors, (5) name of journal (not available for all papers),
and (6) abstract. Abstracts are already in lowercase, common English stopwords have been removed,
and punctuation marks have been removed except for intra-word dashes.

## Results :
0.97059 with F1 score as a metric on the private leaderboard.

A report file is also available describing the problem.

The res file needs to be zipped in the same document as project_submission.

