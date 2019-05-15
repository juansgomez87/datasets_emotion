# MER and SER Data sets

## Summary
### Music Emotion Recognition Data sets
| Dataset | Year | Content | Format | Size | Annotation Type |
|:-------:|:----:|:-------:|:------:|:----:|:---------------:|
|4Q audio emotion|2018|900 excerpts (30s long)|MP3|291MB|Categorical (Quadrants)|
|DEAM/Mediaeval|2018|2058 excerpts (45s long)|MP3|1.4GB|Dimensional (Time-continuous A-V)|
|Soundtracks|2011|360+110 exceprts (15s-1m long)|MP3|216MB|Categorical (tension, anger, fear, happy, sad, tender) and Dimensional (valence, energy, tension)|
|MoodsMIREX|2008|269 excerpts (30s long)|MP3|736MB|Categorical (5 mood clusters)|Yes|
|NTWICM|2010|2648 full songs|MP3|11.7GB|"Discrete" Dimensional|
|CH818|2017|818 excerpts (30s long)|MP3|393MB|Dimensional|

### Speech Emotion Recognition Data sets
| Dataset | Year | Content | Format | Size | Annotation Type | Language |
|:-------:|:----:|:-------:|:------:|:----:|:---------------:|:--------:|
|RECOLA/AVEC2015|2013|9.5 hours of multimodal recordings|WAV,MP4,CSV|3.6GB|Dimensional (Time-continuous A-V)|French|
|SEMAINE-SolidSAL|2012|7.5 hours of speech recordings|WAV,AVI|38.7GB|Dimensional (Time-continuous A-V)|English|
|SEWA|2019|44 hours of multimodal recordings| ? | ? |Dimensional (Time-continuous A-V)|British, German, Hungarian, Greek, Serbian, and Mandarin|
|MMDBESP|2019|xx hours of video recordings|MP4|10.6GB|Categorical (Fear, Surprise, Anger, Sadness, Happiness, Disgust)|Polish|

## Additional information
### Music Emotion Recognition Data sets
#### 4Q Emotion Dataset
* Author: Panda R., Malheiro R., Paiva R. P.
* Description and music styles: Mostly popularly consumed 
* Annotation strategy: Collected from AllMusic API, emotion tags are selected from the original AllMusic Tags by intersecting them with the Warriner’s list. Finally, a manual blind validation is conducted by subjects.
* Paper: *Panda R., Malheiro R., Paiva R. P. (2018). “Musical Texture and Expressivity Features for Music Emotion Recognition”. 19th International Society for Music Information Retrieval Conference – ISMIR 2018, Paris, France.*
* Annotation (categorical): Q1 (A+V+), Q2 (A+V-), Q3(A-V-), Q4 (A-V+)
* Link: http://mir.dei.uc.pt/downloads.html 
* *Languages: English: 724, Spanish: 24, French: 0, German: 0, Other: 16, Unknown: 136, Total (from Metadata): 899*

#### DEAM: MediaEval Database for Emotional Analysis in Music
* Author: Soleymani, M., Aljanaki, A., Yang, Y.
* Description and music styles: Royalty-free music from several sources: freemusicarchive.org (FMA), jamendo.com,
and the medleyDB datase. The excerpts which were annotated are available in the same package song ids between 1 and 2058. The dataset consists of 2014 development set (744 songs), 2014 evaluation set (1000 songs) and 2015 evaluation set (58 songs). Includes rock, pop, soul, blues, electronic, classical, hip-hop, international, experimental, folk, jazz, country and pop genres.
* Annotation strategy: Crowdsourced MTurk with each excerpt annotated at least by 10 workers. Both arousal and valence were annotated separately. Additional static annotations were collected for the whole 45 second exceprts after dynamic annotations. 
* Paper: *Aljanaki A., Yang Y., Soleymani M. (2017) Developing a benchmark for emotional analysis of music. PLoS ONE 12(3): e0173392. https://doi.org/10.1371/journal.pone.0173392*
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: http://cvml.unige.ch/databases/DEAM/
* *Languages: English: 1531, Spanish: 13, French: 0, German: 0, Other: 47, Unknown 211, Total (from Metadata): 1801*

