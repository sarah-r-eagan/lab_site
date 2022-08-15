---
authors:
- zc
categories:
- research
date: "2020-08-13T00:00:00Z"
draft: false
featured: true
image:
  caption: null
  focal_point: ""
  placement: 2
  preview_only: false
lastmod: "2020-08-13T00:00:00Z"
projects: []
subtitle: ""
summary: We can teach the computer to read people's minds based on their eye movements.
tags:
- deep learning
- eye tracking
title: Decoding Eye Movement Data
---

Imagine a world where a computer could determine what you were thinking about by simply monitoring your eye movements. Scary, right? Well it turns out that if you have individuals look at the same image, but ask them to evaluate different characteristics of the image (e.g., _determine the age of the individuals in the image_, or _name the individuals in the image_.), the scan paths created by their eye movements have been shown to visibly differ between tasks. We're exploring the most efficient and effective methods for making that happen! (But don't worry, mind-reading robots are still very far off.)

We are working to teach the computer to use eye movement data to determine what an individual is thinking. More specifically, in this project we had participants search, rate, or memorize scene images while their eye movements were recorded. Then we fed a deep convolutional neural network the eye movement data formatted as a timeline (coordinates and pupil size), and as an image snapshot of each trial which was then categorized. Typically, classification models are built on a cognitive or neurobiological foundation. At the moment, we are interested in exploring the ability of a black box model to decode eye movement data using no explicit theoretical justiciation in the development of our model. Our models were developed using the deep learning toolbox, [DeLINEATE](http://delineate.it), developed by members of Dr. Johnson's lab. Moving forward, we will continue to explore this neural network approach to decoding eye movement data, and other related questions concerning both theoretical and applied purposes.

## Collaborators
* [Matt Johnson, PhD](/author/matthew-r.-johnson-phd/)
* [Mike Dodd, PhD](/author/michael-d.-dodd-phd/)
* Karl Kuntzelman, PhD

## Status
The manuscript for this project is currently under review.

## Pre Print
Cole, Z. J., Kuntzelman, K., Dodd, M. D., & Johnson, M. (2020, September 23). Convolutional neural networks can decode eye movement data: A black box approach to predicting task from eye movements. [https://doi.org/10.31234/osf.io/5a6jm](https://doi.org/10.31234/osf.io/5a6jm)

## Published Abstract
This work has been presented at the [Vision Sciences Society Annual Convention](https://www.visionsciences.org/) in 2019. The conference proceedings were published in the _Journal of Vision_. Find the abstract [here](https://jov.arvojournals.org/article.aspx?articleid=2751172).
