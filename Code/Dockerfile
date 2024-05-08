# Use the official Python image with Python 3.8 (slim version)
FROM python:3.8-slim

# Set the working directory inside the container
WORKDIR /main

# Copy the local code to the container image
COPY . /main
#COPY ../Models/Potato_Model_v3.00 /main


# Install Python dependencies from requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Expose port 8000 to the outside world
EXPOSE 8000

# Command to run the application using Uvicorn
#CMD ["uvicorn", "main.py", "--host", "0.0.0.0", "--port", "8000"]
CMD [ "python", "main.py" ]