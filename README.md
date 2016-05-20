# Tempo Estimation for Music Loops and a Simple Confidence Measure

This repository contains instructions for reproducing the research described in the paper *Font, F., & Serra, X. (2016). Tempo Estimation for Music Loops and a Simple Confidence Measure. In Int. Conf. on Music Information Retrieval (ISMIR) (pp. 1–7)*. The full text of the paper can be [found here](TODOlink). It includes code, data and research analyses.

In order to run the analyses described in the paper you'll need to set up the 
datasets and analyze its content. Below you'll find the instructions gor setting up the datasets, analysis algorithms and scripts. Before setting up any of these, you should create a Python virtual environment and install the requirements
listed in ```requirements.txt```. In addition, you'll need to install [ffmpeg](https://www.ffmpeg.org) (for audio conversion) and, optionally, [rabbitMQ](rabbitMQ) (needed for paralelizing analysis using [Celery](https://docs.getsentry.com/hosted/) distributed task manager).

 * [Instructions for setting up datasets](docs/create_dataset.md)
 * [Instructions for setting up analysis algorithms](docs/setting_up_algorithms.md)
 * [Instructions for analyzing the datasets](docs/analyze_dataset.md)

Once datasets are set up and audio analysis is carried out, you can run the following IPython notebooks which contain the code to generate the results and plots shown in the paper:

 * [Datasets](Datasets.ipynb): information and statistics about the datasets, corresponds to Section 4.1 of the paper.
 * [Confidence measure](Confidence%20measure.ipynb): description of the confidence measure with examples and code, corresponds to Section 3 of the paper.
 * [Tempo estimation results](Tempo%20estimation%20results.ipynb): evaluation of the different tempo estimation algorithms and confidence measure, corresponds to Section 5 of the paper.



