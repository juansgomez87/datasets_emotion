# datasets_emotion
This repository collects information about different data sets for Music Emotion Recognition and Speech Emotion Recognition.

## MER Data sets

| Dataset | Year | Content | Format | Size | Annotation Type | Language |
|:-------:|:----:|:-------:|:------:|:----:|:---------------:|:--------:|
|4Q audio emotion|2018|900 excerpts (30s long)|MP3|291MB|Categorical (Quadrants)|Mainly english, some spanish and portuguese|
|DEAM|2018|2058 excerpts (45s long)|MP3|xxMB|Dimensional (Time-continuous A-V)|xxx|
|Soundtracks|2011|360+110 exceprts (15s-1m long)|MP3|xxMB|Categorical (tension, anger, fear, happy, sad, tender) and Dimensional (Valence-Energy)|Instrumental|
|NTWICM|
|CH818|
|MoodsCLaurier|

## SER Data sets
| Dataset | Year | Content | Format | Size | Annotation Type | Language |
|:-------:|:----:|:-------:|:------:|:----:|:---------------:|:--------:|


## Additional information
### MER Data sets
#### 4Q Emotion Dataset
* Author: Panda R., Malheiro R., Paiva R. P.
* Description and music styles: Mostly popularly consumed 
* Annotation strategy: Collected from AllMusic API, emotion tags are selected from the original AllMusic Tags by intersecting them with the Warriner’s list. Finally, a manual blind validation is conducted by subjects.
* Paper: Panda R., Malheiro R., Paiva R. P. (2018). “Musical Texture and Expressivity Features for Music Emotion Recognition”. 19th International Society for Music Information Retrieval Conference – ISMIR 2018, Paris, France.
* Annotation (categorical): Q1 (A+V+), Q2 (A+V-), Q3(A-V-), Q4 (A-V+)
* Link: http://mir.dei.uc.pt/downloads.html 

#### DEAM: MediaEval Database for Emotional Analysis in Music
* Author: Soleymani, M., Aljanaki, A., Yang, Y.
* Description and music styles: Royalty-free music from several sources: freemusicarchive.org (FMA), jamendo.com,
and the medleyDB datase. The excerpts which were annotated are available in the same package song ids between 1 and 2058. The dataset consists of 2014 development set (744 songs), 2014 evaluation set (1000 songs) and 2015 evaluation set (58 songs).
* Annotation strategy: Resampled the annotations and generated the averaged annotations with 2Hz sampling rate. Collected through three years of MediaEval
* Paper: Aljanaki A, Yang Y-H, Soleymani M (2017) Developing a benchmark for emotional analysis of music. PLoS ONE 12(3): e0173392. https://doi.org/10.1371/journal.pone.0173392
* Annotation (dimensional): Time-continuous arousal and valence annotation
* Link: http://cvml.unige.ch/databases/DEAM/

#### Soundtracks
* Author: Eerola, T. & Vuoskoski, J. K.
* Description and music styles: This dataset we refer to as "Film soundtracks" are designed to overcome at least some of the problems mentioned above since they contain not that well known examples (although some could be identified by film aficionados).
* Annotation strategy: The selection of the excerpts has been done in terms of dimensional and discrete emotion model and evaluated by a pilot study and a larger scale rating study.
* Paper: Eerola, T. & Vuoskoski, J. K. (2011). A comparison of the discrete and dimensional models of emotion in music. Psychology of Music, 39(1), 18-49. https://doi.org/10.1177/0305735610362821
* Annotation: categorical and dimensional
* Link: https://osf.io/p6vkg/

#### NTWICM: Now That's What I Call Music
* Author: 
* Description and music styles: 
* Annotation strategy: 
* Paper: 
* Annotation (dimensional): 
* Link: 

#### CH818
* Author: 
* Description and music styles: 
* Annotation strategy: 
* Paper: 
* Annotation
* Link: 

#### MoodsCLaurier
* Author: Laurier, C.
* Description and music styles: 
* Annotation strategy: 
* Paper: 
* Annotation
* Link: 

### SER Data sets


