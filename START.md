## 🚀 Getting Started

Follow these steps to set up and run the project locally:

### 1. Clone the Repository
Clone the repository to your local machine:
```bash
git clone https://github.com/MicrosoftDocs/mslearn-advanced-copilot.git
cd mslearn-advanced-copilot
```

### 2. Set Up a Virtual Environment
Create and activate a Python virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### 3. Install Dependencies
Install the required Python packages:
```bash
pip install -r requirements.txt
```

### 4. Run the Application
Start the FastAPI application using Uvicorn:
```bash
uvicorn main:app --reload
```

### 5. Access the Application
Open your browser and navigate to:
- **API Documentation**: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- **Root Redirect**: [http://127.0.0.1:8000](http://127.0.0.1:8000)

### 6. Explore the API
Use the `/countries`, `/countries/{country}`, and `/countries/{country}/{city}/{month}` endpoints to interact with the Travel Weather API.

## 🧪 Running Tests
Run the test suite using `pytest` to ensure everything is working correctly:
```bash
pytest
```

## 🐳 Using Docker (Optional)
You can also run the application using Docker:
1. Build the Docker image:
   ```bash
   docker build -t travel-weather-api .
   ```
2. Run the Docker container:
   ```bash
   docker run -p 8000:8000 travel-weather-api
   ```
3. Access the application at [http://127.0.0.1:8000](http://127.0.0.1:8000).

## 📂 Project Structure

Here's an overview of the project structure:

```plaintext
mslearn-advanced-copilot/
├── main.py              # FastAPI application
├── test_main.py         # Test cases for the API
├── weather.json         # Weather data for the API
├── requirements.txt     # Python dependencies
├── Dockerfile           # Docker configuration
├── .devcontainer/       # Dev container configuration
├── .well-known/         # OpenAPI schema
├── START.md             # Getting started guide
└── README.md            # Project documentation
```
