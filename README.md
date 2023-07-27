# Enhancing Adversarial Attack Transferability with the Foolbox Library

2023-2024 Centre for Secure Information Technologies (CSIT), Queen's University Belfast (QUB), Northern Ireland, United Kingdom

Authors: [Ehsan Nowroozi](https://scholar.google.com/citations?user=C0bNkP8AAAAJ&hl=en) Personal Website: www.enowroozi.com, Email: e.nowroozi@qub.ac.uk

This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version. This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details. You should have received a copy of the GNU General Public License along with this program. If not, see <http://www.gnu.org/licenses/>.

---
#  Introduction:
The issue of transferring adversarial examples becomes critical when applying these attacks to Deep Learning (DL) techniques in real-life computer network settings. This document aims to provide guidance on enhancing the transferability of adversarial attacks using the Foolbox library. Adversarial example transferability opens up the possibility of successful counterforensics (CF) attacks, particularly in cases where attackers lack full knowledge of the target system. However, it has been observed that adversarial examples against CNN-based image forensic detectors are generally non-transferrable, especially when using basic attack versions from popular libraries.

# Understanding the Problem:
The problem of adversarial attack transferability is further exacerbated by the design of popular attack software packages, which focus on minimizing embedding distortion for a successful attack. Consequently, attacked samples often reside very close to the decision boundary, making even minor changes to the detector potentially undermine the effectiveness of the attack. In contrast, attackers may prefer introducing larger distortions if it allows them to generate attacked samples that lie deeper within the target region of the attack. This increases the probability of transferability to another network, overcoming the limitations of non-transferrable attacks.

# Proposed Solution:
To address these challenges, we propose a general strategy to enhance the strength of adversarial attacks and evaluate their transferability. This can be achieved by modifying the Foolbox library and varying the attack strength accordingly.

# Steps to Enhance Adversarial Attack Transferability:

## Install Foolbox: 
Ensure you have the Foolbox library installed in your environment. If not, follow the installation instructions provided in the official Foolbox documentation.

## Select Target Models: 
Identify the Deep Learning models that you intend to attack in real-life computer network settings. Consider models commonly used in your domain and assess their robustness to adversarial attacks.

## Experiment with Attack Parameters: 
The Foolbox library offers various attack algorithms and parameters. Experiment with different attack settings, such as epsilon values, attack iterations, and targeted vs. untargeted attacks, to find the best combination for enhancing transferability.

## Adapt Distortion Constraints: 
By carefully choosing distortion constraints, you can control the proximity of attacked samples to the decision boundary. Adjusting these constraints may lead to better transferability while maintaining the attack's effectiveness.

## Evaluate Transferability: 
Use a diverse set of target models to evaluate the transferability of your adversarial attacks. Measure the attack success rate across various models and assess the impact of the modifications made to the Foolbox library.


## Fine-Tune the Strategy: 
Continuously fine-tune your attack strategy based on the results of your evaluations. Iterate on the attack parameters and modifications to improve transferability while still maintaining plausible attack effectiveness.

# If you utilize this code, kindly cite the following papers in your *.bib file:
 1)  For the paper titled "Demystifying the Transferability of Adversarial Attacks in Computer Networks" published in IEEE Transactions on Network and Service Management in 2022:
    
    @ARTICLE{9747933,
  author={Nowroozi, Ehsan and Mekdad, Yassine and Berenjestanaki, Mohammad Hajian and Conti, Mauro and Fergougui, Abdeslam El},
  journal={IEEE Transactions on Network and Service Management}, 
  title={Demystifying the Transferability of Adversarial Attacks in Computer Networks}, 
  year={2022},
  volume={19},
  number={3},
  pages={3387-3400},
  doi={10.1109/TNSM.2022.3164354}
}

3) For the paper titled "On the Transferability of Adversarial Examples against CNN-based Image Forensics" presented at the 2019 IEEE International Conference on Acoustics, Speech, and Signal Processing (ICASSP 2019):
   
   @INPROCEEDINGS{8683772,
  author={Barni, M. and Kallas, K. and Nowroozi, E. and Tondi, B.},
  booktitle={ICASSP 2019 - 2019 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)}, 
  title={On the Transferability of Adversarial Examples against CNN-based Image Forensics}, 
  year={2019},
  volume={},
  number={},
  pages={8286-8290},
  doi={10.1109/ICASSP.2019.8683772}
}
