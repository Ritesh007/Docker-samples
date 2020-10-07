FROM ubuntu

LABEL NAME="Ritesh"
LABEL EMAIL="rithu.ritesh@gmail.com"

# Update aptitude with new repo
RUN apt-get update

# install defaults
RUN apt-get install -y python2 curl
RUN curl https://bootstrap.pypa.io/get-pip.py --output get-pip.py
RUN python2 get-pip.py
RUN apt-get install -y git
RUN pip install flask

RUN git clone https://github.com/Ritesh007/webservice.git
RUN which python2

EXPOSE 5000
CMD ["python2", "webservice/webapp_flask/webapp/webapp.py"]