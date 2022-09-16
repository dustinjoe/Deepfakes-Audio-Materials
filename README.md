# Selected-Deepfakes-Audio-Materials [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated, but probably biased and incomplete, list of awesome Deepfakes resources specially selected for audios.

This collection is enlightened by the work of a general deepfake material collection from (https://github.com/datamllab/awesome-deepfakes-materials).
As both deep learning and deepfakes are evolving fast these days, feel like it would be somehow helpful to create a separate repo here to collect materials on Deepfake audios.
If you want to contribute to this list, feel free to pull a request. 


## What is Deepfakes?

In December 2017, a user with name “DeepFakes” posted realistic looking videos of famous celebrities on Reddit. These fake videos are generated using deep learning, by swapping faces of original adult movies with celebrities’ faces. Since then, the topic of DeepFakes goes viral on internet.

Here, we denote DeepFakes as any fake contents generated by deep learning techniques. DeepFakes comes in different forms, perhaps the most typical ones are: 1) Videos and images, 2) Texts, and 3) Voices. Different deep learning techniques are used to generate DeepFakes. For instance, videos and images are usually created by Generative adversarial networks (GAN), while texts are mostly generated by deep language models based on Transformers.

It is worth pointing out the first type of videos and images are most well known deepfakes. This is relevant to the current high spread speed of videos and images on social media and multimedia websites like Youtube. 

## Table of Contents

