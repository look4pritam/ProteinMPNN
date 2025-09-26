FROM nvidia/cuda:11.7.1-base-ubuntu20.04


# Copy the ProteinMPNN source code from the local machine to the container
# and set the working directory to there.
COPY . /app/ProteinMPNN
WORKDIR /app/ProteinMPNN


RUN apt-get update \
    && apt-get install -y build-essential \
    && apt-get install -y wget \
    && apt-get clean \
    && apt-get install python3 -y\
    && apt-get install python3-pip -y\
    && rm -rf /var/lib/apt/lists/*

RUN pip install --upgrade pip

RUN pip install torch==2.0.1+cu117 torchvision==0.15.2+cu117 torchaudio==2.0.2+cu117 --index-url https://download.pytorch.org/whl/cu117

RUN pip install fastapi[all] 

ENV PYTHONPATH=/app/ProteinMPNN/
ENV PROTEIN_MPNN=/app/ProteinMPNN/

RUN pip3 install biopython


