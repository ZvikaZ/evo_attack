
## Prepare the environment
    conda create -n attackar numpy=1.19 pytorch tensorflow python=3.9
    conda activate attackar
    pip install piqa adversarial-robustness-toolbox
    pip install git+https://github.com/RobustBench/robustbench@v0.2.1

## Download the trained models
- Download model from Google Drive link at https://github.com/huyvnphan/PyTorch_CIFAR10
- Unzip it, to get `state_dicts/*.pt`
- TODO: get `models/*.pth`

## Run
    python main.py --model=inception_v3 --dataset=cifar10 --eps=0.025 --pop=70 --gen=600 --images=1 --tournament=25
