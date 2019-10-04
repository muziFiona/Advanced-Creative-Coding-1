# Advanced Creative Coding 1

## 2019-2020

Professor Mick Grierson

## Introduction

Welcome to Advanced Creative Coding 1. In this course we look at a range of methods for working with media through programming in ways that are specifically useful in Creative Computing contexts. We also refine and develop our understanding of core programming concepts and computatonal techniques used by artists and those in the creative industries generally.

The course is divided in to 2-week blocks that focus on specific areas, exploring them in ways that relate to certain types of coding expertise and technical approaches.

## Schedule:

Sound and Signal processing - Week 1 and 2
 - Looking at waveforms and making basic synths
 - Using filters and waveforms for more altering sounds
 - Building a drum machine
 - Creating soundscapes
 - Programming knowledge - basic structure, variables, arrays and conditionals

2D graphics - Week 3 and 4

 - Image representations
 - Image filters / convolution filters
 - Creating 2D patterns with polar coordinates and loops
Using other algorithms for generating patterns (fractals, packing systems etc.)
 - Programming knowledge - intermediate structure,  more arrays, more conditionals, for loops, polar coordinates, 2D vectors

3D graphics - Week 5 and 6

 - Creating a 3D engine from scratch
 - Creating 3D geometry from scratch
 - Fixed function pipeline approaches
 - Shading and lighting
 - Programming knowledge - 3D vectors, creating perspective, using matrices for transformations


Shaders - Week 7 and 8

 - Fragments shaders
 - Creating basic shapes, lines and noise
 - Vertex Shaders
 - Creating geometry
 - Modifying and lighting Geometry
 - Programming knowledge - GLSL concepts, variables and structure, contemporary graphics pipeline


Basic Machine Learning and information retrieval for Real-time interaction
 - Sound and Image Features
 - Classification
 - Regression


Assessment for this course is through practical and written examination

## How will we learn

- Explore periodic phenomena and creative computing concepts through interactive programming
- Build simple applications that just make sounds,
- Then extend this to moving images
  - John Whitney approach
  - <https://www.youtube.com/watch?v=5eMSPtm6u5Y>

--

## How we will learn

- Explore application ideas slowly
- Incorporate ideas from sound, then apply these to graphics
- Look at a range of image and video approaches (3D etc.)
- Generate artworks as outcomes.
- Move back and forth between ideas and technical concepts
- Gently introduce and refresh technical topics (Variables, Conditionals, Loops, Functions, Objects, objects, types, functions, conditionals, loops.
- Explore through creative application / sound and image making
  - If think you already know what you’re doing, try it this way instead. It’s good fun :-)

---

## Getting started using Maximilian in JavaScript

- www.mimicproject.com _REQUIRES CHROME_
  - Start here
  - https://mimicproject.com/guides/maximJS
  For hot takes on JavaScript, go here and drink it in :-)
  - https://www.w3schools.com/js/default.asp
  And for ES6, which we will also be using:
  - https://www.w3schools.com/js/js_es6.asp


## C++ on Windows

- Windows 10, Visual Studio 2019
  - Windows 10: free with any recent windows license
  - Community Edition - free. Installed on PCs

--

## C++ on MacOS

- El Capitan, High Sierra,... *NOT* Catalina
  - Free
  - Xcode - also free

---

## Download Maximilian

- Designed to make it easy to learn how to do sound and music in C++
- Good for beginners
- Powerful enough to be used in commercial applications
- Free

--

## C++ Track - Download Maximilian

- Maximilian is on GITHUB
- <https://github.com/micknoise/Maximilian>
- use git to clone the repository (you will need to setup your git)
- git@github.com:micknoise/Maximilian.git
- or just download it from the website

--
---

# Oscillation

- Fundamental basis of all periodic phenomena
- Not just useful for sounds, but also images
- `$sin(x)$` function creates a sine wave
- This is a wave, or waveform
- `maxiOsc` object

## Air moving

- Wave goes above 0. --> Speaker moves forward
- Wave goes below 0. --> Speaker moves backward

_The position of the speaker is the PHASE of the wave._

## Frequency

Waves don’t just have a phase. They also have _frequency_

- how often they move up and down each second
- waves that oscillate more than around 20 times per second take on a quality of continuos sounds, and not separate pulses
- Interestingly, the same is roughly true for images (fps)
- Oscillations below 20hz are called “Low Frequency” (LFOs)

--

## All about time

- Both sound and video are time based
- Interesting fusion occurs around 20 Hz
- Getting things to happen at the right time is an important computational problem

--
## Amplitude

Waves also have an amplitude.

- This is how much they move up and down.
- In the real world, this is how much air they are moving.
- In the computer, we have a different situation.

## Adding sounds together

- In the computer, the audio output should vary between -1 and 1
- This is a linear measurement, not in dB - i.e. not logarithmic
- When you add sounds, they combine linearly and can create distortion
- `$1+1=2$` ...not so great for your speakers. But sounds nice.


## Adding sounds together

- When we add sounds together, strange things happen
- The sounds interfere with each other
  - Beating
  - Amplitude modulation

## Recording your output

- Maximilian can record your output to a .wav file automatically
- You can listen back to the audio and use it in your projects

# Session #1 Practical

Work through the first few examples.

Using at least 4 oscillators, create a continuous, drone-based sound texture or sound bed using procedural C++ audio.

Use two of the oscillators to control parameters of the other two oscillators. Try to use a filter.

Make the sound texture vary continuously over a period of 1 minute through the use of low-frequency oscillators, so that the sound texture develops over the entire period.
