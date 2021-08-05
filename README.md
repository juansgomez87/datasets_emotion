# Music Emotion Recognition: towards new robust standards in personalized and context-sensitive applications

## Abstract
In this paper we present a review of the challenges and limitations of Music Emotion Recognition (MER), an interdisciplinary research area addressing the characterization of music in terms of emotion. 
It analyzes music in order to computationally predict the emotions perceived by or induced to a listener. 
Our aims are: (1) to provide insights on the typical approaches currently used in the MER workflow, and (2) hint at how previous research directs to specific future directions. 

We propose a new user-centric conceptualization framework for MER, highlighting where future researchers should focus efforts: (1) open data and experimental reproducibility, (2) inherent subjectivity of concepts and annotations, (3) model explainability and interpretability, (4) cultural and contextual relevance, and (5) ethical implications for MER applications.

This website offers a detailed overview of music and emotion datasets and an extended bibliography. 

## Table of Contents
1. [Music Emotion Recognition Datasets](#music-emotion-recognition-datasets)
    1. [Additional information](#additional-information)
2. [Extended bibliography](#extended-bibliography)
    1. [Reviews on MER](#reviews-on-mer)
    2. [Articles](#articles)
        1. [Music Cognition](#music-cognition)
        2. [MER literature](#mer-literature) 
        3. [Annotation gathering](#annotation-gathering)
        4. [Context-sensitive models](#context-sensitive-models)
        5. [Personalized models](#personalized-models)
    3. [Books](#books)
    4. [PhD Dissertations](#phd-dissertations)
3. [Publication](#publication)

![MER models](https://github.com/juansgomez87/datasets_emotion/blob/master/img/challenges_spm.png)

## Music Emotion Recognition Datasets

| Dataset | Year | Content | Format | Size | Type | Perceived/Induced |
|:-------:|:----:|:-------:|:------:|:----:|:----:|:-----------------:|
|[MoodsMIREX](#moods-mirex)|2007|269 excerpts (30s long)|MP3|736MB|Categorical (5 mood clusters)|Perceived|
|[CAL500](#cal500)|2007|500 full songs|MP3|366MB|Categorical (174 labels)|Perceived|
|[Yang-Dim](#yang-dim)|2008|195 excerpts (25s long)| - | - |Dimensional|Perceived|
|[MoodSwings](#moodswings)|2008|240 excerpts (15s long)| - | - |Dimensional (Time-continuous A-V)|Perceived|
|[NTWICM](#now-thats-what-i-call-music)|2010|2648 full songs|MP3|11.7GB|"Discrete" Dimensional|Perceived|
|[Soundtracks](#soundtracks)|2011|360+110 exceprts (15s-1m long)|MP3|216MB|Categorical (tension, anger, fear, happy, sad, tender) and Dimensional (valence, energy, tension)|Perceived|
|[DEAP](#deap)|2012|120 exceprts (60s long)|Links| - |Dimensional|Induced|
|[AMG1608](#amg1608)|2015|1608 excerpts (30s long)|WAV|4.3GB|"Discrete" Dimensional|Perceived|
|[Emotify](#emotify)|2016|400 excerpts (60s long)|MP3|363MB|Categorical (GEMS)|Induced|
|[CH818](#ch818)|2017|818 excerpts (30s long)|MP3|393MB|Dimensional|Perceived|
|[4Q-emotion](#4q-emotion-dataset)|2018|900 excerpts (30s long)|MP3|291MB|Categorical (Quadrants)|Perceived|
|[DEAM/Mediaeval](#mediaeval-database-for-emotional-analysis-in-music)|2018|2058 excerpts (45s long)|MP3|1.4GB|Dimensional (Time-continuous A-V)|Perceived|
|[PMEmo](#pmemo)|2018|794 full songs|MP3|1.3GB|Dimensional (Time-continuous A-V)|Induced|
|[Jamendo Moods and Themes](#jamendo-mood-and-theme-subset)|2019|18486 full songs|MP3|152GB|Categorical|Perceived|
|[VGMIDI](#vgmidi)|2019|200 MIDI files|MIDI|1.37GB|Dimensional|Perceived|
|[CCMED-WCMED](#ccmed-wcmed)|2020|800 excerpts (8-20s long)|WAV| - |"Discrete" Dimensional|Perceived|

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
* Author: Kim, Y., Schmidt, E., Emelle, L.
* Description and music styles: The authors used US pop music to collect time-varying perception of emotions.
* Annotation strategy: Two players from a game used the mouse to annotate the segment over a continuous AV space.
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: Offline

#### Now That's What I Call Music
* Author: Schuller, B., Dorfner, J., Gerhard, R.
* Description and music styles: For building up a ground truth music database the compilation “Now That’s What I Call Music!” (U. K. series, volumes 1–69, double CDs, each) is selected. It represents very well most music styles which are popular today; that ranges from Pop and Rock music over Rap, R&B to electronic dance music as Techno or House.
* Annotation strategy: 4 raters gave static annotations for complete songs for arousal and valence in a discrete range of [−2,−1, 0, 1, 2]. 
* Annotation (dimensional): Arousal and valence [−2,−1, 0, 1, 2].
* Link: http://openaudio.eu/NTWICM-Mood-Annotation.arff (annotations) 

#### Soundtracks
* Author: Eerola, T. & Vuoskoski, J. K.
* Description and music styles: This dataset we refer to as "Film soundtracks" are designed to overcome at least some of the problems mentioned above since they contain not that well known examples (although some could be identified by film aficionados).
* Annotation strategy: The selection of the excerpts has been done in terms of dimensional and discrete emotion model and evaluated by a pilot study. The initial ratings were made by 12 expert musicologists for both dimensional and discrete models. These ratings were then re-tested with 116 university students.
* Annotation: categorical and dimensional
* Link: https://osf.io/p6vkg/

#### DEAP
* Author: Koelstra, S., Muehl, C., Soleymani, M., Lee, J.-S., Yazdani, A., Ebrahimi, T., Pun, T., Nijholt, A., Patras, I.
* Description and music styles: From the 120 original videos from YouTube, 60 were manually selected, while the remaining 60 were selected via Last.FM affective tags. EEG and physiological signals were recorded and each participant also rated the videos as above. For 22 participants frontal face video was also recorded.
* Annotation strategy: The participants ratings, physiological recordings and face video of an experiment where 32 volunteers (mostly European students) watched a subset of 40 of the above music videos. EEG and physiological signals were recorded and each participant also rated the videos as above. For 22 participants frontal face video was also recorded.
* Annotation: Dimensional (arousal, valence, and dominance)
* Link: http://www.eecs.qmul.ac.uk/mmv/datasets/deap/

#### AMG1608
* Author: Chen, Y.-A, Yang, Y.-H., Wang, J.-C., Chen, H.-H.
* Description and music styles: The dataset contemporary Western music from AMG, which has 34 distinct mood categories defined by music editors.
* Annotation strategy: Each subject is asked to annotate 13 songs and the subject can annotate a song by placing the cursor on the panel to indicate the location of the perceived VA value of the song.
* Annotation (dimensional): Arousal and valence real values between [-1,1] for whole excerpt.
* Link: https://amg1608.blogspot.com/

#### Emotify
* Author: Aljanaki, A., Wiering, F., Veltkamp, R.C.
* Description and music styles: The selected songs include mainly four genres (rock, classical, pop and electronic) music. 
* Annotation strategy: The annotations were collected using GEMS scale (Geneva Emotional Music Scales). The annotations produced by the game are spread unevenly among the songs, which is caused both by design of the experiment and design of the game. Participants could skip songs and switch between genres, and they were encouraged to do so, because induced emotional response does not automatically occur on every music listening occasion. 
* Annotation (categorical): Nine categories (amazement, solemnity, tenderness, nostalgia, calmness, power, joyful activation, tension, sadness)
* Link: http://www2.projects.science.uu.nl/memotion/emotifydata/

#### CH818
* Author: Hu, X., Yang, Y.
* Description and music styles: Chinese Pop songs released in Taiwan, Hong Kong and Mainland China.
* Annotation strategy: Each clip was annotated by three music experts who were born and raised in Mainland China and thus were with a Chinese cultural background. The annotation was done with an interface consisting of two sliding bars of continuous real values between [-10,10]. 
* Annotation (dimensional): Arousal and valence real values between [-10,10] for whole excerpt.
* Link: Offline

#### 4Q Emotion Dataset
* Author: Panda R., Malheiro R., Paiva R. P.
* Description and music styles: The AllMusic API served as the source of musical information, providing metadata such as artist, title, genre and emotion information, as well as 30-second audio clips for most songs. Mostly popularly consumed music.
* Annotation strategy: Collected from AllMusic API, emotion tags are selected from the original AllMusic Tags by intersecting them with the Warriner’s list. Finally, a manual blind validation is conducted by subjects.
* Annotation (categorical): Q1 (A+V+), Q2 (A+V-), Q3(A-V-), Q4 (A-V+)
* Link: http://mir.dei.uc.pt/downloads.html 

#### MediaEval Database for Emotional Analysis in Music
* Author: Soleymani, M., Aljanaki, A., Yang, Y.
* Description and music styles: Royalty-free music from several sources: freemusicarchive.org (FMA), jamendo.com,
and the medleyDB datase. The excerpts which were annotated are available in the same package song ids between 1 and 2058. The dataset consists of 2014 development set (744 songs), 2014 evaluation set (1000 songs) and 2015 evaluation set (58 songs). Includes rock, pop, soul, blues, electronic, classical, hip-hop, international, experimental, folk, jazz, country and pop genres.
* Annotation strategy: Crowdsourced MTurk with each excerpt annotated at least by 10 workers. Both arousal and valence were annotated separately. Additional static annotations were collected for the whole 45 second exceprts after dynamic annotations. 
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: http://cvml.unige.ch/databases/DEAM/

#### PMEmo
* Author: Zhang, K., Zhang, H., Li, S., Yang, C., Sun, L.
* Description and music styles: The authors gathered songs popular all around the world: the Billboard Hot 100, the iTunes Top 100 Songs (USA), and the UK Top 40 Singles Chart. They obtained songs available from these charts from 2016 to 2017.
* Annotation strategy: Similar to DEAM, the annotation was done with the slider to collect dynamic annotations at a sampling rate of 2 Hz. Additionally, annotators should make a static annotation for the whole music excerpt on nine-point scale after finishing dynamic labelling. A total of 457 subjects (236 females and 221 males) are recruited to participate in this work. The electrodermal activity was sampled continuously at a sampling rate of 50 Hz.
* Annotation (dimensional): Time-continuous arousal and valence annotation (2 Hz)
* Link: https://github.com/HuiZhangDB/PMEmo

#### Jamendo Mood and Theme Subset
* Author: Bogdanov, D., Porter A., Tovstogan P., & Won M. 
* Description and music styles: The MTG-Jamendo Dataset is an open dataset for music auto-tagging and a subset of the dataset is used in the Emotion and Theme Recognition in Music Task within MediaEval 2019. The dataset contains 87 genre tags, so there is style diversity. 
* Annotation strategy: The 56 mood/theme tags were crowdsourced from social media tags on the Jamendo platform. Hence, the annotations can be single- or multi-labeled depending on the excerpt. 
* Annotation (categorical): 56 mood/theme tags
* Link: https://multimediaeval.github.io/2019-Emotion-and-Theme-Recognition-in-Music-Task/

#### VGMIDI
* Author: Ferreira, L., Whitehead, J.
* Description and music styles: VGMIDI is a dataset of 200 MIDI labelled piano pieces (video game soundtracks).
* Annotation strategy: Each piece was annotated by 30 human subjects according to a valence-arousal model of emotion. The authors ask the annotators to write two to three sentences describing the short pieces they listened to.
* Annotation (dimensional): Time-continuous arousal and valence annotation
* Link: https://github.com/lucasnfe/vgmidi

#### CCMED-WCMED
* Author: Fan, J., Yang, Y.-H., Gong, K, Pasquier, P.
* Description and music styles: The dataset contains 400 excerpts collected from Western classical music recordings and 400 excerpts collected from Chinese classical music recordings.
* Annotation strategy: Two crowdsourcing experiments were carried out to collect emotional annotations (arousal and valence). The authors used a ranking-based method. Instead of providing absolute ratings, participants do pairwise comparisons by deciding which audio excerpt has higher arousal/valence.
* Annotation (dimensional): Arousal and valence real values between [-1,1] for whole excerpt.
* Link: https://metacreation.net/ccmed_wcmed_soundscape/

## Extended bibliography
#### Reviews on MER
[1] Laurier, C., & Herrera, P. (2009). Automatic detection of emotion in music: Interaction with emotionally sensitive machines. Handbook of Research on Synthetic Emotions and Sociable Robotics: New Applications in Affective Computing and Artificial Intelligence, pp. 9–33. 

[2] Kim, Y. E., et al. (2010). Music Emotion Recognition: A state of the art review. Proceedings of the 11th International Society for Music Information Retrieval Conference (ISMIR), pp. 255–266. 

[3] Yang, Y.-H., & Chen, H. H. (2012). Machine Recognition of Music Emotion: A Review. ACM Transactions on Intelligent Systems and Technology, 3. 

[4] Yang, X, Dong, Y., & Li, J. (2018). Review of data features-based music emotion recognition methods. Multimedia Systems, 24(4), pp. 365–389. 

#### Articles

##### Music cognition

[1] Laukka, P. (2005). Categorical perception of vocal emotion expressions. Emotion, 5, pp. 277–295. 

[2] Gabrielsson, A. (2006). Emotion perceived and emotion felt: Same and different. Musicae Scientiae, 10(2), pp.191–213.

[3] Henrich, J., Heine, S.J., & Norenzayan, A. (2010). The weirdest people in the world? Behavioral and Brain Sciences, 33, pp. 61–135.

[3] Vuoskoski, J. & Eerola, T. (2011). Measuring music-induced emotion. Musicae Scienentiae. 

[4] Eerola, T. (2011). Are the emotions expressed in music genre-specific? An audio- based evaluation of datasets spanning classical, film, pop and mixed genres. Journal of New Music Research. 40, pp. 349–366.

[5] Coutinho, E., & Dibben, N. (2013). Psychoacoustic cues to emotion in speech prosody and music. Cognition and Emotion, 27(4), pp. 658–684.

[6] Song, Y., et al. (2016). Perceived and Induced Emotion Responses to Popular Music: Categorical and Dimensional Models. Music Perception, 33(4), 472-492.

[7] Cespedes-Guevara, J., & Eerola, T. (2018). Music communicates affects, not basic emotions - A constructionist account of attribution of emotional meanings to music. Frontiers in Psychology, 9, pp. 1–19. 

[8] Keltner, D., et al. (2019). What Basic Emotion Theory Really Says for the Twenty-First Century Study of Emotion. Journal of Nonverbal Behavior, 43(2), pp.195–201. 

[9] Warrenburg, L. A. (2020). Choosing the right tune: A review of music stimuli used in emotion research. Music Perception, 37(3), 240–258.


##### MER literature

[1] Schuller, B., et al. (2010). Mister D.J. Cheer Me Up!: Musical and textual features for automatic mood classification. Journal of New Music Research, 39(1), 2010

[2] Barthet, M., Fazekas, G., Sandler, M. (2012). Music Emotion Recognition: From content- to context-based models. In: Aramaki M., Barthet M., Kronland-Martinet R., Ystad S. (eds) From Sounds to Music and Emotions. CMMR 2012. Lecture Notes in Computer Science, vol 7900. Springer, Berlin, Heidelberg.

[3] Soleymani, M. et al. (2012) A multimodal database for affect recognition and implicit tagging. IEEE Transactions on Affective Computing, 3(1), 42-55.

[4] Soleymani, M., Aljanaki, A., & Yang, Y.-H. (2014). Emotional Analysis of Music: A Comparison of Methods. Proceedings of the 22nd ACM International Conference on Multimedia Pages, 1161–1164. 

[5] Soleymani, M., Aljanaki, A., & Yang, Y.-H. (2014). Emotional Analysis of Music: A Comparison of Methods. Proceedings of the 22nd ACM International Conference on Multimedia Pages, 1161–1164. 

[6] Wang, J.C., et al. (2015). Modeling the Affective Content of Music with a Gaussian Mixture Model. IEEE Transcactions on Affective Computing, 6(1).

[7] Saari, P., et al. (2016). Genre-Adaptive Semantic Computing and Audio-Based Modelling for Music Mood Annotation. IEEE Transaction on Affective Computing, 7(2). 

[8] Coutinho, E., & Schuller, B. (2017). Shared acoustic codes underlie emotional communication in music and -speech—evidence from deep transfer learning. PLoS ONE, 12(6).

###### Lyrics

[1] Laurier, C. et al. (2008). Multimodal music mood classification using audio and lyrics. In Proceedings of the 7th International Conference on Machine Learning and Applications, San Diego, USA.

[2] Hu, X. & Downie, J.S. (2010) When lyrics outperform audio for music mood classification: a feature analysis. In Proceedings of the 11th International Society for Music Information Retrieval Conference (ISMIR), Utrecht, The Netherlands, 619-624.

[3] Kermanidis, K. et al. (2014). Combining Language Modeling and LSA on Greek Song "Words" for Mood Classification. International Journal on Artificial Intelligence Tools, 23(2).

[3] Çano, E. & Morisio, M. (2017). MoodyLyrics: A Sentiment Annotated Lyrics Dataset. In Proceeedings of the International Conference on Intelligent Systems, Metaheuristics and Swarm Intelligence (ISMI), 118-124.

[4] Delbouys, R., et al. (2018). Music Mood Detection Based on Audio and Lyrics with Deep Neural Net. In Proceedings of the 19th International Society for Music Information Retrieval Conference (ISMIR). Paris, France.

[5] Malheiro, R., et al. (2018). Emotionally-Relevant Features for Classification and Regression of Music Lyrics. IEEE Transactions on Affective Computing, 9(2). 

##### Annotation gathering

[1] Aljanaki, A., Wiering, F., & Veltkamp, R. C. (2015). Studying emotion induced by music through a crowdsourcing game. Information Processing and Management, 52, 115–128. 

[2] Çano, E. (2017). Crowdsourcing emotions in music domain. International Journal of Artificial Intelligence and Applications, 8(4), 24-40. 

[3] Gómez-Cañón, J.S., et al. (2020). Joyful for you and tender for us: the influence of individual characteristics on emotion labeling and classification. In Proceedings of the 21st International Society for Music Information Retrieval Conference (ISMIR). Montréal, Canada (virtual).

[4] Gómez-Cañón, J.S., et al. (2020). Improving emotion annotation of music using citizen science. In Proceedings of the 16th International Conference on Music Perception and Cognition (ICMPC/ESCOM). Sheffield, United Kingdom (virtual). 

[5] Gutiérrez-Páez, N., et al. (2021). Emotion annotation of music: a citizen science approach. In Proceedings of the 27th International Conference on Collaboration Technologies and Social Computing (CollabTech). Trier, Germany (virtual). 

##### Context-sensitive models

[1] Jackson, J. C., et al. (2019). Emotion semantics show both cultural variation and universal structure. Science, 366(6472), 1517–1522. 

[2] Hu, X., & Yang, Y.-H. (2017). The Mood of Chinese Pop Music: Representation and Recognition. Journal of the American Society for Information Science and Technology, 68(8), pp. 1899–1910. 

[] Patra, B.G., et al. (2018). Multimodal mood classification of Hindi and Western songs. Journal of Intelligent Information Systems, 51, 579-596. 

[3] Fan, J., et al. (2020). A Comparative Study of Western and Chinese Classical Music based on Soundscape Models. In Proceedings of the 45th International Conference on Acoustics, Speech, and Signal Processing (ICASSP), Barcelona, Spain.

[4] Gómez-Cañón, J.S., et al. (2020). Transfer learning from speech to music: towards language-sensitive emotion recognition models. In Proceedings of the 28th European Signal Processing Conference (EUSIPCO). Amsterdam, The Netherlands (virtual)

[5] Gómez-Cañón, J.S., et al. (2021). Language-sensitive Music Emotion Recognition models: are we really there yet? In Proceedings of the 46th IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP). Toronto, Canada (virtual).

##### Personalized models

[1] Yang, Y.-H., et al. (2007). Music Emotion Recognition: The Role of Individuality. Proceedings of the International Workshop on Human-Centered Multimedia, pp. 13–22. 

[2] Yang, Y.-H. & Liu, J.-Y. (2013). Quantitative Study of Music Listening Behavior in a Social and Affective Context. IEEE Transactions on Multimedia (TMM), 15(6), pp. 1304-1315.

[3] Yang, Y.-H. & Liu, J.-Y. (2015). Quantitative Study of Music Listening Behavior in a Smartphone Context. ACM Transactions on Interactive Intelligent Systems (TiiS). 5(3).

[4] Wang, J.C., et al. (2017). Affective Music Informaion Retrieval. In: Tkalčič M., et al. (eds) Emotions and Personality in Personalized Services. Human–Computer Interaction Series. Springer.

[5] Gómez-Cañón, J.S., et al. (2021). Let’s agree to disagree: consensus entropy active learning for personalized music emotion recognition. In Proceedings of the 22nd International Society for Music Information Retrieval Conference (ISMIR). Virtual. 

#### Books
[1] Meyer, L. B. (1961). Emotion and Meaning. University of Chicago Press.

[2] Budd, M. (1992). Music and the Emotion. Routledge.

[3] Picard, R.W. (1997). Affective Computing. MIT Press.

[3] Huron, D. (2006). Sweet Anticipation. MIT Press.

[4] Patel, A. D. (2008). Music, Language and the Brain. Oxford University Press.

[5] Juslin, P. & Sloboda, J. (2010). Handook of Music and Emotion: Theory, Research, Applications. Oxford University Press. 

[6] Krippendorff, K. H. (2004). Content Analysis: An Introduction to Its Methodology. SAGE Publications.

[7] Grekow, J. (2018). From Content-based Music Emotion Recognition to Emotion Maps of Musical Pieces. Springer Nature. 



#### PhD Dissertations
[1] Coutinho, E. (2008). Computational and Psycho-Physiological Investigations of Musical Emotions. University of Plymouth.

[2] Hu, X. (2010). Improving music mood classification using lyrics, audio and social tags. University of Illinois.

[3] Yang, Y.-H. (2010). Dimensional Music Emotion Recognition for Content Retrieval. National Tsing Hua University. 

[4] Laurier, C. (2011). Automatic Classification of Musical Mood by Content-Based Analysis. Universitat Pompeu Fabra. 

[5] Vuoskoski, J.K. (2012). Emotions represented and induced by music: the role of individual differences. University of Jyväskylä.

[6] Schmidt, E. (2012). Modeling and Predicting Emotion in Music. Drexel University. 

[7] Aljanaki, A. (2016). Emotion in Music: representation and computational modeling. Universiteit Utrecht.

[8] da Silva Mahleiro, R. M. (2016). Emotion-based Analysis and Classification of Music Lyrics. Universidade de Coimbra.

[9] Song, Y. (2016). The Role of Emotion and Context in Musical Preference. Queen Mary University of London.

[10] Malheiro, R. (2016). Emotion-based analysis and classification of music lyrics. Universidade de Coimbra.

[11] Barradas, G. T. (2017). A Cross-Cultural Approach to Psychological Mechanisms Underlying Emotional Reactions to Music. Uppsala Universitet.

[12] Çano, E. (2018). Text-based Sentiment Analysis and Music Emotion Recognition. Politecnico di Torino. 

[13] Panda, R. (2019). Emotion-based Analysis and Classification of Audio Music Emotion. Universidade de Coimbra.

[14] Fan, J. (2020). Advances in Soundscape and Music Emotion Recognition. Simon Fraser University.

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
