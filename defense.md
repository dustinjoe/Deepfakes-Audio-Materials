### Datasets and Challenges

* ASVProof Challenge (https://www.asvspoof.org/)  ASVProof Challenge: a contest for fake audo-based attack detection that has been held for several times since 2015. It defines three types of audio attacks including deepfake audios. 
* ICASSP ADD 2022 (https://arxiv.org/abs/2202.08433) ICASSP ADD 2022: the first audio deep synthesis detection challenge(madarin language dataset)
* Voice Privacy Challenge (https://www.voiceprivacychallenge.org) \
VoicePrivacy: develop anonymisation and pseudonymisation solutions which suppress personally identifiable information while preserving linguistic content and speech quality/naturalness. It is worth pointing out, privacy is a very widespread concept. According to the [VoicePrivacy2020 Summary Report](https://arxiv.org/abs/2109.00648), this could include e.g., age, gender, ethnic origin, geographical background, health or emotional state, political orientations, and religious beliefs. Speaker recognition systems can also reveal the speaker’s identity. So we can say DeepFake audios can be regarded as kind of voice privacy leakage. 
* Kaggle Deepfake Detection Challenge (https://www.kaggle.com/c/deepfake-detection-challenge/overview?utm_medium=email&utm_source=intercom&utm_campaign=deepfake-competition-2019)  this contest was conducted in 2019, it is mainly focused on deepfake video detection, however, its dataset includes some modified audio parts
* CSIG Contest(http://fmfcc.net/#introduction)  Chinese audio deepfake contest. They provide a reference list of tools they use for dataset generation: http://fmfcc.net/contest-introduction
* Fake-or-Real(FOR) Dataset (https://bil.eecs.yorku.ca/datasets/#:~:text=The%20Fake%2Dor%2DReal%20(,classifiers%20to%20detect%20synthetic%20speech.)



### Audio Deepfake Defense Review
#### Review and General Papers:  
* ASVspoof 2021: Towards Spoofed and Deepfake Speech Detection in the Wild 
\[[Paper](https://arxiv.org/pdf/2210.02437.pdf)\] \
A summary of the ASVspoof 2021 challenge and the results of 37 participating teams. For the logical access task, results indicate that countermeasures solutions are robust to newly introduced encoding and transmission effects. Results for the physical access task indicate the potential to detect replay attacks in real, as opposed to simulated physical spaces, but a lack of robustness to variations between simulated and real acoustic environments.The
DF task, new to the 2021 edition, targets solutions to the detection of manipulated, compressed speech data posted online. While detection solutions offer some resilience to compression effects, they lack generalization across different source datasets.
* Tutorials/Papers from  NII Yamagishi Lab team. (https://nii-yamagishilab.github.io/, http://tonywangx.github.io/slide.html)

#### Human vs AI
* Human Perception of Audio Deepfakes
\[[Paper](https://arxiv.org/abs/2107.09667)\]
\[[TestSite](https://deepfake-demo.aisec.fraunhofer.de/)\] \
Humans and deepfake detection algorithms share similar strengths and weaknesses, both struggling to detect certain types of attacks. This is in contrast to the superhuman performance of AI in many application areas such as object detection or face recognition. Concerning human success factors, we find that IT professionals have no advantage over non-professionals but native speakers have an advantage over non-native speakers. Additionally, we find that older participants tend to be more susceptible than younger ones. 

#### Detector Design:   
* FastAudio: A Learnable Audio Front-End for Spoof Speech Detection. 
\[[Paper](https://arxiv.org/pdf/2109.02774v1.pdf)\]
\[[Code](https://github.com/magnumresearchgroup/Fastaudio)\]
* Complementing Handcrafted Features with Raw Waveform Using a Light-weight Auxiliary Model. 
\[[Paper](https://arxiv.org/abs/2109.02773)\]
\[[Code](https://github.com/magnumresearchgroup/AuxiliaryRawNet)\]

* Does Audio Deepfake Detection Generalize?
\[[Paper](https://arxiv.org/pdf/2203.16263.pdf)\]
\[[Demo](https://deepfake-demo.aisec.fraunhofer.de/in_the_wild)\]


#### Important Trends: 
* An Initial Investigation for Detecting Partially Spoofed Audio. 
\[[Paper](https://www.isca-speech.org/archive/interspeech_2021/zhang21ca_interspeech.html)\]
* The Attacker’s Perspective on Automatic Speaker Verification: An Overview
\[[Paper](https://arxiv.org/pdf/2004.08849.pdf)\] \
Adversarial machine learning can potentially help to identify the weakest parts of ASV systems and be used to develop attackeraware systems. This paper serves as an overview on this emerging research area by focusing on potential threats of adversarial attacks on ASV, spoofing countermeasures, or both.

### Defensive Audio Processing
#### Attacking Deepfake Generator:  
* Defending Against Deepfakes Using Adversarial Attacks on Conditional Image Translation Networks.   \
This paper is only put here to show this kind of idea, there does not seem to exist similar work on audio this way. 
\[[Paper](https://arxiv.org/abs/2003.01279)\]
\[[Code](https://github.com/natanielruiz/disrupting-deepfakes)\]

#### Anomynization:  
Voice anomynization is catering to the contest of newly organized Voice Privacy Challenge (https://www.voiceprivacychallenge.org).
* Language-Independent Speaker Anonymization Approach using Self-Supervised Pre-Trained Models. 
\[[Paper](https://arxiv.org/abs/2202.13097)\]
\[[Code](https://github.com/nii-yamagishilab/SSL-SAS)\]





