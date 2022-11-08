# Robust-Training on Backdoored Data

### Problem Statement

Backdoor attacks have emerged as the main threat to the safe deployment of DNNs. An adversary poisons some of the training data in such attacks by installing a trigger. The goal is to make the trained DNN output the attacker's desired class whenever the trigger is activated while performing as usual for clean data. Various approaches have recently been proposed to detect/defend malicious backdoored DNNs. However, how to efficiently defend against this attack is still an open question. In this project, we would like you to focus on the project related to backdoor defense:

### Project Goals  

- **Robust Learning on Backdoored Data:** Given backdoored training data, robust learning aims at reducing the backdoor success rate significantly with less affecting the clean accuracy on the poisoned dataset. Recently, Anti-Backdoor learning (ABL) [1] has proposed a robust learning framework that allows the user to train a backdoor-free model even on poisoned backdoored data. ABL introduces a two-stage gradient ascent mechanism for standard training to 1) help isolate backdoor examples at an early training stage, and 2) break the correlation between backdoor examples and the target class at a later training stage. However, ABL is facing trouble when the poisoning rate is very low ($\leg$ 0.5% poisoning rate) and unstable backdoor unlearning. So in this project, we encourage you to address the limitations of ABL and explore a robust, end-to-end training approach like ABL.

### Code of ABL

Code is available at https://github.com/bboylyg/ABL.

### Reference 

[1] Li Y, Lyu X, Koren N, et al. Anti-backdoor learning: Training clean models on poisoned data. NeurIPS, 2021.  