#### Soundtracks
* Author: Eerola, T. & Vuoskoski, J. K.
* Description and music styles: This dataset we refer to as "Film soundtracks" are designed to overcome at least some of the problems mentioned above since they contain not that well known examples (although some could be identified by film aficionados).
* Annotation strategy: The selection of the excerpts has been done in terms of dimensional and discrete emotion model and evaluated by a pilot study. The initial ratings were made by 12 expert musicologists for both dimensional and discrete models. These ratings were then re-tested with 116 university students.
* Paper: *Eerola, T. & Vuoskoski, J. K. (2011). A comparison of the discrete and dimensional models of emotion in music. Psychology of Music, 39(1), 18-49. https://doi.org/10.1177/0305735610362821*
* Annotation: categorical and dimensional
* Link: https://osf.io/p6vkg/
* *Languages: None (instrumental)*

#### Moods MIREX
* Author: Hu, X., Downie, J.S., Laurier, C., Bay, M., Ehmann, A.F.
* Description and music styles: Selection of the libraries of Associated Production Music (APM), “the world’s leading production music library… offering every imaginable music genre from beautiful classical music recordings to vintage rock to current indie band sounds".
* Annotation strategy: The pieces were rated by 3 raters, and only a subset of agreement by 2 out of 3 is extracted. 
* Paper: *Downie, X. H. J. S., Cyril Laurier, and M. B. A. F. Ehmann. “The 2007 MIREX audio mood classification task: Lessons learned.” Proceeding of the 9th International Conference of Music Information Retrieval (ISMIR). 2008.*
* Annotation (categorical): Cluster 1 (passionate, rousing, confident, boisterous, rowdy), Cluster 2 (rollicking, cheerful, fun, sweet, amiable/good natured), Cluster 3 (literate, poignant, wistful, bittersweet, autumnal, brooding), Cluster 4 (humorous, silly, campy, quirky, whimsical, witty, wry), Cluster 5 (aggressive, fiery, tense/anxious, intense, volatile, visceral)
* Link: Offline (on MTB-DB)
* *Languages: No metadata*

#### NTWICM: Now That's What I Call Music
* Author: Schuller, B., Dorfner, J., Gerhard, R.
* Description and music styles: For building up a ground truth music database the compilation “Now That’s What I Call Music!” (U. K. series, volumes 1–69, double CDs, each) is selected. It represents very well most music styles which are popular today; that ranges from Pop and Rock music over Rap, R&B to electronic dance music as Techno or House.
* Annotation strategy: 4 raters gave static annotations for complete songs for arousal and valence in a discrete range of [−2,−1, 0, 1, 2]. 
* Paper: *Björn Schuller, Johannes Dorfner, Gerhard Rigoll: "Determination of Non-Prototypical Valence and Arousal in Popular Music: Features and Performances", EURASIP Journal on Audio, Speech, and Music Processing (JASMP), Special Issue on "Scalable Audio-Content Analysis", vol. 2010, Article ID 735854, 19 pages, 2010.*
* Annotation (dimensional): Arousal and valence [−2,−1, 0, 1, 2].
* Link: Offline 
* *Languages: English: 2491, Spanish: 5, French: 0, German: 0, Other: 6, Unknown 146, Total (from Metadata): 2648*

#### CH818
* Author: Hu, X., Yang, Y.
* Description and music styles: Chinese Pop songs released in Taiwan, Hong Kong and Mainland China.
* Annotation strategy: Each clip was annotated by three music experts who were born and raised in Mainland China and thus were with a Chinese cultural background. The annotation was done with an interface consisting of two sliding bars of continuous real values between [-10,10]. 
* Paper: *X. Hu and Y. Yang, "Cross-Dataset and Cross-Cultural Music Mood Prediction: A Case on Western and Chinese Pop Songs" in IEEE Transactions on Affective Computing, vol. 8, no. 02, pp. 228-240, 2017. doi: 10.1109/TAFFC.2016.2523503*
* Annotation (dimensional): Arousal and valence real values between [-10,10] for whole excerpt.
* Link: *NOT AVAILABLE* (made available by Yi-Hsuan Yang).
* *Languages: Mandarin: 818, Total (from Metadata): 818*

