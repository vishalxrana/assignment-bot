# Home.LLC Assignment - Streamlit Chatbot

This project is a Streamlit chatbot that uses the Gemini API to provide responses. I have used Gemini instead of ChatGPT as the credits of gemini were available. 

## Getting Started

Follow these steps to run the application locally:

**Prerequisites:**

*   **Python 3.7 or higher** installed on your system.
*   **pip** (Python package installer) installed.
*   **Gemini API Key:** You need to obtain a Gemini API key from Google AI for Developers. [https://ai.google.dev/tutorials/setup](https://ai.google.dev/tutorials/setup)

**Steps:**

1.  **Clone the Repository:**

    First, you need to clone the repository to your local machine. Open your terminal and run:

    ```bash
    git clone https://github.com/vishalxrana/assignment-chatbot.git
    ```

    Open CMD from search bar `cd` into your directory
    ```bash
    cd <directory name>
    ```

2.  **Create a Project Directory:**

    Choose a location on your computer and create a new directory for your chatbot project. For example, you can name it `chat_app`.

2.  **Set up a Virtual Environment (Optional but Recommended):**

    It's recommended to use a virtual environment to isolate project dependencies.

    ```bash
    python -m venv venv
    ```

    Activate the virtual environment:

    *   **On Windows:**
        ```bash
        venv\Scripts\activate
        ```
    *   **On macOS and Linux:**
        ```bash
        source venv/bin/activate
        ```

3.  **Create Project Files:**

    Inside your project directory (`my_chatbot_app`), create the following files:

    *   **`index.py`**:  This will contain your Streamlit application code (as provided in the previous code examples).
    *   **`requirements.txt`**: This file lists the Python packages your application depends on. Create this file and add the following lines:

        ```
        streamlit
        google-generativeai
        python-dotenv
        ```
    *   **.env** (Optional, but highly recommended for API key security): Create a file named `.env` in the same directory as `index.py`. You will store your Gemini API key in this file.

4.  **Install Python Packages:**

    Navigate to your project directory in the terminal (where `requirements.txt` is located) and run:

    ```bash
    pip install -r requirements.txt
    ```

    This command will install Streamlit, Google Generative AI library, and `python-dotenv` within your virtual environment.

5.  **Set Up Environment Variables (API Key):**

    Your application needs the Gemini API key to access the Gemini model.

    *   **Create a `.env` file:** If you haven't already, create a file named `.env` in the root directory of your project (same directory as `index.py`).
    *   **Add your API key to `.env`:** Open the `.env` file and add the following line, replacing `<API_KEY>` with your actual Gemini API key that you obtained from Google AI for Developers:

        ```
        API_KEY=<API_KEY>
        ```

        **Important:**  Ensure you use the variable name `API_KEY` as used in the `index.py` code. **Do not commit your `.env` file to version control** (add it to your `.gitignore` file).

6.  **Run the Streamlit Application:**

    In your terminal, make sure your virtual environment is activated. Then, navigate to your project directory and run the following command:

    ```bash
    streamlit run index.py
    ```

    This command will start the Streamlit server. Streamlit will usually automatically open your default web browser and load the chatbot application. If it doesn't open automatically, look at the terminal output for a URL (usually `http://localhost:8501`) and open that URL in your browser.


