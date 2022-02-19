FROM ubuntu:18.04

RUN apt-get update -y 
RUN apt-get python3-pip -y
RUN apt-get install gunicorn3 -y





#Set the working directory
WORKDIR /opt

#copy all the files
COPY . .

#Install th
RUN pip3 install -r requirements.txt


#Run the command
CMD ["gunicorn3","-b","0.0.0.0:8000","app:app","--workers=5"]