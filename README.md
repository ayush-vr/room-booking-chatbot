AI Room Booking Chatbot

A simple AI-powered room booking assistant built using IBM Watson Assistant and IBM Cloud Functions.
This project demonstrates how to automate room reservation requests and trigger email notifications using serverless functions.

Features

Conversational room booking chatbot

Automated booking confirmation email

Serverless backend (IBM Cloud Functions)

Easy to deploy and customize

How to Run the Project
1. Download the Project

Clone or download the repository to your local system.

2. Set Up IBM Watson Assistant

Create or sign in to your IBM Cloud account.

Provision a Watson Assistant service instance.

Open Watson Assistant and create a new assistant.

Add a new Actions/Dialog skill.

Upload the provided skill-Room-Booking.json file.

Your chatbot configuration is now ready.

3. Configure the Email Automation

This project includes a cloud function that sends an email whenever a room booking request is submitted.

Steps

Create a new IBM Cloud Function action.

Select Python 3.7 as the runtime environment.

Paste the code from IBM_Cloud_Function.py into the action editor.

Enable 2-step verification in your Google Account.

Generate an App Password under App Passwords in the Security section.

Replace the email password in the cloud function code with your generated app password.

4. Expose the Cloud Function

Open the Endpoints tab of your cloud function.

Enable Web Action.

Copy the generated endpoint URL.

5. Connect the Chatbot With the Cloud Function

In Watson Assistant, go to Options → Webhooks.

Paste the cloud function URL.

Add .json at the end of the URL.

Your room booking chatbot is now fully connected and functional.

6. Ready to Use

The chatbot can now:

Take booking requests

Trigger email notifications

Process responses automatically

You can customize intents, actions, email formatting, or integrate additional logic based on your requirements.
