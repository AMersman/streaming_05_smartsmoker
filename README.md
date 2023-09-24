# streaming_05_smartsmoker
# Ashley Mersman
## This is module 5 from the Streaming Class at NWMSU. 
## 09/20/2023

# Overview 
This project creates a producer to send messages representing 3 temperatures (smoker, FoodA, FoodB) on three channels respectively. Each is sent to a different consumer queue using RabbitMQ. 

# Data
The temperature measurements are rows from the smoker-temp.csv that can be found in this repository. 

# Requirements
Git
Python 3.11
RabbitMQ Server
Virtual Environment 
    .venv
    source .venv/bin/activate
Pika
    pip install pika

# Run the Code
Navigate to the repo containg the code and activate a virutal environment. Run the producer file using: python3 smoker_temo_producer.py
 
Enter y to open the RabbitMQ admin page in order to monitor the queues (guest is the username and password). n can be entered if you do not wish to open the RabbitMQ admin page. The data will stream messages from each row every 30 seconds and a confirmation message will show in the terminal. The stream will end when the entire file has been streamed or when interrupted using CTRL+c. 

Screenshots




