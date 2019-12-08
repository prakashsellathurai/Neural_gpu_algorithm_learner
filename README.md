# Neural_gpu_programmer
Neural network that learns algorithms based on this arxiv paper https://arxiv.org/abs/1511.08228

Dependencies
 * tensorflow and its's dependencies
 
algorithms implemented are:
* `sort` - Sort a symbol list
* `kvsort` - Sort symbol keys in dictionary
* `id` - Return the same symbol list
* `rev` - Reverse a symbol list
* `rev2` - Reverse a symbol dictionary by key
* `incr` - Add one to a symbol value
* `add` - Long decimal addition
* `left` - First symbol in list
* `right` - Last symbol in list
* `left-shift` - Left shift a symbol list
* `right-shift` - Right shift a symbol list
* `bmul` - Long binary multiplication
* `mul` - Long decimal multiplication
* `dup` - Duplicate a symbol list with padding
* `badd` - Long binary addition
* `qadd` - Long quaternary addition
* `search` - Search for symbol key in dictionary


Training
```
python neural_gpu_trainer.py --problem=$(problem_task_name)
```

While training,  checkpoint model parameters will be
written to `/tmp/neural_gpu/`.

Evaluation
To evaluate a trained model on how well it decodes run:

```
python neural_gpu_trainer.py --problem=$(problem_task_name) --mode=1
```