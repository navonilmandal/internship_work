# FlyRank Backend AI Engineering - Assignment 1 (BE-01)

This repository contains the smallest possible backend server built as part of the Backend AI Engineering track.

## Project Structure
- `server.py`: A simple HTTP server built using Python's standard library `http.server` module. It defines two JSON endpoints.
- `.gitignore`: Configured to exclude Python bytecode (`__pycache__/`) and local environments.

## How to Run
Ensure you have Python 3 installed. Run the following command in your terminal:
```bash
python server.py
```
By default, the server will start on port `8000`.

## JSON Endpoints
Once the server is running, you can call it using `curl` or access it in your browser:

### 1. Root Endpoint (`/`)
Returns a welcome message.
- **Request**: `GET http://localhost:8000/`
- **Response**:
  ```json
  {"message": "Welcome to the smallest backend!", "status": "running"}
  ```
- **cURL Command**:
  ```bash
  curl http://localhost:8000/
  ```

### 2. Status Endpoint (`/status`)
Returns server uptime/status.
- **Request**: `GET http://localhost:8000/status`
- **Response**:
  ```json
  {"status": "OK", "uptime": "alive"}
  ```
- **cURL Command**:
  ```bash
  curl http://localhost:8000/status
  ```
