# Day 2: 30 Day DevOps Challenge

## Project: NBA Game Notifications System

This project is an exercise from the 30 Day DevOps Challenge. It demonstrates how to create an automated notification system for NBA games using AWS Lambda and Amazon SNS, showcasing serverless architecture and event-driven programming.

## Project Overview

The project consists of a Python Lambda function that:

1. Fetches NBA game data from the SportsData.io API
2. Processes and formats game information
3. Sends notifications via Amazon SNS

## Features

### Game Data Processing (`main.py`)

- Fetches NBA games for the current date from SportsData.io API
- Handles different game statuses (Final, InProgress, Scheduled)
- Formats game information including:
  - Team names and scores
  - Game status and timing
  - Channel information
  - Quarter-by-quarter scores
  - Last play updates for in-progress games

### Notification System

- Uses Amazon SNS for message delivery
- Sends formatted game updates to subscribed endpoints
- Includes comprehensive game information in notifications
- Handles multiple games per day with clear separation

## AWS Services Used

- AWS Lambda: For serverless function execution
- Amazon SNS: For message delivery and notifications
- AWS EventBridge: For scheduling and triggering the Lambda function
- AWS SDK (boto3): For AWS service interaction
