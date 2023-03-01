### Datasets and Challenges

* ASVProof Challenge (https://www.asvspoof.org/)  ASVProof Challenge: a contest for fake audo-based attack detection that has been held for several times since 2015. It defines three types of audio attacks including deepfake audios. 
* SASV Challenge (https://sasv-challenge.github.io/) ASV (automatic speaker verification) systems are intrinsically required to reject both non-target (e.g., voice uttered by different speaker) and spoofed (e.g., synthesised or converted) inputs. However, there is little consideration for how ASV systems themselves should be adapted when they are expected to encounter spoofing attacks, nor when they operate in tandem with CMs (spoofing countermeasures), much less how both systems should be jointly optimised. The goal of the first SASV (spoofing-aware speaker verification) challenge is to promote development of integrated systems that can perform ASV and CM simultaneously.
* ICASSP ADD 2022 (https://arxiv.org/abs/2202.08433) ICASSP ADD 2022: the first audio deep synthesis detection challenge(madarin language dataset)
* Voice Privacy Challenge (https://www.voiceprivacychallenge.org) \
VoicePrivacy: develop anonymisation and pseudonymisation solutions which suppress personally identifiable information while preserving linguistic content and speech quality/naturalness. It is worth pointing out, privacy is a very widespread concept. According to the [VoicePrivacy2020 Summary Report](https://arxiv.org/abs/2109.00648), this could include e.g., age, gender, ethnic origin, geographical background, health or emotional state, political orientations, and religious beliefs. Speaker recognition systems can also reveal the speaker’s identity. So we can say DeepFake audios can be regarded as kind of voice privacy leakage. 
* Kaggle Deepfake Detection Challenge (https://www.kaggle.com/c/deepfake-detection-challenge/overview?utm_medium=email&utm_source=intercom&utm_campaign=deepfake-competition-2019)  this contest was conducted in 2019, it is mainly focused on deepfake video detection, however, its dataset includes some modified audio parts
* CSIG Contest(http://fmfcc.net/#introduction)  Chinese audio deepfake contest. They provide a reference list of tools they use for dataset generation: http://fmfcc.net/contest-introduction
* Fake-or-Real(FOR) Dataset (https://bil.eecs.yorku.ca/datasets/#:~:text=The%20Fake%2Dor%2DReal%20(,classifiers%20to%20detect%20synthetic%20speech.)



### Audio Deepfake Defense 
#### Review and General Papers:  
* ASVspoof 2021: Towards Spoofed and Deepfake Speech Detection in the Wild 
\[[Paper](https://arxiv.org/pdf/2210.02437.pdf)\] \
A summary of the ASVspoof 2021 challenge and the results of 37 participating teams. For the logical access task, results indicate that countermeasures solutions are robust to newly introduced encoding and transmission effects. Results for the physical access task indicate the potential to detect replay attacks in real, as opposed to simulated physical spaces, but a lack of robustness to variations between simulated and real acoustic environments.The
DF task, new to the 2021 edition, targets solutions to the detection of manipulated, compressed speech data posted online. While detection solutions offer some resilience to compression effects, they lack generalization across different source datasets.
* A Practical Guide to Logical Access Voice Presentation Attack Detection
\[[Paper](https://arxiv.org/pdf/2201.03321.pdf)\] \
It introduces the basic concept of voice PAD, explains the common techniques, and provides an experimental study using recent methods on a benchmark dataset. This is a comprehensive review paper on fake audio detection topic. It provoides a systematic comparison of methods in the past 10 years and how these methods are evolving. This paper also discussed some background knowledge so it can serve as a tutorial on this topic.
* Tutorials/Papers from  NII Yamagishi Lab team. (https://nii-yamagishilab.github.io/, http://tonywangx.github.io/slide.html)

#### Human vs AI
* Human Perception of Audio Deepfakes
\[[Paper](https://arxiv.org/abs/2107.09667)\]
\[[TestSite](https://deepfake-demo.aisec.fraunhofer.de/)\] \
Humans and deepfake detection algorithms share similar strengths and weaknesses, both struggling to detect certain types of attacks. This is in contrast to the superhuman performance of AI in many application areas such as object detection or face recognition. Concerning human success factors, we find that IT professionals have no advantage over non-professionals but native speakers have an advantage over non-native speakers. Additionally, we find that older participants tend to be more susceptible than younger ones. 
* Warning: Humans Cannot Reliably Detect Speech Deepfakes
\[[Paper](https://arxiv.org/pdf/2301.07829)\]
This paper presented genuine and deepfake audio to n = 529 individuals and asked them to identify the deepfakes. Experiments are run in English and Mandarin to understand if language affects detection performance and decision-making rationale. Detection capability is unreliable. Listeners only correctly spotted the deepfakes 73% of the time, and there was no
difference in detectability between the two languages. Increasing listener awareness by providing examples of speech deepfakes only improves results slightly. The difficulty of detecting speech deepfakes confirms their potential for misuse and signals that defenses against this threat are needed.


#### Fake Audio Detection
bona fide vs spoofed
##### Detector Design:   
* STC Antispoofing Systems for the ASVspoof2019 Challenge
\[[Paper](https://arxiv.org/pdf/1904.05576.pdf)\]
\[[Code](https://github.com/ozora-ogino/LCNN)\] \
This work reports the application of LightCNN architecture for general ASVSpoof 19 LA section. It is a continuing work of their LightCNN work on PA section in the previous ASVSpoof 17 contest in the paper, Audio replay attack detection with deep learning frameworks \[[Paper](https://www.researchgate.net/profile/Galina-Lavrentyeva/publication/319185301_Audio_Replay_Attack_Detection_with_Deep_Learning_Frameworks/links/59bf9e1fa6fdcca8e56fa179/Audio-Replay-Attack-Detection-with-Deep-Learning-Frameworks.pdf)\]. This should be a milestone of deep learning usage for antispoofing in audio area.
* END-TO-END ANTI-SPOOFING WITH RAWNET2
\[[Paper](https://arxiv.org/pdf/2011.01108.pdf)\]
\[[Code](https://github.com/eurecom-asp/rawnet2-antispoofing)\] \
This work reports the first application of RawNet2 to anti-spoofing. RawNet2 ingests raw audio and has potential to learn cues that are not detectable using more traditional countermeasure solutions.
* FastAudio: A Learnable Audio Front-End for Spoof Speech Detection. 
\[[Paper](https://arxiv.org/pdf/2109.02774v1.pdf)\]
\[[Code](https://github.com/magnumresearchgroup/Fastaudio)\]
* Complementing Handcrafted Features with Raw Waveform Using a Light-weight Auxiliary Model. 
\[[Paper](https://arxiv.org/abs/2109.02773)\]
\[[Code](https://github.com/magnumresearchgroup/AuxiliaryRawNet)\] \
This work proposes an Auxiliary Rawnet model to complement handcrafted features with features learned from raw waveforms. The combination of rawnet encoder and the classifical DSP based encoder makes the overall model trainable front end and good performance on ASVSpoof19 LA data.

##### Potential Issues
* Does Audio Deepfake Detection Generalize?
\[[Paper](https://arxiv.org/pdf/2203.16263.pdf)\]
\[[Demo](https://deepfake-demo.aisec.fraunhofer.de/in_the_wild)\]\
The authors systematize audio spoofing detection by re-implementing and uniformly evaluating twelve architectures from related work. The authors find out past work can perform poorly on more real-world data (performance degradation of up to one thousand percent). This could suggest that the community has tailored its solutions too closely to the prevailing ASVspoof benchmark and that deepfakes are much harder to detect outside the lab than previously thought.
* Speech is Silver, Silence is Golden: What do ASVspoof-trained Models Really Learn? 
\[[Paper](https://arxiv.org/pdf/2106.12914.pdf)\] \
This work presents analysis of a significant data artifact in the official 2019/2021 ASVspoof Challenge Dataset. The authors identify an uneven distribution of silence duration in the training and test splits, which tends to correlate with the target prediction label. Bonafide instances tend to have significantly longer leading and trailing silences than spoofed instances. 

##### Important Trends: 
* An Initial Investigation for Detecting Partially Spoofed Audio. 
\[[Paper](https://www.isca-speech.org/archive/interspeech_2021/zhang21ca_interspeech.html)\]\
ADD 2022 is the first challenge to propose the partially fake audio detection task. Such brand new attacks are dangerous and how to tackle such attacks remains an open question.  This paper shows previous detectors no longer work well under this new attack setting.
* The Attacker’s Perspective on Automatic Speaker Verification: An Overview
\[[Paper](https://arxiv.org/pdf/2004.08849.pdf)\] \
Adversarial machine learning can potentially help to identify the weakest parts of ASV systems and be used to develop attackeraware systems. This paper serves as an overview on this emerging research area by focusing on potential threats of adversarial attacks on ASV, spoofing countermeasures, or both.
Although AML on audio tasks has been under research for several years, it has just been added to ASVSpoof in 2023.
* Characterizing the Fusion Strategies for Spoofing-Aware Speaker Verification
\[[Paper](https://sasv-challenge.github.io/pdfs/2022_descriptions/CUHK-NTU.pdf)\] \
Propose a novel multi-model and multi-level fusion strategy to tackle the SASV task from SASV 2022 Challenge mentioned above. Compared with purely scoring fusion and embedding fusion methods, this framework first utilizes embeddings from CM models, propagating CM embeddings into a CM block to obtain a CM score. In the second-level fusion, CM score and ASV scores directly from ASV systems will be concatenated into a prediction block for the final decision. A similar work is, SA-SASV: An End-to-End Spoof-Aggregated Spoofing-Aware Speaker Verification System (https://arxiv.org/pdf/2203.06517.pdf). Also this one, A Probabilistic Fusion Framework for Spoofing Aware Speaker Verification (https://arxiv.org/pdf/2202.05253.pdf).
* The DKU-OPPO System for the 2022 Spoofing-Aware Speaker Verification Challenge
\[[Paper](https://arxiv.org/pdf/2207.07510.pdf)\] \
This is the 2nd place winner for the 2022 SASV Challenge. They show their solution in the paper above. The first place winner is IDVoice from a company solution from IDR&D (https://www.idrnd.ai/idvoice-verified-voice-biometrics-and-anti-spoofing/). So this should be the paper for the highest ranking solution for this problem setting with exposed information.
* Investigating self-supervised front ends for speech spoofing countermeasures
\[[Paper](https://arxiv.org/pdf/2111.07725.pdf)\]
\[[Code](https://github.com/nii-yamagishilab/project-NN-Pytorch-scripts)\]
\[[Video](https://www.youtube.com/watch?v=X4XxddA10xo)\] \
Use of self-supervised models as the front end of speech spoofing CMs. Through experiments on benchmark datasets, we observed that a self-supervised front end pre-trained using diverse speech data performed quite well when it is fixed and combined with a conventional LCNNLSTM back end. More notable improvement is achieved when the front end is fine-tuned for the anti-spoofing task. This work aims to prove the generlization of detections across data.

#### Defensive Audio Processing
##### Attacking Deepfake Generator:  
* Defending Against Deepfakes Using Adversarial Attacks on Conditional Image Translation Networks.   \
This paper is only put here to show this kind of idea, there does not seem to exist similar work on audio this way. 
\[[Paper](https://arxiv.org/abs/2003.01279)\]
\[[Code](https://github.com/natanielruiz/disrupting-deepfakes)\]

##### Anomynization:  
Voice anomynization is catering to the contest of newly organized Voice Privacy Challenge (https://www.voiceprivacychallenge.org).
* Language-Independent Speaker Anonymization Approach using Self-Supervised Pre-Trained Models. 
\[[Paper](https://arxiv.org/abs/2202.13097)\]
\[[Code](https://github.com/nii-yamagishilab/SSL-SAS)\]





