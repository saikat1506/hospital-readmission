#Use Python as Base Image
FROM python:3.6-stretch

#Use Working Directory /app
WORKDIR /diab_prediction


#Installing required packages
COPY requirements.txt /
RUN pip install -r /requirements.txt

#Open post 8000
EXPOSE 8000

#Set Envrironment Variable
ENV diab_prediction app.py

#Run python program
COPY app.py .
CMD ["python","app.py"]

