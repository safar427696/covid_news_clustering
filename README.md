🚀 Project Highlights: COVID-19 News Clustering

Objective: To distinguish between reliable news and "dodgy" social media narratives by automatically extracting, vectorizing, and clustering COVID-19 related articles.
🛠️ The Pipeline

I developed an end-to-end NLP pipeline that transforms raw social media URLs into structured thematic clusters:

    Extraction: Leveraged Newspaper3k to strip HTML and isolate the core article body.

    NLP Processing: Utilized Gensim for automated text summarization and keyword extraction.

    Vectorization: Converted text data into machine-readable format using Word Vectors, calculating the Vector Average per article to represent its unique "semantic fingerprint."

    Clustering: Applied Unsupervised Machine Learning to group articles by topic similarity without the need for manual labeling.

📊 Key Results

    Noise Reduction: Successfully filtered out video-hosting platforms to focus exclusively on text-based news credibility.

    Automated Tagging: Eliminated manual effort by generating keywords and summaries directly from raw URLs.

    Semantic Grouping: The model successfully identified clusters of related articles based on vector averages, providing a scalable way to monitor the spread of information/misinformation.

⚙️ Setup & Requirements
1. External Dependencies

This project utilizes a pre-trained Word2Vec (fastText) model to generate semantic vectors. Due to GitHub's file size limits, the model file (5.5 GB) is not included in this repository.

To run the project, please follow these steps:

    Download the German Wiki vectors from Facebook's fastText mirror:
    👉 Download wiki.de.vec (5.5 GB)

    Move the downloaded file into the /models directory of this project.

    Ensure the filename remains wiki.de.vec for the script to reference it correctly.

2. Environment Setup

Install the necessary NLP and Machine Learning libraries:
pip install -r requirements.txt
