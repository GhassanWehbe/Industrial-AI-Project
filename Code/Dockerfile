# Use the official Python image with Python 3.8 (slim version)
FROM python:3.8-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the local code to the container image
COPY ./requirements.txt ./requirements.txt

# Install Python dependencies from requirements.txt
RUN pip install -r requirements.txt

COPY . .

# Expose port 8000 to the outside world
EXPOSE 8000

# Command to run the application using Uvicorn
CMD ["uvicorn", "api.main:app", "--host", "0.0.0.0", "--port", "8000"]
#CMD [ "python", "./main.py" ]