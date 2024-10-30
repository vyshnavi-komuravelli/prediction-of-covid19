## Training a model
We have provided a Python script to train a VGG16 model on the training data. 
The training script gets a few arguments from the user, such as the training data path, leanring rate, number of epochs, etc. There is a default value for all of these arguments, but if you can specify your own argument too. 

**You can run the training code as (you can of course change the values of arguments):**

```
python VGG16_train.py --dataset_path ./data/ --batch_size 20 --epoch 50 --num_workers 4 --learning_rate 0.001
```

This code fine-tunes a pre-trained VGG16 model on the training dataset. 


## Inference Code


**You can run the inference as:**

```
python inference.py --test_covid_path ./data/test/covid/ --test_non_covid_path ./data/test/non/ --trained_model_path ./covid_vgg16_epoch100.pt
```



