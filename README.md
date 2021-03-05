# Edge computing and machine learning on IoT devices is now possible 
The Coral USB Accelerator is a USB device that provides an Edge TPU as a coprocessor for your computer. It accelerates inferencing for your machine learning models.
![Image from iOS](https://user-images.githubusercontent.com/444888/110067862-c7917400-7d31-11eb-9e55-2d56c64611af.jpg)
```
echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list
curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
```
```

sudo apt-get update
sudo apt-get install libedgetpu1-std
sudo apt-get install libedgetpu1-max
```
```
cd iot-edge-comupting-machine-learning-coral/

source tflite1-env/bin/activate
python3 TFLite_detection_webcam.py --modeldir=Sample_TFLite_model --edgetpu

```
![2021-03-04-210816_1920x1080_scrot](https://user-images.githubusercontent.com/444888/110067034-058d9880-7d30-11eb-9fe6-80a194b4b5f7.png)
![2021-03-04-211024_1920x1080_scrot](https://user-images.githubusercontent.com/444888/110067040-0b837980-7d30-11eb-8ac4-872424e8bc7f.png)
