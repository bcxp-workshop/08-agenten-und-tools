# Start from the official lightweight Python image
FROM mcr.microsoft.com/devcontainers/python:3.11

# Set working directory
WORKDIR /workspaces/${LOCAL_WORKSPACE_FOLDER}

# Copy requirements early (so Codespaces can cache installs)
COPY requirements.txt .

# Install Python dependencies
RUN pip install --no-cache-dir -r requirements.txt
