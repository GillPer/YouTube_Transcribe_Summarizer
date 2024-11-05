# YouTube_Transcribe_Summarizer

This project demonstrates the creation of an end-to-end application using Google gini pro to extract transcripts from YouTube videos and summarize their content.

## Features

- **YouTube Transcript Retrieval**: Uses the YouTube Transcript API to extract video transcripts from video URLs.
- **Summarization with Google Gini Pro**: Integrates with Google Gini Pro for summarizing the extracted transcripts.
- **Customizable Summaries**: Users can modify the summarization prompt to generate summaries tailored to their needs.
- **Streamlit Interface**: A user-friendly interface for inputting video URLs, customizing summaries, and viewing results.

## Setup and Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/youtube-transcribe-summarizer.git
   cd youtube-transcribe-summarizer
   ```

2. **Install Required Packages**:
   Make sure you have Python installed (version 3.7+ recommended). Install the required packages using `requirements.txt`.
   ```bash
   pip install -r requirements.txt
   ```

3. **API Configuration**:
-  **YouTube Transcript API**: Ensure you have API access for retrieving video transcripts.
-  **Google Gini Pro API**: Set up your Google Gini Pro credentials.
-  Create an `.env` file in the root directory and add your API keys:
   ```bash
   GOOGLE_GINI_API_KEY=your_google_gini_pro_api_key
   ```

4. **Run the Application**:
   Launch the Streamlit app by running the following command:
   ```bash
   streamlit run app.py
   ```

## Project Workflow

**Step 1: Input YouTube URL**
- Enter a YouTube video URL in the provided field within the Streamlit interface.

**Step 2: Retrieve Transcript**
- The app uses the YouTube Transcript API to fetch the video's transcript based on the input URL.

**Step 3: Customize Summarization Prompt**
- Modify the summarization prompt to customize the output summary. The default prompt generates a concise summary of around 250 words.
  
**Step 4: Summarize Transcript**
- The app sends the transcript and prompt to Google Gini Pro, which returns a summary tailored to the prompt.

**Step 5: View Transcript and Summary**
- The transcript and generated summary are displayed on the Streamlit interface for easy viewing and interpretation.
