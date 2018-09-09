---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

You can also download my single-paged Resume [__here__](https://wenyuan-vincent-li.github.io/files/Li_Wenyuan_CV_2018_9_9_ENG.pdf).

Education
======
* B.S. in Engineering, Zhejiang University, 2014
* M.S. in Electrical Engineering, University of California, Los Angeles, 2016
* Ph.D in Electrical and Computer Engineering, University of California, Los Angeles, 2020 (expected)

Research Experience
======
* Rare disease detection using Generative Adversarial Network (GAN) (07/18-09/18)
    * Work on developing a semi-supervised rare disease detection 
      framework using a generative adversarial network (GAN). 
      The model performance beats common classifier (logistic regression, 
      neural network, and random forest) by 5% in terms of 
      precision-recall AUC score.

* Medical image segmentation based on multitask learning (11/17-06/18)
    * Design a two-branch deep learning “Path R-CNN” 
      architecture which decouple the classification and segmentation 
      task. Region proposal network inspired by Mask R-CNN was 
      later added to our model. The new architecture boosts 
      the segmentation performance around 5% in mIOU.

* Collective neural dynamics: for better mental disease prediction and faster neuromorphic computing (06/15-09/17)
    * Design and emulate neural dynamics on Neuromorphic Circuits – 
      Spikey; a brain phase diagram was constructed for achieving better 
      mental disease prediction and faster neuromorphic computing.
      [__Read More__](https://wenyuan-vincent-li.github.io/publication/2018-09-30-neuraldynamics)

* Skyrmion tracking by optical flow method (12/14-04/15)
    * Matlab programing to track Skyrmion moving using optical 
      flow algorithm.
      [__Read More__](https://wenyuan-vincent-li.github.io/publication/2016-02-11-skyrmions)

Intern Experience
======
<ul>{% for post in site.experiences %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Skills
======
* Programming
    * Python, Tensorflow, Scikit-learn, Pandas
    * Java
    * C++ 
    * Matlab 
    * Labview
* Machine Learning
    * Random Forest
    * Logistic Regression
    * SVM
    * Monte Carlo Methods
    * Deep Learning
        * Convolutional Neural Network (CNN)
        * Region Based CNN (R-CNN)
        * Generative Adversarial Network

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Activity, Membership, and Service
======
* IEEE student membership
* Member of UCLA-C3S (Chinese-American Students and Scholars Seminar)
* Member of UCLA-CSBD (Chinese Students Ballroom Dance Team)
* Volunteer at China Rainbow Network (CRN) 
