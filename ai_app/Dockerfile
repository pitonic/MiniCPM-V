FROM nvidia/cuda:12.4.1-base-ubuntu22.04

COPY ./requirements.txt requirements.txt

# Install system dependencies
# Install system dependencies
RUN apt-get update && apt-get install -y \
    git \
    # libpoppler-cpp-dev \
    && rm -rf /var/lib/apt/lists/*

# Upgrade pip and install Python dependencies
RUN pip install --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

CMD ["bash", "-c", "sleep infinity"]
#CMD ["bash", "-c", "python api.py"]