* [Introduction](#introduction)
  * [Key Concepts](#generation-papers)
  * [General Architecture](#generation-codes)
  * [General Online Articles of Deepfakes](#general-online-articles-of-deepfakes)
* [Attack Generation](#attack-generation)
  * [Fake Audio Generation](#fake-audio-generation)
  * [Relevant Tools](#relevant-tools)
* [Defense](#defense)
  * [Deepfake Detection](#deepfake-detection)
  * [Attacking Deepfake Generator](#attacking-deepfake-generator)
* [Datasets and Challenges](#datasets-and-challenges)
* [Social Impacts](#social-impacts)
  * [Government Responses](#government-responses)
  * [Potential Threatened Scenarios](#potential-threatened-scenarios)
  


### Introduction


 

### Detection Papers

* Review and General Papers
  * [Deep Learning for Deepfakes Creation and Detection](https://arxiv.org/abs/1909.11573)
  * [DeepFakes and Beyond: A Survey of Face Manipulation and Fake Detection](https://arxiv.org/abs/2001.00179)
  * [Media Forensics and DeepFakes: an overview](https://arxiv.org/abs/2001.06564)
  * [Will Deepfakes Do Deep Damage?](https://cacm.acm.org/magazines/2020/1/241708-will-deepfakes-do-deep-damage/fulltext)


* Relying on Artifacts
  * [Exposing DeepFake Videos By Detecting Face Warping Artifacts](https://arxiv.org/abs/1811.00656)
  * [Exposing Deep Fakes Using Inconsistent Head Poses](https://arxiv.org/abs/1811.00661)
  * [In Ictu Oculi: Exposing AI Generated Fake Face Videos by Detecting Eye Blinking](https://arxiv.org/abs/1806.02877)
  * [Exploiting Visual Artifacts to Expose Deepfakes and Face Manipulations](https://ieeexplore.ieee.org/document/8638330)
  * [Protecting World Leaders Against Deep Fakes](http://openaccess.thecvf.com/content_CVPRW_2019/papers/Media%20Forensics/Agarwal_Protecting_World_Leaders_Against_Deep_Fakes_CVPRW_2019_paper.pdf)

* Binary Classifiers
  * [Capsule-Forensics: Using Capsule Networks to Detect Forged Images and Videos](https://arxiv.org/abs/1810.11215)
  * [FaceForensics++: Learning to Detect Manipulated Facial Images](https://arxiv.org/abs/1901.08971)
  * [Deepfake Video Detection Using Recurrent Neural Networks](https://engineering.purdue.edu/~dgueraco/content/deepfake.pdf)

* Generalization performance
  * [Towards Generalizable Forgery Detection with Locality-aware AutoEncoder](https://arxiv.org/abs/1909.05999)
  * [ForensicTransfer: Weakly-supervised Domain Adaptation for Forgery Detection](https://arxiv.org/abs/1812.02510)
  * [Face X-ray for More General Face Forgery Detection](https://arxiv.org/abs/1912.13458)
  * [On the generalization of GAN image forensics](https://arxiv.org/abs/1902.11153)
  * [Fake Face Detection Methods: Can They Be Generalized?](https://ieeexplore.ieee.org/document/8553251)


### Detection Codes
* [Deepfake detection for the masses](https://github.com/Baukebrenninkmeijer/FakeFynder-Hackathon-for-Good-2019)
* [Exposing DeepFake Videos By Detecting Face Warping Artifacts](https://github.com/danmohaha/CVPRW2019_Face_Artifacts)
* [Vulnerability assessment and detection of Deepfake videos](https://gitlab.idiap.ch/bob/bob.report.deepfakes)


### Datasets and Challenges

* [FaceForensics++](https://github.com/ondyari/FaceForensics)
* [Celeb-DF](http://www.cs.albany.edu/~lsw/celeb-deepfakeforensics.html)
* [Deepfakes detection challenge by Facebook, Microsoft, etc.](https://ai.facebook.com/blog/deepfake-detection-challenge?from=timeline&isappinstalled=0)
* [DeepfakeTIMIT](https://www.idiap.ch/dataset/deepfaketimit)
* [Kaggle Deepfake Detection Challenge](https://www.kaggle.com/c/deepfake-detection-challenge/overview?utm_medium=email&utm_source=intercom&utm_campaign=deepfake-competition-2019)




### General Online Articles of Deepfakes

* [Deepfake: The Good, The Bad and the Ugly - Medium](https://medium.com/twentybn/deepfake-the-good-the-bad-and-the-ugly-8b261ecf0f52)
* [DeepFakes: AI-powered deception machines](http://www.computervisionblog.com/2018/05/deepfakes-ai-powered-deception-machines.html)
* [Exploring DeepFakes - KDnuggets](https://www.kdnuggets.com/2018/03/exploring-deepfakes.html)
* [Family fun with deepfakes. Or how I got my wife onto the Tonight Show - Towards Data Science](https://towardsdatascience.com/family-fun-with-deepfakes-or-how-i-got-my-wife-onto-the-tonight-show-a4454775c011)
* [Deepfake propaganda is not a real problem - The Verge](https://www.theverge.com/2019/3/5/18251736/deepfake-propaganda-misinformation-troll-video-hoax)








## Deepfake Voices

### Papers Mainly on Generation
* [Tacotron: Towards End-to-End Speech Synthesis](https://arxiv.org/abs/1703.10135)
* [Neural Voice Cloning with a Few Samples](https://arxiv.org/abs/1802.06006)
* [Deep Voice 3: Scaling Text-to-Speech with Convolutional Sequence Learning](https://arxiv.org/abs/1710.07654)
* [Deep Voice 3: Efficiently Trainable Text-to-Speech System Based on Deep Convolutional Networks with Guided Attention](https://arxiv.org/abs/1710.08969)


### Codes Mainly on Generation
* [deep-voice-conversion](https://github.com/andabi/deep-voice-conversion)
* [Tacotron](https://github.com/keithito/tacotron)
* [mimic2](https://github.com/MycroftAI/mimic2)
* [Neural Voice Cloning with Few Samples](https://github.com/Sharad24/Neural-Voice-Cloning-with-Few-Samples)
* [Deepvoice3_pytorch](https://github.com/r9y9/deepvoice3_pytorch)
* [Real-Time Voice Cloning](https://github.com/CorentinJ/Real-Time-Voice-Cloning)
* [DeepFake Audio Detection](https://github.com/dessa-public/fake-voice-detection)



### General Online Articles of Deepfake Voices
* [You can now speak using someone else’s voice with Deep Learning](https://towardsdatascience.com/you-can-now-speak-using-someone-elses-voice-with-deep-learning-8be24368fa2b)
* [A Voice Deepfake Was Used To Scam A CEO Out Of $243,000](https://www.forbes.com/sites/jessedamiani/2019/09/03/a-voice-deepfake-was-used-to-scam-a-ceo-out-of-243000/)
