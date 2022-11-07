# Backdoor-Detection-and-Robust-Training

### Problem Statement

Backdoor attacks have emerged as the main threat to the safe deployment of DNNs. An adversary poisons some of the training data in such attacks by installing a trigger. The goal is to make the trained DNN output the attacker's desired class whenever the trigger is activated while performing as usual for clean data. Various approaches have recently been proposed to detect/defend malicious backdoored DNNs. However, how to efficiently defend against this attack is still an open question. In this project, we would like you to focus on the project related to backdoor defense:

### Project Goals  

- **Trojan Model Detection:** Given an untrusted pre-trained network, the goal of trojan detection is to reveal the potential backdoored model (and to identify the infected label, i.e. backdoor related label). Neural cleanse (NC) [1] has proposed a novel and generalizable technique for detecting and reverse engineering hidden triggers embedded inside deep neural networks. However, NC can be easily evaded by more adaptive attacks [2, 3]. So in this project, we encourage you to design or explore a new trojan detection technique against the advanced backdoor attacks.

- **Robust Learning on Backdoored Data:** Given backdoored training data, robust learning aims at reducing the backdoor success rate significantly with less affecting the clean accuracy on the poisoned dataset. Recently, Anti-Backdoor learning (ABL) [4] has proposed a robust learning framework that allows the user to train a backdoor-free model even on poisoned backdoored data. However, ABL is facing trouble when the poisoning rate is very low ($\leg$ 0.5% poisoning rate) and unstable backdoor unlearning. So in this project, we encourage you to address the limitations of ABL and explore a robust, end-to-end training approach like ABL.

`Note：` Consider the challenge of the task above, you can choose one of the topics in which you are interested.

### Trojan Model Zoo

We have randomly sampled a subset of the backdoored model from the Trojan Detection Challenge [5]. You can download from here [link].


### Reference 

[1] Wang B, Yao Y, Shan S, et al. Neural cleanse: Identifying and mitigating backdoor attacks in neural networks[C]//2019 IEEE Symposium on Security and Privacy (SP). IEEE, 2019: 707-723.  
[2] Nguyen A, Tran A. WaNet--Imperceptible Warping-based Backdoor Attack[J]. ICLR, 2021.  
[3] Nguyen T A, Tran A. Input-aware dynamic backdoor attack[J]. NeurIPS, 2021.  
[4] Li Y, Lyu X, Koren N, et al. Anti-backdoor learning: Training clean models on poisoned data. NeurIPS, 2021.  
[5] Trojan Detection Challenge, https://trojandetection.ai/.
