---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 5th year Ph.D. student in the Electrical and Computer Engineering department of the University of Wisconsin - Madison, advised by Professor [Kassem Fawaz](https://kassemfawaz.com/) at Wi-Pi here. My research interests focus on security in cyber-physical systems and user data privacy in the IoT environment. Previously, I investigated the privacy of mute buttons in video conferencing apps, including Webex, zoom, etc., on various desktop operating systems. Before that, I designed and implemented a pedestrian-to-vehicle authentication system based on pedestrian mobility verification using commercial mobile devices. I also implemented a crowd-sourcing pedestrian data collection framework to collect user walking behavior traces for a long duration from volunteered participants. Currently, I'm working on smartphone-based pedestrian abrupt road-crossing prediction to avoid potential traffic conflict in cellular V2X environments. 

# Research Project
## Harnessing Mobile Ad hoc Network (MANET) to Improve Vulnerable Road User Safety
Our goal is to investigate, implement, and demonstrate a mobile ad hoc network (MANET)-based, practical, infrastructure-free and secure framework that improves the safety of vulnerable road users such as pedestrians and cyclists in the situations when their safety is most threatened, e.g.,non-intersection crossings, lightly-lit areas, evening and late-night situations, and jaywalking.

### Data Collection APP
The first step of the project is building a data collection platform to collect data from the road users. We first developed the flow of the data collection framework. This framework includes an Android app that runs on the client side and a server component that handles the collected data. The app encrypts the collected data on the client-side for privacy protection and automatically uploads to our Amazon "Simple Storage Service" (S3) server for temporary storage. The data is stored in encrypted format on S3 storage and downloaded to our local servers for further processing/analysis after decryption. Automatic labeling of data is performed locally on our server. Processed data will later be used for building prediction model on pedestrian's road crossing behavior.

Please check out my data collection app in [Google Store](https://play.google.com/store/apps/details?id=com.mendhak.gpsloggerfhwa&hl=en). The source code of the data collection app can be found in [Wi-Pi DataCollectionApp Github](https://github.com/wi-pi/FHWA_DataCollectionApp).

### Multi-hop Packet Transmission on Android
I developed an Android App for multi-hop communication between vehicles and pedestrians on road. Multi-hop communication can solve the problem of high communication delay in None-Line-of-Sight scenario and communication beyond range.

Thus I designed and implemented a distance based data forwarding algorithms based on Wi-Fi Aware in commodity Android smartphones. This can extend the range of communication compared to single hop communication and reduce the communication delay caused by network congestion at the same time.
### Vehicle to Pedestrian Authentication
With the absence of a centralized entity managing node identities, a malicious entity can inject fake messages into our framework to impede traffic flows. Thus, our goal is to design an authentication mechanism to verify the source of the message in our MANET-based framework.
We designed and implemented PEDRO, a PEDestRian mObility verification mechanism for pedestrians using commodity hardware, where only legitimate mobile pedestrians can be admitted to the ad hoc network consisting of trustworthy vehicles and pedestrians.

Without precise synchronization between vehicles and pedestrians, we leverage RTT of ubiquitously available wireless signal to obtain sequence of location estimations of the prover (a pedestrian or an attacker) over time. Under RTT and GPS errors, PEDRO is able to verify the moving prover while effectively rejecting stationary attacks. With realistic simulation framework as well as through real-world case study, we show that PEDRO can achieve 8.5% Equal-Error-Rate against malicious attackers while maintaining relatively usable verification time of under 8 seconds.
> Yucheng Yang, Kyuin Lee, Younghyun Kim, and Kassem Fawaz, 2021, November. PEDRO: Secure Pedestrian Mobility Verification in V2P Communication using Commercial Off-the-shelf Mobile Devices. [[Pdf]](https://wiscprivacy.com/member/member_yucheng/)

### Personalized Cellular Data based Pedestrian Street Crossing Bahavior Prediction System
Currently, I'm working on predicting pedestrian's road crossing behavior combining GPS, sensory data, and road information from OpenStreetMap. The plan is to deploy the trained and tuned LSTM model into mobile devices, and achieve real-time road crossing prediction on pedestrian's smartphones.


# Publication
>**Are You Really Muted?: A Privacy Analysis of Mute Buttons in Video Conferencing Apps**
>**Yucheng Yang**, Jack West, George K. Thiruvathukal, Neil Klingensmith, and Kassem Fawaz\
>*In the 22nd Privacy Enhancing Technologies Symposium (PETS ’22), 2022.*

>**AeroKey: Using Ambient Electromagnetic Radiation for Secure and Usable Wireless Device Authentication**\
>Kyuin Lee, **Yucheng Yang**, Omkar Prabhune, Aishwarya Lekshmi Chithra, Jack West, Kassem Fawaz, Neil Klingensmith, Suman Banerjee, Younghyun Kim\
>*In Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies (IMWUT ’22), 2022.*

>**PEDRO: Secure Pedestrian Mobility Verification in V2P Communication using Commercial Off-the-shelf Mobile Devices**\
>**Yucheng Yang**, Kyuin Lee, Younghyun Kim, and Kassem Fawaz\
>*In Proceedings of the 2nd Workshop on CPS&IoT Security and Privacy (CPSIoTSec ’21), 2021.*

>**Optimization of fingerprints reporting strategy for WLAN indoor localization**    
>Xiaohua Tian, Wenxin Li, **Yucheng Yang**, Zhehui Zhang, Xinbing Wang    
>*IEEE Transactions on Mobile Computing (TMC), 2017*   

>**Performance analysis of wi-fi indoor localization with channel state information**  
>Xiaohua Tian, Sujie Zhu, Sijie Xiong, Binyao Jiang, **Yucheng Yang**, Xinbing Wang  
>*IEEE Transactions on Mobile Computing (TMC), 2018*

## Contact

* Email: `yang552_AT_wisc_dot_edu`
