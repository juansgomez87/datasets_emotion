# Music Emotion Recognition: towards new robust standards in personalized and context-sensitive applications

## Abstract
In this paper we present a review of the challenges and limitations of Music Emotion Recognition (MER), an interdisciplinary research area addressing the characterization of music in terms of emotion. 
It analyzes music in order to computationally predict the emotions perceived by or induced to a listener. 
Our aims are: (1) to provide insights on the typical approaches currently used in the MER workflow, and (2) hint at how previous research directs to specific future directions. 

We propose a new user-centric conceptualization framework for MER, highlighting where future researchers should focus efforts: (1) open data and experimental reproducibility, (2) inherent subjectivity of concepts and annotations, (3) model explainability and interpretability, (4) cultural and contextual relevance, and (5) ethical implications for MER applications.

## Music Emotion Recognition Datasets
| Dataset | Year | Content | Format | Size | Annotation Type |
|:-------:|:----:|:-------:|:------:|:----:|:---------------:|
|4Q audio emotion|2018|900 excerpts (30s long)|MP3|291MB|Categorical (Quadrants)|
|DEAM/Mediaeval|2018|2058 excerpts (45s long)|MP3|1.4GB|Dimensional (Time-continuous A-V)|
|Soundtracks|2011|360+110 exceprts (15s-1m long)|MP3|216MB|Categorical (tension, anger, fear, happy, sad, tender) and Dimensional (valence, energy, tension)|
|MoodsMIREX|2008|269 excerpts (30s long)|MP3|736MB|Categorical (5 mood clusters)|Yes|
|NTWICM|2010|2648 full songs|MP3|11.7GB|"Discrete" Dimensional|
|CH818|2017|818 excerpts (30s long)|MP3|393MB|Dimensional|
|Emotify|?|?|MP3|?|Categorical (adjectives)|

## Additional information
#### 4Q Emotion Dataset
* Author: Panda R., Malheiro R., Paiva R. P.
* Description and music styles: The AllMusic API served as the source of musical information, providing metadata such as artist, title, genre and emotion information, as well as 30-second audio clips for most songs. Mostly popularly consumed music.
* Annotation strategy: Collected from AllMusic API, emotion tags are selected from the original AllMusic Tags by intersecting them with the Warriner’s list. Finally, a manual blind validation is conducted by subjects.
* Paper: *Panda R., Malheiro R., Paiva R. P. (2018). “Musical Texture and Expressivity Features for Music Emotion Recognition”, in Proceedings of the 19th International Society for Music Information Retrieval Conference (ISMIR) 2018, Paris, France.*
* Annotation (categorical): Q1 (A+V+), Q2 (A+V-), Q3(A-V-), Q4 (A-V+)
* Link: http://mir.dei.uc.pt/downloads.html 
* *Languages: English: 724, Spanish: 24, French: 0, German: 0, Other: 16, Unknown: 136, Total (from Metadata): 899*

#### DEAM: MediaEval Database for Emotional Analysis in Music
* Author: Soleymani, M., Aljanaki, A., Yang, Y.
* Description and music styles: Royalty-free music from several sources: freemusicarchive.org (FMA), jamendo.com,
and the medleyDB datase. The excerpts which were annotated are available in the same package song ids between 1 and 2058. The dataset consists of 2014 development set (744 songs), 2014 evaluation set (1000 songs) and 2015 evaluation set (58 songs). Includes rock, pop, soul, blues, electronic, classical, hip-hop, international, experimental, folk, jazz, country and pop genres.
* Annotation strategy: Crowdsourced MTurk with each excerpt annotated at least by 10 workers. Both arousal and valence were annotated separately. Additional static annotations were collected for the whole 45 second exceprts after dynamic annotations. 
* Paper: *Aljanaki A., Yang Y., Soleymani M. (2017) Developing a benchmark for emotional analysis of music. PLoS ONE 12(3): e0173392.*
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: http://cvml.unige.ch/databases/DEAM/
* *Languages: English: 1531, Spanish: 13, French: 0, German: 0, Other: 47, Unknown 211, Total (from Metadata): 1801*

#### Soundtracks
* Author: Eerola, T. & Vuoskoski, J. K.
* Description and music styles: This dataset we refer to as "Film soundtracks" are designed to overcome at least some of the problems mentioned above since they contain not that well known examples (although some could be identified by film aficionados).
* Annotation strategy: The selection of the excerpts has been done in terms of dimensional and discrete emotion model and evaluated by a pilot study. The initial ratings were made by 12 expert musicologists for both dimensional and discrete models. These ratings were then re-tested with 116 university students.
* Paper: *Eerola, T. & Vuoskoski, J. K. (2011). A comparison of the discrete and dimensional models of emotion in music. Psychology of Music, 39(1), 18-49.*
* Annotation: categorical and dimensional
* Link: https://osf.io/p6vkg/
* *Languages: None (instrumental)*