### Speech Emotion Recognition Data sets
#### RECOLA
* Author: Ringeval, F., Sonderegger, A., Sauer, J., Lalanne, D.
* Description: Participants were recorded in dyads during a video conference while completing a task requiring collaboration. Different multimodal data, i.e., audio, video, ECG and EDA, were recorded continuously and synchronously.
* Annotation strategy: 6 annotators measured emotion continuously on two dimensions: arousal and valence, as well as social behavior labels on five dimensions. The annotation is made with an open source web-based annotation tool (ANNEMO).
* Paper: *F. Ringeval, A. Sonderegger, J. Sauer and D. Lalanne, "Introducing the RECOLA Multimodal Corpus of Remote Collaborative and Affective Interactions", 2nd International Workshop on Emotion Representation, Analysis and Synthesis in Continuous Time and Space (EmoSPACE), in Proc. of IEEE Face & Gestures 2013, Shanghai (China), April 22-26 2013.*
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: https://diuf.unifr.ch/main/diva/recola/download.html

#### SEMAINE
* Author: McKeown, G., Valstar, M., Cowie, R., Pantic, M., Schroder, M.
* Description: The interactions involve two parties, a “user” (who is always human) and an “operator” (either a machine or a
person simulating a machine). A key objective of the Solid SAL scenario was to record behaviors (mainly nonverbal) that a human operator shows in fluent face-to-face conversation, including their relationships to user behavior—notably  backchanneling, eye contact, various synchronies, and so on.
* Annotation strategy:  For user clips, four sessions have been annotated by eight raters, 17 by 6, and the remainder by
at least three. For operator clips three have been annotated by four raters, the rest by one rater.
* Paper: *McKeown, G., Valstar, M., Cowie, R., Pantic, M., Schroder, M. The SEMAINE Database: Annotated Multi-modal Records of Emotionally Colored Conversations between a Person and a Limited Agent. IEEE Transactions on Affective Computing. 2012; 3:5–17. https://doi.org/10.1109/T-AFFC.2011.20*
* Annotation (dimensional): Time-continuous arousal and valence annotation (1 Hz)
* Link: https://semaine-db.eu/

#### SEWA
* Author: Kossaifi, J., Walecki, R., Panagakis, Y., Shen, J., Schmitt, M., Ringeval, F., Han, J. et al.
* Description: Subjects were recorded in two different contexts: while watching adverts and while discussing adverts in a video chat. The database includes rich annotations of the recordings in terms of facial landmarks, facial action units (FAU), various vocalisations, mirroring, and continuously valued valence, arousal, liking, agreement, and prototypic examples of (dis)liking. 
* Annotation strategy:
* Paper: *Kossaifi, J., Walecki, R., Panagakis, Y., Shen, J., Schmitt, M., Ringeval, F., Han, J. et al. "SEWA DB: A Rich Database for Audio-Visual Emotion and Sentiment Research in the Wild." arXiv preprint arXiv:1901.02839 (2019).*
* Annotation: 538 short (10-30s) video-chat recording segments were manually selected to form the fully-annotated basic SEWA dataset. These segments were selected based on the subjects to the subjects emotional state of low / high valance, low / high arousal, and liking / disliking. All 6 cultures were evenly represented in the basic SEWA dataset, with approximately 90 segments selected from each culture based on the consensus of at least 3 annotators from the same culture.
* Link: https://db.sewaproject.eu/

#### MMDBESP: Multimodal Database of Emotional Speech in Polish
* Author: Sapiński T., Kamińska D., Pelikant A., Ozcinar C., Avots E., Anbarjafari G. 
* Description: Before the recording all actors were presented with a short scenario describing the sequence of emotions they had to present in order: neutral state, sadness, surprise, fear, disgust, anger, happiness. In addition they were asked to utter a short sentence in Polish, same for all emotional states Każdy z nas odczuwa emocje na swój sposób (English translation: Each of us perceives emotions in a different manner). 
* Annotation strategy: Enacted emotions - not ecologically valid. 
* Paper: *Sapiński, T., Kamińska, D., Pelikant, A., Ozcinar, C., Avots, E., Anbarjafari, G. (2019) Multimodal Database of Emotional Speech, Video and Gestures. In: Zhang Z., Suter D., Tian Y., Branzan Albu A., Sidère N., Jair Escalante H. (eds) Pattern Recognition and Information Forensics. ICPR 2018. Lecture Notes in Computer Science, vol 11188*
* Annotation (categorical): Fear, Surprise, Anger, Sadness, Happiness, Disgust - basic emotions. 
* Link: https://competitions.codalab.org/competitions/22249
