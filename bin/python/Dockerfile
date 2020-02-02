FROM python:3.7.3-stretch

LABEL Maintainer="Giuseppe Maccario <g_maccario@hotmail.com>"

# install build utilities
RUN apt-get update && \
    pip3 install --upgrade pip

COPY . /app

WORKDIR /app

COPY requirements.txt /tmp/

RUN pip3 install --no-cache-dir -r /tmp/requirements.txt

CMD ["python3"]