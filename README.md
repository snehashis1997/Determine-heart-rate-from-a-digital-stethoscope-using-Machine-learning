# Determine heart rate from a digital stethoscope using Machine learning
I worked Sensordrop Networks (http://www.sensordropsnetworks.com/) from 20th July,2020 to 20th Sept,2020 as an intern. During this time I worked with Heart beat signals as .wav format. My work was to build a statistical model to predict heart rate from this signals. Also, I tried to develop an accurate peak detection algorithm.

## In this project we worked two different heart beats dataset
* [Challenge dataset]
* Dataset provided by Organization

[Challenge dataset]:https://www.peterjbentley.com/heartchallenge/

### Time domain visualization of the Heart beat audio signal before and after Bandpass filtering
![image](https://user-images.githubusercontent.com/33135767/92559609-8d697d00-f28e-11ea-8cf0-0884caaf44a5.png) ![image](https://user-images.githubusercontent.com/33135767/92559650-9fe3b680-f28e-11ea-95ac-489af75adfc3.png)

### MFCC features plot of the Heart beat audio signal before and after Bandpass filtering

![image](https://user-images.githubusercontent.com/33135767/96450729-34e5b200-1234-11eb-97fb-67387a7dde1c.png) ![image](https://user-images.githubusercontent.com/33135767/96450775-43cc6480-1234-11eb-9178-be83fe2acb1c.png)


### Actual vs Predicted values of Heart beats in my test set
<img src="https://user-images.githubusercontent.com/33135767/92330440-73f8e300-f08c-11ea-9347-f831828e0f3c.png" width="600" height="400"/> ![image](https://user-images.githubusercontent.com/33135767/92560103-724b3d00-f28f-11ea-96eb-0172c1f30e22.png)

## Peak detection part
### Actual signal before and after Band pass filtering and avereging
![image](https://user-images.githubusercontent.com/33135767/96450438-d7516580-1233-11eb-80cb-6b3aa631c88f.png) ![image](https://user-images.githubusercontent.com/33135767/96450364-bab52d80-1233-11eb-810a-ba4697e78b4b.png)

### Detected peaks but here we can see some unwanted peaks

Try to remove unwanted peaks. Here I used two metods.

* thresholding: set the threshold value maximum of signal value multiply with a factor 0.1

* distance: I consider an original peak should be have maintain a distance 1500 from it's previous and next peak

![image](https://user-images.githubusercontent.com/33135767/96450193-82155400-1233-11eb-89ab-0a9b14c7e9bc.png)

### After filtering peaks
![image](https://user-images.githubusercontent.com/33135767/96450142-6e69ed80-1233-11eb-895d-f130c09ad63d.png)

### Plot the time interval between two peaks
![image](https://user-images.githubusercontent.com/33135767/96450058-55613c80-1233-11eb-8f42-0edff502d03f.png)

