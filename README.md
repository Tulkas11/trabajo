 Analysis of GitHub Profiles

 Synopsis
This application is an API that examines GitHub profiles to extract useful data about a user's coding habits, favorite languages, and overall activity.

 Guidelines

 Configuring the Virtual Environment

1. Create and activate a virtual environment:    
    python -m venv venv
    source venv/bin/activate   On Windows: .\venv\Scripts\activate   

 Setting Up Requirements
2. Install the required dependencies using the following command:
    pip install -r requirements.txt
 Launching the Program
3. Launch the program by running:    
    python app.py 
4. Access the Swagger documentation at
 http://localhost:5000/swagger
 Endpoints
 GET /user-insights/{username}

- Description: Get a GitHub user's analysis.
- Parameters:
  - `username` (path): GitHub username.
- Response:
  - `200 OK`: Successful response with analysis data.
  - `404 Not Found`: User not found.
  - `500 Internal Server Error`: Error occurred while attempting to retrieve data from GitHub.

 Crucial Information

Make sure to replace `your token` in `app.py` with a valid GitHub personal access token.
