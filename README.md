# Detecting COVID-19 in X-ray images using deep learning in Google Colab







## dataset
> the x-ray images from canadian hospital are divided in two groups one folder is named `covid` and another folder folder is named `normal`,each folder has 25 chest x-ray images.

> notice:you can be able to use your own dataset by putting them in these folders.

## .pptx file
> my peresentation about this project contents such as model,Code,dataset,... is explained in this file. 

## covid-colab.ipynb
>  this file is prepared for runing code in google colab,before running code,,you must set the correct path in code file that is showed below:

```
#dataset path 
dataset = "/content/drive/My Drive/keras-covid-19/dataset"
```
> after setting the dataset path ,you can be able to running each cell in colab,and see the results,finally after training different epochs,the model will create the `savedmodelcolab` with `.h5` format(weight file) and `result chart.png`


## result chart
> see the training loss and accuracy in this chart that illustrates the loss is decrasing and the accuracy is increasing in both of them (training and validation)

## License
>[Detecting COVID-19 in X-ray images with Keras, TensorFlow, and Deep Learning by Adrian Rosebrock](https://www.pyimagesearch.com/2020/03/16/detecting-covid-19-in-x-ray-images-with-keras-tensorflow-and-deep-learning/)
