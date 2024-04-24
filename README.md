# OpenAI Assistant Message Extractor


## Introduction:

This project aims to streamline the process of extracting historical conversation data from OpenAI Assistant thread platform and storing it in a Google Sheet for further analysis or record-keeping. By automating this task, users can efficiently manage and archive their interactions with the AI assistant, facilitating better organization and utilization of the data.

### Video Demo

![](./open_ai_assistant_history_store_in_google_sheet__online-video-cutter.com___1_.mp4)

## Problem Statement:

Manually retrieving and storing conversation data from the OpenAI platform can be time-consuming and error-prone. Additionally, managing this data in a structured format for analysis or reference purposes presents further challenges. This project addresses these issues by providing an automated solution to extract conversation history and store it in a Google Sheet, enhancing accessibility and usability for users.


## Prerequisites

Before running the script, ensure you have the following dependencies installed:

- Python 3.x
- openai 
- shelve 
- dotenv 
- pandas 
- gspread
- google-auth
- pydrive

Additionally, you'll need a Google Cloud Platform project with the Google Sheets and Google Drive APIs enabled. Obtain the service account credentials JSON file and share the target Google Sheet with the service account email address.

## Configuration

1. Replace `your_thread_id` with the ID of your OpenAI Assistant thread.
2. Specify the `start_timestamp` and `end_timestamp` variables to define the desired time range for message extraction.
3. Set `api_key` to your OpenAI API key.
4. Set `assestent_id` to your OpenAI Assistant ID.
5. Provide the path to your service account credentials JSON file in the `Credentials.from_service_account_file()` function call.

## Usage

1. Clone the repository or copy the script to your local environment.
2. Install the required dependencies listed in the "Prerequisites" section.
3. Configure the script as described in the "Configuration" section.
4. Run the script using `python app.py`.


## To run the OpenAI Assistant Message Extractor:

- First, install the required dependencies by running:
```
pip install -r requirements.txt
```
Then,Fill credentials and execute the script using:
```
python app.py
```

By following these steps, you can automate the extraction and storage of conversation data from your OpenAI Assistant thread into a Google Sheet.

## Features

- Extracts messages from an OpenAI Assistant thread within a specified time range.
- Handles text content and file attachments.
- Updates a Google Sheet with the extracted message data.

## Example

The script connects to your specified OpenAI Assistant thread, extracts messages from April 1, 2024, to April 2, 2024, retrieves text content and file URLs, and updates a Google Sheet with the extracted data.

# Conclusion
In conclusion, the OpenAI Assistant Message Extractor automates the retrieval and storage of conversation data from OpenAI threads. It seamlessly integrates with Google Sheets, simplifying data management. With automated extraction, handling of text and file attachments, and customizable configuration options, it offers a user-friendly solution for organizing and analyzing conversation history.


## Acknowledgments
This project is inspired by the capabilities of OpenAI's GPT-3.5 model and aims to demonstrate how it can be utilized in conversational systems.

## License
This project is licensed under the ML1
