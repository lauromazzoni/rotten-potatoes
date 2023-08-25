FROM python:3.8-slim-buster
ENV PYTHONUNBUFFERED=1
WORKDIR /app
RUN pip install python-dotenv
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
COPY . .
EXPOSE 5000
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=5000"]








# # Use an official Python runtime as the base image
# FROM python

# # Set the working directory in the container
# WORKDIR /app

# # Copy the current directory contents into the container at /app
# COPY . /app/

# # Copy the requirements file into the container at /app
# COPY requirements.txt /app/

# RUN pip install python-dotenv
# # Install any needed packages specified in requirements.txt
# RUN pip install -r /app/requirements.txt


# # Make port 80 available to the world outside this container
# EXPOSE 5000

# # Define environment variable for MongoDB connection
# ENV MONGO_DB_HOST=mongodb
# ENV MONGO_DB_PORT=27017
# ENV MONGO_DB_DATABASE=admin
# ENV MONGO_DB_USERNAME=mongouser
# ENV MONGO_DB_PASSWORD=mongopwd

# # Run app.py when the container launches
# CMD ["python", "app.py"]








# # Use uma imagem base do Python
# FROM python:3.9

# # Define um diretório de trabalho no contêiner
# WORKDIR /app

# # Copia o arquivo de requisitos e instala as dependências
# COPY requirements.txt requirements.txt
# RUN pip install -r requirements.txt
# RUN pip install python-dotenv

# # Copia o código do aplicativo para o contêiner
# COPY . .

# # Expõe a porta em que o aplicativo estará em execução (se o aplicativo estiver ouvindo em uma porta específica)
# EXPOSE 5000

# # Define variáveis de ambiente para a conexão com o banco de dados MongoDB
# #ENV MONGO_URI=mongodb://root:root@db:27017/movies?authSource=admin

# # Comando para executar o aplicativo Python
# CMD ["python", "app.py"]








# # FROM python:3.8
# # #ADD . /app
# # COPY requirements.txt /app/
# # RUN pip3 install python-dotenv
# # RUN pip3 install -r /app/requirements.txt

# # WORKDIR /app
# # #COPY . .

# # ENV FLASK_APP=app

# # CMD  ["flask", "run", "--host", "0.0.0.0", "--port", "5000"]

# # # FROM python:3.8

# # # COPY requirements.txt /opt/
# # # RUN pip3 install python-dotenv
# # # RUN pip3 install -r /opt/requirements.txt

# # # WORKDIR /opt
# # # #COPY . .

# # # ENV FLASK_APP=app
# # # ENV FLASK_DEBUG=1
# # # CMD  ["flask", "run", "--host", "0.0.0.0", "--port", "5000"]