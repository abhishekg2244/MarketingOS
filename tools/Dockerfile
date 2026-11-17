# FROM python:3.12-slim

# WORKDIR /app

# COPY tools/src/ .

# EXPOSE 8002

# CMD ["python", "app.py"]


FROM python:3.12-slim

# Update OS packages to get security fixes
RUN apt-get update \
    && apt-get upgrade -y \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app

COPY tools/src/ .

EXPOSE 8002

CMD ["python", "app.py"]
