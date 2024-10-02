# **YouTube Playlist Comments Scraper**

This project allows you to scrape comments from all the videos in a YouTube playlist using the Google YouTube API. The script iterates over the videos in the playlist and extracts the comments, storing them for further analysis or processing.

## **Features**
* Extracts comments from all videos in a YouTube playlist.
* Uses the Google YouTube API for accurate data retrieval.
* Stores comments in an easy-to-use format (JSON, CSV, or other).
* Handles pagination to get all comments even for videos with many responses.
* Includes error handling to manage API rate limits and other potential issues.

## *Requirements*
Make sure to install the following dependencies:
~~~
pip install google-api-python-client
~~~
Other necessary libraries might include:
~~~
pip install pandas
pip install requests
~~~

## *How to Use*
1. Set up your Google YouTube API:
   * Go to the Google Cloud Console.
   * Create a new project.
   * Enable the YouTube Data API v3 for your project.
   * Generate API credentials (OAuth 2.0 or API Key).
   * Download your API credentials file ( **client_secrets.json** or note down your API key).  
2. Add your API key in the code or ensure the script references your **client_secrets.json**.
3. Run the script:
~~~
python Scraping_Youtube_Comments_From_Playlist.ipynb
~~~
4.The comments will be saved in your desired format for further use.

# **Google YouTube API Setup**
## **Steps to Enable and Use the YouTube Data API**
1. Enable the YouTube Data API v3:
   * Go to the Google Cloud Console.
   * Select your project and navigate to the API & Services section.
   * Search for YouTube Data API v3 and click on "Enable".
2. Obtain API Credentials:
   * After enabling the API, go to the Credentials section.
   * Create a new API key or OAuth 2.0 Client ID, depending on your access method.
   * If using OAuth, download the client_secrets.json file and place it in your project directory.
3. Set API Key or Client Secrets in Code:
   * If using an API Key, set it in the script where required:
     
    ~~~
    api_key = "YOUR_API_KEY"
    ~~~
   * If using OAuth, ensure the client_secrets.json is correctly referenced for the authentication flow.

# **Output**
The script can be modified to save the scraped comments in different formats, such as:
  * CSV for easy data manipulation.
  * JSON for structured data storage.
  * SQL Database for advanced querying.
    
