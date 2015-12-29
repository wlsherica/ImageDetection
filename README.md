# ImageDetection
Process on image detection with tensorflow library in Python

## Environment 
- Python 2.7
- Mac OS, CPU only
 
## Install tensorflow 

```shell
sudo pip install --upgrade https://storage.googleapis.com/tensorflow/mac/tensorflow-0.6.0-py2-none-any.whl
# then you will get "Successfully installed numpy-1.10.2 protobuf-3.0.0a3 setuptools-19.2 tensorflow-0.6.0 wheel-0.26.0"
```
- Requirement already up-to-date: six>=1.10.0 in /Library/Python/2.7/site-packages (from tensorflow==0.6.0)
- Requirement already up-to-date: protobuf==3.0.0a3 in /Library/Python/2.7/site-packages (from tensorflow==0.6.0)
- Requirement already up-to-date: wheel in /Library/Python/2.7/site-packages (from tensorflow==0.6.0)
- Requirement already up-to-date: numpy>=1.8.2 in /Library/Python/2.7/site-packages (from tensorflow==0.6.0)
- Requirement already up-to-date: setuptools in /Library/Python/2.7/site-packages (from protobuf==3.0.0a3->tensorflow==0.6.0)

## Error!?
```python
...
ImportError: numpy.core.multiarray failed to import
```
## How to fix this?
```shell
ls /System/Library/Frameworks/Python.framework/Versions/2.6/Extras/lib/python/
```
to be continued ...

## Test your tensorflow
```python
import tensorflow as tf
hello = tf.constant('Hello, TensorFlow!')
sess = tf.Session()
print(sess.run(hello))

a = tf.constant(10)
b = tf.constant(32)
print(sess.run(a + b))
#42
>>>

```

## Reference
- [Tensorflow tutorial](https://www.tensorflow.org)
