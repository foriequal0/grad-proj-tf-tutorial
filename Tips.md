Notes
=====

## See GPU usage status

```
gupstat
```

## Limit GPU device

```python
import os
os.environ['CUDA_VISIBLE_DEVICES']='1'
```

## GPU Memory allocation on demand

```python
config = tf.ConfigProto()
config.gpu_options.allow_growth = True
sess = tf.Session(config=config)
```