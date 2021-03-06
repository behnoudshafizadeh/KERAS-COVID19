# Detecting COVID-19 in X-ray images using deep learning in Google Colab
>* [dataset](#dataset)
>* [pptx_file](#pptx_file)
>* [code](#code)
>* [result_chart](#result_chart)
>* [model_output](#model_output)
>* [License](#License)


## dataset
> the x-ray images from canadian hospital are divided in two groups one folder is named `covid` and another folder folder is named `normal`,each folder has 25 chest x-ray images.

> notice:you can be able to use your own dataset by putting them in these folders.

## pptx_file
> my peresentation about this project contents such as model,Code,dataset,... is explained in `covid 19 with VGG16.pptx`. 

## code
>  `covid-colab.ipynb` is prepared for runing code in google colab,before running code,,you must set the correct path in code file that is showed below:

```
#dataset path 
dataset = "/content/drive/My Drive/keras-covid-19/dataset"
```
> after setting the dataset path ,you can be able to running each cell in colab,and see the results,finally after training different epochs,the model will create the `saved_model` with `.model` format(weight file) and `result chart.png`

## result_chart
> see the training loss and accuracy in this chart that illustrates the loss is decrasing and the accuracy is increasing in both of them (training and validation)

![result chart](https://user-images.githubusercontent.com/53394692/106428180-cbee1700-647d-11eb-8bbd-4c36c45fc935.png)

## model_output 
> for seeing the model result in covid+ and covid- images,run the following command in your `covid-colab.ipynb` file and see results in `Results.png and newResults.png` files:

```
--image:directory of images , --model:directory of saved weight
!python load_model.py --images dataset/covid --model saved_model.model
```

![newResults](https://user-images.githubusercontent.com/53394692/106427649-f8edfa00-647c-11eb-9e52-d324e9f7aaf4.png)
![Results](https://user-images.githubusercontent.com/53394692/106427996-7fa2d700-647d-11eb-9a34-7ab79c0fb0c2.png)


## License
>[Detecting COVID-19 in X-ray images with Keras, TensorFlow, and Deep Learning by Adrian Rosebrock](https://www.pyimagesearch.com/2020/03/16/detecting-covid-19-in-x-ray-images-with-keras-tensorflow-and-deep-learning/)
