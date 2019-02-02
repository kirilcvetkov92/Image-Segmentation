# Image-Segmentation

Keras impementation of BiseNet Image Segmentation Model (Paper : [Link](https://arxiv.org/pdf/1808.00897.pdf))

| Image	|  Semantic Segmentation    |Semantic_Video_Segmatnation(Youtube)|
|:-----------:|:----------:|:---------:|
| ![Introduction video](test_img.png)|![Semantic segmentation](output_image.png)|![Video](https://img.youtube.com/vi/cxAuoHRf1z4/0.jpg)| 

## Pretrained model
Pretrained Model Download ([Link](https://drive.google.com/uc?id=11ghYNpY4osChcteBV-fefqY8ufDjhcrq&export=download))

## Dataset  
Download CamVid dataset from [Semantic-Segmentation-Suite](https://github.com/GeorgeSeif/Semantic-Segmentation-Suite/tree/master/CamVid)  
Thanks [GeorgeSeif](https://github.com/GeorgeSeif) for his great job!

## Suport
**Prediction supports the following file formats : (Video : Mp4, Picture : .png)**

### Model prediction arguments

```
mandatory arguments:
  -media MEDIA_DIR, --media_dir MEDIA_DIR
                        Media Directorium for prediction (mp4,png)
optional arguments:
  -save SAVE_DIR, --save_dir SAVE_DIR
                        Save Directorium
  -model MODEL_DIR, --model_dir MODEL_DIR
                        Model Directorium
```

### Example semantic Image segmentation : 

```
python predict.py -media test_img.png
```

### Example semantic Video segmentation :
```
python predict.py -media test_video.mp4
```


## Model training arguments:

```
optional arguments:
  -eph EPOCHS, --epochs EPOCHS
                        Number of epochs
  -lr LEARNING_RATE, --learning_rate LEARNING_RATE
                        Learning rate
  -save MODEL_DIR, --model_dir MODEL_DIR
                        Save checkpoints directory
  -batches BATCH_SIZE, --batch_size BATCH_SIZE
                        Number of batches per train
```                        
