

# OpenAI Assistant Integration

This Flask application integrates with OpenAI's API to create and manage conversation threads, allowing users to interact with an AI assistant.

## Getting Started

These instructions will help you get the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Python 3.10 or higher
- Flask
- OpenAI Python SDK

### Installing

1. **Clone the Repository**
   ```
   git clone [repository URL]
   ```

2. **Navigate to the Project Directory**
   ```
   cd [local repository]
   ```

3. **Install Required Packages**
   ```
   pip install -r requirements.txt
   ```

4. **Set Up Environment Variables**
   - Create a `.env` file in your project root directory.
   - Add the following line to the `.env` file:
     ```
     OPENAI_API_KEY=your_openai_api_key_here
     ```
   - Replace `your_openai_api_key_here` with your actual OpenAI API key.

### Running the Application

1. **Start the Flask Server**
   ```
   flask run
   ```

2. **Interact with the Application**
   - Send a GET request to `/start` to initiate a new conversation thread.
   - Send a POST request to `/chat` with `thread_id` and `message` in the JSON body to interact with the assistant.

## Notes

- The application checks for the correct version of the OpenAI SDK and initializes a Flask server.
- It handles creating new conversation threads and processing user messages.
- Ensure your OpenAI API key is kept secure and not exposed.

