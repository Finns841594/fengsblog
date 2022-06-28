---
toc: true
layout: post
description: Quesionnaire of the lesson 4
categories: [markdown]
title: Questionnaire 04
---

1. How is a grayscale image represented on a computer? How about a color image?
A grayscale image is stored as a matrix with same columns and rows as the resolution size. Each number in this matrix is ranged within 0~255, which represents the darkness of the pixel. A color image has three matrix which stored the information of the image by three channels: red, green, blue.

2. How are the files and folders in the 'MNIST_SAMPLE' dataset structured? Why?
The 'MNIST' datasets follows a common layout for machine learning datasets: seperate folders for the trainning set and the validation set(and/or test set).

3. Explain how the "pixel similarity" approach to classifying digits works.
Based on the matrix we mentioned for the question one. We assume that the image of a number should have similar gray pixel distribution as other images of the same number. So we caculate the average number of the matrix which presents the images of a number as a 'standard', when we classifying a test image, we compare the piexel number of it to our 'standard', and give the inference result based on the similarity.

4. What is a list comprehension? Create one now that selects odd numbers from a list and doubles them.