An Adaptive Transformer-Based Model with Entropy-Driven Knowledge Distillation for Single-Channel EEG REM Sleep Detection.
Abstract
Accurate detection of rapid eye movement (REM) sleep is critical for neurophysiological monitoring and early identification of sleep-related disorders. 
We propose an entropy-driven adaptive knowledge distillation framework integrated with a lightweight Transformer to enable robust REM sleep detection from single-channel electroencephalogram (EEG) signals. 
By dynamically adjusting temperature scaling and distillation weighting based on teacher–student entropy, the proposed approach explicitly models uncertainty inherent in REM sleep.
Evaluated under subject-independent cross-validation on three public datasets (Sleep-EDF, ISRUC-Sleep, and MASS), the proposed model consistently outperforms CNN, LSTM, and standard Transformer baselines, achieving an average accuracy of 93.2% and an F1 score of 92.8%. Moreover, the distilled student model reduces training time and memory usage by approximately 30%, supporting efficient deployment in real-time and wearable EEG applications. These results demonstrate that uncertainty-aware adaptive distillation enables accurate, efficient, and scalable REM sleep detection from a single-channel EEG.
Keywords: REM sleep, Electroencephalogram (EEG), Knowledge Distillation (KD), Transformer, Sleep stage
