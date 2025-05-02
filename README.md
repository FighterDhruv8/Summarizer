# Overview

This personal project was made by me as my first peek into Transformers and Natural Language Processing.

The first attempt was [Summarizer.ipynb](https://github.com/FighterDhruv8/Summarizer/blob/main/Summarizer.ipynb). It worked decently for shorter inputs, however the bart model's input token limit caused the model to give truncated summaries for longer inputs.

To rectify this, I searched online and found the summarizer used in [kmeans_summarizer.ipynb](https://github.com/FighterDhruv8/Summarizer/blob/main/kmeans_summarizer.ipynb). As I understand it, the input is split into chunks and the k-means algorithm is applied to the vector embeddings of these chunks. The centroids of the k-means clusters are then picked and these centroid vectors are fed to the summarizer model, greatly reducing the input tokens while preserving semantic context.

I've also heard about something called RAG (Retrieval-Augmented Generation), and I'm excited to see how it can help with summarization tasks.
