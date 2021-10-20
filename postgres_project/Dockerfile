# Pull base image
FROM python:3.9

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE = 1
ENV PYTHONUNBUFFERED = 1

# Set work directory
WORKDIR /postgres_project

# Install dependencies
RUN pip install --upgrade pip
COPY  ./requirements.txt /postgres_project/
RUN pip install -r requirements.txt

# Copy project
COPY . /postgres_project/