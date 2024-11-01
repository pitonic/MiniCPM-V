FROM python:3.10-slim

COPY ./requirements.txt requirements.txt

# Install system dependencies
# Install system dependencies
RUN apt-get update && apt-get install -y \
    git \
    # python3 python3-pip \
    # libpoppler-cpp-dev \
    && rm -rf /var/lib/apt/lists/*

# Set the CUDA_HOME environment variable
# ENV CUDA_HOME=/usr/local/cuda

# Upgrade pip and install Python dependencies
RUN pip install --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

CMD ["bash", "-c", "sleep infinity"]
#CMD ["bash", "-c", "python api.py"]
