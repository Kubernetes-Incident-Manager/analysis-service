# Analysis Service

## Overview
The **Analysis Service** is a microservice responsible for generating insights and analytics based on incident data within the Incident Tracker ecosystem. It processes historical and real-time incident metrics to provide valuable trends, root-cause analysis support, and reporting capabilities.

## Features
- Provides aggregate metrics and insights for incident trends.
- Analyzes resolution times and correlates incidents to dependencies.
- Built with Python and FastAPI.

## Getting Started

### Prerequisites
- Python 3.10+
- `pip` package manager
- Docker (optional for containerized deployment)

### Installation
1. Navigate to the service directory:
   ```bash
   cd services/analysis-service
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Service
To run the service locally for development:
```bash
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

## Docker
Build the Docker image:
```bash
docker build -t incident-tracker/analysis-service .
```
Run the Docker container:
```bash
docker run -p 8000:8000 incident-tracker/analysis-service
```
