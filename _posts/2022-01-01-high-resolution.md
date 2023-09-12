---
layout: publication
title: "High-Resolution Spectral Analysis and Signal Segregation Using the Polyphase Channelizer"
short_title: "Polyphase Channelizer"
tags: Spectrum-Sensing
cover: /assets/images/pubpic/asilomar.png
authors: "Richard Bell, Radhika Mathuria, Fred Harris, Peter Gerstoft, Dinesh Bharadia"
conference: "Asilomar 2022"
paper: https://wcsng.ucsd.edu/channogram/
---

The windowed fast Fourier transform (FFT) is the ubiquitous transform for spectral analysis. We will show how the polyphase channelizer can be used to replace the FFT for fundamental spectrum estimates such as Welch’s power spectral density (PSD) and the short time Fourier transform (STFT) based spectrogram. We refer to the polyphase channelizer equivalents of these respectively as the cPSD and the Channogram. It will be shown that the spectral resolution of the cPSD and Channogram improves upon the well established FFT based estimators for a given FFT length while introducing minimal processing overhead. We will then introduce Parseval’s theorem equivalent for the polyphase channelizer. Finally it will be shown that the polyphase channelizer approach leads to straight forward signal segregation when signals of random and unknown center frequencies are encountered.