FROM python:3.12-slim-bookworm

RUN apt-get update && apt-get install -y \
    gcc \
    make \
    libpq-dev \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app

RUN pip install uv
COPY pyproject.toml uv.lock /app/
RUN uv sync
COPY . /app/
