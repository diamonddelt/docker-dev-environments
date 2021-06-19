# Declare the base image to use as the container's "Operating System"
FROM python:3.8

# Set the starting directory on the running container
WORKDIR /code

# Copy any dependency files into the WORKDIR
COPY requirements.txt .

# Run a command while building the container (install dependencies via requirements.txt)
RUN pip install -r requirements.txt

# Copy the contents from src/ on the host machine to the WORKDIR within the container
COPY src/ .

# Set the command to run on container start
CMD [ "python", "./your-python-file-here.py"]

