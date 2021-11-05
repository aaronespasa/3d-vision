## Course Information ##

This class is a general introduction to computer vision. It covers standard techniques in image processing like filtering, edge detection, stereo, flow, etc. (old-school vision), as well as newer, machine-learning based computer vision. 

### Instructor ###
Joseph Redmon
- Email: pjreddie@cs.washington.edu
- Office Hours: Tu/Thur 10:00-11:20 am
    

### TAs ###

Fatemeh Ghezloo
- fghezloo@cs.washington.edu

Greg Guo
- grgrggtr@cs.washington.edu

Nishat Khan
- nkhan51@cs.washington.edu

Peter Michael
- petermic@cs.washington.edu

Paul Yoo
- yoosehy@cs.washington.edu

Slides are a mishmash of lots of other people's work. Special thanks to: Rob Fergus, Linda Shapiro, Harvey Rhody, Rick Szeliski, Ali Farhadi, Robert Collins. Lectures 8 and 9 on Flow, 3d, and stereo are given by [Connor Schenck](https://homes.cs.washington.edu/~schenckc/).

All of the slides, videos, and homeworks are free to use, modify, redistribute as you like without permission. Just make your own copy of the slides on Google Docs, don't ask to modify mine!

## Homeworks ##

The class has 6 homeworks where you will build out a computer vision library in C. We cover basic image manipulations, filtering, features, stitching, optical flow, machine learning, and convolutional neural networks.

