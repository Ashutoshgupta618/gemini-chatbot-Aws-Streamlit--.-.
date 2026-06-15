# Gemini AI Chatbot (AWS & Streamlit) 🤖

An advanced Generative AI chatbot built with Streamlit and powered by the Google Gemini API. The application is containerized using Docker and deployed on AWS for a reliable, scalable production environment.

🚀 **Live Demo:** You can test the hosted application live right here: [Streamlit Chatbot App](https://chatbot-7zcsnegcduzeveea3fpsgc.streamlit.app)

---

## 🛠️ Tech Stack & Features

* **GenAI Engine:** Google Gemini API for advanced conversational capabilities.
* **Frontend UI:** Streamlit for a fast, responsive, and clean user interface.
* **Containerization:** Docker for consistent environment setups across local and cloud builds.
* **Cloud Hosting:** Deployed and scaled on AWS.
* **Package Management:** Efficiently managed via `uv` and `pyproject.toml`.

---

## 📋 Prerequisites

Before running the chatbot locally, you will need a **Gemini API Key**. You can obtain one from Google AI Studio and configure it in your local environment variables.

### Installation
Ensure you have your dependencies installed. You can install them using pip:

bash
pip install -r requirement.txt

(Alternatively, if you use the uv package manager, simply run uv sync)

## 💻 How to Run Locally

# Option 1: Running with Python
Clone the repository:

Bash
git clone [https://github.com/Ashutoshgupta618/gemini-chatbot-Aws-Streamlit--.-..git](https://github.com/Ashutoshgupta618/gemini-chatbot-Aws-Streamlit--.-..git)
Navigate into the project directory:

Bash
cd gemini-chatbot-Aws-Streamlit--.-.


Run the Streamlit application:

Bash
streamlit run app.py


# Option 2: Running with Docker 🐳
If you prefer running the application inside a container:

Bash
# Build the docker image
docker build -t genai-chatbot .

# Run the docker container
docker run -p 8501:8501 -e GEMINI_API_KEY="your_api_key_here" genai-chatbot


## 📦 Project Structure

app.py / main.py — Core application script, Gemini API integration, and Streamlit UI.

Dockerfile — Instructions to containerize the app for Docker and AWS deployment.

requirement.txt — Python dependencies layout.

pyproject.toml / uv.lock — Modern Python packaging configuration files.

.devcontainer/ — Pre-configured development container environments.
