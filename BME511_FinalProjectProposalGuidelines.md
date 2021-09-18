# Final Project Proposal
**Due date**: November 11, 2021 by end of day


Feedback will be provided regarding aims (item #5 below) by November 18, 2021


The final project for this course is an *individual* project that will ideally be in your field of interest. If you are working towards a thesis as part of your degree program, this could also help you make progress within that context as long as the work involves signal processing. The scope of the project is similar to that of a single conference project (e.g., BMES, SfN, ARO, etc.) in your field, but only the data analysis formulation and implementation part of it. You could replicate something that is already published in your field. Novelty is **not** a requirement here; feel free to use this as an opportunity to learn/understand some signal-processing technique that is standard in your field if you so desire. The only constraint for the project is that it should involve a significant signal processing component (e.g., one or more of de-noising, decision making from data, estimation of unobservable quantities from raw data, etc.), and should address a problem that is of interest to your field.


**Problem formulation**, i.e., being able to go from an application-domain description of the problem (item #1 below), to a signal-processing problem description (item #3 below) is an important part of the process and is essentially the main focus of this proposal. With that in mind, please provide a one-page project proposal (being as specific as possible) that addresses the following issues about your project idea. Examples are provided for the first three questions to illustrate the kind of response that is appropriate.

## 1) What is the scientific question/biomedical/clinical application you will address and why is it important?

### Example response 1:
When physical symptoms of a brain tumor present to the clinic, imaging with MRI can provide confirmatory diagnostics and if necessary, help with surgical planning. However, often there is a significant window between MRI data acquisition and follow-up care owing to high demands to expert radiologists’ time.  We aim to develop a system to automatically segment out brain tumors from MRI images. This can reduce the window between MRI acquisition and clinical follow-up by priming/assisting radiologists with a pre-labeled set of suspected tumor regions. Furthermore, in the long run, such automated and semi-automated procedures can also reduce human errors and even aid in image-guided surgery.

### Example response 2:
Continuous monitoring of cardiac activity is valuable for a range of applications such as personal exercise and fitness assessments, early warning systems for arrhythmic activity, drug overdose detection, etc. Photoplethysmography (PPG) through wearable devices such as smart watches and smart rings is well suited for such applications. However, the PPG signal is noisy, suffering from movement artifacts. We aim to develop and validate a method for denoising of PPG signals by automatically removing motion artifacts. In particular, we will leverage signals from surrogate sensors that are placed in the smart device (smart watch in our case) alongside the LEDs and photosensors that are used for primary PPG measurements.
	
## 2) What data you will use and where it will come from? Briefly describe the dataset.

It is best not to rely on any data that is yet to be collected. If you really want to work on data that is soon to be collected or is in the process of being collected, it is strongly recommended that you do so only if you have a very high degree of confidence that the data collection endeavor will be successful and timely. You are welcome to use datasets from your own research, or from publicly available repositories like.

Some public repositories that may be useful are:
- https://openneuro.org/
- https://datadryad.org
- https://figshare.com/
- https://www.kaggle.com/datasets
- https://archive.ics.uci.edu/ml/datasets.php
- https://www.ncbi.nlm.nih.gov/gds

This is, of course, not an exhaustive list. Please feel free to explore and leverage any repositories that may exist in your field.


### Example response 1: 
The brain tumor dataset from Cheng et al., 2016 is available online at https://figshare.com/articles/brain_tumor_dataset/151242. This brain tumor dataset contains 3064 T1-weighted contrast-enhanced images from 233 patients with three kinds of brain tumor: meningioma (708 slices), glioma (1426 slices), and pituitary tumor (930 slices).

Cheng, J et al. Retrieval of Brain Tumors by Adaptive Spatial Pooling and Fisher Vector Representation. PloS one 11.6 (2016).

### Example response 2:
Data is available in the YYY lab from three human participants using smart watches, each over a two hour period and engaging in everyday activities such as sitting, walking, typing, stair climbing etc. In addition to the raw PPG signal, simultaneously acquired triaxial accelormeter data is available that can capture movements. Besides accelerometers, a secondary light source which provides a measure of wrist-movement-related artifacts is also included with the watch. This secondary light source is separate and of a different wavelength from the main source that is used for PPG. Simultaneous chest EKG data is also available for providing ground truth information.
	
## 3) Formulation of the scientific question in signal processing problem terms, and how success will be evaluated.

### Example response 1
Given 2D slices of MR images, the goal is to automatically label each pixel as representing a tumor pixel or not. Of the 3064 images, 2000 will be used to train the signal-processing algorithm and learn the analysis parameters. The remaining 1064 images will be used to test the efficacy of the algorithm by quantifying the hit rate and false-alarm rate of the classification performance. Any hit-rate and false alarm rate statistically above chance level with P < 0.01 will be considered a success for this course.

### Example response 2
Given two hours raw PPG data from 3 subjects, triaxial accelerometer data, and data from secondary light source, the problem is to return a "cleaned" version of the PPG signal by reducing noise that is movement related. The accelerometer and secondary source provide reference signals that capture motion. The quality of the "cleaning" will be quantified by estimating an average heart rate over 30-second windows (240 windows) from the raw PPG signal and also separately from the cleaned PPG signal. These 240 heart-rate values (each from raw and cleaned PPG) will be compared to heart-rate values over the same 30-second windows estimated from the chest EKG signal (i.e., the ground truth). The proportion of windows over which there is agreement (within 3 beats per second)  will be quantified as a measure of quality. It is expected that the cleaned PPG signal will have a significantly higher proportion of windows of agreement with the groud truth compared to the raw PPG signal -- this will be statistically tested.
	
## 4) What approaches (signal processing techniques) will you try? 

This can be exploratory for the purposes of the proposal, but it is good to get to some specifics soon. 


## 5) Describe two project objectives/aims that outline the extent of implementation for your project to earn an “A” grade for content; similarly describe what you would complete to earn a “B” grade. 

It is useful to think of this section as two small aims where you complete both for an “A” and one of the two for a “B”.

The idea here is that this is an agreement between you and the instructors. It protects you in the sense that we agree ahead of time that if you finish this much by the end, you’ll get an A for content, i.e., no expanding expectations on my part. On the other hand, it protects the instructors in the sense that you can’t put your project off until the end and then claim you did not have enough time to make significant progress.


## 6) Any other relevant issues, literature, and factors influencing feasibility.



Please discuss any issues that you face while planning or implementing the project sooner rather than later.
