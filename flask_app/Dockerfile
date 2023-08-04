FROM python:3.8

# Set the working directory
WORKDIR /app

# Copy the current directory contents into the container
COPY . /app

# Install required dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Make the port available outside of the container
EXPOSE 5001

# Define the command to run the app
CMD [ "python", "./app.py" ]
