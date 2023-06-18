# Use an official Python runtime as a parent image
FROM python:3.8

# Set environment variables

# Set work directory
WORKDIR /code

# Install dependencies
COPY requirements.txt /code/
RUN pip install --no-cache-dir -r requirements.txt

# Copy the current directory contents into the container at /code
COPY . /code/

# Set the command to run your application
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
