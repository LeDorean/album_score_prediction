# Album Score Prediction

## Project Summary


This project is aimed at predicting the key characteristics of what makes an album a critical success.
The information on the characteristics was retrieved through Spotify's own method of evaluation. While these metrics can seem a bit arbitrary, it's one of the few methods of quantifying some key musical characteristics, and the abundance of information (directly proportionate to the quantity of music available on the platform) makes it perfect for a study on what makes a song successful.
The information on album rating was obtained with Pitchfork's reviews. Pitchfork began as an online indie music magazine but now reviews mainstream music as well. They are know for giving notoriously harsh reviews and they review albums on a scale of 0 to 10.


## Contents of the repository

This repository contains 5 notebooks with the following contents:

- Pitchfork Webscraping
- Spotify API Calls
- Data Cleaning
- Exploratory Data Analysis
- Modeling for Predicting Pitchfork Score

The data used comes from a combination of a Kaggle dataset containing the reviews of over 18000 albums since 1997 and audio features retrieved through Spotify's API.

Pitchfork data can be downloaded from here: https://www.kaggle.com/nolanbconaway/pitchfork-data

## Audio Features

Spotify uses a relatively sophisticated set of original values along with traditional ones (such as key and tempo) to describe every song on the platform. The features are the following:

- duration_ms: The duration of the track in milliseconds.
- key:	The estimated overall key of the track. Integers map to pitches using standard Pitch Class notation . E.g. 0 = C, 1 = C♯/D♭, 2 = D, and so on. If no key was detected, the value is -1.
- mode:	Mode indicates the modality (major or minor) of a track, the type of scale from which its melodic content is derived. Major is represented by 1 and minor is 0.
- time_signature: An estimated overall time signature of a track. The time signature (meter) is a notational convention to specify how many beats are in each bar (or measure).
- acousticness: A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
- danceability: Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
- energy Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy.
- instrumentalness: Predicts whether a track contains no vocals. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content.
- liveness: Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live.
- loudness: The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks.
- speechiness: Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value.
- valence: A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track.
- tempo: The overall estimated tempo of a track in beats per minute (BPM). 
