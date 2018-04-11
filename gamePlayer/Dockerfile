FROM tensorflow/tensorflow

RUN apt-get update

RUN apt-get install -y \
    cmake \
    libgtk2.0-dev\
    pkg-config \
    libavcodec-dev \
    libavformat-dev \
    libswscale-dev \
    libtbb2 \
    libtbb-dev \
    libjpeg-dev \
    libpng-dev \
    libtiff-dev \
    libjasper-dev \
    libdc1394-22-dev

COPY . .

RUN pip install --upgrade pip

# RUN ls -alt

RUN pip install -r requirements.txt

CMD ["python", "./atari.py", "--game", "SpaceInvaders-v0"]