Most of the homeworks will use [this repository](https://github.com/pjreddie/uwimg/). The individual homeworks can be found in the `src/` folder.

- [Homework 0: Fun with Color!](https://github.com/pjreddie/uwimg/tree/main/src/hw0), Due April 8th
- [Homework 1: Resizing](https://github.com/pjreddie/uwimg/tree/main/src/hw1), Due April 15th
- [Homework 2: Filtering and Convolutions](https://github.com/pjreddie/uwimg/tree/main/src/hw2), Due April 22nd
- [Homework 3: Panoramas!](https://github.com/pjreddie/uwimg/tree/main/src/hw3), Due April 29th
- [Homework 4: Optical Flow](https://github.com/pjreddie/uwimg/tree/main/src/hw4), Due May 6th 
- [Homework 5: Neural Networks and Machine Learning](https://github.com/pjreddie/uwimg/tree/main/src/hw5), Due May 13th

**Note:** due date subject to change if we haven't covered relevant material in time for the assignment.

## Final Project: ##

There is a final project worth 20% of the final grade.

Pick any area of computer vision that interests you and pursue some independent work in that area. Each project should have a significant technical component, software implementation, or large-scale study. Projects can focus on developing new techniques or tools in computer vision or applying existing tools to a new domain. If you don't have an idea you can train a classifier on birds and compete in the Kaggle competition posted on the Ed discussion board.

## Lectures ##

### Week 1: Image Basics ###

This week we cover the basics of computer vision. There's an introduction to the three levels of vision, **low-level** vision mostly concerns the pixels or groups of nearby pixels, **mid-level** vision starts to connect images to each other and the real world, and **high-level** vision connects images to semantics and meaning. There's background information on the human visual system, color, light, what an image actually is, and how it's stored in a computer. All fun stuff! Once you've learned the basics you should be ready for [Homework 0](https://github.com/pjreddie/uwimg/tree/main/src/hw0), which is mostly an introduction to the codebase we'll be using for the assignments.

#### Lecture 1: Introduction
- [Slides](https://docs.google.com/presentation/d/1VqTJEVC0gwxfY5TbINgBKyWqAmdxLYxgj_yIiphJj34/edit?usp=sharing)
- [Video](https://washington.zoom.us/rec/play/C83fxzyzYd78yhX-PElkUMeUgWe-8QOiYoF2U49pcrXqd2BBKCr6gwxVev5h5WWMn_ROJNCCt7jYt9_B.GsCgluaBokDdpycY)


#### Lecture 2: Human Vision, Color Spaces, Transforms ####
- [Slides](https://docs.google.com/presentation/d/1YBK7QkBW9t4kuZ8bJdwXLspyyeSpEJJldHvAhVcSsiM/edit?usp=sharing)
- [Video](https://www.youtube.com/watch?v=-nt80JUNwlw)

--------

### Week 2: Image Transformations ###

In week 2 we start to dive into low-level vision and image processing. You learn how to manipulate images and perform operations like resizing, sharpening, smoothing, and more. You'll apply this knowledge as you get started on [Homework 1](https://github.com/pjreddie/uwimg/tree/main/src/hw1).

#### Lecture 3: Image Coordinates, Resizing
- [Slides](https://docs.google.com/presentation/d/1ZkGgPPUzlGOdoGK6YNgiVLNouJW1ZaWzKEupDKmYM_4/edit?usp=sharing)
- [Video](https://youtu.be/hpqrDUuk7HY?t=129)

#### Lecture 4: Resizing, Filters, Convolutions
- [Slides](https://docs.google.com/presentation/d/18f0cWwS40jwbP5u37LKvM9ZaHEtRQFUKQ7MCtMdGLmA/edit?usp=sharing)
- [Video](https://youtu.be/5xdbJ7z4Nrc?t=119)

#### Supplementary Content:
- [Overview of Homework Codebase](https://washington.zoom.us/rec/play/H4Wgk8W40k1t5iS2YDoyrAgtxxKDisqtnoGzXYZ84NEYIKvLidB1tNeU4Nh3UG_sJ4yLbotPYBlXGtUr.AQhHZItzxFSBRAQR)
- [Debugging Using GDB and Valgrind](https://washington.zoom.us/rec/play/51JkwP7X_MIkl2MoAChPeGrdrdtsFJKn0TRB_yBTJby2utJXqVjET4uYjUKqHOAft1WlgVPgObvXm-Rr.0k6seTt67QxllWLF)

--------

### Week 3: Edges and Features

Time to put those convolutions to use! For week 3 we delve in to what makes images interesting, what makes them unique, how to find correspondences between images, and how to fit models with a large number of outliers in the data.

#### Lecture 5: Edges and Features

- [Video](https://www.youtube.com/watch?v=z5WSV6CXsxs)
- [Slides](https://docs.google.com/presentation/d/1_ZOtT17Ih2P-MRbWtZ8CTRQaJBz9V6-5_VA00QebiQQ/edit?usp=sharing)

#### Lecture 6: Harris, Matching, RANSAC

- [Video](https://www.youtube.com/watch?v=bn4KHa_zWuQ)
- [Slides](https://docs.google.com/presentation/d/1GLPcw-hQB1D94mOzTZKdMwAa8NKuqgih-bWl1vJS0tE/edit?usp=sharing)

-------

### Week 4: Features and Flow

#### Lecture 7: Matching, RANSAC, HOG, and SIFT

- [Video](https://www.youtube.com/watch?v=taty6lPVcmA)
- [Slides](https://docs.google.com/presentation/d/1h2Az_a28qjKvLpbkwXoW0eut9HTwmjTkjCtk876PYN8/edit?usp=sharing)

#### Lecture 8: Optical Flow

- [Video](https://www.youtube.com/watch?v=a-v5_8VGV0A)
- [Slides](https://docs.google.com/presentation/d/1guQ0hGL7tfHibiYID6gULCUO2OJJpNaWu6VYJXScdeY/edit?usp=sharing)

---------

### Week 5: Depth and ML Review

#### Lecture 9: 3D, Depth, and Stereo

- [Video](https://www.youtube.com/watch?v=AA8FEwutsVk)
- [Slides](https://docs.google.com/presentation/d/1ZaFvVx8U7hJpGqaqk4Fxjj5QU-EHt8B8zmYbK6uaEaI/edit?usp=sharing)

#### Lecture 10: Machine Learning for Computer Vision

- [Video](https://www.youtube.com/watch?v=AIL5PuvRAPI)
- [Slides](https://docs.google.com/presentation/d/1QgvrxpjVJLcYPWPVm9gXvqLjQth4um1nJpc0R00SNpg/edit?usp=sharing)

--------

### Week 6: Machine Learning and Neural Networks

#### Lecture 11: More Machine Learning for Computer Vision

- [Video](https://www.youtube.com/watch?v=3fCrfabOm8U)
- [Slides](https://docs.google.com/presentation/d/1sU-rMMkWXMuQYhjJkhPFAD7VifZnxXMBxOfevdwOOKU/edit?usp=sharing)

#### Lecture 12: Neural Networks

- [Video](https://www.youtube.com/watch?v=fXuIpJ-2MR4)
- [Slides](https://docs.google.com/presentation/d/1NLdRUsxH30tSNe46OOd3rPa-xoKFkDR-fYH8rnh0POo/edit?usp=sharing)

#### Supplementary Content:
- Introduction to PyTorch
    - [Video](https://washington.zoom.us/rec/play/EUQaMXTPPkSK0FBDO9NSA96tmDtcJs_K51BFzSIxxQaKM_sIMwf3_MPokKDSeUUMtpzwlKwsLYGYYBU.YrQPydKxfPp2W1b5)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial1%20-%20pytorch-introduction.ipynb)
- Neural Networks in PyTorch
    - [Video](https://washington.zoom.us/rec/play/CIHYnXKlJwQLdMTLlnWJpcY3vGoo1XcSj9uESV463lxZ3fjqaoK_2d62uIalmAzb8NK8IQ01hHH11KXE.pX0Z2uLsjH1xoD7a)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial1%20-%20pytorch-introduction.ipynb)

--------

### Week 7: Convolutional Neural Networks

#### Lecture 13: Convolutional Neural Networks

- [Video](https://www.youtube.com/watch?v=RnD0OFbZGbA)
- [Slides](https://docs.google.com/presentation/d/1LwTvykcPzDoAzQyAZB4cbP5Lh_czqfBAMGnBddVHbxs/edit?usp=sharing)

#### Lecture 14: Network Architectures

- [Video](https://www.youtube.com/watch?v=-XK_uMVD2CY)
- [Slides](https://docs.google.com/presentation/d/1Y5q24TUmhKTZXYVOqrcqCkHP1CMQGG1CveS8KNNztms/edit?usp=sharing)

#### Supplementary Content:
- CNNs in PyTorch
    - [Video](https://washington.zoom.us/rec/play/IiKayqa8x6D4Ra1jrXynEJF5_-sfSti9WE3OjpBITdgrH8ngJRaUscOjgrXVMrzzvjTG7XSqHfcXwz4e.8p8tANHTf7EfRA5E)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial2_cnns_in_pytorch.ipynb)

---------

### Week 8

#### Lecture 15: Semantic Segmentation

- [Video](https://www.youtube.com/watch?v=4vd8zQQb7bk&feature=youtu.be)
- [Slides](https://docs.google.com/presentation/d/1XFr96QGJFHoRr0HyydnrLntulH7vNlIQd_SHm88yLNk/edit#slide=id.g3600a767f6_1_21)

#### Lecture 16: Object Detection

- [Video](https://www.youtube.com/watch?v=7e0umTYMv_Y&feature=youtu.be)
- [Slides](https://docs.google.com/presentation/d/1CLVryBPNddEn8TwM2ngy1bHnlJC4t33OhERzVixFGj4/edit#slide=id.g3600a767f6_1_21)

#### Supplementary Content:
- Experiments with CNNs
    - [Video](https://washington.zoom.us/rec/play/ODgc3irot86ycaY0I1JAZ8ptp-27PPcRlPGoHE6kjcT7PVkiWsvmsDY6sr5kMdkSMKVMd7747CCWBjS1.yQGlCHwLGacAwJcB)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial2_cnns_in_pytorch.ipynb)
- Transfer Learning: ImageNet -> CIFAR-10
    - [Video](https://washington.zoom.us/rec/play/2QV2dYzYZLA4p2eZwNtciOFSQqW4a37yubk6djdRNAfgG_cCU4bac-Eb_xcqVmWJVEYlfO0W45zBLx8g.h48-9o9PL0bOqCTz)
    - [iPynb](https://colab.research.google.com/drive/1EBz4feoaUvz-o_yeMI27LEQBkvrXNc_4#scrollTo=X7IHgrsqd-W0)

----------

### Week 9

#### Lecture 17: Instance Segmentation
- [Video](https://www.youtube.com/watch?v=oW9qwD62Ljs)
- [Slides](https://docs.google.com/presentation/d/1mqzWsN1Zt4_e3W5NXwDDnQZvjqC99NVJndOZvI1fPck/edit#slide=id.g37ded8bff5_0_88)

#### Lecture 18: Vision and Language
- [Video](https://www.youtube.com/watch?v=6CYsaaCY_u0)
- [Slides](https://docs.google.com/presentation/d/1GsphfNerVfEoolZFxQIbAf0VdZ6ftGEzM5AUAwUewOo/edit#slide=id.g7a8786fbee_0_174)

#### Supplementary Content:
- Transfer Learning: ImageNet -> Birds
    - [Video](https://washington.zoom.us/rec/play/8RNCCJ7omCQbF1fAfrsat9AxUlkh14upJtrJc0LK2nVI9rMphMePi8bCm7PnFj8AptkBIb6A5up4BVA7.0LU7HIAsEWFqiPnU)
    - [iPynb](https://colab.research.google.com/drive/1kHo8VT-onDxbtS3FM77VImG35h_K_Lav#scrollTo=yRzPDiVzsyGz)

### Week 10

#### Lecture 19: Generative Adversarial Networks
- [Video](https://www.youtube.com/watch?v=um7jjHyFItE)
- [Slides](https://docs.google.com/presentation/d/1NgicaHQhluKQ0r39U4IWo8AtOBJUAQ2aBGCDq_DpgkA/edit?usp=sharing)

#### Lecture 20: Transformers and Vision



**Note:** due date subject to change if we haven't covered relevant material in time for the assignment.

## Final Project: ##

There is a final project worth 20% of the final grade.

Pick any area of computer vision that interests you and pursue some independent work in that area. Each project should have a significant technical component, software implementation, or large-scale study. Projects can focus on developing new techniques or tools in computer vision or applying existing tools to a new domain. If you don't have an idea you can train a classifier on birds and compete in the Kaggle competition posted on the Ed discussion board.

## Lectures ##

### Week 1: Image Basics ###

This week we cover the basics of computer vision. There's an introduction to the three levels of vision, **low-level** vision mostly concerns the pixels or groups of nearby pixels, **mid-level** vision starts to connect images to each other and the real world, and **high-level** vision connects images to semantics and meaning. There's background information on the human visual system, color, light, what an image actually is, and how it's stored in a computer. All fun stuff! Once you've learned the basics you should be ready for [Homework 0](https://github.com/pjreddie/uwimg/tree/main/src/hw0), which is mostly an introduction to the codebase we'll be using for the assignments.

#### Lecture 1: Introduction
- [Slides](https://docs.google.com/presentation/d/1VqTJEVC0gwxfY5TbINgBKyWqAmdxLYxgj_yIiphJj34/edit?usp=sharing)
- [Video](https://washington.zoom.us/rec/play/C83fxzyzYd78yhX-PElkUMeUgWe-8QOiYoF2U49pcrXqd2BBKCr6gwxVev5h5WWMn_ROJNCCt7jYt9_B.GsCgluaBokDdpycY)


#### Lecture 2: Human Vision, Color Spaces, Transforms ####
- [Slides](https://docs.google.com/presentation/d/1YBK7QkBW9t4kuZ8bJdwXLspyyeSpEJJldHvAhVcSsiM/edit?usp=sharing)
- [Video](https://www.youtube.com/watch?v=-nt80JUNwlw)

--------

### Week 2: Image Transformations ###

In week 2 we start to dive into low-level vision and image processing. You learn how to manipulate images and perform operations like resizing, sharpening, smoothing, and more. You'll apply this knowledge as you get started on [Homework 1](https://github.com/pjreddie/uwimg/tree/main/src/hw1).

#### Lecture 3: Image Coordinates, Resizing
- [Slides](https://docs.google.com/presentation/d/1ZkGgPPUzlGOdoGK6YNgiVLNouJW1ZaWzKEupDKmYM_4/edit?usp=sharing)
- [Video](https://youtu.be/hpqrDUuk7HY?t=129)

#### Lecture 4: Resizing, Filters, Convolutions
- [Slides](https://docs.google.com/presentation/d/18f0cWwS40jwbP5u37LKvM9ZaHEtRQFUKQ7MCtMdGLmA/edit?usp=sharing)
- [Video](https://youtu.be/5xdbJ7z4Nrc?t=119)

#### Supplementary Content:
- [Overview of Homework Codebase](https://washington.zoom.us/rec/play/H4Wgk8W40k1t5iS2YDoyrAgtxxKDisqtnoGzXYZ84NEYIKvLidB1tNeU4Nh3UG_sJ4yLbotPYBlXGtUr.AQhHZItzxFSBRAQR)
- [Debugging Using GDB and Valgrind](https://washington.zoom.us/rec/play/51JkwP7X_MIkl2MoAChPeGrdrdtsFJKn0TRB_yBTJby2utJXqVjET4uYjUKqHOAft1WlgVPgObvXm-Rr.0k6seTt67QxllWLF)

--------

### Week 3: Edges and Features

Time to put those convolutions to use! For week 3 we delve in to what makes images interesting, what makes them unique, how to find correspondences between images, and how to fit models with a large number of outliers in the data.

#### Lecture 5: Edges and Features

- [Video](https://www.youtube.com/watch?v=z5WSV6CXsxs)
- [Slides](https://docs.google.com/presentation/d/1_ZOtT17Ih2P-MRbWtZ8CTRQaJBz9V6-5_VA00QebiQQ/edit?usp=sharing)

#### Lecture 6: Harris, Matching, RANSAC

- [Video](https://www.youtube.com/watch?v=bn4KHa_zWuQ)
- [Slides](https://docs.google.com/presentation/d/1GLPcw-hQB1D94mOzTZKdMwAa8NKuqgih-bWl1vJS0tE/edit?usp=sharing)

-------

### Week 4: Features and Flow

#### Lecture 7: Matching, RANSAC, HOG, and SIFT

- [Video](https://www.youtube.com/watch?v=taty6lPVcmA)
- [Slides](https://docs.google.com/presentation/d/1h2Az_a28qjKvLpbkwXoW0eut9HTwmjTkjCtk876PYN8/edit?usp=sharing)

#### Lecture 8: Optical Flow

- [Video](https://www.youtube.com/watch?v=a-v5_8VGV0A)
- [Slides](https://docs.google.com/presentation/d/1guQ0hGL7tfHibiYID6gULCUO2OJJpNaWu6VYJXScdeY/edit?usp=sharing)

---------

### Week 5: Depth and ML Review

#### Lecture 9: 3D, Depth, and Stereo

- [Video](https://www.youtube.com/watch?v=AA8FEwutsVk)
- [Slides](https://docs.google.com/presentation/d/1ZaFvVx8U7hJpGqaqk4Fxjj5QU-EHt8B8zmYbK6uaEaI/edit?usp=sharing)

#### Lecture 10: Machine Learning for Computer Vision

- [Video](https://www.youtube.com/watch?v=AIL5PuvRAPI)
- [Slides](https://docs.google.com/presentation/d/1QgvrxpjVJLcYPWPVm9gXvqLjQth4um1nJpc0R00SNpg/edit?usp=sharing)

--------

### Week 6: Machine Learning and Neural Networks

#### Lecture 11: More Machine Learning for Computer Vision

- [Video](https://www.youtube.com/watch?v=3fCrfabOm8U)
- [Slides](https://docs.google.com/presentation/d/1sU-rMMkWXMuQYhjJkhPFAD7VifZnxXMBxOfevdwOOKU/edit?usp=sharing)

#### Lecture 12: Neural Networks

- [Video](https://www.youtube.com/watch?v=fXuIpJ-2MR4)
- [Slides](https://docs.google.com/presentation/d/1NLdRUsxH30tSNe46OOd3rPa-xoKFkDR-fYH8rnh0POo/edit?usp=sharing)

#### Supplementary Content:
- Introduction to PyTorch
    - [Video](https://washington.zoom.us/rec/play/EUQaMXTPPkSK0FBDO9NSA96tmDtcJs_K51BFzSIxxQaKM_sIMwf3_MPokKDSeUUMtpzwlKwsLYGYYBU.YrQPydKxfPp2W1b5)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial1%20-%20pytorch-introduction.ipynb)
- Neural Networks in PyTorch
    - [Video](https://washington.zoom.us/rec/play/CIHYnXKlJwQLdMTLlnWJpcY3vGoo1XcSj9uESV463lxZ3fjqaoK_2d62uIalmAzb8NK8IQ01hHH11KXE.pX0Z2uLsjH1xoD7a)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial1%20-%20pytorch-introduction.ipynb)

--------

### Week 7: Convolutional Neural Networks

#### Lecture 13: Convolutional Neural Networks

- [Video](https://www.youtube.com/watch?v=RnD0OFbZGbA)
- [Slides](https://docs.google.com/presentation/d/1LwTvykcPzDoAzQyAZB4cbP5Lh_czqfBAMGnBddVHbxs/edit?usp=sharing)

#### Lecture 14: Network Architectures

- [Video](https://www.youtube.com/watch?v=-XK_uMVD2CY)
- [Slides](https://docs.google.com/presentation/d/1Y5q24TUmhKTZXYVOqrcqCkHP1CMQGG1CveS8KNNztms/edit?usp=sharing)

#### Supplementary Content:
- CNNs in PyTorch
    - [Video](https://washington.zoom.us/rec/play/IiKayqa8x6D4Ra1jrXynEJF5_-sfSti9WE3OjpBITdgrH8ngJRaUscOjgrXVMrzzvjTG7XSqHfcXwz4e.8p8tANHTf7EfRA5E)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial2_cnns_in_pytorch.ipynb)

---------

### Week 8

#### Lecture 15: Semantic Segmentation

- [Video](https://www.youtube.com/watch?v=4vd8zQQb7bk&feature=youtu.be)
- [Slides](https://docs.google.com/presentation/d/1XFr96QGJFHoRr0HyydnrLntulH7vNlIQd_SHm88yLNk/edit#slide=id.g3600a767f6_1_21)

#### Lecture 16: Object Detection

- [Video](https://www.youtube.com/watch?v=7e0umTYMv_Y&feature=youtu.be)
- [Slides](https://docs.google.com/presentation/d/1CLVryBPNddEn8TwM2ngy1bHnlJC4t33OhERzVixFGj4/edit#slide=id.g3600a767f6_1_21)

#### Supplementary Content:
- Experiments with CNNs
    - [Video](https://washington.zoom.us/rec/play/ODgc3irot86ycaY0I1JAZ8ptp-27PPcRlPGoHE6kjcT7PVkiWsvmsDY6sr5kMdkSMKVMd7747CCWBjS1.yQGlCHwLGacAwJcB)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial2_cnns_in_pytorch.ipynb)
- Transfer Learning: ImageNet -> CIFAR-10
    - [Video](https://washington.zoom.us/rec/play/2QV2dYzYZLA4p2eZwNtciOFSQqW4a37yubk6djdRNAfgG_cCU4bac-Eb_xcqVmWJVEYlfO0W45zBLx8g.h48-9o9PL0bOqCTz)
    - [iPynb](https://colab.research.google.com/drive/1EBz4feoaUvz-o_yeMI27LEQBkvrXNc_4#scrollTo=X7IHgrsqd-W0)

----------

### Week 9

#### Lecture 17: Instance Segmentation
- [Video](https://www.youtube.com/watch?v=oW9qwD62Ljs)
- [Slides](https://docs.google.com/presentation/d/1mqzWsN1Zt4_e3W5NXwDDnQZvjqC99NVJndOZvI1fPck/edit#slide=id.g37ded8bff5_0_88)

#### Lecture 18: Vision and Language
- [Video](https://www.youtube.com/watch?v=6CYsaaCY_u0)
- [Slides](https://docs.google.com/presentation/d/1GsphfNerVfEoolZFxQIbAf0VdZ6ftGEzM5AUAwUewOo/edit#slide=id.g7a8786fbee_0_174)

#### Supplementary Content:
- Transfer Learning: ImageNet -> Birds
    - [Video](https://washington.zoom.us/rec/play/8RNCCJ7omCQbF1fAfrsat9AxUlkh14upJtrJc0LK2nVI9rMphMePi8bCm7PnFj8AptkBIb6A5up4BVA7.0LU7HIAsEWFqiPnU)
    - [iPynb](https://colab.research.google.com/drive/1kHo8VT-onDxbtS3FM77VImG35h_K_Lav#scrollTo=yRzPDiVzsyGz)

### Week 10

#### Lecture 19: Generative Adversarial Networks
- [Video](https://www.youtube.com/watch?v=um7jjHyFItE)
- [Slides](https://docs.google.com/presentation/d/1NgicaHQhluKQ0r39U4IWo8AtOBJUAQ2aBGCDq_DpgkA/edit?usp=sharing)

#### Lecture 20: Transformers and Vision



**Note:** due date subject to change if we haven't covered relevant material in time for the assignment.

## Final Project: ##

There is a final project worth 20% of the final grade.

Pick any area of computer vision that interests you and pursue some independent work in that area. Each project should have a significant technical component, software implementation, or large-scale study. Projects can focus on developing new techniques or tools in computer vision or applying existing tools to a new domain. If you don't have an idea you can train a classifier on birds and compete in the Kaggle competition posted on the Ed discussion board.

## Lectures ##

### Week 1: Image Basics ###

This week we cover the basics of computer vision. There's an introduction to the three levels of vision, **low-level** vision mostly concerns the pixels or groups of nearby pixels, **mid-level** vision starts to connect images to each other and the real world, and **high-level** vision connects images to semantics and meaning. There's background information on the human visual system, color, light, what an image actually is, and how it's stored in a computer. All fun stuff! Once you've learned the basics you should be ready for [Homework 0](https://github.com/pjreddie/uwimg/tree/main/src/hw0), which is mostly an introduction to the codebase we'll be using for the assignments.

#### Lecture 1: Introduction
- [Slides](https://docs.google.com/presentation/d/1VqTJEVC0gwxfY5TbINgBKyWqAmdxLYxgj_yIiphJj34/edit?usp=sharing)
- [Video](https://washington.zoom.us/rec/play/C83fxzyzYd78yhX-PElkUMeUgWe-8QOiYoF2U49pcrXqd2BBKCr6gwxVev5h5WWMn_ROJNCCt7jYt9_B.GsCgluaBokDdpycY)


#### Lecture 2: Human Vision, Color Spaces, Transforms ####
- [Slides](https://docs.google.com/presentation/d/1YBK7QkBW9t4kuZ8bJdwXLspyyeSpEJJldHvAhVcSsiM/edit?usp=sharing)
- [Video](https://www.youtube.com/watch?v=-nt80JUNwlw)

--------

### Week 2: Image Transformations ###

In week 2 we start to dive into low-level vision and image processing. You learn how to manipulate images and perform operations like resizing, sharpening, smoothing, and more. You'll apply this knowledge as you get started on [Homework 1](https://github.com/pjreddie/uwimg/tree/main/src/hw1).

#### Lecture 3: Image Coordinates, Resizing
- [Slides](https://docs.google.com/presentation/d/1ZkGgPPUzlGOdoGK6YNgiVLNouJW1ZaWzKEupDKmYM_4/edit?usp=sharing)
- [Video](https://youtu.be/hpqrDUuk7HY?t=129)

#### Lecture 4: Resizing, Filters, Convolutions
- [Slides](https://docs.google.com/presentation/d/18f0cWwS40jwbP5u37LKvM9ZaHEtRQFUKQ7MCtMdGLmA/edit?usp=sharing)
- [Video](https://youtu.be/5xdbJ7z4Nrc?t=119)

#### Supplementary Content:
- [Overview of Homework Codebase](https://washington.zoom.us/rec/play/H4Wgk8W40k1t5iS2YDoyrAgtxxKDisqtnoGzXYZ84NEYIKvLidB1tNeU4Nh3UG_sJ4yLbotPYBlXGtUr.AQhHZItzxFSBRAQR)
- [Debugging Using GDB and Valgrind](https://washington.zoom.us/rec/play/51JkwP7X_MIkl2MoAChPeGrdrdtsFJKn0TRB_yBTJby2utJXqVjET4uYjUKqHOAft1WlgVPgObvXm-Rr.0k6seTt67QxllWLF)

--------

### Week 3: Edges and Features

Time to put those convolutions to use! For week 3 we delve in to what makes images interesting, what makes them unique, how to find correspondences between images, and how to fit models with a large number of outliers in the data.

#### Lecture 5: Edges and Features

- [Video](https://www.youtube.com/watch?v=z5WSV6CXsxs)
- [Slides](https://docs.google.com/presentation/d/1_ZOtT17Ih2P-MRbWtZ8CTRQaJBz9V6-5_VA00QebiQQ/edit?usp=sharing)

#### Lecture 6: Harris, Matching, RANSAC

- [Video](https://www.youtube.com/watch?v=bn4KHa_zWuQ)
- [Slides](https://docs.google.com/presentation/d/1GLPcw-hQB1D94mOzTZKdMwAa8NKuqgih-bWl1vJS0tE/edit?usp=sharing)

-------

### Week 4: Features and Flow

#### Lecture 7: Matching, RANSAC, HOG, and SIFT

- [Video](https://www.youtube.com/watch?v=taty6lPVcmA)
- [Slides](https://docs.google.com/presentation/d/1h2Az_a28qjKvLpbkwXoW0eut9HTwmjTkjCtk876PYN8/edit?usp=sharing)

#### Lecture 8: Optical Flow

- [Video](https://www.youtube.com/watch?v=a-v5_8VGV0A)
- [Slides](https://docs.google.com/presentation/d/1guQ0hGL7tfHibiYID6gULCUO2OJJpNaWu6VYJXScdeY/edit?usp=sharing)

---------

### Week 5: Depth and ML Review

#### Lecture 9: 3D, Depth, and Stereo

- [Video](https://www.youtube.com/watch?v=AA8FEwutsVk)
- [Slides](https://docs.google.com/presentation/d/1ZaFvVx8U7hJpGqaqk4Fxjj5QU-EHt8B8zmYbK6uaEaI/edit?usp=sharing)

#### Lecture 10: Machine Learning for Computer Vision

- [Video](https://www.youtube.com/watch?v=AIL5PuvRAPI)
- [Slides](https://docs.google.com/presentation/d/1QgvrxpjVJLcYPWPVm9gXvqLjQth4um1nJpc0R00SNpg/edit?usp=sharing)

--------

### Week 6: Machine Learning and Neural Networks

#### Lecture 11: More Machine Learning for Computer Vision

- [Video](https://www.youtube.com/watch?v=3fCrfabOm8U)
- [Slides](https://docs.google.com/presentation/d/1sU-rMMkWXMuQYhjJkhPFAD7VifZnxXMBxOfevdwOOKU/edit?usp=sharing)

#### Lecture 12: Neural Networks

- [Video](https://www.youtube.com/watch?v=fXuIpJ-2MR4)
- [Slides](https://docs.google.com/presentation/d/1NLdRUsxH30tSNe46OOd3rPa-xoKFkDR-fYH8rnh0POo/edit?usp=sharing)

#### Supplementary Content:
- Introduction to PyTorch
    - [Video](https://washington.zoom.us/rec/play/EUQaMXTPPkSK0FBDO9NSA96tmDtcJs_K51BFzSIxxQaKM_sIMwf3_MPokKDSeUUMtpzwlKwsLYGYYBU.YrQPydKxfPp2W1b5)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial1%20-%20pytorch-introduction.ipynb)
- Neural Networks in PyTorch
    - [Video](https://washington.zoom.us/rec/play/CIHYnXKlJwQLdMTLlnWJpcY3vGoo1XcSj9uESV463lxZ3fjqaoK_2d62uIalmAzb8NK8IQ01hHH11KXE.pX0Z2uLsjH1xoD7a)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial1%20-%20pytorch-introduction.ipynb)

--------

### Week 7: Convolutional Neural Networks

#### Lecture 13: Convolutional Neural Networks

- [Video](https://www.youtube.com/watch?v=RnD0OFbZGbA)
- [Slides](https://docs.google.com/presentation/d/1LwTvykcPzDoAzQyAZB4cbP5Lh_czqfBAMGnBddVHbxs/edit?usp=sharing)

#### Lecture 14: Network Architectures

- [Video](https://www.youtube.com/watch?v=-XK_uMVD2CY)
- [Slides](https://docs.google.com/presentation/d/1Y5q24TUmhKTZXYVOqrcqCkHP1CMQGG1CveS8KNNztms/edit?usp=sharing)

#### Supplementary Content:
- CNNs in PyTorch
    - [Video](https://washington.zoom.us/rec/play/IiKayqa8x6D4Ra1jrXynEJF5_-sfSti9WE3OjpBITdgrH8ngJRaUscOjgrXVMrzzvjTG7XSqHfcXwz4e.8p8tANHTf7EfRA5E)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial2_cnns_in_pytorch.ipynb)

---------

### Week 8

#### Lecture 15: Semantic Segmentation

- [Video](https://www.youtube.com/watch?v=4vd8zQQb7bk&feature=youtu.be)
- [Slides](https://docs.google.com/presentation/d/1XFr96QGJFHoRr0HyydnrLntulH7vNlIQd_SHm88yLNk/edit#slide=id.g3600a767f6_1_21)

#### Lecture 16: Object Detection

- [Video](https://www.youtube.com/watch?v=7e0umTYMv_Y&feature=youtu.be)
- [Slides](https://docs.google.com/presentation/d/1CLVryBPNddEn8TwM2ngy1bHnlJC4t33OhERzVixFGj4/edit#slide=id.g3600a767f6_1_21)

#### Supplementary Content:
- Experiments with CNNs
    - [Video](https://washington.zoom.us/rec/play/ODgc3irot86ycaY0I1JAZ8ptp-27PPcRlPGoHE6kjcT7PVkiWsvmsDY6sr5kMdkSMKVMd7747CCWBjS1.yQGlCHwLGacAwJcB)
    - [iPynb](https://github.com/pjreddie/uwimg/blob/main/tutorial2_cnns_in_pytorch.ipynb)
- Transfer Learning: ImageNet -> CIFAR-10
    - [Video](https://washington.zoom.us/rec/play/2QV2dYzYZLA4p2eZwNtciOFSQqW4a37yubk6djdRNAfgG_cCU4bac-Eb_xcqVmWJVEYlfO0W45zBLx8g.h48-9o9PL0bOqCTz)
    - [iPynb](https://colab.research.google.com/drive/1EBz4feoaUvz-o_yeMI27LEQBkvrXNc_4#scrollTo=X7IHgrsqd-W0)

----------

### Week 9

#### Lecture 17: Instance Segmentation
- [Video](https://www.youtube.com/watch?v=oW9qwD62Ljs)
- [Slides](https://docs.google.com/presentation/d/1mqzWsN1Zt4_e3W5NXwDDnQZvjqC99NVJndOZvI1fPck/edit#slide=id.g37ded8bff5_0_88)

#### Lecture 18: Vision and Language
- [Video](https://www.youtube.com/watch?v=6CYsaaCY_u0)
- [Slides](https://docs.google.com/presentation/d/1GsphfNerVfEoolZFxQIbAf0VdZ6ftGEzM5AUAwUewOo/edit#slide=id.g7a8786fbee_0_174)

#### Supplementary Content:
- Transfer Learning: ImageNet -> Birds
    - [Video](https://washington.zoom.us/rec/play/8RNCCJ7omCQbF1fAfrsat9AxUlkh14upJtrJc0LK2nVI9rMphMePi8bCm7PnFj8AptkBIb6A5up4BVA7.0LU7HIAsEWFqiPnU)
    - [iPynb](https://colab.research.google.com/drive/1kHo8VT-onDxbtS3FM77VImG35h_K_Lav#scrollTo=yRzPDiVzsyGz)

### Week 10

#### Lecture 19: Generative Adversarial Networks
- [Video](https://www.youtube.com/watch?v=um7jjHyFItE)
- [Slides](https://docs.google.com/presentation/d/1NgicaHQhluKQ0r39U4IWo8AtOBJUAQ2aBGCDq_DpgkA/edit?usp=sharing)

#### Lecture 20: Transformers and Vision


