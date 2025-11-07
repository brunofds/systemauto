# backend/Dockerfile

FROM python:3.11-slim

# Define variáveis de ambiente
ENV PYTHONUNBUFFERED 1
ENV APP_HOME /app

# Cria o diretório de trabalho
WORKDIR $APP_HOME

# Instala dependências e copia o código
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .