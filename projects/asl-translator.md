---
title: ASL Translator - Sprint 3 Project
layout: page
---

## Inspiration

Sign Language is an efficient way of communicating for people with disabilities. But people who don't understand sign language can find it quite difficult to comprehend it and communicate with them.

In today's day and age of communication via web conferencing, the communication can become even more difficult without having a translator around to help people assist in ensuring communication.

## What it does

ASL-Translator is a video conferencing application built using webrtc and tensorflow.js that detects sign language and converts it into English text. The web cam stream is set up between two people using socket.io and the stream which detects sign language sends the frames to a machine learning model using tf.js and it helps detect the signs and these get converted into text. A grammar API analyzes the collection of letters and converts them into meaningful words.

## How we built it

We have created a WebRTC based video conferencing application using SocketJS and WebRTC. We trained a machine learning model using CNN with American Sign Language Dataset from Kaggle in Python. And then converted this into TensorFlowJS model using TFJS converter. Then we captured the frames from the video stream and sent them to the TFJS model to predict the sign from the frame and send them as a collection of letters which are then displayed on the screen to the person who isnt using the sign language as a means to understand the sign language.

## Challenge we ran into

The biggest challenge was definitely implementing TF.JS by first converting the Python based model into Javascript and then capturing the frames and analyzing them. Setting up web rtc connection with Flask also appeared to be quite challenging.

## Try it out

[ASL Translator repo](https://github.com/nathanlm511/ASLTranslator)