# Detect Network Attacks

## Context
Network security is important for home networks as well as in the business world therefore a solid network security system helps catch attackers (hackers) before they do real damage to a network and reduce the risk of data loss, theft and sabotage.

## Description
In this project we will have to predict which are the malicious attempts or attacks. We have 3 data files: traindata.csv, testdata.csv and sampleSubmission.csv.

We will use the training data (traindata.csv) to build our model. Then obtain the predictions for the test set examples (provided in file testdata.csv). The file sampleSubmission.csv is an example of a submission file.

## Evaluation Metric

The evaluation metric for this competition is the F1 Score. The F1 score, commonly used in information retrieval, measures accuracy using the statistics precision prec and recall rec. Precision is the ratio of true positives tp to all predicted positives tp+fp. Recall is the ratio of true positives to all actual positives tp+fn. The F1 score is given by:

$$F1 = 2\frac{PrecisionRecall}{Precision+Recall} = \frac{2TP}{2TP+FP+FN}$$

The F1 score is the harmonic mean of the precision and recall. The highest possible value of F1 is 1, indicating perfect precision and recall, and the lowest possible value is 0, if either the precision or the recall is zero.

The F1 metric weights recall and precision equally, and a good retrieval algorithm will maximize both precision and recall simultaneously. Thus, moderately good performance on both will be favored over extremely good performance on one and poor performance on the other.

## Features:
["ID", "Flow ID", "Source IP", "Source Port", "Destination IP", "Destination Port", "Protocol", "Timestamp", "Flow Duration", "Total Fwd Packets", "Total Backward Packets", "Total Length of Fwd Packets", "Total Length of Bwd Packets", "Fwd Packet Length Max", "Fwd Packet Length Min", "Fwd Packet Length Mean", "Fwd Packet Length Std", "Bwd Packet Length Max", "Bwd Packet Length Min", "Bwd Packet Length Mean", "Bwd Packet Length Std", "Flow Bytes/s", "Flow Packets/s", "Flow IAT Mean", "Flow IAT Std", "Flow IAT Max", "Flow IAT Min", "Fwd IAT Total", "Fwd IAT Mean", "Fwd IAT Std", "Fwd IAT Max", "Fwd IAT Min", "Bwd IAT Total", "Bwd IAT Mean", "Bwd IAT Std", "Bwd IAT Max", "Bwd IAT Min", "Fwd PSH Flags", "Bwd PSH Flags", "Fwd URG Flags", "Bwd URG Flags", "Fwd Header Length", "Bwd Header Length", "Fwd Packets/s", "Bwd Packets/s", "Min Packet Length", "Max Packet Length", "Packet Length Mean", "Packet Length Std", "Packet Length Variance", "FIN Flag Count", "SYN Flag Count", "RST Flag Count", "PSH Flag Count", "ACK Flag Count", "URG Flag Count", "CWE Flag Count", "ECE Flag Count", "Down/Up Ratio", "Average Packet Size", "Avg Fwd Segment Size", "Avg Bwd Segment Size", "Fwd Header Length.1", "Fwd Avg Bytes/Bulk", "Fwd Avg Packets/Bulk", "Fwd Avg Bulk Rate", "Bwd Avg Bytes Bulk", "Bwd Avg Packets/Bulk", "Bwd Avg Bulk Rate", "Subflow Fwd Packets", "Subflow Fwd Bytes", "Subflow Bwd Packets", "Subflow Bwd Bytes", "Init Win_bytes_forward", "Init_Win_bytes_backward", "act_data_pkt_fwd", "min_seg_size_forward", "Active Mean", "Active Std", "Active Max", "Active Min", "Idle Mean", "Idle Std", "Idle Max", "Idle Min", "SimillarHTTP", "Inbound", "Label"]

## Accuracy of Baseline Models
![Accuracy of Baseline Models](https://github.com/alansary/Detect-Network-Attacks/blob/main/images/Accuracy-of-Baseline-Models.png)

## Champion Model Confusion Matrix
![Champion Model Confusion Matrix](https://github.com/alansary/Detect-Network-Attacks/blob/main/images/Champion-Model-Confusion-Matrix.png)
