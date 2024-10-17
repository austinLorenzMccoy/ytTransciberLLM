# YouTube Transcript to Detailed Notes Converter

This Streamlit-based app extracts YouTube video transcripts and summarizes the content using Google Gemini AI. It's designed to take a YouTube video link, generate the transcript, and produce a concise, point-based summary of the video within 250 words.

## Features
- **Extract Transcript**: Fetches and compiles the transcript of a YouTube video using `YouTubeTranscriptApi`.
- **AI Summary**: Summarizes the transcript using Google Gemini Pro's `gemini-1.5-flash` model, providing key points in under 250 words.
- **YouTube Thumbnail Display**: Shows the thumbnail of the video.
- **Streamlit Interface**: User-friendly web app built with Streamlit.

## Prerequisites
- **Python 3.8+**
- **Google Generative AI API Key**

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/austinLorenzMccoy/ytTransciberLLM.git
    ```

2. Navigate to the project directory:
    ```bash
    cd ytTransciberLLM
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Set up your environment variables:
    - Create a `.env` file in the root directory.
    - Add your Google API key:
    ```bash
    GOOGLE_API_KEY=your-google-generativeai-api-key
    ```

## Usage

1. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

2. Enter a YouTube video link into the text input box.

3. Click on "Get Detailed Notes" to generate the summarized transcript.

## File Structure

- **app.py**: Main application file that handles video transcript extraction and AI-generated summarization.
- **requirements.txt**: Lists the required Python libraries.
- **.env**: Holds sensitive environment variables like the Google API key.
- **.gitignore**: Specifies files and directories to be ignored by Git, such as `.env` and other environment-specific files.

## Libraries Used
- `streamlit`: For building the web app.
- `youtube_transcript_api`: To extract YouTube video transcripts.
- `google-generativeai`: To interact with Google Gemini's API.
- `python-dotenv`: To load environment variables from the `.env` file.
- `pathlib`: For handling file paths.

## Notes
- The app uses `Google Gemini 1.5 Flash` for summarizing the transcript. Ensure that you have sufficient access and quotas for using the Google Generative AI API.
  
## Contribution
Feel free to fork this project, raise issues, or make pull requests. Any contributions are highly appreciated.

