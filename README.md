# Starbucks-Capstone-Challenge
Capstone challenge Udacity Data Science

## Table of contents

- [Blog](#medium-blog)
- [Installation](#installation)
- [Project motivation](#project-motivation)
- [Data Source](#data-source)
- [File descriptions](#file-descriptions)
- [Results](#results)
- [Author](#Author)

## Medium Blog 

https://data-clash.medium.com/starbucks-capstone-challenge-5aecf64763e9 

## Installation

The code in the project can be executed using Anaconda distribution of Python ver 3.x and does not require any additional scripts.

## Project motivation

Explore Starbucks data and create a model to predict member action on getting an offer. 

## Data Source

The program used to create the data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers.
Each person in the simulation has some hidden traits that influence their purchasing patterns and are associated with their observable traits. People produce various events, including receiving offers, opening offers, and making purchases.

As a simplification, there are no explicit products to track. Only the amounts of each transaction or offer are recorded.
There are three types of offers that can be sent: buy-one-get-one (BOGO), discount, and informational. In a BOGO offer, a user needs to spend a certain amount to get a reward equal to that threshold amount. In a discount, a user gains a reward equal to a fraction of the amount spent. In an informational offer, there is no reward, but neither is there a requisite amount that the user is expected to spend. Offers can be delivered via multiple channels.

The basic task is to use the data to identify which groups of people are most responsive to each type of offer, and how best to present each type of offer.

<br>**profile.json**
<br>Rewards program users (17000 users x 5 fields)
<br>gender: (categorical) M, F, O, or null
<br>age: (numeric) missing value encoded as 118
<br>id: (string/hash)
<br>became_member_on: (date) format YYYYMMDD
<br>income: (numeric)

<br>**portfolio.json**
<br>Offers sent during 30-day test period (10 offers x 6 fields)
<br>reward: (numeric) money awarded for the amount spent
<br>channels: (list) web, email, mobile, social
<br>difficulty: (numeric) money required to be spent to receive reward
<br>duration: (numeric) time for offer to be open, in days
<br>offer_type: (string) bogo, discount, informational
<br>id: (string/hash)

<br>**transcript.json**
<br>Event log (306648 events x 4 fields)
<br>person: (string/hash)
<br>event: (string) offer received, offer viewed, transaction, offer completed
<br>value: (dictionary) different values depending on event type
<br>offer id: (string/hash) not associated with any "transaction"
<br>amount: (numeric) money spent in "transaction"
<br>reward: (numeric) money gained from "offer completed"
<br>time: (numeric) hours after start of test

## File descriptions
<br>There are 4 files available in the project
<br>1. Readme.md 
<br>2. Starbuck_Capstone.ipynb (the python Notebook)
<br>3. Starbuck_Capstone.html (HTML page for quick viewing)
<br>4. data (transcript.json | profile.json | portfolio.json)
<br>5. pic1.png and pic2.png for the notebook instructions

## Author

Anuja Jadhav
- https://github.com/data-clash/
- www.linkedin.com/in/anuja-jadhav-80632a54
- anuja.a.jadhav@gmail.com
