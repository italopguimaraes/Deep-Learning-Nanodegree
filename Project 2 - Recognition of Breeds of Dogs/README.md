[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Keras Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

Welcome to the Convolutional Neural Networks (CNN) project at AI Nanodegree! In this project, a pipeline has been developed that can be used in a web or mobile application to process actual images provided by the user. Given an image of a dog, the algorithm will identify an estimate of the breed of the canine. If provided an image of a human, the code will identify the breed of the dog similar.

![Sample Output][image1]

Our goal is that by completing this lab, in addition to exploring state-of-the-art CNN models for classification, the student will make important design decisions about the user experience for the application and understand the challenges involved in assembling a series of models designed to perform multiple tasks in a data-processing pipeline. Each model has its strengths and weaknesses, and engineering a real-world application often involves solving many problems without a perfect answer. This imperfect solution, however, will create a fun user experience!

This project is part of Udacity's deep learning nanodegree program, if you are interested, see [repository](https://github.com/udacity/dog-project) of the original project.

## Software dependencies

Make sure the  `h5py`, `scipy`, `tqdm`, `keras`, `sklearn`, `pillow`, `opencv-python`, `numpy`, `matplotlib`, `tensorflow`, `ipykernel` and `jupyter notebook` are installed:

`conda install h5py scipy tqdm keras sklearn pillow opencv-python numpy matplotlib tensorflow ipykernel jupyter notebook`

View the software dependencies according to your hardware and operating system below:

[dependencies](requirements/)

## Project Instructions

1. Clone the repository.
```	
git clone https://github.com/Italo-Pereira-Guimaraes/Deep-Learning-Nanodegree.git
```
2. And navigate to the **Project 2 - Recognition of Breeds of Dogs/** folder by the terminal `cd Project 2 - Recognition of Breeds of Dogs`.

3. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/Project 2 - Recognition of Breeds of Dogs/dogImages`. 

4. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/Project 2 - Recognition of Breeds of Dogs/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

5. Donwload the [VGG-16 bottleneck features](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG16Data.npz) for the dog dataset.  Place it in the repo, at location `path/to/Project 2 - Recognition of Breeds of Dogs/bottleneck_features`.

6. In the browser, open the file **dog_app.ipynb**

7. Follow the instructions on the notebook that lead you through the project.

8. (Optional) __If you plan to install TensorFlow with GPU support on your local machine__, follow [the guide](https://www.tensorflow.org/install/) to install the necessary NVIDIA software on your system.  If you are using an EC2 GPU instance, you can skip this step.

9. (Optional) **If you are running the project on your local machine (and not using AWS)**, create (and activate) a new environment.

	- __Linux__ (to install with __GPU support__, change `requirements/dog-linux.yml` to `requirements/dog-linux-gpu.yml`): 
	```
	conda env create -f requirements/dog-linux.yml
	source activate dog-project
	```  
	- __Mac__ (to install with __GPU support__, change `requirements/dog-mac.yml` to `requirements/dog-mac-gpu.yml`): 
	```
	conda env create -f requirements/dog-mac.yml
	source activate dog-project
	```  
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/dog-windows.yml` to `requirements/dog-windows-gpu.yml`):  
	```
	conda env create -f requirements/dog-windows.yml
	activate dog-project
	```

10. (Optional) **If you are running the project on your local machine (and not using AWS)** and Step 6 throws errors, try this __alternative__ step to create your environment.

	- __Linux__ or __Mac__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`): 
	```
	conda create --name dog-project python=3.5
	source activate dog-project
	pip install -r requirements/requirements.txt
	```
	**NOTE:** Some Mac users may need to install a different version of OpenCV
	```
	conda install --channel https://conda.anaconda.org/menpo opencv3
	```
	- __Windows__ (to install with __GPU support__, change `requirements/requirements.txt` to `requirements/requirements-gpu.txt`):  
	```
	conda create --name dog-project python=3.5
	activate dog-project
	pip install -r requirements/requirements.txt
	```
	
11. (Optional) **If you are using AWS**, install Tensorflow.
```
sudo python3 -m pip install -r requirements/requirements-gpu.txt
```
	
12. Switch [Keras backend](https://keras.io/backend/) to TensorFlow.
	- __Linux__ or __Mac__: 
		```
		KERAS_BACKEND=tensorflow python -c "from keras import backend"
		```
	- __Windows__: 
		```
		set KERAS_BACKEND=tensorflow
		python -c "from keras import backend"
		```

13. (Optional) **If you are running the project on your local machine (and not using AWS)**, create an [IPython kernel](http://ipython.readthedocs.io/en/stable/install/kernel_install.html) for the `dog-project` environment. 
```
python -m ipykernel install --user --name dog-project --display-name "dog-project"
```

14. Open the notebook.
```
jupyter notebook dog_app.ipynb
```

15. (Optional) **If you are running the project on your local machine (and not using AWS)**, before running code, change the kernel to match the dog-project environment by using the drop-down menu (**Kernel > Change kernel > dog-project**). Then, follow the instructions in the notebook.

__NOTE:__ While some code has already been implemented to get you started, you will need to implement additional functionality to successfully answer all of the questions included in the notebook. __Unless requested, do not modify code that has already been included.__

## Evaluation

This project was reviewed by a reviewer Udacity against the CNN project heading. All the criteria found in the [rubric](https://review.udacity.com/#!/rubrics/810/view) met the specifications.

## license
 
For more information see:

[license](LICENSE.txt)


