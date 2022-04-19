# Current: Vanilla A3c Actor Critic

~This code runs on CPU. I am working on making it GPU acessible.~


## Usage
```bash
# Works only wih Python 3.
python main.py --env-name "PongDeterministic-v4" --num-processes 16
```

This code runs evaluation in a separate thread in addition to 16 processes.

## Results

With 16 processes it converges for PongDeterministic-v4 in 15 minutes.

For BreakoutDeterministic-v4 it takes more than several hours.
