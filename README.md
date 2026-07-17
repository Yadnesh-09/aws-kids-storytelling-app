# AWS Kids Storytelling App

A serverless storytelling web application that converts children’s stories into speech using **Amazon Polly**.

Users can enter a story, generate audio, view completed stories, and play the generated narration directly from the website.

## Live Demo

[Open AWS Kids Storytelling App](https://yadnesh-09.github.io/aws-kids-storytelling-app/)

## Features

- Upload or enter children’s stories
- Convert story text into speech
- Generate MP3 audio using Amazon Polly
- Store generated audio files in Amazon S3
- Store story information in Amazon DynamoDB
- Display previously generated stories
- Play generated audio directly from the website
- Responsive web interface
- Serverless AWS architecture
- Public frontend hosted using GitHub Pages

## AWS Services Used

- **Amazon API Gateway** — exposes backend API endpoints
- **AWS Lambda** — processes stories and manages requests
- **Amazon Polly** — converts text into natural speech
- **Amazon S3** — stores generated MP3 audio files
- **Amazon DynamoDB** — stores story details and processing status
- **AWS IAM** — controls permissions between AWS services
- **Amazon CloudWatch** — stores Lambda logs and errors

## Architecture

```text
User Browser
     |
     v
GitHub Pages Frontend
     |
     v
Amazon API Gateway
     |
     v
AWS Lambda
     |
     +--------------------+
     |                    |
     v                    v
Amazon Polly        Amazon DynamoDB
Text-to-Speech      Story Metadata
     |
     v
Amazon S3
Generated MP3 Audio
     |
     v
Website Audio Player