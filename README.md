# CASPER
Interpretable gravitational-wave signal classification with a lightweight ResNet and FastSHAP explanations
ZENODO ID- https://zenodo.org/records/23895002
Refer for datasets
Classifiers for gravitational-wave strain data that are both interpretable and computationally accessible remain
an active area of research in spite of matched filtering continuing to be the statistical gold standard for
modeled signals. Although deep-learning classifiers have been shown to offer high sensitivity levels, many
of these classifiers rely on computationally expensive architectures and provide limited interpretability at high
computational cost. We present CASPER — Classification with Attribution via ShaPley in Residual neural
networks — an interpretable binary classifier. CASPER combines per-prediction interpretability via FastSHAP,
CPU-only deployability, a lightweight ResNet architecture, training on real GWOSC strain without synthetic
injections, and an event-level evaluation protocol. Concretely, CASPER combines: (i) lightweight seven-layer
ResNet CNN classifier trained on real GWOSC strain without synthetic injections; (ii) FastSHAP pixel-wise
attribution maps that localize the time–frequency features responsible for each prediction within a single
forward pass; (iii) Platt-calibrated output probabilities validated by Expected Calibration Error (ECE) and Brier
score; and (iv) CPU-only inference at 34 ms per segment. Evaluated on a held out set of 66 GWOSC events
(7250 spectrograms, event-level split, no data leakage), CASPER yields mean event AUC = 0.906 (Segment level
: 95% CI: [0.899, 0.914]) with Brier score = 0.099, outperforming a simple (non-residual) CNN baseline (mean
event AUC = 0.864) trained under identical preprocessing conditions. FastSHAP attribution maps recover
the inspiral chirp morphology and respond faithfully to pixel masking with reduced faithfulness at low SNR,
consistent with the classifier’s use of physically meaningful signal features which serves as input for classifier.
The full list of GWTC event identifiers assigned to the training and test sets will be released with the code
and trained weights via a permanent GitHub + Zenodo repository upon acceptance.


#If used without citations plagiarism will be considered
