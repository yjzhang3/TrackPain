# TrackPain

## installation dependencies

Get pomegranate installed in Python3:

`pip3 install pomegranate`

Or get the latest version of pomegranate

`git clone https://github.com/jmschrei/pomegranate
cd pomegranate
python setup.py install`


Please refer to https://pgmpy.org/models/bayesiannetwork.html for more tutorials on creating a Bayesian network

## Introduction

This is the third part of the Hack$rare solution Trackpain, an inference model that can help predict pain levels for non-communicative children. Please refer to [this page](https://www.synapse.org/#!Synapse:syn26015614/wiki/) for the complete solution.

To show a proof of concept, we use an imaginary person whose biological data and pain scales are recorded. We will show how to construct a network for this particular individual patient. 

## Data preparation

- The sensor will collect biological data including heart rate variability, respiration rate, actigraphy, and skin conductance
- The phone app will collect self-reported metrics obtained from visual pain analog, including facial and emotional scores; the third party caregivers can also make observations about eating, sleeping, social, and verbal patterns. 
- Refer to [this notebook](https://github.com/yjzhang3/TrackPain/blob/main/Data-Pro.ipynb) for data cleaning probabilty calculation. 

## Modeling and inference
- Given probabilities value, create a static binary discrete Bayesian network
- Refer to [this notebook](https://github.com/yjzhang3/TrackPain/blob/main/TrackPain-Bayesian-Preliminary.ipynb) for model creation and prediction

## Future consideration 
- Make a continuous instead of discrete network
- following this pipeline, construct a dynamic network that fits all patients data

## Debug
- Note that we are trying to solve the error in network creation. See [Issue Section](https://github.com/yjzhang3/TrackPain/issues).

## Newest version on google colab
- We've updated the model so it can make predictions now! Please check this link: https://colab.research.google.com/drive/1N4vU16H4AUoZejXxH6Op-ekH4pLF4KF3?authuser=1#scrollTo=GIaJfuIqr0E5

