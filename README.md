Triple Feature Fusion Based Adversarial Example Detection Against Second-Round Adversarial Attacks
Detection of adversarial examples using a triple fusion of CNN deep features, SRM handcrafted features, and Discrete Wavelet Transform (DWT) frequency features. Achieves robust detection against second-round adversarial attacks that simultaneously fool both the base model and the detector.

Method
Three parallel feature extraction pipelines (CNN + SRM + Wavelet) are concatenated and passed into a fusion classifier. Tested on CIFAR-10 and Tiny-ImageNet using ResNet18 as the base model.

Results
Achieves up to 100% clean accuracy and ~99%+ detection rate against PGD and second-round attacks on CIFAR-10. Wavelet features significantly improve stability on Tiny-ImageNet over SRM-only fusion.

Stack
Python · PyTorch · PyWavelets · scikit-learn

How to Run
-Recommended to run on Google Colab with T4 GPU or higher.
-The code will ask you to choose a dataset between CIFAR-10 and Tiny-ImageNet.
-No manual dataset download is needed. Datasets are fetched automatically.

Report
-See report.pdf for full details, experiments, and references.
