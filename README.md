# Fruit-Prediction-Machine-Learning
You can predict anything from different classify of your image using my machine learning


![image](https://user-images.githubusercontent.com/71108329/178641475-bb4f5a45-8b85-44ad-a5fe-ce003fc598b6.png)
I am using Tesla T4 GPU for running the program in google colab, it might be different for every device who run the program

![image](https://user-images.githubusercontent.com/71108329/178641572-199b3cdc-11fb-4f24-b2bd-314255c58cd2.png)
cloning the template for library YoloV5, we are importing the requirement it is explained like we are using AI then for differentiate from 1 to another image we must using eye right? so we import the Eyes to completed our AI

![image](https://user-images.githubusercontent.com/71108329/178641687-6585110a-c18c-4828-a0c8-d17408ef19c0.png)
in here we import the image which has trained and validated from roboflow, so we only use the final program(trained and tested image) from the roboflow,
need to underlined if how good is your prediction program is depend on how good your annotate, how big is your dataset, and how good is your model created.

in here I'am using 100 datasets, consist of 50 health apple and 50 sick apple
![image](https://user-images.githubusercontent.com/71108329/178641934-e0f1c70b-5685-4b24-be02-2de1125939fb.png)

![image](https://user-images.githubusercontent.com/71108329/178641978-ab04dad3-4716-468b-87a5-8a174620a5ac.png)
in this code we can know where do we save the image for train and validation, in Yolov5 only use train and validation image, and in here we have 2 classes classify it is health apple and sick apple from the roboflow
after we know the folder place for image, we import the data or the image
then we create the template for Yolov5, Yolo v5 has 5 version such as s,m,l,x, which have their own size to run the program, but in this program we use yolov5.s, it is the smallest and the fastest models so we could run it in a short time. in here there is an architecture for model yolo v5s, there is depth and width multiple also anchors, backbone, and head, the way our AI run is similar as the neural network in our body, from the bottom giving signal to the backbone and then give again to the brain. we also could change the parameter but for me this models is the best for our program. the more bigger model in Yolo v5 is the bigger time you need, but it will be more accurate

![image](https://user-images.githubusercontent.com/71108329/178642105-80fba940-edcf-4961-b493-285586b6dcbd.png)
import the model yolov5,this is the custom yolov5s, we can change all the models in here

![image](https://user-images.githubusercontent.com/71108329/178642190-77e01b57-7be6-4eb7-9fa2-3d22cc286f0a.png)
now we can train our models, we using 150 epochs(more epochs more intelligence), and batch size32, epochs is the looping program for training, and batch size is dividing the total image into the batch and then will looping from the epochs, for example if we have 100 dataset and our batch size is 5 so firstly is will took 5 image first from 100, then after get trained, took another 5 image until 20 batch /100image, and this is only 1 epochs if we use 100 epochs then it will looping until 100 times, we trained for 45 minutes.
the training data will give the best program and the best program will we use to testing

![image](https://user-images.githubusercontent.com/71108329/178642349-fda70684-c2c9-4e27-be0b-7f40270a34f0.png)
this is the testing program, we can see for the health image giving 93% prediction and sick apple giving 80%

now we can predict the image from our program we can see if the apple is health or sick

![image](https://user-images.githubusercontent.com/71108329/178642434-95137b44-8c07-4131-aefa-1d0918a1b590.png)

![image](https://user-images.githubusercontent.com/71108329/178642467-254ad892-dc0c-4d4e-8ad8-dd83da8675af.png)

![image](https://user-images.githubusercontent.com/71108329/178642484-d71c3875-2a38-4357-9c0e-ced07034aeb7.png)

![image](https://user-images.githubusercontent.com/71108329/178642530-da5f0cde-a03c-4743-be44-abc7ec164d9f.png)


Thankyou and see you in my another project
