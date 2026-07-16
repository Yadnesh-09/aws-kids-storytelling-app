# AWS Kids Storytelling App

A serverless web application that converts text stories into audio using
Amazon Polly.

## Project Screenshots

### Home Page

![Home Page](home-page.png)

### Story Upload

![Story Upload](story-upload.png)

### Generated Audio Stories

![Generated Stories](generated-audio.png)

## AWS Services Used

- Amazon S3
- AWS Lambda
- Amazon API Gateway
- Amazon Polly
- Amazon DynamoDB
- Amazon CloudWatch
- AWS IAM

## Application Flow

1. The user uploads a `.txt` story file.
2. API Gateway invokes the upload Lambda function.
3. The story file is stored in Amazon S3.
4. An S3 event triggers the processing Lambda.
5. Amazon Polly converts the story into speech.
6. The generated MP3 file is stored in S3.
7. Story information is saved in DynamoDB.
8. The website displays the generated audio story.

## Features

- Upload text stories
- Convert text to speech
- Generate MP3 audio
- Store files in Amazon S3
- Display and play generated stories
- Serverless AWS architecture
- Responsive web interface

## Run Locally

```powershell
py -m http.server 5500

<!-- STORY_SCREENSHOTS_START -->

---

## Application Screenshots

### Storytelling Website

<table>
  <tr>
    <td width="50%" align="center">
      <strong>Application Home Page</strong>
      <br><br>
      <img
        src="screenshots/01-storytelling-home.png"
        alt="AWS Kids Storytelling App home page"
        width="100%">
    </td>

    <td width="50%" align="center">
      <strong>Story Upload Form</strong>
      <br><br>
      <img
        src="screenshots/02-story-upload-form.png"
        alt="Kids storytelling story upload form"
        width="100%">
    </td>
  </tr>

  <tr>
    <td width="50%" align="center">
      <strong>Generated Story List</strong>
      <br><br>
      <img
        src="screenshots/03-generated-story-list.png"
        alt="Generated stories list"
        width="100%">
    </td>

    <td width="50%" align="center">
      <strong>Generated Audio Player</strong>
      <br><br>
      <img
        src="screenshots/04-story-audio-player.png"
        alt="Generated story audio player"
        width="100%">
    </td>
  </tr>
</table>

<!-- STORY_SCREENSHOTS_END -->
