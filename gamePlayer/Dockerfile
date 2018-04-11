FROM python:3

RUN apt-get update
RUN apt-get install -y \
    apt-utils \
    cmake

COPY . /

RUN pip install --upgrade pip

RUN pip install -r requirements.txt

CMD ["python", "./atari.py", "--game", "SpaceInvaders-v0"]
