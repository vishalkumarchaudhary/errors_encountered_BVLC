# errors_encountered_BVLC
This repo is made to help starters to create deep neural nets with the help of caffe ...

1) 
```
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
  File "/home/mabrin/caffe-master/python/caffe/classifier.py", line 29, in __init__
    in_ = self.inputs[0]
IndexError: list index out of range
```
If you are loading the model for prediction then and during loading the above error occured
This means that input layer during training is changed when we want to load the model for predicions.
```
layer {
    name: "data"
    type: "Input"
    top: "data1"
    input_param { shape: { dim: 1 dim: 3 dim: 256 dim: 256 } }
}
```
2)
# save python of any size 
```
np.save("a.npy" ,var_name )
x = np.load(".npy")
```


