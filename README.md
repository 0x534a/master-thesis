# Master Thesis
This repository contains my master thesis with the title *Signature-Based Detection of Behavioural Malware Features with Windows API Calls*. I finished my degree Master of Science in Digital Forensics with this thesis at the [University of Applied Sciences Albstadt-Sigmaringen](https://www.hs-albsig.de/hochschule/organisation/international-office/information-in-english/) in 2020. The work was supervised by Prof. Felix Freiling ([Friedrich-Alexander-University Erlangen-Nuremberg](https://www.fau.eu)).

In companion with the thesis, the slides of the defence presentation are provided. The slides may be a good starting point to get an overview of the research project.


## License
This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg


## Thesis Abstract
The rising complexity of IT infrastructures in general offers a large surface for cyber attacks and adversaries to understand how to take great advantage of this. Malicious software plays thereby a key role in compromising a victim's infrastructure as it is used to carry out the attack and gain persistence. As a consequence, effectively protecting against cyber attacks is directly correlated with the reliable detection of malicious software. However, it is not only the complexity of IT infrastructures that is rising, but also that of the malicious software.

In this work, we introduce the signature-based detection approach *dynmx* which helps domain experts to efficiently analyse malicious software based on its behavioural characteristics. Therefore, a concise and easy-to-learn domain specific language is proposed in order to allow domain experts to specify known behavioural malware features in a precise and consistent manner. This, in turn, enables domain experts to collaboratively share these specified behaviour signatures. Since recent research has shown that the API call usage is a valuable resource for analysing malicious software, it is exactly this abstraction layer that we make use of for the definition of malware features. The source of information used for our proposed detection approach are function logs - chronologically ordered sequences of API functions called by a certain process which is monitored by a sandbox. For the detection of such signatures in function logs, we propose a detection algorithm based on the solution to the longest common subsequence (LCS) problem. For the sake of simplicity, the detection approach introduced in this work can be classified as equivalent to the well-adopted YARA framework but for behavioural instead of static characteristics.

All of the theoretic concepts presented in this work were implemented as a fully-working prototype application. This prototype application formed the basis to evaluate our approach in three dimensions - the detection quality, the capabilities of the signature DSL and the detection performance. In conclusion of this work, it is shown that the *dynmx* detection approach has the potential to improve the malware analysis process in general as it allows domain experts to precisely and efficiently detect known malicious behaviour with the help of signatures.
