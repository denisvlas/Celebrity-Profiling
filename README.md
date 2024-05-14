The dataset you can download here - https://zenodo.org/records/3530253


PAN19 Authorship Analysis: Celebrity Profiling

Description

Celebrities are among the most prolific users of social media, promoting their personas and rallying followers. This activity is closely tied to genuine writing samples, rendering them worthy research subjects in many respects, not least author profiling.

The Celebrity Profiling task this year is to predict four traits of a celebrity from their social media communication. The traits are the degree of fame, occupation, age, and gender. The social media communication is given as the teaser messages from past tweets. The goal is to develop a piece of software which predicts celebrity traits from the teaser history.

The training dataset contains two files: a feeds.ndjson as input and a labels.ndjson as output. Each file lists all celebrities as JSON objects, one per line and identified by the id key.

The input file contains the cid and a list of all teaser messages for each celebrity.

{"id": 1234, "text": ["a tweet", "another tweet", ...]}
The output file contains the cid and a value for each trait for each celebrity from the input file.

{"id": 1234, "fame": "star", "occupation": "sports", "gender": "female", "birthyear": 2002}
The following values are possible for each of the traits:

fame := {rising, star, superstar} 
occupation := {sports, performer, creator, politics, manager, science, professional, religious} 
birthyear := {1940, ..., 2012} 
gender := {male, female, nonbinary}
