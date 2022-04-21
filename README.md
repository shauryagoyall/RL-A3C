# Current: Vanilla A3c Actor Critic

This code runs on CPU.

## Updates:
Optimizer (my_optim.py) was updated as per latest pytorch functions \
~I am working on making it GPU acessible.~ \
Current: working on making it accessible to the latest gym  \

## Dependencies (Last I checked)
python 3.x \
pytorch 1.11 \
gym 0.9.6  \
numpy 

gym has strict requirements of the version + games have to be added via https://github.com/openai/atari-py#roms


## Usage
```bash
python main.py --env-name "PongDeterministic-v4" --num-processes 16 \
python main.py --env-name "Breakout-v5" --num-processes 1 
```

This code runs evaluation in a separate thread in addition to 16 processes.

## Results

With 16 processes it should converge for PongDeterministic-v4 in 15 minutes.

For BreakoutDeterministic-v4 it should takes more than several hours.
