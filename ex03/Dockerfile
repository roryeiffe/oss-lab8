# base image:
FROM python:3.5

# First Instruction:
RUN apt-get update

# Install Python packages
RUN pip install Flask

# Add file to the container:
ADD . /opt/webapp/

# Add environment variable:
ENV FLASK_APP=hello.py

# Set the working directory for our container:
WORKDIR /opt/webapp

# Expose the port:
EXPOSE 5000

# Run the application:
CMD ["flask","run","--host=0.0.0.0"]

