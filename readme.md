
## Prepare the environment
    conda create -n evo_attack numpy pytorch
    conda activate evo_attack
    pip install piqa

## Download the trained models
- Download model from Google Drive link at https://github.com/huyvnphan/PyTorch_CIFAR10
- Unzip it, to get `state_dicts/*.pt`

## Run
- python main.py --model=inception_v3 --dataset=cifar10 --eps=0.025 --pop=70 --gen=600 --images=1 --tournament=25
