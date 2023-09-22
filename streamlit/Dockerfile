# Use an official Python runtime as the parent image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Copy the local code and requirements to the container
COPY . .

# Install any dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Make sure you have streamlit in your requirements.txt
# e.g., requirements.txt contains:
# streamlit==1.2.0
# ... (other dependencies)

# Expose port 8080 for Streamlit
EXPOSE 8080

# Define the Streamlit command to run on boot
CMD ["streamlit", "run", "app.py", "--server.port", "8080"]
