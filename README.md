# Procgen PPO Code Base

### Installation
1. Create a new conda environment
    ``` bash
    conda create -n ppo_procgen python=3.7
    conda activate ppo_procgen
    ```
2. Install the required packages and Procgen benchmark
    ``` bash
    pip install -r requirements.txt
    pip install procgen
    ```
3. Install the baselines package
    ``` bash
    git clone https://github.com/openai/baselines.git
    cd baselines 
    python setup.py install 
    ```

### Training
To train a model, run the following command:
``` bash
python train.py --env_name coinrun --algo ppo --ppo_epoch 3
```


### Acknowledgements
This code was based on the [IDAAC](https://github.com/rraileanu/idaac) project. It has been streamlined to focus exclusively on Proximal Policy Optimization (PPO) related code, making it more suitable for secondary development targeting the Procgen Environment.