#### Moods MIREX
* Author: Hu, X., Downie, J.S., Laurier, C., Bay, M., Ehmann, A.F.
* Description and music styles: Selection of the libraries of Associated Production Music (APM), “the world’s leading production music library… offering every imaginable music genre from beautiful classical music recordings to vintage rock to current indie band sounds".
* Annotation strategy: The pieces were rated by 3 raters, and only a subset of agreement by 2 out of 3 is extracted. 
* Paper: *Downie, X. H. J. S., Cyril Laurier, and M. B. A. F. Ehmann. “The 2007 MIREX audio mood classification task: Lessons learned.” in Proceedings of the 9th International Society of Music Information Retrieval (ISMIR). 2008.*
* Annotation (categorical): Cluster 1 (passionate, rousing, confident, boisterous, rowdy), Cluster 2 (rollicking, cheerful, fun, sweet, amiable/good natured), Cluster 3 (literate, poignant, wistful, bittersweet, autumnal, brooding), Cluster 4 (humorous, silly, campy, quirky, whimsical, witty, wry), Cluster 5 (aggressive, fiery, tense/anxious, intense, volatile, visceral)
* Link: Offline (on MTB-DB)
* *Languages: No metadata*

#### NTWICM: Now That's What I Call Music
* Author: Schuller, B., Dorfner, J., Gerhard, R.
* Description and music styles: For building up a ground truth music database the compilation “Now That’s What I Call Music!” (U. K. series, volumes 1–69, double CDs, each) is selected. It represents very well most music styles which are popular today; that ranges from Pop and Rock music over Rap, R&B to electronic dance music as Techno or House.
* Annotation strategy: 4 raters gave static annotations for complete songs for arousal and valence in a discrete range of [−2,−1, 0, 1, 2]. 
* Paper: *Björn Schuller, Johannes Dorfner, Gerhard Rigoll: "Determination of Non-Prototypical Valence and Arousal in Popular Music: Features and Performances", EURASIP Journal on Audio, Speech, and Music Processing (JASMP), Special Issue on "Scalable Audio-Content Analysis", vol. 2010.*
* Annotation (dimensional): Arousal and valence [−2,−1, 0, 1, 2].
* Link: Offline 
* *Languages: English: 2491, Spanish: 5, French: 0, German: 0, Other: 6, Unknown 146, Total (from Metadata): 2648*

#### CH818
* Author: Hu, X., Yang, Y.
* Description and music styles: Chinese Pop songs released in Taiwan, Hong Kong and Mainland China.
* Annotation strategy: Each clip was annotated by three music experts who were born and raised in Mainland China and thus were with a Chinese cultural background. The annotation was done with an interface consisting of two sliding bars of continuous real values between [-10,10]. 
* Paper: *X. Hu and Y. Yang, "Cross-Dataset and Cross-Cultural Music Mood Prediction: A Case on Western and Chinese Pop Songs" in IEEE Transactions on Affective Computing, vol. 8, no. 02, pp. 228-240, 2017.*
* Annotation (dimensional): Arousal and valence real values between [-10,10] for whole excerpt.
* Link: *NOT AVAILABLE* (made available by Yi-Hsuan Yang).
* *Languages: Mandarin: 818, Total (from Metadata): 818*

## Extended bibliography
#### Books
[1] Meyer, L. B. (1961). Emotion and Meaning. University of Chicago Press.
[2] Budd, M. (1992). Music and the Emotion. Routledge.
[3] Huron, D. (2006). Sweet Anticipation. MIT Press.
[4] Patel, A. D. (2008). Music, Language and the Brain. Oxford University Press.
[5] Juslin, P. & Sloboda, J. (2010). Handook of Music and Emotion: Theory, Research, Applications. Oxford University Press.
[6] Krippendorff, K. H. (2004). Content Analysis: An Introduction to Its Methodology. SAGE Publications.
[7] Tkalčič, M., De Carolis, B., de Gemmis, M., Odić, A., & Košir, A. (2016). Emotions and Personality in Personalized Services. Springer Nature.
[8] Grekow, J. (2018). From Content-based Music Emotion Recognition to Emotion Maps of Musical Pieces. Springer Nature. 

#### Articles


#### PhD Thesis
[1] Coutinho, E. (2008). Computational and Psycho-Physiological Investigations of Musical Emotions. University of Plymouth
[2] Hu, X. (2010). Improving music mood classification using lyrics, audio and social tags. University of Illinois.
[3] Yang, Y.-H. (2010). Dimensional Music Emotion Recognition for Content Retrieval. National Tsing Hua University. 
Laurier, C. (2011). Automatic Classification of Musical Mood by Content-Based Analysis. Universitat Pompeu Fabra. 
Schmidt, E. (2012). Modeling and Predicting Emotion in Music. Drexel University. 
Aljanaki, A. (2016). Emotion in Music: representation and computational modeling. Universiteit Utrecht.
da Silva Mahleiro, R. M. (2016). Emotion-based Analysis and Classification of Music Lyrics. Universidade de Coimbra
Song, Y. (2016). The Role of Emotion and Context in Musical Preference. Queen Mary University of London.
Barradas, G. T. (2017). A Cross-Cultural Approach to Psychological Mechanisms Underlying Emotional Reactions to Music. Upsala Universitet.
Panda, R. (2019). Emotion-based Analysis and Classification of Audio Music Emotion. Universidade de Coimbra.

## Publication
[Link to paper - *Not available yet*]()
```
@article{Gómez-Cañón2021,
author = {{Gómez-Cañón, Juan Sebastián and Cano, Estefanía and Gómez, Emilia and Herrera, Perfecto and Hu, Xiao and Yang, Yi-Hsuan}},
title = {{Music Emotion Recognition: towards new robust standards in personalized and context-sensitive applications}},
year = {2021},
journal = {},
number = {},
pages = {},
publisher = {},
volume = {},
}
```
