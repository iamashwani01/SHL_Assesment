# Assessment
🔍 SHL Assessment Recommendation Engine The SHL Assessment Recommendation Engine is a smart web application built to assist HR professionals in selecting the most suitable SHL assessments based on a given job role and its key competencies. 


🛠️ My Approach
Backend Setup (FastAPI):
Created a FastAPI app with two main routes:

/: A form-based HTML interface to input job role and competencies.

/recommend: Handles the POST request, computes recommendations, and returns them in the same HTML page.

/api/recommend: An additional GET endpoint that takes input via query parameters and returns JSON responses.

AI-Powered Recommendation Logic:

Built a recommender module using sentence-transformers from Hugging Face.

Used the all-MiniLM-L6-v2 model to embed both the input and predefined SHL assessment data.

Cosine similarity was used to return the top matches based on semantic similarity.

Frontend:

Used Jinja2 templates to render HTML dynamically with user inputs and recommendations.

Simple and clean design for easy interaction.


Deployment:

Deployed the FastAPI app on Render.

Verified port configuration and environment dependencies (jinja2, python-dotenv, etc.).

Ensured the service responds on both frontend and API endpoints.
