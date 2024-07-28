# USPTO Explainable AI for Patent Professionals 
## Overview

This repository contains the code used for the USPTO Explainable AI for Patent Professionals competition. The goal of the competition is to generate Boolean search queries that effectively characterize collections of patent documents. The challenge is to create a query generation model that, given an input set of related patents, outputs a Boolean query that returns the same set of patent documents.

## Methods Used in the Notebooks

### Large Language Model (LLM) - Mistral Instruct 7B
The Mistral Instruct 7B notebook utilizes a Large Language Model (LLM) fine-tuned for instruction-following tasks. LLMs are advanced AI models trained on vast amounts of text data, enabling them to understand and generate human-like text. In this context, the LLM is used to generate Boolean search queries. The model's ability to comprehend and produce complex text structures makes it well-suited for creating accurate and efficient search queries based on the input patent documents.

### Simulated Annealing
The Annealing notebook employs Simulated Annealing, an optimization technique inspired by the annealing process in metallurgy. This probabilistic method is used to find an approximate global optimum of a function. It involves:

<li> 
<ul>Generating Initial Solutions: Starting with an initial set of Boolean search queries.</ul>
<ul>Iterative Improvement: Making small changes to the queries and evaluating their performance.</ul>
<ul>Acceptance Probability: Deciding whether to accept the changes based on a probability that decreases over time, allowing for exploration of the solution space and avoiding local optima.</ul>
<ul>Simulated Annealing is effective for refining queries to maximize their precision and recall.</ul>

</li>

### cuDF and Pandas
The cuDF and Pandas notebook leverages cuDF, a GPU-accelerated library for data manipulation, alongside Pandas, a widely-used data analysis library in Python.

<li>
<ul>cuDF: Enables rapid data processing and manipulation by offloading tasks to the GPU, significantly speeding up operations that would be slow on a CPU.</ul>
<ul>Pandas: Provides powerful data structures and functions for data manipulation and analysis. It is used for more complex operations where fine-tuned control and flexibility are needed.</ul>
<ul>Combining cuDF and Pandas allows for efficient handling of large datasets, facilitating the extraction and analysis of relevant information to construct effective Boolean queries.</ul>

</li>
