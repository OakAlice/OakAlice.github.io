---
layout: post
title: "So What Actually Do You Do For Work?"
date: 2024-10-27
categories: [PhD, Accelerometry]
---

## Like a Sports Watch for Animals
I’ve told my mum to tell her friends I build sports watches for wild animals. While not entirely true — for one, it’s generally a collar, not a watch — in most cases, this answer is close enough. Similar to your trusty FitBit or Garmin or AppleWatch, I use collars to track animal sleep and steps, activities, energy expenditure, and even try to estimate stress (“Being chased by a lion delayed your recovery! Try taking it easy tomorrow.”). Unlike human sports watches, however, animal data can be used for more than just humble-bragging on Strava. A full activity history, integrated with GPS, can be used to develop detailed maps with behaviour and movement across space and time for each collared animal. We can see where they slept, for how long, which trees they climbed, and whether they fed there, the distance they travelled, and at what speed they went; as well as every other little thing they did. In a time of increasing biodiversity loss due to land clearing, urbanisation, and dwindling natural resources, there is an increasing need for high-resolution technologies to understand and embed individuals within the context of their local, as well as regional and ecosystem-level environment. Accelerometry, a kind of sports watch for animals, enables us to do this.

Technically, I’m not the one who actually builds these collars either. I’m part of a larger research group, the ‘Biomechanics and Biorobotics Lab’ at the University of the Sunshine Coast, Australia, and I mainly do the AI bit. We have two brilliant engineers who build our satellite and blue-tooth enabled 9-axis accelerometer timed drop-off collars (if you don’t know what that means, it just means the collars are really cool). Our postdoc is working on using the magnetometers and GPS to develop high-resolution dead-reckoning movement pathways. The dedicated ecologists, PhD, honours, and undergraduate students, ask the ecological questions, hunt down animals, secure near-mythically difficult ethical approval, then integrate the data with the animal physiology. Although I’m involved with and enjoy all the stages of this shared project (e.g., see images below, out on fieldwork), my main job is to turn the collar accelerometer data into meaningful behavioural histories.

<div style="display: flex; justify-content: space-between; align-items: center;">
  <div style="text-align: center;">
    <img src="https://github.com/user-attachments/assets/24b67955-cd32-4601-9eb6-dfbc695108db" alt="Me with koala" style="width: 200px;"/>
    <p><em>Koala catching during my honours year (2022)</em></p>
  </div>
  <div style="text-align: center;">
    <img src="https://github.com/user-attachments/assets/01900146-11e7-41e3-bf7c-def40b7e01a2" alt="Me with joey" style="width: 200px;"/>
    <p><em>Playing with a joey at our Roma kangaroo research site (2023)</em></p>
  </div>
</div>

## Why A Biologist is Doing A PhD in Machine Learning
Accelerometers and gyroscopes measure changes in instantaneous acceleration multiple times per second, capturing detailed movement data often represented as a time-series signal resembling a soundwave. These devices are practically ubiquitous, found in rockets, cars, smartphones, and, of course, sports watches, with the signals providing insights into the behaviour of any object the accelerometer is attached to. Discreet, replicable movements (e.g., raising an arm, taking a step, etc.) create recognisable patterns in the data. By identifying these patterns, we can then recreate exactly what the wearer did. Because these devices are deployed for weeks to months at a time, collecting several gigabytes of movement data, finding all those patterns manually would take too long. Instead, we classify the behaviours using machine learning.

Machine learning is a branch of AI that involves using models that can learn without being explicitly taught. In this case, we typically use supervised categorisation models, which independently learn to identify the characteristics of each behaviour by analysing labelled examples, and then find those same characteristics in new, unlabelled, data to predict behaviours. Making the models find the right behaviours, quickly, reliably, and across many different individuals, datasets, and species is my responsibility. Doing it in a systematised and rigorous way is the focus of my PhD.

Using machine learning to detect specific fine-scale behaviours in animal accelerometer data is not new. First pioneered in the early 2000s and subsequently implemented on over 250 species, we are said to currently be in the golden age of “biologging”. As with all golden ages, this means it is also the age of method discovery and experimentation. Despite machine learning accelerometry having been used in hundreds of published studies, there is, as yet, no widely accepted, rigorously verified, single workflow for its implementation . Each new research group has been developing custom approaches; independently inventing, reinventing, and modifying this wheel for each dataset and classification goal. Some of the existing solutions work better than others, most were developed to solve a one-off problem with low transferability to new scenarios, many—unfortunately—are not rigorously verified or documented. 

Machine learning, as powerful as it can be when it works, often is quite hard. Decisions can be far from intuitive, jargon is dense, code is king, and totally useless models masquerade as perfect. Breaking down the difficult bits, combining the best of it, discarding the worst, and wrapping it all up into a nice piece of software is the aim of my PhD. My point of difference is that I aim not to just implement machine learning to solve an ecological question, but to understand the analysis on a deeper level, so that we can make it better. Every species through a single, customisable, workflow. One program, too easy.

## After the Thesis
When I left my job as a data analyst at an ecology consultancy to pursue this PhD, the people I worked with thought I was giving up a perfectly good conservation job to pursue blue-sky research that will never make an impact. I respectfully disagree with them. Already accelerometry has revolutionised the study of animal behaviour in academia and I believe it has potential for industry and government too. I believe accelerometry will do for behaviour what GPS did for movement, and when it is as easy to implement and interpret as GPS, will become equally as widespread.

For instance, in habitat assessment before land clearing, high-resolution GPS and accelerometry can provide more than presence/absence or telemetry. These technologies enable targeted, precision conservation by quantifying specific habitat usage, identifying corridors, and critical zones. Following wildlife rehabilitation, accelerometry could be invaluable for assessing the welfare and normalcy of animals post-release, monitoring their adjustment to the wild. This fine-scale approach also allows us to understand populations on an individual level, which could play a role in understanding decision-making in threat scenarios, such as road crossings, and informing the development of smarter conservation infrastructure.

While in the day-to-day of my PhD, I spend a lot of time in the nerdy data weeds joyously counting beans, in the long term, I, like all PhD students, hope that my research can be a brick higher in the stack of making the world a better place. My goal is to democratise the use of this amazing high-resolution biologging technology for the good of researchers and wild animals everywhere. 

For a real-world example of how this technology can be used for understanding koala-vehicle collisions, see my honours research with koalas in South East Queensland (not written yet but will put a link here when it is).
