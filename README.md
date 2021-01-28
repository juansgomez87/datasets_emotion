# Music Emotion Recognition: towards new robust standards in personalized and context-sensitive applications

## Abstract
In this paper we present a review of the challenges and limitations of Music Emotion Recognition (MER), an interdisciplinary research area addressing the characterization of music in terms of emotion. 
It analyzes music in order to computationally predict the emotions perceived by or induced to a listener. 
Our aims are: (1) to provide insights on the typical approaches currently used in the MER workflow, and (2) hint at how previous research directs to specific future directions. 

We propose a new user-centric conceptualization framework for MER, highlighting where future researchers should focus efforts: (1) open data and experimental reproducibility, (2) inherent subjectivity of concepts and annotations, (3) model explainability and interpretability, (4) cultural and contextual relevance, and (5) ethical implications for MER applications.

This website offers a detailed overview of music and emotion datasets and extended bibliography. 

![MER models](https://github.com/juansgomez87/datasets_emotion/blob/master/img/challenges_spm.png)

## Music Emotion Recognition Datasets

| Dataset | Year | Content | Format | Size | Type | Perceived/Induced |
|:-------:|:----:|:-------:|:------:|:----:|:----:|:-----------------:|
|MoodsMIREX|2007|269 excerpts (30s long)|MP3|736MB|Categorical (5 mood clusters)|Perceived|
|CAL500|2007|500 full songs|MP3|366MB|Categorical (174 labels)|Perceived|
|Yang-Dim|2008|195 excerpts (25s long)| - | - |Dimensional|Perceived|
|MoodSwings|2008|240 excerpts (15s long)|
|NTWICM|2010|2648 full songs|MP3|11.7GB|"Discrete" Dimensional|Perceived|
|Soundtracks|2011|360+110 exceprts (15s-1m long)|MP3|216MB|Categorical (tension, anger, fear, happy, sad, tender) and Dimensional (valence, energy, tension)|Perceived|
|CH818|2017|818 excerpts (30s long)|MP3|393MB|Dimensional|Perceived|
|4Q audio emotion|2018|900 excerpts (30s long)|MP3|291MB|Categorical (Quadrants)|Perceived|
|DEAM/Mediaeval|2018|2058 excerpts (45s long)|MP3|1.4GB|Dimensional (Time-continuous A-V)|Perceived|
|DEAP| | |MP3| | |Induced
|Emotify|?|?|MP3|?|Categorical (adjectives)|Perceived|

## Additional information
#### Moods MIREX
* Author: Hu, X., Downie, J.S., Laurier, C., Bay, M., Ehmann, A.F.
* Description and music styles: Selection of the libraries of Associated Production Music (APM), “the world’s leading production music library… offering every imaginable music genre from beautiful classical music recordings to vintage rock to current indie band sounds".
* Annotation strategy: The pieces were rated by 3 raters, and only a subset of agreement by 2 out of 3 is extracted. 
* Annotation (categorical): Cluster 1 (passionate, rousing, confident, boisterous, rowdy), Cluster 2 (rollicking, cheerful, fun, sweet, amiable/good natured), Cluster 3 (literate, poignant, wistful, bittersweet, autumnal, brooding), Cluster 4 (humorous, silly, campy, quirky, whimsical, witty, wry), Cluster 5 (aggressive, fiery, tense/anxious, intense, volatile, visceral)
* Link: Offline

#### CAL500
* Author: Turnbull, D., Barrington, L., Torres, D., Lanckriet G. 
* Description and music styles: Songs were picked from the authors' personal collection of western popular 
music recorded within the last 50 years.
* Annotation strategy: The authors paid 66 undergraduate students to annotate the CAL500 corpus with semantic 
concepts from the vocabulary.  Participants were rewarded $10 for a one hour annotation block spent listening to the music.
* Annotation (categorical): 18 emotions, found by Skowronek et al. (2006) to be both important and easy to identify, were rated on a scale from one to three (e.g., not happy, neutral, happy).
* Link: http://calab1.ucsd.edu/~datasets/cal500/

#### Yang-Dim
* Author: Yang, Y.-H., Lin, Y.-C, Su, Y.-F, Chen, H.-H. 
* Description and music styles: The dataset contains 195 popular songs from Western, Chinese, and Japanese albums. 
* Annotation strategy: Subjects (most college students) are asked to listen to a subset of music dataset and to choose two values, each ranges from -1.0 to 1.0 in 11 levels, to indicate their feeling about the AV values of the music sample. The ground truth is set as the mean of the AV values of all subjects tested. On the average, more than ten pairs of AV values are collected from the subjective test for each music sample.
* Annotation (dimensional): Arousal and valence
* Link: http://mac.citi.sinica.edu.tw/~yang/MER/taslp08/#Data

#### MoodSwings
* Author: 
* Description and music styles: The dataset contains 195 popular songs from Western, Chinese, and Japanese albums. 
* Annotation strategy: The authors US pop music to collect arousal and valence values in a time continuous annotations. Two players from a game used the mouse to annotate the segment over a continuous AV space.
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: http://music.ece.drexel.edu/research/emotion/moodswingsturk

#### 4Q Emotion Dataset
* Author: Panda R., Malheiro R., Paiva R. P.
* Description and music styles: The AllMusic API served as the source of musical information, providing metadata such as artist, title, genre and emotion information, as well as 30-second audio clips for most songs. Mostly popularly consumed music.
* Annotation strategy: Collected from AllMusic API, emotion tags are selected from the original AllMusic Tags by intersecting them with the Warriner’s list. Finally, a manual blind validation is conducted by subjects.
* Annotation (categorical): Q1 (A+V+), Q2 (A+V-), Q3(A-V-), Q4 (A-V+)
* Link: http://mir.dei.uc.pt/downloads.html 


#### DEAM: MediaEval Database for Emotional Analysis in Music
* Author: Soleymani, M., Aljanaki, A., Yang, Y.
* Description and music styles: Royalty-free music from several sources: freemusicarchive.org (FMA), jamendo.com,
and the medleyDB datase. The excerpts which were annotated are available in the same package song ids between 1 and 2058. The dataset consists of 2014 development set (744 songs), 2014 evaluation set (1000 songs) and 2015 evaluation set (58 songs). Includes rock, pop, soul, blues, electronic, classical, hip-hop, international, experimental, folk, jazz, country and pop genres.
* Annotation strategy: Crowdsourced MTurk with each excerpt annotated at least by 10 workers. Both arousal and valence were annotated separately. Additional static annotations were collected for the whole 45 second exceprts after dynamic annotations. 
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: http://cvml.unige.ch/databases/DEAM/


#### Soundtracks
* Author: Eerola, T. & Vuoskoski, J. K.
* Description and music styles: This dataset we refer to as "Film soundtracks" are designed to overcome at least some of the problems mentioned above since they contain not that well known examples (although some could be identified by film aficionados).
* Annotation strategy: The selection of the excerpts has been done in terms of dimensional and discrete emotion model and evaluated by a pilot study. The initial ratings were made by 12 expert musicologists for both dimensional and discrete models. These ratings were then re-tested with 116 university students.
* Annotation: categorical and dimensional
* Link: https://osf.io/p6vkg/



#### NTWICM: Now That's What I Call Music
* Author: Schuller, B., Dorfner, J., Gerhard, R.
* Description and music styles: For building up a ground truth music database the compilation “Now That’s What I Call Music!” (U. K. series, volumes 1–69, double CDs, each) is selected. It represents very well most music styles which are popular today; that ranges from Pop and Rock music over Rap, R&B to electronic dance music as Techno or House.
* Annotation strategy: 4 raters gave static annotations for complete songs for arousal and valence in a discrete range of [−2,−1, 0, 1, 2]. 
* Annotation (dimensional): Arousal and valence [−2,−1, 0, 1, 2].
* Link: Offline 


#### CH818
* Author: Hu, X., Yang, Y.
* Description and music styles: Chinese Pop songs released in Taiwan, Hong Kong and Mainland China.
* Annotation strategy: Each clip was annotated by three music experts who were born and raised in Mainland China and thus were with a Chinese cultural background. The annotation was done with an interface consisting of two sliding bars of continuous real values between [-10,10]. 
* Annotation (dimensional): Arousal and valence real values between [-10,10] for whole excerpt.
* Link: Offline

## Extended bibliography
#### Reviews on MER
[1] Laurier, C., & Herrera, P. (2009). Automatic detection of emotion in music: Interaction with emotionally sensitive machines. Handbook of Research on Synthetic Emotions and Sociable Robotics: New Applications in Affective Computing and Artificial Intelligence, pp. 9–33. 

[2] Kim, Y. E., et al. (2010). Music Emotion Recognition: A state of the art review. Proceedings of the 11th International Society for Music Information Retrieval Conference (ISMIR), pp. 255–266. 

[3] Yang, Y.-H., & Chen, H. H. (2012). Machine Recognition of Music Emotion: A Review. ACM Transactions on Intelligent Systems and Technology, 3. 

[4] Yang, X, Dong, Y., & Li, J. (2018). Review of data features-based music emotion recognition methods. Multimedia Systems, 24(4), pp. 365–389. 


#### Articles

[1] Laukka, P. (2005). Categorical perception of vocal emotion expressions. Emotion, 5, pp. 277–295. 

[2] Gabrielsson, A. (2006). Emotion perceived and emotion felt: Same and different. Musicae Scientiae, 10(2), pp.191–213.

[3] Yang, Y.-H., et al. (2007). Music Emotion Recognition: The Role of Individuality. Proceedings of the International Workshop on Human-Centered Multimedia, pp. 13–22. 

[4] Henrich, J., Heine, S.J., & Norenzayan, A. (2010). The weirdest people in the world? Behavioral and Brain Sciences, 33, pp. 61–135.

[5] Eerola, T. (2011). Are the emotions expressed in music genre-specific? An audio- based evaluation of datasets spanning classical, film, pop and mixed genres. Journal of New Music Research. 40, pp. 349–366.

[6] Barthet, M., Fazekas, G., Sandler, M. (2012). Music Emotion Recognition: From content- to context-based models. In: Aramaki M., Barthet M., Kronland-Martinet R., Ystad S. (eds) From Sounds to Music and Emotions. CMMR 2012. Lecture Notes in Computer Science, vol 7900. Springer, Berlin, Heidelberg.

[7] Yang, Y.-H. & Liu, J.-Y. (2013). Quantitative Study of Music Listening Behavior in a Social and Affective Context. IEEE Transactions on Multimedia (TMM), 15(6), pp. 1304-1315.

[8] Coutinho, E., & Dibben, N. (2013). Psychoacoustic cues to emotion in speech prosody and music. Cognition and Emotion, 27(4), pp. 658–684.

[9] Yang, Y.-H. & Liu, J.-Y. (2015) Quantitative Study of Music Listening Behavior in a Smartphone Context. ACM Transactions on Interactive Intelligent Systems (TiiS). 5(3), Article 14.

[10] Coutinho, E., & Schuller, B. (2017). Shared acoustic codes underlie emotional communication in music and speech—evidence from deep transfer learning. PLoS ONE, 12(6).

[11] Hu, X., & Yang, Y.-H. (2017). The Mood of Chinese Pop Music: Representation and Recognition Xiao. Journal of the American Society for Information Science and Technology, 68(8), pp. 1899–1910. 

[12] Cespedes-Guevara, J., & Eerola, T. (2018). Music communicates affects, not basic emotions - A constructionist account of attribution of emotional meanings to music. Frontiers in Psychology, 9, pp. 1–19. 

[13] Jackson, J. C. et al. (2019). Emotion semantics show both cultural variation and universal structure. Science, pp. 1517–1522.

[14] Keltner, D., et al. (2019). What Basic Emotion Theory Really Says for the Twenty-First Century Study of Emotion. Journal of Nonverbal Behavior, 43(2), pp.195–201. 

#### Books
[1] Meyer, L. B. (1961). Emotion and Meaning. University of Chicago Press.

[2] Budd, M. (1992). Music and the Emotion. Routledge.

[3] Huron, D. (2006). Sweet Anticipation. MIT Press.

[4] Patel, A. D. (2008). Music, Language and the Brain. Oxford University Press.

[5] Juslin, P. & Sloboda, J. (2010). Handook of Music and Emotion: Theory, Research, Applications. Oxford University Press. 

[6] Krippendorff, K. H. (2004). Content Analysis: An Introduction to Its Methodology. SAGE Publications.

[7] Tkalčič, M., De Carolis, B., de Gemmis, M., Odić, A., & Košir, A. (2016). Emotions and Personality in Personalized Services. Springer Nature.

[8] Grekow, J. (2018). From Content-based Music Emotion Recognition to Emotion Maps of Musical Pieces. Springer Nature. 

#### PhD Dissertations
[1] Coutinho, E. (2008). Computational and Psycho-Physiological Investigations of Musical Emotions. University of Plymouth.

[2] Hu, X. (2010). Improving music mood classification using lyrics, audio and social tags. University of Illinois.

[3] Yang, Y.-H. (2010). Dimensional Music Emotion Recognition for Content Retrieval. National Tsing Hua University. 

[4] Laurier, C. (2011). Automatic Classification of Musical Mood by Content-Based Analysis. Universitat Pompeu Fabra. 

[5] Schmidt, E. (2012). Modeling and Predicting Emotion in Music. Drexel University. 

[6] Aljanaki, A. (2016). Emotion in Music: representation and computational modeling. Universiteit Utrecht.

[7] da Silva Mahleiro, R. M. (2016). Emotion-based Analysis and Classification of Music Lyrics. Universidade de Coimbra.

[8] Song, Y. (2016). The Role of Emotion and Context in Musical Preference. Queen Mary University of London.

[9] Barradas, G. T. (2017). A Cross-Cultural Approach to Psychological Mechanisms Underlying Emotional Reactions to Music. Uppsala Universitet.

[10] Panda, R. (2019). Emotion-based Analysis and Classification of Audio Music Emotion. Universidade de Coimbra.

## Publication
[Link to paper - *Not available yet*]()
```
@article{Gómez-Cañón2021,
    author = {{Gómez-Cañón, Juan Sebastián and 
               Cano, Estefanía and 
               Eerola, Tuomas and
               Gómez, Emilia and 
               Herrera, Perfecto and 
               Hu, Xiao and 
               Yang, Yi-Hsuan}},
    title = {{Music Emotion Recognition: towards new robust standards in personalized and context-sensitive applications}},
    year = {2021},
    journal = {},
}
```
