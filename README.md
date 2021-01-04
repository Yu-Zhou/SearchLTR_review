# SearchLTR_review
Literature review for learning to rank in search engines. This repo is my notes about papers/posts in the Search Engine Learning to Rank (LTR) domain. My goal is to provide a short summary for each paper, including the following aspect:
- Problem statement
- What is novel about the solution raised in this paper?
- Performance & the most suitable use case
- Core techniques


## Papers
1. [Optimizing Search Engines using Clickthrough Data - Joachims 2002](https://www.cs.cornell.edu/people/tj/publications/joachims_02c.pdf) (:star::star::star::star::star:)
> Previous methods rely on manually labeled training data, which are expensive to get. Rather, this paper proposed a framework to extract users' preferrance from query logs, which, to put specifically, are which links the users click on (did not considered the clicking order). 
> The paper pointed out that reviewing the clickthrough data as evidence for absolute relevance is wrong (since people will rarely evaluate all documents), but we should view it as **relative** relevance in top `l` retrieved results.	
> (Core techniques) Adapted Kendall's <img src="https://render.githubusercontent.com/render/math?math=\tau">, which is originally designed for ordinal correlation of two random variables. The formula involve the number of **concordant pairs** and the number of **discordant** (inversions) pairs. Experimentation: show the learning method can really decrease the percent of pairwise preference constraints that are not fulfilled in the test set (by queries); ... present two rankings at the same time... for online. experiment.
