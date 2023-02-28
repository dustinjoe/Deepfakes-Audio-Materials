### Deepfake Detection
#### Review and General Papers:  
* Deep Learning for Deepfakes Creation and Detection (https://arxiv.org/abs/1909.11573).   
* DeepFakes and Beyond: A Survey of Face Manipulation and Fake Detection (https://arxiv.org/abs/2001.00179)  
* Media Forensics and DeepFakes: an overview (https://arxiv.org/abs/2001.06564).   
* Will Deepfakes Do Deep Damage? (https://cacm.acm.org/magazines/2020/1/241708-will-deepfakes-do-deep-damage/fulltext). 
* Tutorials/Papers from  NII Yamagishi Lab team. (https://nii-yamagishilab.github.io/, http://tonywangx.github.io/slide.html)

#### Detector Design:   
* FastAudio: A Learnable Audio Front-End for Spoof Speech Detection. 
\[[Paper](https://arxiv.org/pdf/2109.02774v1.pdf)\]
\[[Code](https://github.com/magnumresearchgroup/Fastaudio)\]
* Complementing Handcrafted Features with Raw Waveform Using a Light-weight Auxiliary Model. 
\[[Paper](https://arxiv.org/abs/2109.02773)\]
\[[Code](https://github.com/magnumresearchgroup/AuxiliaryRawNet)\]
* An Initial Investigation for Detecting Partially Spoofed Audio. 
\[[Paper](https://www.isca-speech.org/archive/interspeech_2021/zhang21ca_interspeech.html)\]

### Defensive Audio Processing
#### Attacking Deepfake Generator:  
* Defending Against Deepfakes Using Adversarial Attacks on Conditional Image Translation Networks.    
\[[Paper](https://arxiv.org/abs/2003.01279)\]
\[[Code](https://github.com/natanielruiz/disrupting-deepfakes)\]

#### Anomynization:  
* Language-Independent Speaker Anonymization Approach using Self-Supervised Pre-Trained Models. 
\[[Paper](https://arxiv.org/abs/2202.13097)\]
\[[Code](https://github.com/nii-yamagishilab/SSL-SAS)\]





## Datasets and Challenges

* ASVProof Challenge (https://www.asvspoof.org/)  ASVProof Challenge: a contest for fake audo-based attack detection that has been held for several times since 2015. It defines three types of audio attacks including deepfake audios. 
* ICASSP ADD 2022 (https://arxiv.org/abs/2202.08433) ICASSP ADD 2022: the first audio deep synthesis detection challenge(madarin language dataset)
* Voice Privacy Challenge (https://www.voiceprivacychallenge.org) VoicePrivacy: develop anonymisation and pseudonymisation solutions which suppress personally identifiable information while preserving linguistic content and speech quality/naturalness. It is worth pointing out, privacy is a very widespread concept. According to the [VoicePrivacy2020 Summary Report](https://arxiv.org/abs/2109.00648), this could include e.g., age, gender, ethnic origin, geographical background, health or emotional state, political orientations, and religious beliefs. Speaker recognition systems can also reveal the speaker’s identity. So we can say DeepFake audios can be regarded as kind of voice privacy leakage. 
* Kaggle Deepfake Detection Challenge (https://www.kaggle.com/c/deepfake-detection-challenge/overview?utm_medium=email&utm_source=intercom&utm_campaign=deepfake-competition-2019)  this contest was conducted in 2019, it is mainly focused on deepfake video detection, however, its dataset includes some modified audio parts
* CSIG Contest(http://fmfcc.net/#introduction)  Chinese audio deepfake contest. They provide a reference list of tools they use for dataset generation: http://fmfcc.net/contest-introduction
* Fake-or-Real(FOR) Dataset (https://bil.eecs.yorku.ca/datasets/#:~:text=The%20Fake%2Dor%2DReal%20(,classifiers%20to%20detect%20synthetic%20speech.)
