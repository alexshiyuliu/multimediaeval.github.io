---
# static info
layout: task
year: 2021
hide: false 

# required info
title: "Medico: Transparency in Medical Image Segmentation"
subtitle:
blurb: "The Medico task explores the use of transparent approaches to automatically segment images collected from the human colon."
---

<!-- # please respect the structure below-->
*See the [MediaEval 2021 webpage](https://multimediaeval.github.io/editions/2021/) for information on how to register and participate.*

#### Task Description
The fight against colorectal cancer requires better diagnosis tools. Computer-aided diagnosis systems can reduce the chance that diagnosticians overlook a polyp during a colonoscopy. As machine learning becomes more common, even in high-risk fields like medicine, the need for transparent systems becomes more critical. In this case, transparency is defined as giving as much detail as possible on the different parts that make up a machine learning pipeline, including everything from data collection to final prediction. This task focuses on robust, transparent, and efficient algorithms for polyp and instrument segmentation. 

The data consists of a large number of endoscopic images of the colon, which have been labeled by expert gastroenterologists.

*Subtask 1: Polyp Segmentation:* The polyp segmentation task asks participants to develop algorithms for segmenting polyps in images taken from endoscopies. The main focus of this task is to achieve high segmentation metrics on the supplied test dataset. Since [Medico 2020](https://multimediaeval.github.io/editions/2020/tasks/medico/), we have extended the development dataset and created a new testing dataset to which the submissions will be evaluated on.

*Subtask 2: Instrument Segmentation* Similar to the polyp segmentation task, the instrument segmentation task asks participants to develop algorithms for segmenting instruments present in colonoscopy videos. The main focus of this task is to achieve high segmentation metrics on the supplied test dataset. 

<!-- # People might get confused on the difference between transparency, explainability, and interpretibility when it comes to machine learning. Could this be made clearer?-->
*Subtask 3: Transparent Machine Learning Systems* The transparency task tries to measure the transparency of the systems used for the aforementioned segmentation tasks. The main focus for this task is to evaluate systems from a transparency point of view, meaning for example explanations of how the model was trained, the data that was used, and interpretation of a model's predictions.

Participants are encouraged to make their code public with their submission.

#### Motivation and background
Medical image segmentation is a topic that has garnered a lot of attention over the last few years. Compared to classification and object detection, segmentation gives a more precise region of interest for a given class. This is immensely useful for the doctors as it not only specifies that an image contains something interesting but also where to look at which also provides some kind of inherent explanation. Colonoscopies are a perfect use-case for medical image segmentation as they contain a great variety of different findings that may be easily overlooked during the procedure. Furthermore, transparent and interpretable machine learning systems are important to explain the *whys* and the *hows* of the predictions. This is especially important in medicine, where conclusions based on wrong decisions resulted from either biased or incorrect data, faulty evaluation or simply a bad model could be fatal. For this reason, the *Medico: Transparency in Medical Image Segmentation* task aims to develop automatic segmentation systems that are transparent and explainable.

#### Target group
The task is of interest to the researchers working with multimedia segmentation, deep learning (semantic segmentation), and computer vision. We especially encourage young researchers to contribute to the field of endoscopy by developing an automated computer-aided diagnosis system that could be potentially used in clinical settings.  

#### Data
*Subtask 1: Polyp Segmentation:* We will use a slightly modified version of the segmentation part of HyperKvasir [1] that will include additional polyps for training and a separate testing dataset. 

*Subtask 2: Instrument Segmentation* For the instrument segmentation task, we will use Kvasir-Instrument [2] for the development dataset and a different testing dataset. 

*Subtask 3: Transparent Machine Learning Systems* The transparent machine learning system task will be based on the previous two tasks and will use each respective dataset.

#### Ground truth
The ground truth for the provided dataset was created by an experienced computer scientist and medical doctor, which was then verified by an expert gastroenterologist with over ten years of experience.

#### Evaluation methodology
*Subtask 1: Polyp Segmentation and Subtask 2: Instrument Segmentation* We will use the standard metrics commonly used to evaluate segmentation tasks, similar to what was presented in [Medico 2020](https://multimediaeval.github.io/editions/2020/tasks/medico/). This includes the Dice coefficient, pixel accuracy, and the Intersection-Over-Union (Jaccard index). The metric which will be used to rank submissions will be the Intersection-Over-Union coefficient.

<!-- # Please considering adding: We also encourage participants to carry out a failure analysis of their results in order to gain insight in the mistakes that their classifiers make.-->

*Subtask 3: Transparent Machine Learning Systems:* We perform a qualitative evaluation of the submission. Here, a multi-disciplinary team will evaluate the submissions based on how transparent and understandable they are. We encourage participants to perform failure analysis on their results, which will contribute to more insight into where a model makes mistakes, contributing to the overall transparency of the system.

#### References and recommended reading
<!-- # Please use the ACM format for references https://www.acm.org/publications/authors/reference-formatting (but no DOI needed)-->
<!-- # Please add the links! The paper title should be a hyperlink leading to the paper online-->
<!-- # Adding more literature on explainability would be helpful-->
[1] Borgli, H., Thambawita, V., Smedsrud, P.H. et al. HyperKvasir, a comprehensive multi-class image and video dataset for gastrointestinal endoscopy. Sci Data 7, 283 (2020).

[2] Jha D. et al. (2021) Kvasir-Instrument: Diagnostic and Therapeutic Tool Segmentation Dataset in Gastrointestinal Endoscopy. In: Lokoč J. et al. (eds) MultiMedia Modeling. MMM 2021. Lecture Notes in Computer Science, vol 12573.

[3] Ronneberger O, Fischer P, Brox T. U-net: Convolutional networks for biomedical image segmentation. In Proceeding of International Conference on Medical image computing and computer-assisted intervention (MICCAI), 234-241, 2015.

[4] Weller A. Transparency: motivations and challenges. InExplainable AI: Interpreting, Explaining and Visualizing Deep Learning 2019 (pp. 23-40). Springer, Cham.

#### Task organizers
* Steven Hicks, SimulaMet, Norway steven (at) simula.no
* Debesh Jha, SimulaMet, Norway  debesh (at) simula.no
* Vajira Thambawita, SimulaMet and OsloMet, Norway 
* Thomas de Lange, Bærum Hospital, Norway
* Sravanthi Parasa, Swedish Medical Center, Sweden
* Michael Riegler, SimulaMet, Norway  
* Pål Halvorsen, SimulaMet and OsloMet, Norway 

#### Task Schedule
* 1 July: Data release <!-- # Replace XX with your date. We suggest setting the date in June-July-->
* 1 November: Runs due <!-- # Replace XX with your date. We suggest setting enough time in order to have enough time to assess and return the results by the Results returned deadline-->
* 7 November: Results returned  <!-- Replace XX with your date. Latest possible should be 15 November-->
* 22 November: Working notes paper  <!-- Fixed. Please do not change. Exact date to be decided-->
* Beginning December: MediaEval 2020 Workshop <!-- Fixed. Please do not change. Exact date to be decided-->