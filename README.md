# Current: Vanilla A3c Actor Critic

This code runs on CPU.

## Updates:
Optimizer (my_optim.py) was updated as per latest pytorch functions
~I am working on making it GPU acessible.~
Current: working on making it accessible to the latest gym 

## Dependencies (Last I checked)
python 3.x
pytorch 1.11
gym 0.9.6 
numpy

gym has the strict requirement of the version


## Usage
```bash
# Works only wih Python 3.
python main.py --env-name "PongDeterministic-v4" --num-processes 16
```

This code runs evaluation in a separate thread in addition to 16 processes.

## Results

With 16 processes it converges for PongDeterministic-v4 in 15 minutes.

For BreakoutDeterministic-v4 it takes more than several hours.
