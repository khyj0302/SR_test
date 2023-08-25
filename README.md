# SR_test
dental project SR model test

- create conda env by environment yml

GPU: conda install pytorch==1.1.0 torchvision==0.3.0 cudatoolkit=10.0 -c pytorch

CPU Only: conda install pytorch-cpu==1.1.0 torchvision-cpu==0.3.0 cpuonly -c pytorch

Train Model:
!python main.py --LR_path custom_dataset/train_LR --GT_path custom_dataset/train_HR

Test Model:
!python main.py --mode test_only --LR_path test_data/syn --generator_path ./model/pretrained_model.pt
