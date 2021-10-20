# Pull base image
FROM python:3.10

# Set environment vsrisbles
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 10

# Set work directory
WORKDIR /hello_project

# Install dependencies
RUN pip install --upgrade pip
COPY ./requirements.txt /hello_project/
RUN pip install -r requirements.txt

# Copy project
COPY . /hello_project/