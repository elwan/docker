FROM python:3.7

MAINTAINER Waly Ndiaye "wndiaye@securiport.com"

#RUN apt-get update -y
#RUN apt-get install -y python3-pip python3.7-dev build-essential

# We copy just the requirements.txt first to leverage Docker cache
COPY . /app
WORKDIR /app
RUN pip3 install -r requirements.txt

ENTRYPOINT [ "python" ]

CMD [ "flightstats_api.py" ]
