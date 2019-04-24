# datasets_emotion
This repository collects information about different data sets for Music Emotion Recognition and Speech Emotion Recognition.

## MER Data sets

| Dataset | Year | Content | Format | Size | Annotation Type | Language | Obtained |
|:-------:|:----:|:-------:|:------:|:----:|:---------------:|:--------:|:--------:|
|4Q audio emotion|2018|900 excerpts (30s long)|MP3|291MB|Categorical (Quadrants)|Mainly english, some spanish and portuguese|Yes|
|DEAM/Mediaeval/AMG1608|2018|2058 excerpts (45s long)|MP3|1.4GB|Dimensional (Time-continuous A-V)|Mainly english, italian, spanish, portuguese|Yes|
|Soundtracks|2011|360+110 exceprts (15s-1m long)|MP3|216MB|Categorical (tension, anger, fear, happy, sad, tender) and Dimensional (valence, energy, tension)|Instrumental|Yes|
|MoodsMIREX|2008|269 excerpts (30s long)|MP3|736MB|Categorical (5 mood clusters)|Mainly english|Yes|
|NTWICM|2010|2648 full songs|MP3|11.7GB|"Discrete" Dimensional|Mainly english|Yes|
|CH818|2017|818 excerpts (30s long)|?|?|?|Mandarin|No|

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
and the medleyDB datase. The excerpts which were annotated are available in the same package song ids between 1 and 2058. The dataset consists of 2014 development set (744 songs), 2014 evaluation set (1000 songs) and 2015 evaluation set (58 songs). Includes rock, pop, soul, blues, electronic, classical, hip-hop, international, experimental, folk, jazz, country and pop genres.
* Annotation strategy: Crowdsourced MTurk with each excerpt annotated at least by 10 workers. Both arousal and valence were annotated separately. Additional static annotations were collected for the whole 45 second exceprts after dynamic annotations. 
* Paper: Aljanaki A., Yang Y., Soleymani M. (2017) Developing a benchmark for emotional analysis of music. PLoS ONE 12(3): e0173392. https://doi.org/10.1371/journal.pone.0173392
* Annotation (dimensional): Time-continuous arousal and valence annotation
* Link: http://cvml.unige.ch/databases/DEAM/

#### Soundtracks
* Author: Eerola, T. & Vuoskoski, J. K.
* Description and music styles: This dataset we refer to as "Film soundtracks" are designed to overcome at least some of the problems mentioned above since they contain not that well known examples (although some could be identified by film aficionados).
* Annotation strategy: The selection of the excerpts has been done in terms of dimensional and discrete emotion model and evaluated by a pilot study. The initial ratings were made by 12 expert musicologists for both dimensional and discrete models. These ratings were then re-tested with 116 university students.
* Paper: Eerola, T. & Vuoskoski, J. K. (2011). A comparison of the discrete and dimensional models of emotion in music. Psychology of Music, 39(1), 18-49. https://doi.org/10.1177/0305735610362821
* Annotation: categorical and dimensional
* Link: https://osf.io/p6vkg/

#### Moods MIREX
* Author: Hu, X., Downie, J.S., Laurier, C., Bay, M., Ehmann, A.F.
* Description and music styles: Selection of the libraries of Associated Production Music (APM), “the world’s leading production music library… offering every imaginable music genre from beautiful classical music recordings to vintage rock to current indie band sounds".
* Annotation strategy: The pieces were rated by 3 raters, and only a subset of agreement by 2 out of 3 is extracted. 
* Paper: Downie, X. H. J. S., Cyril Laurier, and M. B. A. F. Ehmann. “The 2007 MIREX audio mood classification task: Lessons learned.” Proceeding of the 9th International Conference of Music Information Retrieval (ISMIR). 2008.
* Annotation (categorical): Cluster 1 (passionate, rousing, confident, boisterous, rowdy), Cluster 2 (rollicking, cheerful, fun, sweet, amiable/good natured), Cluster 3 (literate, poignant, wistful, bittersweet, autumnal, brooding), Cluster 4 (humorous, silly, campy, quirky, whimsical, witty, wry), Cluster 5 (aggressive, fiery, tense/anxious, intense, volatile, visceral)
* Link: Offline (on MTB-DB)

#### NTWICM: Now That's What I Call Music
* Author: Schuller, B., Dorfner, J., Gerhard, R.
* Description and music styles: For building up a ground truth music database the compilation “Now That’s What I Call Music!” (U. K. series, volumes 1–69, double CDs, each) is selected. It represents very well most music styles which are popular today; that ranges from Pop and Rock music over Rap, R&B to electronic dance music as Techno or House.
* Annotation strategy: 4 raters gave static annotations for complete songs for arousal and valence in a discrete range of {−2,−1, 0, 1, 2}. 
* Paper: Björn Schuller, Johannes Dorfner, Gerhard Rigoll: "Determination of Non-Prototypical Valence and Arousal in Popular Music: Features and Performances", EURASIP Journal on Audio, Speech, and Music Processing (JASMP), Special Issue on "Scalable Audio-Content Analysis", vol. 2010, Article ID 735854, 19 pages, 2010.
* Annotation (dimensional): Arousal and valence {−2,−1, 0, 1, 2}.
* Link: Offline 

#### CH818
* Author: Hu, X., Yang, Y.
* Description and music styles: Chinese Pop songs released in Taiwan, Hong Kong and Mainland China.
* Annotation strategy: Each clip was annotated by three music experts who were born and raised in Mainland China and thus were with a Chinese cultural background. The annotation was done with an interface consisting of two sliding bars of continuous real values between [-10,10]. 
* Paper: X. Hu and Y. Yang, "Cross-Dataset and Cross-Cultural Music Mood Prediction: A Case on Western and Chinese Pop Songs" in IEEE Transactions on Affective Computing, vol. 8, no. 02, pp. 228-240, 2017. doi: 10.1109/TAFFC.2016.2523503
* Annotation (dimensional): Arousal and valence continuous real values between [-10,10].
* Link: *NOT AVAILABLE*

### SER Data sets


